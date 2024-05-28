# Comparing `tmp/cpyvpn-1.6.1.tar.gz` & `tmp/cpyvpn-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpyvpn-1.6.1.tar", last modified: Mon Jul 17 09:06:01 2023, max compression
+gzip compressed data, was "cpyvpn-1.6.2.tar", last modified: Tue May 28 10:43:35 2024, max compression
```

## Comparing `cpyvpn-1.6.1.tar` & `cpyvpn-1.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/
--rw-r--r--   0 nick      (1000) nick      (1000)      400 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)    35147 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/LICENSE-GPLv3
--rw-r--r--   0 nick      (1000) nick      (1000)       52 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     8423 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     7432 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/README.md
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.236914 cpyvpn-1.6.1/cpyvpn/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      176 2023-07-17 09:06:00.000000 cpyvpn-1.6.1/cpyvpn/__version__.py
--rw-r--r--   0 nick      (1000) nick      (1000)    24527 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/appdirs.py
--rw-r--r--   0 nick      (1000) nick      (1000)    15413 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/auth.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4804 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/cfg.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16821 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6742 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/crt.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3454 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/cui.py
--rw-r--r--   0 nick      (1000) nick      (1000)    23744 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/ma.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4037 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/rsa.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1029 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/snx.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.237914 cpyvpn-1.6.1/cpyvpn/srv/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.239914 cpyvpn-1.6.1/cpyvpn/srv/data/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cert.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cl_cert.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/cl_key.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/key.pem
--rw-r--r--   0 nick      (1000) nick      (1000)     7998 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/srv/data/rr.js
--rw-r--r--   0 nick      (1000) nick      (1000)     1242 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/data/rsa.keys
--rw-r--r--   0 nick      (1000) nick      (1000)    28150 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/srv/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4615 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/ssl_ctx.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2724 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/cpyvpn/trutils.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9587 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/utils.py
--rw-r--r--   0 nick      (1000) nick      (1000)    14263 2023-07-17 09:01:15.000000 cpyvpn-1.6.1/cpyvpn/vna.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-07-17 09:06:01.237914 cpyvpn-1.6.1/cpyvpn.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     8423 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      695 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       71 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        7 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/top_level.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-07-17 09:06:01.000000 cpyvpn-1.6.1/cpyvpn.egg-info/zip-safe
--rw-r--r--   0 nick      (1000) nick      (1000)      171 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1104 2023-07-17 09:06:01.240914 cpyvpn-1.6.1/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)     1756 2023-03-24 10:17:25.000000 cpyvpn-1.6.1/setup.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:43:35.339851 cpyvpn-1.6.2/
+-rw-r--r--   0 nick      (1000) nick      (1000)      400 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)    35147 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/LICENSE-GPLv3
+-rw-r--r--   0 nick      (1000) nick      (1000)       52 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     9055 2024-05-28 10:43:35.339851 cpyvpn-1.6.2/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     8064 2024-01-03 09:38:31.000000 cpyvpn-1.6.2/README.md
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:43:35.335851 cpyvpn-1.6.2/cpyvpn/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      176 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn/__version__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    24527 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/appdirs.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16247 2024-05-28 10:03:59.000000 cpyvpn-1.6.2/cpyvpn/auth.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4804 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/cfg.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16689 2024-05-16 10:27:52.000000 cpyvpn-1.6.2/cpyvpn/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6742 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/crt.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3454 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/cui.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    23744 2023-07-17 09:01:15.000000 cpyvpn-1.6.2/cpyvpn/ma.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4037 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/rsa.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1029 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/snx.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:43:35.337851 cpyvpn-1.6.2/cpyvpn/srv/
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:43:35.338851 cpyvpn-1.6.2/cpyvpn/srv/data/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/cert.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1326 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/cl_cert.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/cl_key.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     1704 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/key.pem
+-rw-r--r--   0 nick      (1000) nick      (1000)     9452 2024-01-03 09:38:31.000000 cpyvpn-1.6.2/cpyvpn/srv/data/rr.js
+-rw-r--r--   0 nick      (1000) nick      (1000)     1242 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/srv/data/rsa.keys
+-rw-r--r--   0 nick      (1000) nick      (1000)    28205 2024-01-03 09:38:31.000000 cpyvpn-1.6.2/cpyvpn/srv/server.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4764 2024-05-28 10:03:59.000000 cpyvpn-1.6.2/cpyvpn/ssl_ctx.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2724 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/cpyvpn/trutils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9587 2023-07-17 09:01:15.000000 cpyvpn-1.6.2/cpyvpn/utils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    14563 2024-05-19 15:42:47.000000 cpyvpn-1.6.2/cpyvpn/vna.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:43:35.339851 cpyvpn-1.6.2/cpyvpn.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     9055 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)      695 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       71 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        7 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/top_level.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-05-28 10:43:35.000000 cpyvpn-1.6.2/cpyvpn.egg-info/zip-safe
+-rw-r--r--   0 nick      (1000) nick      (1000)      171 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1104 2024-05-28 10:43:35.340851 cpyvpn-1.6.2/setup.cfg
+-rw-r--r--   0 nick      (1000) nick      (1000)     1756 2023-03-24 10:17:25.000000 cpyvpn-1.6.2/setup.py
```

### Comparing `cpyvpn-1.6.1/LICENSE-GPLv3` & `cpyvpn-1.6.2/LICENSE-GPLv3`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/PKG-INFO` & `cpyvpn-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpyvpn
-Version: 1.6.1
+Version: 1.6.2
 Summary: Check Point VPN client written in Python.
 Home-page: https://gitlab.com/cpvpn/cpyvpn
 Author: Nikolay A. Krylov
 Author-email: krylovna@gmail.com
 License: GPL3
 Project-URL: PyPI, https://pypi.org/project/cpyvpn
 Project-URL: Source, https://gitlab.com/cpvpn/cpyvpn
@@ -159,14 +159,17 @@
 
 * Certificate renewal:
 
     `cp_client --rc new_cert.p12 -c ./cert.p12 vpn.example.org`
 
     Conversion notes applies here likewise.
 
+# RSA SecurID as a first login factor
+In case you have a hardware device with permanent 6 digit PIN plus 60s expiring TOKEN and first authentication factor configured as `factor_type (securid)` and `securid_card_type (any)` (this info is inside the debug log here: `CCCserverResponse -> ResponseData -> login_options_data -> login_options_list -> [option index] -> factors -> 0`) some adjustments are needed. You have to either explicitly select authorization mode (`-m k`) or concatenate TOKEN and PIN to form proper password/passcode. E.g. if your TOKEN is 0011...eeff and PIN is 123456, then your passcode is 0011...eeff123456.
+
 # Performance
 Python incurs extra overhead and the maximum bitrate will be 2-3 times lower than the bitrate achievable with the native client or openconnect. However it will only be noticable when the link speed is >100MB/s.
 
 # Known Issues
 * Early R81 gateway versions were 'enhanced' in a way affecting user experience. One of the enhancements (or a bug) prevents multiple tunnel initializations from the same Web Portal session. Any client doing second connection attempt just hangs.
 In this case either logout manually after each cp_client run, use cpga logout or add --force_logout to perform automatic signout after tunnel shutdown to workaround this issue.
```

