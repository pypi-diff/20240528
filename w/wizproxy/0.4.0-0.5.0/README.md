# Comparing `tmp/wizproxy-0.4.0.tar.gz` & `tmp/wizproxy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizproxy-0.4.0.tar", max compression
+gzip compressed data, was "wizproxy-0.5.0.tar", max compression
```

## Comparing `wizproxy-0.4.0.tar` & `wizproxy-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,32 @@
--rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.4.0/LICENSE
--rw-r--r--   0        0        0     4649 2023-07-10 20:21:23.444091 wizproxy-0.4.0/README.md
--rw-r--r--   0        0        0      564 2023-07-10 20:22:09.337409 wizproxy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.4.0/wizproxy/__init__.py
--rw-r--r--   0        0        0     2554 2023-07-10 12:44:36.771515 wizproxy-0.4.0/wizproxy/__main__.py
--rw-r--r--   0        0        0     3510 2023-07-09 20:05:55.402319 wizproxy-0.4.0/wizproxy/aes.py
--rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.4.0/wizproxy/key_chain.py
--rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.4.0/wizproxy/plugin/__init__.py
--rw-r--r--   0        0        0     3422 2023-07-10 19:55:03.579090 wizproxy-0.4.0/wizproxy/plugin/builtin.py
--rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.4.0/wizproxy/plugin/filter.py
--rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.4.0/wizproxy/plugin/interface.py
--rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.4.0/wizproxy/plugin/log.py
--rw-r--r--   0        0        0     2129 2023-07-09 21:18:01.787007 wizproxy-0.4.0/wizproxy/plugin/scapy.py
--rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.4.0/wizproxy/proto/__init__.py
--rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.4.0/wizproxy/proto/bytes.py
--rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.4.0/wizproxy/proto/dml.py
--rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.4.0/wizproxy/proto/frame.py
--rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.4.0/wizproxy/proto/handshake.py
--rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.4.0/wizproxy/proxy.py
--rw-r--r--   0        0        0     4019 2023-07-10 20:05:51.461947 wizproxy-0.4.0/wizproxy/session.py
--rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.4.0/wizproxy/shard.py
--rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.4.0/wizproxy/stream.py
--rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 wizproxy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4649 2023-07-10 20:21:23.444091 wizproxy-0.5.0/README.md
+-rw-r--r--   0        0        0      606 2024-05-28 13:56:20.737030 wizproxy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-24 17:40:02.714987 wizproxy-0.5.0/wizproxy/__init__.py
+-rw-r--r--   0        0        0     3285 2023-10-26 10:17:50.556879 wizproxy-0.5.0/wizproxy/__main__.py
+-rw-r--r--   0        0        0       66 2023-10-24 21:56:16.461093 wizproxy-0.5.0/wizproxy/core/__init__.py
+-rw-r--r--   0        0        0      545 2023-10-24 19:10:22.548980 wizproxy-0.5.0/wizproxy/core/parcel.py
+-rw-r--r--   0        0        0     2086 2023-10-26 10:17:37.109646 wizproxy-0.5.0/wizproxy/core/proxy.py
+-rw-r--r--   0        0        0     5718 2023-10-26 16:32:07.103403 wizproxy-0.5.0/wizproxy/core/shard.py
+-rw-r--r--   0        0        0       76 2023-10-22 16:25:28.743476 wizproxy-0.5.0/wizproxy/crypto/__init__.py
+-rw-r--r--   0        0        0     5607 2023-10-26 16:32:33.611850 wizproxy-0.5.0/wizproxy/crypto/aes.py
+-rw-r--r--   0        0        0     2568 2023-10-25 13:48:12.158553 wizproxy-0.5.0/wizproxy/crypto/key_chain.py
+-rw-r--r--   0        0        0      112 2023-10-24 19:00:32.069218 wizproxy-0.5.0/wizproxy/plugin/__init__.py
+-rw-r--r--   0        0        0     1182 2023-10-24 18:41:03.328637 wizproxy-0.5.0/wizproxy/plugin/_filter.py
+-rw-r--r--   0        0        0     3962 2023-10-25 22:28:27.997986 wizproxy-0.5.0/wizproxy/plugin/builtin.py
+-rw-r--r--   0        0        0     4359 2023-10-25 21:28:14.599992 wizproxy-0.5.0/wizproxy/plugin/interface.py
+-rw-r--r--   0        0        0      498 2023-10-26 10:17:19.545036 wizproxy-0.5.0/wizproxy/plugin/log.py
+-rw-r--r--   0        0        0     2563 2023-10-25 22:38:14.335423 wizproxy-0.5.0/wizproxy/plugin/scapy.py
+-rw-r--r--   0        0        0      169 2023-10-26 16:35:12.635536 wizproxy-0.5.0/wizproxy/proto/__init__.py
+-rw-r--r--   0        0        0      412 2023-10-26 16:34:59.989368 wizproxy-0.5.0/wizproxy/proto/addr.py
+-rw-r--r--   0        0        0     2727 2023-10-25 17:34:23.825001 wizproxy-0.5.0/wizproxy/proto/bytes.py
+-rw-r--r--   0        0        0     1358 2023-10-25 22:07:16.594426 wizproxy-0.5.0/wizproxy/proto/dml.py
+-rw-r--r--   0        0        0     2290 2023-10-26 16:32:45.385938 wizproxy-0.5.0/wizproxy/proto/frame.py
+-rw-r--r--   0        0        0     2130 2023-10-26 16:33:06.346873 wizproxy-0.5.0/wizproxy/proto/handshake.py
+-rw-r--r--   0        0        0       76 2023-10-25 18:46:40.212978 wizproxy-0.5.0/wizproxy/session/__init__.py
+-rw-r--r--   0        0        0      462 2023-10-25 18:52:12.953189 wizproxy-0.5.0/wizproxy/session/challenges/__init__.py
+-rw-r--r--   0        0        0     4051 2023-10-25 22:14:08.530629 wizproxy-0.5.0/wizproxy/session/challenges/client_sig.py
+-rw-r--r--   0        0        0     4895 2023-10-26 10:46:58.823237 wizproxy-0.5.0/wizproxy/session/impl.py
+-rw-r--r--   0        0        0       40 2023-10-24 17:40:43.924769 wizproxy-0.5.0/wizproxy/transport/__init__.py
+-rw-r--r--   0        0        0     3304 2023-10-26 16:36:05.859451 wizproxy-0.5.0/wizproxy/transport/packet_buffer.py
+-rw-r--r--   0        0        0     1682 2023-10-26 16:38:15.477424 wizproxy-0.5.0/wizproxy/transport/stream.py
+-rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 wizproxy-0.5.0/PKG-INFO
```

### Comparing `wizproxy-0.4.0/LICENSE` & `wizproxy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wizproxy-0.4.0/README.md` & `wizproxy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wizproxy-0.4.0/pyproject.toml` & `wizproxy-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "wizproxy"
-version = "0.4.0"
+version = "0.5.0"
 description = "A proxy for handling encrypted Wizard101 traffic"
 authors = ["Valentin B. <valentin.be@protonmail.com>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
+click = "^8.1.7"
 loguru = "^0.7.0"
 pycryptodome = "^3.18.0"
 scapy = "^2.5.0"
 trio = "^0.22.0"
+exceptiongroup = "^1.1.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
```

### Comparing `wizproxy-0.4.0/wizproxy/__main__.py` & `wizproxy-0.5.0/wizproxy/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,120 @@
-import argparse
 import json
 import platform
 import socket
 from pathlib import Path
+from typing import Optional
 
+import click
 import trio
 from loguru import logger
 
-from .key_chain import KeyChain
-from .plugin import ScapyPlugin, VerboseLog
+from .core import Proxy
+from .crypto import KeyChain
+from .plugin.log import VerboseLogPlugin
+from .plugin.scapy import ScapyPlugin
 from .proto import SocketAddress
-from .proxy import Proxy
+from .session import ClientSig
 
 
-async def main(args):
+async def main(
+    key_dir: Path,
+    host: Optional[str],
+    login: SocketAddress,
+    capture: Optional[Path],
+    verbose: bool,
+):
     key_chain = KeyChain(
-        json.loads((args.keys / "ki_keys.json").read_text()),
-        json.loads((args.keys / "injected_keys.json").read_text()),
+        json.loads((key_dir / "ki_keys.json").read_text()),
+        json.loads((key_dir / "injected_keys.json").read_text()),
     )
 
-    if args.host is None and platform.system() == "Windows":
+    client_sig_path = key_dir / "ClientSig.dec.bin"
+    if client_sig_path.exists():
+        client_sig = ClientSig(client_sig_path.read_bytes())
+    else:
+        client_sig = None
+
+    if host is None and platform.system() == "Windows":
         # Windows default wildcard interface behaves funky and
         # "0.0.0.0" causes trouble when the game client attempts
         # to connect to the proxy.
         #
         # This is not an issue under Wine (Linux and macOS), so
         # we want to use the proper local interface as a default
         # on Windows.
-        args.host = socket.gethostbyname(socket.gethostname())
+        host = socket.gethostbyname(socket.gethostname())
 
     async with trio.open_nursery() as nursery:
-        proxy = Proxy(args.host, key_chain, nursery)
+        proxy = Proxy(host, key_chain, client_sig, nursery)
 
         # If requested, enable the scapy plugin.
-        if args.capture:
-            scapy = ScapyPlugin.from_file(args.capture)
+        if capture is not None:
+            scapy = ScapyPlugin.from_file(capture)
 
-            logger.info(f"Capturing packets to {args.capture.resolve()}")
+            logger.info(f"Capturing packets to {capture.resolve()}")
             proxy.add_plugin(scapy)
         else:
             scapy = None
 
         # If requested, enable verbose packet logging.
-        if args.verbose:
-            proxy.add_plugin(VerboseLog())
+        if verbose:
+            proxy.add_plugin(VerboseLogPlugin())
 
-        await proxy.spawn_shard(SocketAddress(args.login, args.port))
+        # Spawn the initial shard to proxy the login server.
+        await proxy.spawn_shard(login)
 
         try:
             await proxy.run()
         finally:
             if scapy is not None:
                 scapy.writer.close()
 
 
-def run():
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "keys", type=Path, help="The directory with the two key JSON files"
-    )
-    parser.add_argument(
-        "--host",
-        type=str,
-        help="The host interface to bind shard sockets to",
-    )
-    parser.add_argument(
-        "-l",
-        "--login",
-        type=str,
-        default="login.us.wizard101.com",
-        help="The Login Server IP to proxy",
-    )
-    parser.add_argument(
-        "-p",
-        "--port",
-        type=int,
-        default=12000,
-        help="The TCP port to spawn the Login Server on",
-    )
-    parser.add_argument(
-        "-c",
-        "--capture",
-        type=Path,
-        help="Path to the pcapng file to write captures to",
-    )
-    parser.add_argument(
-        "-v", "--verbose", help="Enables verbose logging", action="store_true"
-    )
-
-    trio.run(main, parser.parse_args())
+@click.command()
+@click.argument(
+    "key_dir",
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, path_type=Path),
+)
+@click.option("-h", "--host", help="The host interface to bind sockets to")
+@click.option(
+    "-l",
+    "--login",
+    default="login.us.wizard101.com",
+    show_default=True,
+    help="The Login Server IP",
+)
+@click.option(
+    "-p",
+    "--port",
+    default=12000,
+    show_default=True,
+    help="The TCP port of the Login Server",
+)
+@click.option(
+    "-c",
+    "--capture",
+    type=click.Path(path_type=Path),
+    help="Captures packets to a pcapng file.",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="Enables verbose logging.",
+)
+def run(key_dir, host, login, port, capture, verbose):
+    """Starts the proxy with required files in the key directory.
+
+    The expected files are 'ki_keys.json', a dump of recent client public
+    keys and 'injected_keys.json', a controlled key pair for the client
+    connecting to the proxy.
+
+    Optionally, if a 'ClientSig.dec.bin' file exists, it will be used to
+    make the client communicate with the proxy in plaintext.
+    """
+    login = SocketAddress(login, port)
+    trio.run(main, key_dir, host, login, capture, verbose)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `wizproxy-0.4.0/wizproxy/aes.py` & `wizproxy-0.5.0/wizproxy/transport/packet_buffer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,109 @@
-from typing import Self
+from enum import IntEnum
+from struct import Struct
+from typing import Optional
 
-from Crypto.Cipher import AES
-from Crypto.Random import get_random_bytes
+from wizproxy.crypto import AesContext
 
-CLIENT_CHUNK = 0x100 * AES.block_size
-SERVER_CHUNK = 0x1000 * AES.block_size
+FRAME_HEADER = Struct("<HHI")
 
-NONCE_SIZE = AES.block_size
-TAG_SIZE = AES.block_size
 
+class State(IntEnum):
+    EMPTY = 0
+    GOT_ENCRYPTED_FOOD = 1
+    GOT_FOOD = 2
+
+
+def is_plaintext_frame(raw: memoryview) -> bool:
+    return raw[1] == 0xF0 and raw[0] == 0x0D
 
-class AesContext:
-    """
-    Symmetric AES-GCM processing context.
 
-    After the session handshake, all data will be sent encrypted. Each peer
-    maintains separate states for sending and receiving packets, which is
-    replicated by the encrypt/decrypt routines.
-
-    After construction, the class manages its own key material and will
-    rotate nonces as mandated during data processing.
-
-    :param key: The 16-byte AES encryption key.
-    :param nonce: The 16-byte GCM nonce.
-    :param chunk_size: The size of each chunk before nonce rotation.
+def is_large_frame(size: int) -> bool:
+    return size >= 0x8000
+
+
+class PacketBuffer:
     """
+    Buffers incoming TCP data and splits it into protocol frames.
 
-    def __init__(self, key: bytes, nonce: bytes, chunk_size: int):
-        self._key = key
-        self.chunk_size = chunk_size
-
-        self.encryptor = AES.new(key, AES.MODE_GCM, nonce=nonce)
-        self.encrypted = 0
-
-        self.decryptor = AES.new(key, AES.MODE_GCM, nonce=nonce)
-        self.decrypted = 0
-
-    @classmethod
-    def client(cls, key: bytes, nonce: bytes) -> Self:
-        return cls(key, nonce, CLIENT_CHUNK)
-
-    @classmethod
-    def server(cls, key: bytes, nonce: bytes) -> Self:
-        return cls(key, nonce, SERVER_CHUNK)
-
-    def encrypt(self, data: bytes) -> bytes:
-        output = b""
-
-        data_len = len(data)
-        while data_len > 0:
-            remaining = self.chunk_size - self.encrypted
-
-            # Split data into current chunk and remainder.
-            current = data[:remaining]
-            data = data[remaining:]
-
-            # Encrypt the chunk and update processed bytes accordingly.
-            output += self.encryptor.encrypt(current)
-            self.encrypted = (self.encrypted + len(current)) % self.chunk_size
-
-            # If the chunk is exhausted, regenerate the AES context.
-            # A MAC over all processed data and a new nonce are attached.
-            if self.encrypted == 0:
-                output += self.encryptor.digest()
-                self.encryptor = AES.new(
-                    self._key,
-                    AES.MODE_GCM,
-                    nonce=get_random_bytes(NONCE_SIZE),
-                )
-                output += self.encryptor.nonce
-
-            data_len -= len(current)
-
-        return output
-
-    def decrypt(self, data: bytes) -> bytes:
-        output = b""
-
-        data_len = len(data)
-        while data_len > 0:
-            remaining = self.chunk_size - self.decrypted
-
-            # Split data into current chunk and remainder.
-            current = data[:remaining]
-            data = data[remaining:]
-
-            # Decrypt the chunk and update processed bytes accordingly.
-            output += self.decryptor.decrypt(current)
-            self.decrypted = (self.decrypted + len(current)) % self.chunk_size
-
-            # If the chunk is exhausted, regenerate the AES context.
-            # A MAC over all processed data is verified and a new nonce is loaded.
-            if self.decrypted == 0:
-                self.decryptor.verify(data[:TAG_SIZE])
-                self.decryptor = AES.new(
-                    self._key,
-                    AES.MODE_GCM,
-                    nonce=data[TAG_SIZE : TAG_SIZE + NONCE_SIZE],
-                )
+    This class is meant to be reusable; each connection should
+    maintain an instance and reuse the memory to reduce the
+    number of allocations in the program.
+    """
 
-                data = data[TAG_SIZE + NONCE_SIZE :]
-                data_len -= TAG_SIZE + NONCE_SIZE
+    def __init__(self):
+        self.buf = bytearray()
+        self.buf_len = 0
+
+        self._state = State.EMPTY
+        self._food = None
+
+    def feed(self, data: bytes):
+        self.buf.extend(data)
+        self.buf_len += len(data)
+
+    def split_off(self, nbytes: int) -> bytes:
+        data = self.buf[:nbytes]
+
+        self.buf = self.buf[nbytes:]
+        self.buf_len -= nbytes
+
+        return data
+
+    def _required_bytes(self, aes: Optional[AesContext], nbytes: int) -> int:
+        if aes is not None:
+            return aes.calculate_decryption_overhead(nbytes)
+        else:
+            return nbytes
+
+    def _poll_header(self, aes: Optional[AesContext]):
+        if self._state == State.EMPTY:
+            # Make sure we have enough bytes to consume the frame header.
+            food_bytes = self._required_bytes(aes, 8)
+            if self.buf_len < food_bytes:
+                return
+
+            # Determine if the frame is encrypted by some magic header bytes.
+            encrypted = aes is not None and not is_plaintext_frame(self.buf)
+
+            self._food = self.split_off(food_bytes)
+            if encrypted:
+                self._food = aes.decrypt(self._food)
+                self._state = State.GOT_ENCRYPTED_FOOD
+            else:
+                self._state = State.GOT_FOOD
+
+    def poll_frame(self, aes: Optional[AesContext]) -> Optional[tuple[bool, bytes]]:
+        # Read and decrypt the next frame's header, or wait for more data.
+        self._poll_header(aes)
+        if self._state == State.EMPTY:
+            return None
+
+        # Unpack the header data and make sure we can consume the frame.
+        magic, size, large_size = FRAME_HEADER.unpack(self._food)
+
+        # Validate the header magic to make sure the data is valid.
+        if magic != 0xF00D:
+            raise ValueError("received unsupported frame data")
+
+        # Unpack the size and compute how many bytes we still need to consume.
+        if is_large_frame(size):
+            size = large_size
+        else:
+            # We already consumed the first 4 bytes of the body prematurely
+            # to make sure our header is big enough.
+            size -= 4
+        size = self._required_bytes(aes, size)
+
+        # If we don't have enough data yet, wait for more.
+        if self.buf_len < size:
+            return None
+
+        # Extract the frame body and decrypt it, if necessary.
+        body = self.split_off(size)
+        encrypted = self._state == State.GOT_ENCRYPTED_FOOD
+        if encrypted:
+            body = aes.decrypt(body)
 
-            data_len -= len(current)
+        self._state = State.EMPTY
 
-        return output
+        return encrypted, self._food + body
```

