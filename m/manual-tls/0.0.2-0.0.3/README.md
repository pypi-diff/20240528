# Comparing `tmp/manual_tls-0.0.2.tar.gz` & `tmp/manual_tls-0.0.3.tar.gz`

## Comparing `manual_tls-0.0.2.tar` & `manual_tls-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rwxr-xr-x   0        0        0     1106 2020-02-02 00:00:00.000000 manual_tls-0.0.2/client.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.2/manual_tls/__init__.py
--rwxr-xr-x   0        0        0    38465 2020-02-02 00:00:00.000000 manual_tls-0.0.2/manual_tls/manual_tls.py
--rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.2/.gitignore
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.2/README.md
--rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 manual_tls-0.0.3/client.py
+-rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 manual_tls-0.0.3/client_key.pem
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.3/manual_tls/__init__.py
+-rwxr-xr-x   0        0        0    41158 2020-02-02 00:00:00.000000 manual_tls-0.0.3/manual_tls/manual_tls.py
+-rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.3/README.md
+-rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.3/PKG-INFO
```

### Comparing `manual_tls-0.0.2/client.py` & `manual_tls-0.0.3/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import socket
 from manual_tls.manual_tls import ManualComm, ManualTls
 
-HOST = "habr.com"
-PORT = 443
+# HOST = "habr.com"
+# PORT = 443
+HOST = "localhost"
+PORT = 4433
 TIMEOUT = 10
 REQUEST = b"HEAD /ru/company/habr/blog/522330/ HTTP/1.1\r\nHost: habr.com\r\nConnection: close\r\n\r\n"
 
 class SocektComm(ManualComm):
     def __init__(self, host, port, timeout) -> None:
         self.host = host
         self.port = port
         self.timeout = timeout
         self.tx_buf = b""
-    
+
     def connect(self) -> None:
         self.s = socket.create_connection((self.host, self.port), self.timeout)
 
     def prepare_send(self, data) -> None:
         self.tx_buf = self.tx_buf + data
 
     def sendall(self, data) -> None:
         self.s.sendall(self.tx_buf + data)
         self.tx_buf = b""
 
     def recv(self, bufsize: int) -> bytes:
         return self.s.recv(bufsize)
-    
+
 
 print(f"Connecting to {HOST}:{PORT}")
 comm = SocektComm(HOST, PORT, TIMEOUT)
 comm.connect()
 
 tls = ManualTls(comm)
 
-pub_key_x, pub_key_y = tls.generate_client_key()
+# pub_key_x, pub_key_y = tls.generate_client_key()
+pub_key_x, pub_key_y = tls.load_client_key("client_key.pem")
+
+print(f"pub_key_x: {pub_key_x.hex()}")
+print(f"pub_key_y: {pub_key_y.hex()}")
 
 tls.establish()
 resp = tls.transmit(REQUEST)
 print(resp.decode(errors='ignore'))
-tls.transmit(None)
+tls.transmit(None)
```

### Comparing `manual_tls-0.0.2/manual_tls/manual_tls.py` & `manual_tls-0.0.3/manual_tls/manual_tls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 
 from abc import ABC, abstractmethod
 from enum import IntEnum
 from hashlib import sha256
 from ecdsa import VerifyingKey, SigningKey, NIST256p
-from ecdsa.util import sigdecode_der
+from ecdsa.util import sigdecode_der, sigencode_der
 
 # in tls 1.3 the version tls 1.2 is sent for better compatibility
 LEGACY_TLS_VERSION = b"\x03\x03"
 TLS_AES_128_GCM_SHA256 = b"\x13\x01"
 
 CHANGE_CIPHER = b"\x14"
 ALERT = b"\x15"
@@ -375,63 +375,60 @@
 
 class ManualTls:
     def __init__(self, comm: ManualComm) -> None:
         self.comm = comm
         self.server_certificate_type = 0
         self.client_certificate_type = 0
         self.signature_algorithms = []
-    
+        self.client_certificate_requested = False
+
     # NETWORK AND LOW LEVEL TLS PROTOCOL HELPERS
     def recv_num_bytes(self, num):
         ret = bytearray()
         while len(ret) < num:
             data = self.comm.recv(min(4096, num - len(ret)))
             if not data:
                 raise BrokenPipeError
             ret += data
         return bytes(ret)
 
-
     def recv_tls(self):
         rec_type = self.recv_num_bytes(1)
-        #tls_version = self.recv_num_bytes(s, 2)
+        # tls_version = self.recv_num_bytes(s, 2)
         _ = self.recv_num_bytes(2)
-        
+
         # "The value of TLSPlaintext.legacy_record_version MUST be ignored by all implementations.""