### Comparing `cpyvpn-1.6.1/README.md` & `cpyvpn-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,17 @@
 
 * Certificate renewal:
 
     `cp_client --rc new_cert.p12 -c ./cert.p12 vpn.example.org`
 
     Conversion notes applies here likewise.
 
+# RSA SecurID as a first login factor
+In case you have a hardware device with permanent 6 digit PIN plus 60s expiring TOKEN and first authentication factor configured as `factor_type (securid)` and `securid_card_type (any)` (this info is inside the debug log here: `CCCserverResponse -> ResponseData -> login_options_data -> login_options_list -> [option index] -> factors -> 0`) some adjustments are needed. You have to either explicitly select authorization mode (`-m k`) or concatenate TOKEN and PIN to form proper password/passcode. E.g. if your TOKEN is 0011...eeff and PIN is 123456, then your passcode is 0011...eeff123456.
+
 # Performance
 Python incurs extra overhead and the maximum bitrate will be 2-3 times lower than the bitrate achievable with the native client or openconnect. However it will only be noticable when the link speed is >100MB/s.
 
 # Known Issues
 * Early R81 gateway versions were 'enhanced' in a way affecting user experience. One of the enhancements (or a bug) prevents multiple tunnel initializations from the same Web Portal session. Any client doing second connection attempt just hangs.
 In this case either logout manually after each cp_client run, use cpga logout or add --force_logout to perform automatic signout after tunnel shutdown to workaround this issue.