### Comparing `wizproxy-0.4.0/wizproxy/key_chain.py` & `wizproxy-0.5.0/wizproxy/crypto/key_chain.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,27 +32,33 @@
     format is the output JSONs it produces.
 
     :param ki_keys: KingsIsle public key material from a client.
     :param injected_keys: Private key material to injected client keys.
     """
 
     def __init__(self, ki_keys: dict[str, Any], injected_keys: dict[str, Any]):
-        self.key_buf = b64decode(ki_keys["raw"].encode())
+        self.ki_key_buf = b64decode(ki_keys["raw"].encode())
         self.public_keys = [
             RSA.import_key(b64decode(key["public"].encode()))
             for key in ki_keys["decoded"]
         ]
 
+        self.injected_key_buf = b64decode(injected_keys["raw"].encode())
         self.private_keys = [
             RSA.import_key(b64decode(key["private"].encode()))
             for key in injected_keys["decoded"]
         ]
 
     def hash_key_buf(self, offset: int, length: int) -> int:
-        return fnv_1a(self.key_buf[offset : offset + length])
+        return fnv_1a(self.ki_key_buf[offset : offset + length])
+
+    def verify_key_hash(self, offset: int, length: int, expected: int):
+        buf_hash = fnv_1a(self.injected_key_buf[offset : offset + length])
+        if buf_hash != expected:
+            raise ValueError("key hash mismatch; algorithm changed?")
 
     def sign(self, key_slot: int, data: bytes) -> bytes:
         key = self.private_keys[key_slot]
         data_hash = SHA1.new(data)
 
         return pkcs1_15.new(key).sign(data_hash)
```

### Comparing `wizproxy-0.4.0/wizproxy/plugin/builtin.py` & `wizproxy-0.5.0/wizproxy/plugin/builtin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,115 @@
-from ..proto import Frame, SocketAddress, dml
+from wizproxy.proto import Frame, SocketAddress, dml
+
 from . import Context, Direction, Plugin, listen
 
 MSG_CHARACTERSELECTED = dml.Layout(
-    (
-        ("IP", dml.Type.STR),
-        ("TCPPort", dml.Type.INT),
-        ("UDPPort", dml.Type.INT),
-        ("Key", dml.Type.STR),
-        ("UserID", dml.Type.GID),
-        ("CharID", dml.Type.GID),
-        ("ZoneID", dml.Type.GID),
-        ("ZoneName", dml.Type.STR),
-        ("Location", dml.Type.STR),
-        ("Slot", dml.Type.INT),
-        ("PrepPhase", dml.Type.INT),
-        ("Error", dml.Type.INT),
-        ("LoginServer", dml.Type.STR),
-    )
+    ("IP", dml.Type.STR),
+    ("TCPPort", dml.Type.INT),
+    ("UDPPort", dml.Type.INT),
+    ("Key", dml.Type.STR),
+    ("UserID", dml.Type.GID),
+    ("CharID", dml.Type.GID),
+    ("ZoneID", dml.Type.GID),
+    ("ZoneName", dml.Type.STR),
+    ("Location", dml.Type.STR),
+    ("Slot", dml.Type.INT),
+    ("PrepPhase", dml.Type.INT),
+    ("Error", dml.Type.INT),
+    ("LoginServer", dml.Type.STR),
 )
 
 MSG_SERVERTRANSFER = dml.Layout(
-    (
-        ("IP", dml.Type.STR),
-        ("TCPPort", dml.Type.INT),
-        ("UDPPort", dml.Type.INT),
-        ("Key", dml.Type.INT),
-        ("UserID", dml.Type.GID),
-        ("CharID", dml.Type.GID),
-        ("ZoneName", dml.Type.STR),
-        ("ZoneID", dml.Type.GID),
-        ("Location", dml.Type.STR),
-        ("Slot", dml.Type.INT),
-        ("SessionID", dml.Type.GID),
-        ("SessionSlot", dml.Type.INT),
-        ("TargetPlayerID", dml.Type.GID),
-        ("FallbackIP", dml.Type.STR),
-        ("FallbackTCPPort", dml.Type.INT),
-        ("FallbackUDPPort", dml.Type.INT),
-        ("FallbackKey", dml.Type.INT),
-        ("FallbackZone", dml.Type.STR),
-        ("FallbackZoneID", dml.Type.GID),
-        ("TransitionID", dml.Type.INT),
-    )
+    ("IP", dml.Type.STR),
+    ("TCPPort", dml.Type.INT),
+    ("UDPPort", dml.Type.INT),
+    ("Key", dml.Type.INT),
+    ("UserID", dml.Type.GID),
+    ("CharID", dml.Type.GID),
+    ("ZoneName", dml.Type.STR),
+    ("ZoneID", dml.Type.GID),
+    ("Location", dml.Type.STR),
+    ("Slot", dml.Type.INT),
+    ("SessionID", dml.Type.GID),
+    ("SessionSlot", dml.Type.INT),
+    ("TargetPlayerID", dml.Type.GID),
+    ("FallbackIP", dml.Type.STR),
+    ("FallbackTCPPort", dml.Type.INT),
+    ("FallbackUDPPort", dml.Type.INT),
+    ("FallbackKey", dml.Type.INT),
+    ("FallbackZone", dml.Type.STR),
+    ("FallbackZoneID", dml.Type.GID),
+    ("TransitionID", dml.Type.INT),
+)
+
+MSG_CONNECTIONSTATS = dml.Layout(
+    ("ServerHostname", dml.Type.STR),
+    ("ServerPort", dml.Type.INT),
+    ("ConnectMS", dml.Type.INT),
+    ("Timeouts", dml.Type.INT),
+    ("Errors", dml.Type.INT),
 )
 
 
-class Builtin(Plugin):
+class BuiltinPlugin(Plugin):
     """
     Core functionality of the proxy, modeled as a built-in plugin.
 
