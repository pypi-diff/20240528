# Comparing `tmp/stocknotebridgenew-4.0.4.tar.gz` & `tmp/stocknotebridgenew-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-4.0.4.tar", last modified: Tue May 28 06:22:39 2024, max compression
+gzip compressed data, was "stocknotebridgenew-4.0.5.tar", last modified: Tue May 28 06:29:02 2024, max compression
```

## Comparing `stocknotebridgenew-4.0.4.tar` & `stocknotebridgenew-4.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:22:39.174062 stocknotebridgenew-4.0.4/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 06:22:39.174126 stocknotebridgenew-4.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 06:22:39.174376 stocknotebridgenew-4.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      918 2024-05-28 06:22:21.000000 stocknotebridgenew-4.0.4/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:22:39.172683 stocknotebridgenew-4.0.4/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-4.0.4/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.4/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   236969 2024-05-28 06:22:15.000000 stocknotebridgenew-4.0.4/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:22:39.173961 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 06:22:39.000000 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 06:22:39.000000 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 06:22:39.000000 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       47 2024-05-28 06:22:39.000000 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 06:22:39.000000 stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:29:02.883220 stocknotebridgenew-4.0.5/
+-rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/LICENSE
+-rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 06:29:02.883284 stocknotebridgenew-4.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/README.md
+-rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 06:29:02.883547 stocknotebridgenew-4.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) wheel        (0)      918 2024-05-28 06:28:46.000000 stocknotebridgenew-4.0.5/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:29:02.881928 stocknotebridgenew-4.0.5/snapi_py_client/
+-rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/snapi_py_client/__init__.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/snapi_py_client/api_client.py
+-rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-4.0.5/snapi_py_client/configuration.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-4.0.5/snapi_py_client/rest.py
+-rwxrwxrwx   0 root         (0) wheel        (0)   236962 2024-05-28 06:27:52.000000 stocknotebridgenew-4.0.5/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 06:29:02.883117 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 06:29:02.000000 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 06:29:02.000000 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 06:29:02.000000 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       47 2024-05-28 06:29:02.000000 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 06:29:02.000000 stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-4.0.4/LICENSE` & `stocknotebridgenew-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-4.0.4/PKG-INFO` & `stocknotebridgenew-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 4.0.4
+Version: 4.0.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-4.0.4/README.md` & `stocknotebridgenew-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-4.0.4/setup.py` & `stocknotebridgenew-4.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='4.0.4',
+version='4.0.5',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
-install_requires=['future', 'requests','websocket','websocket_client','six'],
+install_requires=['future', 'requests','websocket','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
 keywords = ['stocknote api', 'stocknote python sdk','samco api trading','samco algo trading', 'stock markets samco'],
 classifiers=[
     'Intended Audience :: Developers',
```

### Comparing `stocknotebridgenew-4.0.4/snapi_py_client/api_client.py` & `stocknotebridgenew-4.0.5/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-4.0.4/snapi_py_client/configuration.py` & `stocknotebridgenew-4.0.5/snapi_py_client/configuration.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-4.0.4/snapi_py_client/rest.py` & `stocknotebridgenew-4.0.5/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-4.0.4/snapi_py_client/snapi_bridge.py` & `stocknotebridgenew-4.0.5/snapi_py_client/snapi_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 # import websocket
 from json import dumps
 
-from websocket.client import WebSocketApp
+from websocket import WebSocketApp
 
 from snapi_py_client.api_client import ApiClient
 
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
```

### Comparing `stocknotebridgenew-4.0.4/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-4.0.5/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 4.0.4
+Version: 4.0.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