-        #assert tls_version == LEGACY_TLS_VERSION
+        # assert tls_version == LEGACY_TLS_VERSION
 
         rec_len = bytes_to_num(self.recv_num_bytes(2))
         rec = self.recv_num_bytes(rec_len)
         return rec_type, rec
 
-
     def prepare_send_tls(self, rec_type, msg):
         tls_record = rec_type + LEGACY_TLS_VERSION + num_to_bytes(len(msg), 2) + msg
         self.comm.prepare_send(tls_record)
-        
+
     def send_tls(self, rec_type, msg):
         tls_record = rec_type + LEGACY_TLS_VERSION + num_to_bytes(len(msg), 2) + msg
         self.comm.sendall(tls_record)
 
-
     def recv_tls_and_decrypt(self, key, nonce, seq_num):
         rec_type, encrypted_msg = self.recv_tls()
         assert rec_type == APPLICATION_DATA
 
         msg_type, msg = do_authenticated_decryption(key, nonce, seq_num, APPLICATION_DATA, encrypted_msg)
         print(f"Received handshake type: {msg[0]} ({HandshakeType(msg[0]).name})")
         return msg_type, msg
 
     def parse_extension(self, buff, offset):
         type = bytes_to_num(buff[offset : offset + 2])
         len = bytes_to_num(buff[offset + 2 : offset + 4])
         value = buff[offset + 4 : offset + 4 + len]
-        
-        return type, len, value
 
+        return type, len, value
 
     # PACKET GENERATORS AND HANDLERS
     def gen_client_hello(self, client_random, ecdh_pubkey_x, ecdh_pubkey_y):
         CLIENT_HELLO = b"\x01"
 
         session_id = b""
         compression_method = b"\x00"  # no compression
@@ -505,15 +502,14 @@
         print(f"        Extension len is {bytes_to_num(key_share_length)}: {key_share_length.hex()}")
         print(f"        Extension field len is {bytes_to_num(another_key_share_length)}: {another_key_share_length.hex()}")
         print(f"        Key length {len(ecdh_pubkey)}: {key_exchange_len.hex()}")
         print(f"        Key is: {ecdh_pubkey.hex()}")
 
         return client_hello_tlv
 
-
     def handle_server_hello(self, server_hello):
         handshake_type = server_hello[0]
 
         SERVER_HELLO = 0x2
         assert handshake_type == SERVER_HELLO
 
         server_hello_len = server_hello[1:4]
@@ -564,36 +560,34 @@
         print(f"    Cipher suite is TLS_AES_128_GCM_SHA256: {cipher_suite.hex()}")
         print(f"    Compression method is no compression: {compression_method.hex()}")
         print(f"    Extensions len is {extensions_length}: {num_to_bytes(extensions_length, 2).hex()}")
         print(f"    Extension parsing was skipped, but public_ec_key is {public_ec_key.hex()}")
 
         return server_random, session_id, public_ec_key_x, public_ec_key_y
 
-
     def handle_encrypted_extensions(self, msg):
         assert msg[0] == HandshakeType.ENCRYPTED_EXTENSIONS
         extensions_length = bytes_to_num(msg[1:4])
         assert len(msg[4:]) >= extensions_length
-        
+
         offset = 4
         extensions_length = bytes_to_num(msg[offset:offset + 2])
         offset += 2
         while extensions_length > 0:
             type, length, value = self.parse_extension(msg, offset)
             offset += length + 4
             extensions_length -= length + 4
-            
+
             print(f"        Encrypted_Extension: {ExtensionType(type).name} - {value.hex()}")
 
             if type == ExtensionType.SERVER_CERTIFICATE_TYPE:
                 self.server_certificate_type = value[0]
             elif type == ExtensionType.CLIENT_CERTIFICATE_TYPE:
                 self.client_certificate_type = value[0]
 
-
     def handle_cert_request(self, cert_request_data):
         offset = 0
         handshake_type = cert_request_data[offset]
         offset += 1
 
         assert handshake_type == HandshakeType.CERTIFICATE_REQUEST
 
@@ -603,39 +597,40 @@
 
         self.client_certificate_ctx = b""
         context_len = cert_request_data[offset]
         offset += 1
         if context_len > 0:
             self.client_certificate_ctx = cert_request_data[offset : offset+context_len]
             offset += context_len
-        
+
         extensions_length = bytes_to_num(cert_request_data[offset:offset + 2])
         offset += 2
         while extensions_length > 0:
             type, length, value = self.parse_extension(cert_request_data, offset)
             offset += length + 4
             extensions_length -= length + 4