-    This does the crypto handshake for successful proxying and
-    handles redirects of the client to other shards.
+    This does the crypto handshake for successful proxying and handles
+    redirects of the client to other shards.
     """
 
     @listen(Direction.SERVER_TO_CLIENT, opcode=0)
     async def patch_session_offer(self, ctx: Context, frame: Frame):
-        frame.payload = ctx.session.session_offer(frame.payload)
+        ctx.session.session_offer(frame)
 
     @listen(Direction.CLIENT_TO_SERVER, opcode=5)
     async def patch_session_accept(self, ctx: Context, frame: Frame):
-        frame.payload = ctx.session.session_accept(frame.payload)
+        ctx.session.session_accept(frame)
 
     @listen(Direction.SERVER_TO_CLIENT, service_id=7, order=3)
     async def redirect_character_selected(self, ctx: Context, frame: Frame):
         msg = MSG_CHARACTERSELECTED.decode(frame.payload)
 
         # Extract the server that should be proxied and check validity.
         socket = SocketAddress(msg["IP"], msg["TCPPort"])
         if not socket.ip and not socket.port:
             return
 
-        # Spawn a new shard to proxy the new server connection.
-        local = await ctx.spawn_shard(socket)
+        # Spawn a shard to proxy the new server connection.
+        shard = await ctx.spawn_shard(socket)
 
         # Fix up the client packet to make it connect to the shard.
-        msg["IP"] = local.ip.encode()
-        msg["TCPPort"] = local.port
+        msg["IP"] = shard.ip
+        msg["TCPPort"] = shard.port
 
         frame.payload = MSG_CHARACTERSELECTED.encode(msg)
 
     @listen(Direction.SERVER_TO_CLIENT, service_id=5, order=221)
     async def redirect_server_transfer(self, ctx: Context, frame: Frame):
         msg = MSG_SERVERTRANSFER.decode(frame.payload)
 
-        # Spawn a new shard to proxy the new server connection.
-        local = await ctx.spawn_shard(SocketAddress(msg["IP"], msg["TCPPort"]))
-        fallback = ctx.shard()
+        # Spawn a new shard to proxy the server connection.
+        addr = SocketAddress(msg["IP"], msg["TCPPort"])
+        shard = await ctx.spawn_shard(addr)
+        fallback = ctx.shard_addr
 
         # Fix up the client packet to make it connect to the shard.
         # Use the current shard's socket as the fallback just in case.
-        msg["IP"] = local.ip.encode()
-        msg["TCPPort"] = local.port
-        msg["FallbackIP"] = fallback.ip.encode()
+        msg["IP"] = shard.ip
+        msg["TCPPort"] = shard.port
+        msg["FallbackIP"] = fallback.ip
         msg["FallbackTCPPort"] = fallback.port
 
         frame.payload = MSG_SERVERTRANSFER.encode(msg)
+
+    @listen(Direction.CLIENT_TO_SERVER, service_id=53, order=67)
+    async def patch_connection_stats(self, ctx: Context, frame: Frame):
+        msg = MSG_CONNECTIONSTATS.decode(frame.payload)
+
+        # Client reports the host it is connected to to the server every now and then.
+        # We need to spoof the address here or the server sees that we're proxying.
+        remote = ctx.remote_addr
+        msg["ServerHostname"] = remote.ip
+        msg["ServerPort"] = remote.port
+
+        frame.payload = MSG_CONNECTIONSTATS.encode(msg)
```

### Comparing `wizproxy-0.4.0/wizproxy/plugin/filter.py` & `wizproxy-0.5.0/wizproxy/plugin/_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Optional
 
-from ..proto import Frame
+from wizproxy.proto import Frame
 
 
 class Direction(Enum):
-    """The direction in which a frame is traveling."""
+    """The direction in which a frame is travelling."""
 
-    #: Listener is only invoked for frames going from server to client.
     SERVER_TO_CLIENT = auto()
-
-    #: Listener is only invoked for frames going from client to server.
     CLIENT_TO_SERVER = auto()
 
 
-@dataclass
-class _Filter:
-    direction: Direction
-
-    opcode: Optional[int]
-    service_id: Optional[int]
-    order: Optional[int]
+class Filter:
+    def __init__(
+        self,
+        direction: Direction,
+        opcode: Optional[int],
+        service_id: Optional[int],
+        order: Optional[int],
+    ):
+        if opcode is not None and service_id is not None:
+            raise ValueError("unsupported filter for control and data frames")
+
+        if order is not None and service_id is None:
+            raise ValueError("cannot filter by order without service")
+
+        self.direction = direction
+        self.opcode = opcode
+        self.service_id = service_id
+        self.order = order
 
     def can_dispatch(self, frame: Frame) -> bool:
         if self.opcode is not None:
             return frame.opcode == self.opcode
 
         elif self.service_id is not None:
             if self.order is None:
                 return frame.service_id == self.service_id
 
             return frame.service_id == self.service_id and frame.order == self.order
 
         return True
-
-
-def _make_filter(
-    direction: Direction,
-    opcode: Optional[int],
-    service_id: Optional[int],
-    order: Optional[int],
-) -> _Filter:
-    if opcode is not None and service_id is not None:
-        raise ValueError("Unsupported filter for control and data frames")
-
-    if order is not None and service_id is None:
-        raise ValueError("Cannot filter by order without service")
-
-    return _Filter(direction, opcode, service_id, order)
```

### Comparing `wizproxy-0.4.0/wizproxy/plugin/scapy.py` & `wizproxy-0.5.0/wizproxy/plugin/scapy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 
-# Silence overly verbose scapy logging except for errors.
-logging.getLogger("scapy.runtime").setLevel(logging.ERROR)
-
 import trio
 from scapy.layers.inet import IP, TCP, Ether
 from scapy.utils import PcapNgWriter
 
-from ..proto import Bytes, Frame, SocketAddress
+from wizproxy.proto import Frame, SocketAddress
+
 from . import Context, Direction, Plugin, listen
 
+# Silence overly verbose scapy logging except for errors.
+logging.getLogger("scapy.runtime").setLevel(logging.ERROR)
+
 
 class ScapyPlugin(Plugin):
     """
     A plugin which writes frame data to pcapng files.
 