```

### Comparing `cpyvpn-1.6.1/cpyvpn/appdirs.py` & `cpyvpn-1.6.2/cpyvpn/appdirs.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/auth.py` & `cpyvpn-1.6.2/cpyvpn/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # Created on 02.12.2020
 # Copyright © 2020-2021 Nick Krylov.
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import re
 import json
+import uuid
+import hashlib
 import urllib
 import secrets
 import datetime
 import logging
 
 from . import utils, ssl_ctx
 from .cfg import CPRR
@@ -103,24 +105,40 @@
               }
               }).serialize()[:-1]
         logger.info("Cert. login")
         ssl_ctx.require_user_cert()
         return self._extract_ac(self.url + self.cert_path, body)
 
     def do_login(self):
-
+        hnode = hashlib.md5(hex(uuid.getnode()).encode()).hexdigest()
+        dev_id = uuid.uuid5(uuid.NAMESPACE_OID, hnode)
+        ctx = ssl_ctx.get_ssl_context()
         logger.info("Standard login")
         body = CPRR({"CCCclientRequest":
               {"RequestHeader":{
                   "id":2,
                   "type":"UserPass",
                   "session_id":""
                   },
               "RequestData":{
                   "client_type":self.ct,
+                  "client_logging_data":{
+                      "client_name":"\"Mobile VPN\"",
+                      "client_ver":"\"1.601.29\"",
+                      "client_build_number":"\"29\"",
+                      "os_name":"\"Android\"",
+                      "os_version":"\"13\"",
+                      "device_type":"",
+                      "hardware_model":ctx.hostname,
+                      "machine_name":ctx.hostname,
+                      "device_id":str(dev_id),
+                      "mac_address":"",
+                      "physical_ip":ctx.client_ip,
+                      "is_compliant":"\"N/A\""
+                  },
                   "username":enc(self.login),
                   "password":enc(self.pwd),
                   "selectedLoginOption":self._logopt
                   }
               }
               }).serialize()[:-1]
 
@@ -381,16 +399,16 @@
                     pwd = optpwd
                 else:
                     if mode == "l":
                         qpwd = self.ui.ask_pwd(pwd_prompt)
                     elif mode == "p":
                         qpwd = self.ui.ask_pwd("Passcode")
                     elif mode == "k":
-                        qpwd = self.ui.ask_pwd("PIN")
-                        qpwd2 = self.ui.ask_pwd("Tokencode")
+                        qpwd = self.ui.ask_pwd("Tokencode")
+                        qpwd2 = self.ui.ask_pwd("PIN")
                     elif mode in ["h", "u"]:  # TODO: check username_only on Capsule!
                         pwd = ""
                     else:
                         raise Exception("Bad mode!")
 
                 vals = self.ui.wait_input([v for v in [qlogin, qpwd, qpwd2] if v is not None])
                 if qlogin is not None:
```

### Comparing `cpyvpn-1.6.1/cpyvpn/cfg.py` & `cpyvpn-1.6.2/cpyvpn/cfg.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/client.py` & `cpyvpn-1.6.2/cpyvpn/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,21 +212,19 @@
 
     def send_vna_packet(self):
         data = self.vna.tundev().read()
         if data is not None:
             self.send_packet(data)
 
     def on_connection_lost(self, exc):
