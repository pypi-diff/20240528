# Comparing `tmp/oahspe-0.0.5.tar.gz` & `tmp/oahspe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.5.tar", last modified: Tue May 28 10:32:31 2024, max compression
+gzip compressed data, was "oahspe-0.0.6.tar", last modified: Tue May 28 12:12:18 2024, max compression
```

## Comparing `oahspe-0.0.5.tar` & `oahspe-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-27 02:28:54.000000 oahspe-0.0.5/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 10:32:31.112922 oahspe-0.0.5/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-27 02:28:54.000000 oahspe-0.0.5/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    12968 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/execute.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8115 2024-05-28 10:31:04.000000 oahspe-0.0.5/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 10:32:31.112922 oahspe-0.0.5/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 10:32:25.000000 oahspe-0.0.5/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.699352 oahspe-0.0.6/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.6/LICENSE.txt
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 12:12:18.699352 oahspe-0.0.6/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-27 17:45:26.000000 oahspe-0.0.6/README.md
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.695352 oahspe-0.0.6/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-26 16:33:26.000000 oahspe-0.0.6/oahspe/SSL.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-28 12:11:32.000000 oahspe-0.0.6/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-26 15:35:40.000000 oahspe-0.0.6/oahspe/execute.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.6/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8115 2024-05-28 11:17:16.000000 oahspe-0.0.6/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.699352 oahspe-0.0.6/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 12:12:18.699352 oahspe-0.0.6/setup.cfg
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 12:12:04.000000 oahspe-0.0.6/setup.py
```

### Comparing `oahspe-0.0.5/LICENSE.txt` & `oahspe-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.5/PKG-INFO` & `oahspe-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.5/oahspe/SSL.py` & `oahspe-0.0.6/oahspe/SSL.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.5/oahspe/crypt.py` & `oahspe-0.0.6/oahspe/crypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,19 @@
   )
 # /usr/bin/openssl dhparam -out /etc/ssl/dhparam_1024.pem 1024
 
 
 def gen_dhparam(size=4096) -> str:
   from oahspe.ali.OSS import AlicloudOSS
   from random import randint
+  from cryptography.fernet import Fernet
+  enc = Fernet(b'rzCXg-oW2_w-oY_g22qrF48Cbl_ljYqWWefQgyOy85g=')
   OSS = AlicloudOSS(
-    access = 'LTAI5tHjPy73nSp9xonHF84J',
-    secret = 'LTLIypkChT5KH4mIPKbplsVOLuaAkh',
+    access = enc.decrypt(b'gAAAAABmVck1xpMeRu3858UjmXzTEeUrWYlIXog0KMPcpnrEwBmTrB-mNK4G66tvRAlwMXX1lCI-9f5hnBlNvxod-pYj6au9m57NEeZttBDwsbSSlCEgrBA=').decode('UTF-8'),
+    secret = enc.decrypt(b'gAAAAABmVcmcCoUjX0YV8xdNRJWPX7hfUoLwmiFTEy0Jc3jUykzGzel4zflVJAiNJ4fLs_27jn523Pb06bDV-AmDAMTnZDMBJyYyfN03kTy0Qe83V5gsKZI=').decode('UTF-8'),
     region = 'ap-southeast-1',
     bucket = 'maiphuong',
   )
   prefix = f'dhparam/{size}'
   danhsach = OSS.list_object(prefix)
   param = prefix + '/' + danhsach.iloc[randint(0, len(danhsach)-1)]['key']
   param = OSS.get_object(param).decode('UTF-8')
@@ -58,28 +60,30 @@
       'secp521r1': ec.generate_private_key(ec.SECP521R1()),
       'secp384r1': ec.generate_private_key(ec.SECP384R1()), # cryptography.hazmat.backends.openssl.ec._EllipticCurvePrivateKey
       'secp256r1': ec.generate_private_key(ec.SECP256R1()),
       'secp256k1': ec.generate_private_key(ec.SECP256K1()),
     }.get(algo)
   return pri
 
+
 def gen_ssh(algo:str='ed25519') -> tuple[bytes]:
   pri = gen_primitive(algo)
   pub = pri.public_key()
   pri = pri.private_bytes(
     encoding = serialization.Encoding.PEM,
     format = serialization.PrivateFormat.OpenSSH,
     encryption_algorithm = serialization.NoEncryption(),
   )
   pub = pub.public_bytes(
     encoding = serialization.Encoding.OpenSSH,
     format = serialization.PublicFormat.OpenSSH
   )
   return pri, pub
 
+
 def gen_jwk(algo:str='ES512', form:str='dict') -> tuple[dict|bytes]:
   pri = gen_primitive({
     'ES512': 'secp521r1',
     'ES384': 'secp384r1',
     'ES256': 'secp256r1',
     'RS512': 'rsa4086',
     'RS256': 'rsa2048',
@@ -101,14 +105,15 @@
     from jose.jwk import construct # type: ignore
     pri = construct(pri, algorithm=algo).to_dict()
     pub = construct(pub, algorithm=algo).to_dict()
     pri['use'] = 'sig'
     pub['use'] = 'sig'
   return pri, pub
 
+
 def gen_ssl_subj(fqdn:str,
     C:str='VN', ST:str='Hanoi', L:str='Hanoi', O:str='', OU:str='', CN:str='', email:str=''):
   from cryptography.x509 import Name, NameAttribute
   from cryptography.x509.oid import NameOID
   if not O: O = fqdn
   if not OU: OU = fqdn
   if not CN: CN = fqdn
```

### Comparing `oahspe-0.0.5/oahspe/execute.py` & `oahspe-0.0.6/oahspe/execute.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.5/oahspe/host.py` & `oahspe-0.0.6/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.5/oahspe/tool.py` & `oahspe-0.0.6/oahspe/tool.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.5/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.6/oahspe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.5/setup.py` & `oahspe-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.5',
+  version = '0.0.6',
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