-    Each packet is written as TCP, pretending to be directly
-    exchanged between a local client and the remote server.
+    Each packet is written as TCP, pretending to be directly exchanged
+    between a local client and the remote server.
 
-    Each packet has a comment attached, describing the local
-    shard that produced it and what client it was.
+    Each frame has a machine-parseable comment attached, describing
+    the local shard that produced the frame and what client it was.
     """
 
     def __init__(self, writer: PcapNgWriter):
         super().__init__()
 
         self.writer = writer
 
@@ -35,38 +36,44 @@
             now = datetime.now()
             path = path / now.strftime("wizproxy_%Y-%m-%d_%H-%M-%S.pcapng")
 
         writer = PcapNgWriter(str(path.resolve()))
         return cls(writer)
 
     async def write_to_file(
-        self, ctx: Context, source: SocketAddress, dest: SocketAddress, raw: bytes
+        self, ctx: Context, src: SocketAddress, dest: SocketAddress, frame: Frame
     ):
-        shard = ctx.shard()
+        shard = ctx.shard_addr
+
+        comment = [
+            f"Shard {shard}",
+            f"Session {ctx.session.sid}",
+            f"Client {ctx.session.client}",
+            f"Server {ctx.session.server}",
+        ]
+        if frame.opcode == 5:
+            # When this is a Session Accept frame, also include the
+            # AES key and nonce for reference.
+            aes_context = ctx.session.server_aes
+            if aes_context is not None:
+                comment.append(f"AES-Key: {aes_context.key.hex()}")
+                comment.append(f"AES-Nonce: {aes_context.decryptor.nonce.hex()}")
 
         packet = (
             Ether()
-            / IP(src=source.ip, dst=dest.ip)
-            / TCP(sport=source.port, dport=dest.port)
-            / raw
-        )
-        packet.comment = (
-            f"Shard {shard.ip}:{shard.port}, client {ctx.session.sid}".encode()
+            / IP(src=src.ip, dst=dest.ip)
+            / TCP(sport=src.port, dport=dest.port)
+            / frame.original
         )
+        packet.comment = "\n".join(comment)
 
         await trio.to_thread.run_sync(self.writer.write, packet)
 
-    @listen(Direction.CLIENT_TO_SERVER)
+    @listen(Direction.CLIENT_TO_SERVER, dirty=False)
     async def clientbound(self, ctx: Context, frame: Frame):
-        bytes = Bytes()
-        frame.write(bytes)
-
         session = ctx.session
-        await self.write_to_file(ctx, session.client, session.server, bytes.getvalue())
+        await self.write_to_file(ctx, session.client, session.server, frame)
 
-    @listen(Direction.SERVER_TO_CLIENT)
+    @listen(Direction.SERVER_TO_CLIENT, dirty=False)
     async def serverbound(self, ctx: Context, frame: Frame):
-        bytes = Bytes()
-        frame.write(bytes)
-
         session = ctx.session
-        await self.write_to_file(ctx, session.server, session.client, bytes.getvalue())
+        await self.write_to_file(ctx, session.server, session.client, frame)
```

### Comparing `wizproxy-0.4.0/wizproxy/proto/bytes.py` & `wizproxy-0.5.0/wizproxy/proto/bytes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 import io
 import struct
 from typing import Any
 
+U8 = struct.Struct("B")
+I8 = struct.Struct("b")
+U16 = struct.Struct("<H")
+I16 = struct.Struct("<h")
+U32 = struct.Struct("<I")
+I32 = struct.Struct("<i")
+U64 = struct.Struct("<Q")
+F32 = struct.Struct("<f")
+F64 = struct.Struct("<d")
+
 
 class Bytes(io.BytesIO):
     """