+        self.evt.set()
         if exc is None:
             self.reconnect = True
-        else:
-            logger.error("Exception occured in the event loop!\n{}".format("".join(traceback.format_exception(exc))))
         if self._ka_handle:
             self._ka_handle.cancel()
-        self.evt.set()
 
 
 class PidFile:
 
     def __init__(self, name):
         self.name = name
```

### Comparing `cpyvpn-1.6.1/cpyvpn/crt.py` & `cpyvpn-1.6.2/cpyvpn/crt.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/cui.py` & `cpyvpn-1.6.2/cpyvpn/cui.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/ma.py` & `cpyvpn-1.6.2/cpyvpn/ma.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/rsa.py` & `cpyvpn-1.6.2/cpyvpn/rsa.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/snx.py` & `cpyvpn-1.6.2/cpyvpn/snx.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/cert.pem` & `cpyvpn-1.6.2/cpyvpn/srv/data/cert.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/cl_cert.pem` & `cpyvpn-1.6.2/cpyvpn/srv/data/cl_cert.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/cl_key.pem` & `cpyvpn-1.6.2/cpyvpn/srv/data/cl_key.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/key.pem` & `cpyvpn-1.6.2/cpyvpn/srv/data/key.pem`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/rr.js` & `cpyvpn-1.6.2/cpyvpn/srv/data/rr.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -63,27 +63,27 @@
                                         "username": "\"User name\"",
                                         "password": "Password"
                                     }
                                 }
                             }
                         },
                         "1": {
-                            "id": "vpn2",
+                            "id": "vpn_RSA_SecurID",
                             "secondary_realm_hash": "00112233445566778899aabbccddeeff",
-                            "display_name": "Legacy",
+                            "display_name": "RSA SecurID",
                             "show_realm": 1,
                             "factors": {
                                 "0": {
-                                    "factor_type": "password",
-                                    "securid_card_type": "",
+                                    "factor_type": "securid",
+                                    "securid_card_type": "keyfob",
                                     "certificate_storage_type": "",
                                     "custom_display_labels": {
-                                        "header": "\"1Please provide your credentials\"",
-                                        "username": "\"Login\"",
-                                        "password": "Password"
+                                        "header": "\"Please provide your credentials\"",
+                                        "username": "\"User name\"",
+                                        "password": "\"RSA Passcode\""
                                     }
                                 }
                             }
                         },
                         "2": {
                             "id": "vpn_cert",
                             "secondary_realm_hash": "00112233445566778899aabbccddeeff",
```

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/data/rsa.keys` & `cpyvpn-1.6.2/cpyvpn/srv/data/rsa.keys`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/srv/server.py` & `cpyvpn-1.6.2/cpyvpn/srv/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,15 @@
         p = auth.dec(rq.find("password"))
         opts = self.opts
 
         s, ak = self._gen_session()
 
         ou, op = opts.user, opts.pwd
         auth_variants = set(((ou, op), (ou, ""), (ou, op + opts.otp)))
+        logger.debug("user: {}, pwd: {}".format(u, p))
 
         rd = resp.find("ResponseData")
         if (u, p) in auth_variants:
             rd["active_key"] = ak
             rd["session_id"] = s.sid
         else:
             for k in list(rd.keys()):
```

### Comparing `cpyvpn-1.6.1/cpyvpn/ssl_ctx.py` & `cpyvpn-1.6.2/cpyvpn/ssl_ctx.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
     context = __ssl_cont__
     if __ssl_strict__:
         context.verify_mode = ssl.CERT_REQUIRED
     else:
         context.check_hostname = False
         context.verify_mode = ssl.CERT_NONE
+    context.client_ip = ""
+    context.hostname = ""
     return context
 
 
 # Build pem cache if does not exist
 def _make_pem():
 
     if os.access(cached_pem, os.F_OK):
@@ -126,14 +128,16 @@
     cert = ssl.get_server_certificate(addr)
     _fetch_all(_get_aia(ssl.PEM_cert_to_DER_cert(cert)))
 
 
 def _test_wrap(host, port):
     with closing(socket.create_connection((host, port))) as sock:
         context = get_ssl_context()