-            
+
             print(f"        Cert_request_extension: {ExtensionType(type).name} - {value.hex()}")
 
             if type == ExtensionType.SIGNATURE_ALGORITHMS:
                 sig_scheme_length = bytes_to_num(value[:2])
                 pos = 0
                 while pos < sig_scheme_length:
                     alg = bytes_to_num(value[2 + pos : 2 + pos + 2])
                     pos += 2
                     self.signature_algorithms.append(alg)
 
         for alg in self.signature_algorithms:
             print(f"            Signature_alg: {hex(alg)} ({SignatureScheme(alg).name})")
 
+        self.client_certificate_requested = True
 
     def handle_server_cert(self, server_cert_data):
         p = Parser(server_cert_data)
-        
+
         handshake_type = p.get_uint8()
         assert handshake_type == HandshakeType.CERTIFICATE
 
         certificate_field_len = p.get_uint24()
         assert certificate_field_len == p.bytes_left()
 
         certificates = []
@@ -648,25 +643,25 @@
         certificate_field_len = p.get_uint24()
 
         while p.bytes_left() > 0:
             cert_len = p.get_uint24()
             cert = p.get_data(cert_len)
             print(f"cert: {cert.hex()}")
             certificates.append(cert)
-            
+
             # skip extensions
             ext_len = p.get_uint16()
             if ext_len > 0:
                 _ = p.get_data(ext_len)
-            
+
         return certificates
 
     def handle_cert_verify(self, cert_verify_data, rsa, msgs_so_far):
         p = Parser(cert_verify_data)
-        
+
         handshake_type = p.get_uint8()
         assert handshake_type == HandshakeType.CERTIFICATE_VERIFY
 
         cert_verify_len = p.get_uint24()
         assert cert_verify_len == p.bytes_left()
 
         algorithm = p.get_uint16()
@@ -682,44 +677,99 @@
             pub_key = VerifyingKey.from_der(self.server_certs[0])
             valid = pub_key.verify(signature, tbs, sha256, sigdecode=sigdecode_der)
             return valid
         else:
             # not implemented
             return True
 
-
     def handle_finished(self, finished_data, server_finished_key, msgs_so_far):
         handshake_type = finished_data[0]
 
         assert handshake_type == HandshakeType.FINISHED
 
         verify_data_len = bytes_to_num(finished_data[1:4])
         verify_data = finished_data[4:4+verify_data_len]
 
         hmac_digest = hmac_sha256(server_finished_key, one_shot_sha256(msgs_so_far))
         return verify_data == hmac_digest
 
-
     def gen_change_cipher(self):
         CHANGE_CIPHER_SPEC_MSG = b"\x01"
         return CHANGE_CIPHER_SPEC_MSG
 
-
     def gen_encrypted_finished(self, client_write_key, client_write_iv, client_seq_num, client_finish_val):
         FINISHED = b"\x14"
         msg = FINISHED + num_to_bytes(len(client_finish_val), 3) + client_finish_val
 
         return do_authenticated_encryption(client_write_key, client_write_iv, client_seq_num,
                                         HANDSHAKE, msg)
 
+    def gen_encrypted_client_certificate(
+        self, client_write_key, client_write_iv, client_seq_num
+    ):
+
+        spk = VerifyingKey.to_der(self.client_key.verifying_key)
+        certificate_entry = num_to_bytes(len(spk), 3) + spk + bytes(b"\x00\x00")
+        certificate = (
+            bytes(b"\x00") + num_to_bytes(len(certificate_entry), 3) + certificate_entry
+        )
+
+        msg = (
+            bytes([HandshakeType.CERTIFICATE])
+            + num_to_bytes(len(certificate), 3)
+            + certificate
+        )
+
+        return (
+            do_authenticated_encryption(
+                client_write_key, client_write_iv, client_seq_num, HANDSHAKE, msg
+            ),
+            msg,
+        )
+
+    def gen_encrypted_client_certificate_verify(
+        self, client_write_key, client_write_iv, client_seq_num, msgs_so_far
+    ):
+
+        digest = one_shot_sha256(msgs_so_far)
+        print(f"digest: {digest.hex()}")
+
+        tbs = b" " * 64 + b"TLS 1.3, client CertificateVerify" + b"\x00" + digest
+
+        signature = self.client_key.sign(tbs, hashfunc=sha256, sigencode=sigencode_der)
+        certificate_verify = (
+            num_to_bytes(SignatureScheme.ECDSA_SECP256R1_SHA256, 2)
+            + num_to_bytes(len(signature), 2)
+            + signature
+        )
+
+        msg = (
+            bytes([HandshakeType.CERTIFICATE_VERIFY])
+            + num_to_bytes(len(certificate_verify), 3)
+            + certificate_verify
+        )
+
+        return (
+            do_authenticated_encryption(
+                client_write_key, client_write_iv, client_seq_num, HANDSHAKE, msg
+            ),
+            msg,
+        )
+
     def generate_client_key(self):
         self.client_key = SigningKey.generate(curve=NIST256p)
         pub_key = self.client_key.verifying_key.to_string()
         return pub_key[0:32], pub_key[32:64]
 