-    A :class:`io.BytesIO` with support for structured data.
+    Provides reading and writing support for structured binary data.
 
     All operations assume little-endian byte ordering.
     """
 
-    def _read_fmt(self, fmt: str) -> Any:
-        size = struct.calcsize(fmt)
-        unpacked = struct.unpack(fmt, self.read(size))
-
-        return unpacked[0] if len(unpacked) == 1 else unpacked
+    def load_frame(self, raw: bytes):
+        self.seek(0)
+        self.write(raw)
+        self.truncate()
+
+    def read_struct(self, s: struct.Struct) -> Any:
+        value = s.unpack(self.read(s.size))
+        return value[0] if len(value) == 1 else value
 
-    def _write_fmt(self, fmt: str, *args) -> int:
-        packed = struct.pack(fmt, *args)
+    def write_struct(self, s: struct.Struct, *args) -> int:
+        packed = s.pack(*args)
         return self.write(packed)
 
     def u8(self) -> int:
-        return self._read_fmt("B")
+        return self.read_struct(U8)
 
-    def write_u8(self, value: int) -> int:
-        return self._write_fmt("B", value)
+    def write_u8(self, v: int) -> int:
+        return self.write_struct(U8, v)
 
     def i8(self) -> int:
-        return self._read_fmt("b")
+        return self.read_struct(I8)
 
-    def write_i8(self, value: int) -> int:
-        return self._write_fmt("b", value)
+    def write_i8(self, v: int) -> int:
+        return self.write_struct(I8, v)
 
     def u16(self) -> int:
-        return self._read_fmt("<H")
+        return self.read_struct(U16)
 
-    def write_u16(self, value: int) -> int:
-        return self._write_fmt("<H", value)
+    def write_u16(self, v: int) -> int:
+        return self.write_struct(U16, v)
 
     def i16(self) -> int:
-        return self._read_fmt("<h")
+        return self.read_struct(I16)
 
-    def write_i16(self, value: int) -> int:
-        return self._write_fmt("<h", value)
+    def write_i16(self, v: int) -> int:
+        return self.write_struct(I16, v)
 
     def u32(self) -> int:
-        return self._read_fmt("<I")
+        return self.read_struct(U32)
 
-    def write_u32(self, value: int) -> int:
-        return self._write_fmt("<I", value)
+    def write_u32(self, v: int) -> int:
+        return self.write_struct(U32, v)
 
     def i32(self) -> int:
-        return self._read_fmt("<i")
+        return self.read_struct(I32)
 
-    def write_i32(self, value: int) -> int:
-        return self._write_fmt("<i", value)
+    def write_i32(self, v: int) -> int:
+        return self.write_struct(I32, v)
 
     def u64(self) -> int:
-        return self._read_fmt("<Q")
+        return self.read_struct(U64)
 
-    def write_u64(self, value: int) -> int:
-        return self._write_fmt("<Q", value)
+    def write_u64(self, v: int) -> int:
+        return self.write_struct(U64, v)
 
     def f32(self) -> float:
-        return self._read_fmt("<f")
+        return self.read_struct(F32)
 
-    def write_f32(self, value: float) -> int:
-        return self._write_fmt("<f", value)
+    def write_f32(self, v: float) -> int:
+        return self.write_struct(F32, v)
 
     def f64(self) -> float:
-        return self._read_fmt("<d")
+        return self.read_struct(F64)
 
-    def write_f64(self, value: float) -> int:
-        return self._write_fmt("<d", value)
+    def write_f64(self, v: float) -> int:
+        return self.write_struct(F64, v)
 
     def string(self) -> bytes:
         size = self.u16()
         return self.read(size)
 
     def write_string(self, data: bytes) -> int:
         written = 0
@@ -84,17 +97,17 @@
         written += self.write_u16(len(data))
         written += self.write(data)
 
         return written
 
     def wstr(self) -> str:
         size = self.u16()
-        return self.read(size).decode("utf-16-le")
+        return self.read(size * 2).decode("utf-16-le")
 
     def write_wstr(self, data: str) -> int:
         raw = data.encode("utf-16-le")
         written = 0
 
-        written += self.write_u16(len(raw))
+        written += self.write_u16(len(data))
         written += self.write(raw)
 
         return written
```

### Comparing `wizproxy-0.4.0/wizproxy/proto/dml.py` & `wizproxy-0.5.0/wizproxy/proto/dml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Any, Iterable
 
 from .bytes import Bytes
 
-_DML_DECODE_LOOKUP = [
+_DML_DECODE_LOOKUP = (
     (Bytes.i8, Bytes.write_i8),
     (Bytes.u8, Bytes.write_u8),
     (Bytes.u16, Bytes.write_u16),
     (Bytes.i32, Bytes.write_i32),
     (Bytes.u32, Bytes.write_u32),
     (Bytes.u64, Bytes.write_u64),
     (Bytes.string, Bytes.write_string),
     (Bytes.wstr, Bytes.write_wstr),
     (Bytes.f32, Bytes.write_f32),
     (Bytes.f64, Bytes.write_f64),
-]
+)
 
 
 class Type(IntEnum):
-    """Enumeration of supported DML types."""
+    """Supported DML types."""
 
     BYT = 0
     UBYT = 1
     USHRT = 2
     INT = 3
     UINT = 4
     GID = 5
@@ -35,28 +35,29 @@
 
 @dataclass
 class Layout:
     """Describes the data layout of a DML message."""
 
     layout: Iterable[tuple[str, Type]]
 
+    def __init__(self, *args: tuple[str, Type]):
+        self.layout = args
+
     def encode(self, msg: dict[str, Any]) -> bytes:
         buf = Bytes()
 
         for name, typ in self.layout:
             value = msg[name]
             _, encode = _DML_DECODE_LOOKUP[typ]
-
             encode(buf, value)
 
         return buf.getvalue()
 
     def decode(self, raw: bytes) -> dict[str, Any]:
         buf = Bytes(raw)
         msg = {}
 
         for name, typ in self.layout:
             decode, _ = _DML_DECODE_LOOKUP[typ]
-
             msg[name] = decode(buf)
 
         return msg
```

### Comparing `wizproxy-0.4.0/wizproxy/proto/frame.py` & `wizproxy-0.5.0/wizproxy/proto/frame.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,87 @@
-from dataclasses import dataclass
-from typing import Optional, Self
+from dataclasses import dataclass, field
+from typing import Optional
 
 from .bytes import Bytes
 
 
 @dataclass
 class Frame:
     """
     Parsed representation of a KingsIsle network frame.
 
     The payload portion needs implementation-defined handling
