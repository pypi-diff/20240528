# Comparing `tmp/oahspe-0.0.4.tar.gz` & `tmp/oahspe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.4.tar", last modified: Sun May 26 15:39:09 2024, max compression
+gzip compressed data, was "oahspe-0.0.5.tar", last modified: Tue May 28 10:32:31 2024, max compression
```

## Comparing `oahspe-0.0.4.tar` & `oahspe-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 15:39:09.055666 oahspe-0.0.4/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.4/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 15:39:09.055666 oahspe-0.0.4/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-26 13:43:14.000000 oahspe-0.0.4/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 15:39:09.055666 oahspe-0.0.4/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3840 2024-05-26 13:20:10.000000 oahspe-0.0.4/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    12967 2024-05-26 13:20:10.000000 oahspe-0.0.4/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-26 15:35:40.000000 oahspe-0.0.4/oahspe/execute.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.4/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     4648 2024-05-26 13:20:10.000000 oahspe-0.0.4/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 15:39:09.055666 oahspe-0.0.4/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 15:39:09.000000 oahspe-0.0.4/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      238 2024-05-26 15:39:09.000000 oahspe-0.0.4/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-26 15:39:09.000000 oahspe-0.0.4/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-26 15:39:09.000000 oahspe-0.0.4/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-26 15:39:09.055666 oahspe-0.0.4/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-26 15:39:04.000000 oahspe-0.0.4/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-27 02:28:54.000000 oahspe-0.0.5/LICENSE.txt
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 10:32:31.112922 oahspe-0.0.5/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-27 02:28:54.000000 oahspe-0.0.5/README.md
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/SSL.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    12968 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/execute.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-27 02:28:54.000000 oahspe-0.0.5/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8115 2024-05-28 10:31:04.000000 oahspe-0.0.5/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 10:32:31.112922 oahspe-0.0.5/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 10:32:31.000000 oahspe-0.0.5/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 10:32:31.112922 oahspe-0.0.5/setup.cfg
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 10:32:25.000000 oahspe-0.0.5/setup.py
```

### Comparing `oahspe-0.0.4/LICENSE.txt` & `oahspe-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.4/PKG-INFO` & `oahspe-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.4/oahspe/SSL.py` & `oahspe-0.0.5/oahspe/SSL.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
       bucket = bucket,
     )
     self.cas = AlicloudCAS(
       access = access,
       secret = secret,
       region = region,
     )
+
   
 
   def list_domain(self):
     danhsach = []
     for cert in self.oss.list_object('ssl')['prefix'].unique():
       cert = cert[4:].split('/')
       if len(cert) == 2 and cert[0] == self.domain:
```

### Comparing `oahspe-0.0.4/oahspe/crypt.py` & `oahspe-0.0.5/oahspe/crypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   from cryptography.hazmat.primitives.asymmetric import dh
   return dh.generate_parameters(generator=2, key_size=size).parameter_bytes(
     encoding=serialization.Encoding.PEM,
     format=serialization.ParameterFormat.PKCS3
   )
 # /usr/bin/openssl dhparam -out /etc/ssl/dhparam_1024.pem 1024
 
+
 def gen_dhparam(size=4096) -> str:
   from oahspe.ali.OSS import AlicloudOSS
   from random import randint
   OSS = AlicloudOSS(
     access = 'LTAI5tHjPy73nSp9xonHF84J',
     secret = 'LTLIypkChT5KH4mIPKbplsVOLuaAkh',
     region = 'ap-southeast-1',
```

### Comparing `oahspe-0.0.4/oahspe/execute.py` & `oahspe-0.0.5/oahspe/execute.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.4/oahspe/host.py` & `oahspe-0.0.5/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.4/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.5/oahspe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.4/setup.py` & `oahspe-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.4',
+  version = '0.0.5',
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