+    def load_client_key(self, key_file):
+        with open(key_file, "r") as file:
+            pem = file.read()
+            self.client_key = SigningKey.from_pem(pem)
+            pub_key = self.client_key.verifying_key.to_string()
+            return pub_key[0:32], pub_key[32:64]
 
     def establish(self):
         print("Generating params for a client hello, the first message of TLS handshake")
         SECP256R1_P = 0xffffffff00000001000000000000000000000000ffffffffffffffffffffffff
         SECP256R1_A = 0xffffffff00000001000000000000000000000000fffffffffffffffffffffffc
         SECP256R1_G = (0x6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296,
                     0x4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5)
@@ -804,17 +854,17 @@
         assert rec_type == HANDSHAKE
         server_seq_num += 1
 
         if server_cert[0] == HandshakeType.CERTIFICATE_REQUEST:
             print(f"    Certificate_request: {server_cert.hex()}")
 
             self.handle_cert_request(server_cert)
-            
+
             msgs_so_far = msgs_so_far + server_cert
-            
+
             rec_type, server_cert = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
             assert rec_type == HANDSHAKE
             server_seq_num += 1
 
         print(f"    Certificate: {server_cert.hex()}")
 
         self.server_certs = self.handle_server_cert(server_cert)
@@ -851,28 +901,51 @@
         ###########################
         print("Handshake: sending a change cipher msg")
         self.prepare_send_tls(CHANGE_CIPHER, self.gen_change_cipher())
 
         ###########################
         # All client messages beyond this point are encrypted
         msgs_so_far = msgs_so_far + finished
+
+        if self.client_certificate_requested == True:
+            client_certificate_msg, msg = self.gen_encrypted_client_certificate(
+                client_write_key, client_write_iv, client_seq_num
+            )
+            self.prepare_send_tls(APPLICATION_DATA, client_certificate_msg)
+            client_seq_num += 1
+
+            msgs_so_far = msgs_so_far + msg
+
+            client_certificate_verify_msg, msg = (
+                self.gen_encrypted_client_certificate_verify(
+                    client_write_key, client_write_iv, client_seq_num, msgs_so_far
+                )
+            )
+
+            msgs_so_far = msgs_so_far + msg
+
+            self.prepare_send_tls(APPLICATION_DATA, client_certificate_verify_msg)
+            client_seq_num += 1
+
         msgs_sha256 = one_shot_sha256(msgs_so_far)
+
         client_finish_val = hmac_sha256(client_finished_key, msgs_sha256)
 
         print("Handshake: sending an encrypted finished msg")
-        encrypted_hangshake_msg = self.gen_encrypted_finished(client_write_key, client_write_iv, client_seq_num,
-                                                        client_finish_val)
+        encrypted_handshake_msg = self.gen_encrypted_finished(
+            client_write_key, client_write_iv, client_seq_num, client_finish_val
+        )
         print(f"    Client finish value {client_finish_val.hex()}")
-        self.send_tls(APPLICATION_DATA, encrypted_hangshake_msg)
+        self.send_tls(APPLICATION_DATA, encrypted_handshake_msg)
         client_seq_num += 1
 
         print("Handshake finished, regenerating secrets for application data")
 
         ###########################
-        # rederive application secrets
+        # derive application secrets
         msgs_so_far_hash = one_shot_sha256(msgs_so_far)
         premaster_secret = derive_secret(b"derived", data=one_shot_sha256(b""), key=handshake_secret, hash_len=32)
         master_secret = hmac_sha256(key=premaster_secret, data=b"\x00" * 32)
         server_secret = derive_secret(b"s ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
         self.server_write_key = derive_secret(b"key", data=b"", key=server_secret, hash_len=16)
         self.server_write_iv = derive_secret(b"iv", data=b"", key=server_secret, hash_len=12)
         client_secret = derive_secret(b"c ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
```

### Comparing `manual_tls-0.0.2/.gitignore` & `manual_tls-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.2/LICENSE` & `manual_tls-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.2/README.md` & `manual_tls-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.2/pyproject.toml` & `manual_tls-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "manual_tls"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alexander Bersenev / Adam Augustyn", email="watsug@gmail.com" },
 ]
 description = "A tiny TLS 1.3 pure Python implementation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `manual_tls-0.0.2/PKG-INFO` & `manual_tls-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: manual_tls
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tiny TLS 1.3 pure Python implementation
 Project-URL: Homepage, https://github.com/watsug/manual-tls
 Project-URL: Issues, https://github.com/watsug/manual-tls
 Author-email: Alexander Bersenev / Adam Augustyn <watsug@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