-    depending on whether it is a control or data frame.
+    depending on whether it is a control or data frame. It is
+    not parsed by default.
     """
 
+    original: bytes
+
     opcode: Optional[int]
     service_id: Optional[int]
     order: Optional[int]
     payload: bytes
 
+    # Controls whether a frame needs to be reserialized after a change.
+    dirty: bool = field(default=False)
+
     @classmethod
-    def read(cls, buf: Bytes) -> Self:
-        buf.u16()
+    def read(cls, buf: Bytes) -> "Frame":
+        buf.seek(0)
+        original = buf.getvalue()
+
+        assert buf.u16() == 0xF00D
 
         size = buf.u16()
         if size >= 0x8000:
             size = buf.u32()
 
         is_control = buf.u8() != 0
         opcode = buf.u8()
-        buf.u16()
+        buf.u16()  # Reserved.
 
         if is_control:
-            service_id = None
-            order = None
-            payload = buf.read()
+            service_id, order = None, None
+            payload = buf.read(size - 4)
         else:
             service_id = buf.u8()
             order = buf.u8()
             payload_len = buf.u16()
             payload = buf.read(payload_len - 4)
+            buf.u8()  # Trailing null byte.
 
-        return cls(opcode if is_control else None, service_id, order, payload)
+        return cls(original, opcode if is_control else None, service_id, order, payload)
 
     def write(self, buf: Bytes) -> int:
         buf.seek(0)
+
         written = 0
+        payload_len = len(self.payload)
 
-        size = 4 + len(self.payload)
+        size = 4 + payload_len
         if self.opcode is None:
             size += 5
 
         written += buf.write_u16(0xF00D)
         if size < 0x8000:
             written += buf.write_u16(size)
         else:
             written += buf.write_u16(0x8000)
             written += buf.write_u32(size)
 
         is_control = self.opcode is not None
 
-        written += buf.write_u8(int(is_control))
+        written += buf.write_u8(1 if is_control else 0)
         written += buf.write_u8(self.opcode or 0)
         written += buf.write_u16(0)
 
         if is_control:
             written += buf.write(self.payload)
         else:
-            written += buf.write_u8(self.service_id)  # type:ignore
-            written += buf.write_u8(self.order)  # type:ignore
-            written += buf.write_u16(len(self.payload) + 4)
+            written += buf.write_u8(self.service_id)
+            written += buf.write_u8(self.order)
+            written += buf.write_u16(payload_len + 4)
             written += buf.write(self.payload)
             written += buf.write_u8(0)
 
         buf.truncate()
         return written
```

### Comparing `wizproxy-0.4.0/wizproxy/shard.py` & `wizproxy-0.5.0/wizproxy/core/shard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,158 +1,166 @@
 import itertools
 from functools import partial
-from typing import Generic, Optional, TypeVar
+from typing import Optional
 
 import trio
+from exceptiongroup import ExceptionGroup, catch
 from loguru import logger
 
-from .key_chain import KeyChain
-from .plugin import Context, Direction, PluginCollection
-from .proto import Bytes, Frame, SocketAddress
-from .session import Session
-from .stream import SessionStream
+from wizproxy.crypto import KeyChain
+from wizproxy.plugin import Context, Direction, PluginCollection
+from wizproxy.proto import Bytes, Frame, SocketAddress
+from wizproxy.session import ClientSig, Session
+from wizproxy.transport import FrameStream
 
-Request = TypeVar("Request")
-Response = TypeVar("Response")
+from .parcel import Parcel
 
 _DUMMY_ADDR = SocketAddress("0.0.0.0", 0)
 
 
-class Parcel(Generic[Request, Response]):
-    """
-    A parcel for request-response communication between a
-    :class:`Shard` and the proxy.
-    """
-
-    def __init__(self, data: Request):
-        self.data = data
-
-        tx, rx = trio.open_memory_channel(1)
-        self.sender = tx
-        self.receiver = rx
-
-    async def wait(self) -> Response:
-        return await self.receiver.receive()
-
-    def answer(self, response: Response):
-        self.sender.send_nowait(response)
-
-
 class Shard:
     """
     Representation of an individual server in the proxy.
 
     Each shard is bound to one specific game server and all clients
     that would normally connect to that server will connect to the
     shard instead.
 
     Shards are modeled as an actor system where the proxy supervises
