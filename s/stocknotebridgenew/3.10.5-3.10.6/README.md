# Comparing `tmp/stocknotebridgenew-3.10.5.tar.gz` & `tmp/stocknotebridgenew-3.10.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-3.10.5.tar", last modified: Tue May 28 05:18:22 2024, max compression
+gzip compressed data, was "stocknotebridgenew-3.10.6.tar", last modified: Tue May 28 05:36:47 2024, max compression
```

## Comparing `stocknotebridgenew-3.10.5.tar` & `stocknotebridgenew-3.10.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.664446 stocknotebridgenew-3.10.5/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:18:22.664533 stocknotebridgenew-3.10.5/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 05:18:22.664798 stocknotebridgenew-3.10.5/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      919 2024-05-28 05:18:09.000000 stocknotebridgenew-3.10.5/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.663036 stocknotebridgenew-3.10.5/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-3.10.5/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   155146 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.664327 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       47 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:36:47.828519 stocknotebridgenew-3.10.6/
+-rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/LICENSE
+-rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/MANIFEST.in
+-rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:36:47.828581 stocknotebridgenew-3.10.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/README.md
+-rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 05:36:47.828812 stocknotebridgenew-3.10.6/setup.cfg
+-rwxrwxrwx   0 root         (0) wheel        (0)      919 2024-05-28 05:33:58.000000 stocknotebridgenew-3.10.6/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:36:47.827268 stocknotebridgenew-3.10.6/snapi_py_client/
+-rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/snapi_py_client/__init__.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/snapi_py_client/api_client.py
+-rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-3.10.6/snapi_py_client/configuration.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.6/snapi_py_client/rest.py
+-rwxrwxrwx   0 root         (0) wheel        (0)   236960 2024-05-28 05:33:46.000000 stocknotebridgenew-3.10.6/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:36:47.828407 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:36:47.000000 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 05:36:47.000000 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 05:36:47.000000 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       47 2024-05-28 05:36:47.000000 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 05:36:47.000000 stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-3.10.5/LICENSE` & `stocknotebridgenew-3.10.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.5/PKG-INFO` & `stocknotebridgenew-3.10.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 3.10.5
+Version: 3.10.6
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-3.10.5/README.md` & `stocknotebridgenew-3.10.6/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.5/setup.py` & `stocknotebridgenew-3.10.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='3.10.5',
+version='3.10.6',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
 install_requires=['future', 'requests','websocket','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
```

### Comparing `stocknotebridgenew-3.10.5/snapi_py_client/api_client.py` & `stocknotebridgenew-3.10.6/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.5/snapi_py_client/configuration.py` & `stocknotebridgenew-3.10.6/snapi_py_client/configuration.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.5/snapi_py_client/rest.py` & `stocknotebridgenew-3.10.6/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-3.10.6/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 3.10.5
+Version: 3.10.6
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