+        context.client_ip = sock.getsockname()
+        context.hostname = socket.gethostname()
         context.wrap_socket(sock, server_hostname=host)
 
 
 def check_ssl_mode(host, port, nocert):
 
         ssl_strict = True
         logger.info("Checking SSL mode.")
@@ -149,10 +153,11 @@
                     _resolve_cert_chain((host, port))
                     _test_wrap(host, port)
                 else:
                     ssl_strict = False
         set_ssl_strict_mode(ssl_strict)
         logger.info("SSL mode is: {}.".format("strict" if ssl_strict else "permissive"))
 
+
 def require_user_cert():
     if not get_ssl_context().has_user_cert:
         raise RuntimeError("Certificate-based login mode selected, but user certificate is not set! Use '-c' option.")
```

### Comparing `cpyvpn-1.6.1/cpyvpn/trutils.py` & `cpyvpn-1.6.2/cpyvpn/trutils.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/utils.py` & `cpyvpn-1.6.2/cpyvpn/utils.py`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/cpyvpn/vna.py` & `cpyvpn-1.6.2/cpyvpn/vna.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,17 +162,16 @@
 
     def fileno(self):
         return self.fd
 
     def close(self):
         self.f.close()
 
-# Use  Network Manager to setup tun in user mode (without root)
-# https://mail.gnome.org/archives/networkmanager-list/2016-January/msg00053.html
-
+class VNAUnavailable(Exception):
+    pass
 
 class VNABase(object):
 
     def __init__(self, up_on_init=False):
         self.addr = None
         self.is_up = up_on_init
 
@@ -219,21 +218,26 @@
 
 __def_snx_name__ = "snxtun"
 
 STDOUT = subprocess.STDOUT
 PIPE = subprocess.PIPE
 DEVNULL = subprocess.DEVNULL
 
+# Use  Network Manager to setup tun in user mode (without root)
+# https://mail.gnome.org/archives/networkmanager-list/2016-January/msg00053.html
 
 class VNANM(VNABase):
 
     @staticmethod
     def run_nmcli(cmd, opt=[]):
         cmd = ["nmcli", "-c", "no", "-t"] + opt + ["c"] + cmd
-        ret = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, check=True)
+        try:
+            ret = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, check=True)
+        except subprocess.CalledProcessError as e:
+            raise RuntimeError("nmcli failed with retcode={}. Error message: {}".format(e.returncode, e.stderr)) from None
         return ret.stdout
 
     @staticmethod
     def gen_ranges(ip_min, ip_max):
         mask32 = 0xffffffff
         ret = []
         ip = ip_min
@@ -251,14 +255,18 @@
                     break
             ret.append((utils.ipint2str(ip), 32 - mask.bit_length(), utils.ipint2str(~mask & mask32)))
             ip += mask + 1
         return ret
 
     def __init__(self, args):
         super(VNANM, self).__init__()
+        try:
+            self.run_nmcli([])
+        except:
+            raise VNAUnavailable()
         self.name = name = args.get("interface", __def_snx_name__)
         self.tun = tun = args.get("tun", True)
         self.nopi = nopi = args.get("nopi", True)
         self.mtu = mtu = args.get("mtu", 1500)
 
         uid = os.getuid()
         newtun = True
@@ -274,15 +282,15 @@
                     if uid == tunuid:
                         newtun = False
                         break
         if newtun:
             if ntun != 0:
                 self.run_nmcli(["del" , self.name ])
             self.run_nmcli(["add", "type", "tun", "ifname", name, "con-name", name , "mode", "tun" if tun else "tap", "tun.pi", "no" if nopi else "yes",
-                       "owner", str(uid), "autoconnect", "no", "ip4", "0.0.0.0"])
+                       "owner", str(uid), "autoconnect", "no", "ip4", "192.0.0.8"])
         self.set_mtu(mtu)
 
         self.run_nmcli(["up" , self.name ])
         self._init_dev()
         self.down()
 
     def _init_dev(self):
@@ -326,15 +334,15 @@
 
 
 class VNAVPNC(VNABase):
 
     def __init__(self, args):
         self._vpnc = args.get("script")
         if not self._vpnc:
-            raise RuntimeError("vpnc script name not set!")
+            raise VNAUnavailable()
         super(VNAVPNC, self).__init__()
         self._uid = args.get("uid")  # !
         defname = args.get("interface", __def_snx_name__)
         self._env = {"VPNPID":str(os.getpid()), "TUNDEV":defname, "INTERNAL_IP4_MTU":"1500"}
 
         self.run_vpnc("pre-init")
 
@@ -438,15 +446,15 @@
 
 class VNAProxy(VNABase):
 
     def __init__(self, args):
         super(VNAProxy, self).__init__()
         self._script = args.get("script_tun")
         if not self._script:
-            raise RuntimeError("Script name not set")
+            raise VNAUnavailable()
 
         self.dev = SocketPairDev()
         self._dns = ""
         self._sc_proc = None
         self.mtu = args.get("mtu", 1500)
 
     def set_mtu(self, mtu):
@@ -493,14 +501,14 @@
     if args.get("null_vna"):
         cls_list = [VNANull]
     inst = None
     for cls in cls_list:
         try:
             inst = cls(args)
             break
-        except:
+        except VNAUnavailable:
             pass
     if isinstance(inst, VNANull):
         logger.warning("Initializing null VNA for debugging. Network packet transfer won't be available.")
     if inst is None:
         raise RuntimeError("VNA initialisation failed! Check your -s/-S option, make sure Network Manager can handle TUN interfaces, use --null_vna hidden option.")
     return inst
```