-    each shard. Shard actors talk to the proxy to spawn more siblings,
-    as required during the processing of network packets.
+    each shard. Shard actors talk to the proxy to spawn siblings in
+    response to a connected client trying to switch servers.
 
     :param plugins: The globally registered proxy plugins.
     :param key_chain: The :class:`KeyChain` for asymmetric crypto.
+    :param client_sig: Optionally, a decrypted ClientSig if present.
     :param proxy_tx: The channel for sending commands to the supervisor.
     """
 
     def __init__(
         self,
         plugins: PluginCollection,
         key_chain: KeyChain,
+        client_sig: Optional[ClientSig],
         proxy_tx: trio.abc.SendChannel[Parcel[SocketAddress, SocketAddress]],
     ):
         self.plugins = plugins
         self.key_chain = key_chain
+        self.client_sig = client_sig
         self.proxy_tx = proxy_tx
 
-        self.addr = _DUMMY_ADDR
+        self.self_addr = _DUMMY_ADDR
+        self.remote_addr = _DUMMY_ADDR
 
         self._id_generator = itertools.count()
 
-    def socket(self) -> str:
-        return f"{self.addr.ip}:{self.addr.port}"
+    def __str__(self) -> str:
+        return str(self.self_addr)
 
-    async def _client_task(
+    async def tunnel(
         self,
+        direction: Direction,
         ctx: Context,
         stream: trio.SocketStream,
         peer: trio.SocketStream,
     ):
-        async for res in SessionStream(stream, ctx.session, True):
+        is_client = direction == Direction.CLIENT_TO_SERVER
+        session = ctx.session
+        buf = Bytes()
+
+        async for res in FrameStream(stream, session, is_client):
             encrypted, frame = res
 
-            bytes = Bytes(frame)
-            frame = Frame.read(bytes)
+            # Deserialize the next received frame.
+            buf.load_frame(frame)
+            frame = Frame.read(buf)
+
+            # Run all plugins on the frame and decide if it should be omitted.
+            if not await self.plugins.dispatch(direction, ctx, frame):
+                continue
+
+            # if the frame is marked dirty, re-serialize it.
+            # Otherwise, just reuse the original data we backed up.
+            if frame.dirty:
+                frame.write(buf)
+                raw = buf.getvalue()
+            else:
+                raw = frame.original
 
-            await self.plugins.dispatch(Direction.CLIENT_TO_SERVER, ctx, frame)
+            # Encrypt the frame data, if necessary.
+            if encrypted:
+                if is_client:
+                    raw = session.client_aes.encrypt(raw)
+                else:
+                    raw = session.server_aes.encrypt(raw)
 
-            frame.write(bytes)
-            frame = bytes.getvalue()
+            await peer.send_all(raw)
 
-            if encrypted:
-                frame = ctx.session.client_aes.encrypt(frame)  # type:ignore
+        buf.close()
 
-            await peer.send_all(frame)
+    async def _client_task(
+        self,
+        ctx: Context,
+        stream: trio.SocketStream,
+        peer: trio.SocketStream,
+    ):
+        await self.tunnel(Direction.CLIENT_TO_SERVER, ctx, stream, peer)
 
     async def _server_task(
         self,
         ctx: Context,
         stream: trio.SocketStream,
         peer: trio.SocketStream,
     ):
-        async for res in SessionStream(stream, ctx.session, False):
-            encrypted, frame = res
+        await self.tunnel(Direction.SERVER_TO_CLIENT, ctx, stream, peer)
 
-            bytes = Bytes(frame)
-            frame = Frame.read(bytes)
-
-            await self.plugins.dispatch(Direction.SERVER_TO_CLIENT, ctx, frame)
-
-            frame.write(bytes)
-            frame = bytes.getvalue()
-
-            if encrypted:
-                frame = ctx.session.server_aes.encrypt(frame)  # type:ignore
-
-            await peer.send_all(frame)
-
-    async def run(
-        self, host: Optional[str], nursery: trio.Nursery, remote: SocketAddress
+    async def start(
+        self,
+        host: Optional[str],
+        nursery: trio.Nursery,
+        remote: SocketAddress,
     ) -> SocketAddress:
         async def accept_tcp_client(stream: trio.SocketStream):
-            outward = await trio.open_tcp_stream(*remote)
+            outward = await trio.open_tcp_stream(remote.ip, remote.port)
+            client_sock = stream.socket.getsockname()
 
-            client = SocketAddress(*stream.socket.getsockname()[:2])  # type:ignore
+            client = SocketAddress(client_sock[0], client_sock[1])
             sid = next(self._id_generator)
-            session = Session(client, remote, sid, self.key_chain)
-
+            session = Session(client, remote, sid, self.key_chain, self.client_sig)
             context = Context(self, session)
 
-            logger.info(
-                f"[{self.socket()}] Client {sid} ({client.ip}:{client.port}) connected"
-            )
-
-            try:
-                async with trio.open_nursery() as nursery:
-                    nursery.start_soon(self._client_task, context, stream, outward)
-                    nursery.start_soon(self._server_task, context, outward, stream)
+            logger.info(f"[{self}] Client {sid} ({client}) connected")
 
-            except* trio.BrokenResourceError:
+            def broken_resource_handler(eg: ExceptionGroup):
                 # We were pranked by a client disconnecting unexpectedly.
                 # In that case, we shall just ignore it without bringing
                 # the whole shard down.
                 pass
 
-            except* ValueError as eg:
+            def too_slow_handler(eg: ExceptionGroup):
+                logger.info(f"[{self}] Client {sid} disconnected due to inactivity")
+
+            def value_error_handler(eg: ExceptionGroup):
                 # We received invalid data and can't continue processing.
                 for e in eg.exceptions:
-                    logger.error(f"[{self.socket()}] Client {sid} crashed: {e}")
+                    logger.error(f"[{self}] Client {sid} crashed: {e}")
 
-        # Port 0 makes the OS pick for us. So we need to remember the real socket
-        # address after the server has started.
+            with catch({
+                trio.BrokenResourceError: broken_resource_handler,
+                trio.TooSlowError: too_slow_handler,
+                ValueError: value_error_handler,
+            }):
+                async with trio.open_nursery() as nursery:
+                    nursery.start_soon(self._client_task, context, stream, outward)
+                    nursery.start_soon(self._server_task, context, outward, stream)
+
+        # Port 0 makes the OS pick for us. So we need to remember the
+        # assigned address after the server has started.
         serve_tcp = partial(trio.serve_tcp, host=host, handler_nursery=nursery)
         listeners = await nursery.start(serve_tcp, accept_tcp_client, 0)
-        self.addr = SocketAddress(*listeners[0].socket.getsockname()[:2])  # type:ignore
 
-        logger.info(f"[{self.socket()}] Spawning shard to {remote}...")
+        server_sock = listeners[0].socket.getsockname()
+        self.self_addr = SocketAddress(server_sock[0], server_sock[1])
+        self.remote_addr = remote
+
+        logger.info(f"[{self}] Spawning shard to {remote}..")
 
-        return self.addr
+        return self.self_addr
```

### Comparing `wizproxy-0.4.0/PKG-INFO` & `wizproxy-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: wizproxy
-Version: 0.4.0
+Version: 0.5.0
 Summary: A proxy for handling encrypted Wizard101 traffic
 License: ISC
 Author: Valentin B.
 Author-email: valentin.be@protonmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: exceptiongroup (>=1.1.3,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # wizproxy
```