### Comparing `cpyvpn-1.6.1/cpyvpn.egg-info/PKG-INFO` & `cpyvpn-1.6.2/cpyvpn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpyvpn
-Version: 1.6.1
+Version: 1.6.2
 Summary: Check Point VPN client written in Python.
 Home-page: https://gitlab.com/cpvpn/cpyvpn
 Author: Nikolay A. Krylov
 Author-email: krylovna@gmail.com
 License: GPL3
 Project-URL: PyPI, https://pypi.org/project/cpyvpn
 Project-URL: Source, https://gitlab.com/cpvpn/cpyvpn
@@ -159,14 +159,17 @@
 
 * Certificate renewal:
 
     `cp_client --rc new_cert.p12 -c ./cert.p12 vpn.example.org`
 
     Conversion notes applies here likewise.
 
+# RSA SecurID as a first login factor
+In case you have a hardware device with permanent 6 digit PIN plus 60s expiring TOKEN and first authentication factor configured as `factor_type (securid)` and `securid_card_type (any)` (this info is inside the debug log here: `CCCserverResponse -> ResponseData -> login_options_data -> login_options_list -> [option index] -> factors -> 0`) some adjustments are needed. You have to either explicitly select authorization mode (`-m k`) or concatenate TOKEN and PIN to form proper password/passcode. E.g. if your TOKEN is 0011...eeff and PIN is 123456, then your passcode is 0011...eeff123456.
+
 # Performance
 Python incurs extra overhead and the maximum bitrate will be 2-3 times lower than the bitrate achievable with the native client or openconnect. However it will only be noticable when the link speed is >100MB/s.
 
 # Known Issues
 * Early R81 gateway versions were 'enhanced' in a way affecting user experience. One of the enhancements (or a bug) prevents multiple tunnel initializations from the same Web Portal session. Any client doing second connection attempt just hangs.
 In this case either logout manually after each cp_client run, use cpga logout or add --force_logout to perform automatic signout after tunnel shutdown to workaround this issue.
```

### Comparing `cpyvpn-1.6.1/cpyvpn.egg-info/SOURCES.txt` & `cpyvpn-1.6.2/cpyvpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/setup.cfg` & `cpyvpn-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cpyvpn-1.6.1/setup.py` & `cpyvpn-1.6.2/setup.py`

 * *Files identical despite different names*

