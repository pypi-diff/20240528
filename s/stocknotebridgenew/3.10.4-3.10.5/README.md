# Comparing `tmp/stocknotebridgenew-3.10.4.tar.gz` & `tmp/stocknotebridgenew-3.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-3.10.4.tar", last modified: Mon May 27 13:56:11 2024, max compression
+gzip compressed data, was "stocknotebridgenew-3.10.5.tar", last modified: Tue May 28 05:18:22 2024, max compression
```

## Comparing `stocknotebridgenew-3.10.4.tar` & `stocknotebridgenew-3.10.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-27 13:56:11.438347 stocknotebridgenew-3.10.4/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-27 13:56:11.438492 stocknotebridgenew-3.10.4/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-27 13:56:11.438712 stocknotebridgenew-3.10.4/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      913 2024-05-27 13:55:41.000000 stocknotebridgenew-3.10.4/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-27 13:56:11.436884 stocknotebridgenew-3.10.4/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-3.10.4/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   155146 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.4/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-27 13:56:11.438249 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-27 13:56:11.000000 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-27 13:56:11.000000 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-27 13:56:11.000000 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       43 2024-05-27 13:56:11.000000 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-27 13:56:11.000000 stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.664446 stocknotebridgenew-3.10.5/
+-rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/LICENSE
+-rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/MANIFEST.in
+-rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:18:22.664533 stocknotebridgenew-3.10.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/README.md
+-rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 05:18:22.664798 stocknotebridgenew-3.10.5/setup.cfg
+-rwxrwxrwx   0 root         (0) wheel        (0)      919 2024-05-28 05:18:09.000000 stocknotebridgenew-3.10.5/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.663036 stocknotebridgenew-3.10.5/snapi_py_client/
+-rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/__init__.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/api_client.py
+-rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-3.10.5/snapi_py_client/configuration.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/rest.py
+-rwxrwxrwx   0 root         (0) wheel        (0)   155146 2024-05-27 13:30:50.000000 stocknotebridgenew-3.10.5/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 05:18:22.664327 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)      818 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       47 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 05:18:22.000000 stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-3.10.4/LICENSE` & `stocknotebridgenew-3.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/PKG-INFO` & `stocknotebridgenew-3.10.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 3.10.4
+Version: 3.10.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-3.10.4/README.md` & `stocknotebridgenew-3.10.5/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/setup.py` & `stocknotebridgenew-3.10.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='3.10.4',
+version='3.10.5',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
-install_requires=['future', 'requests','websocket','websocket-client'],
+install_requires=['future', 'requests','websocket','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
 keywords = ['stocknote api', 'stocknote python sdk','samco api trading','samco algo trading', 'stock markets samco'],
 classifiers=[
     'Intended Audience :: Developers',
```

### Comparing `stocknotebridgenew-3.10.4/snapi_py_client/api_client.py` & `stocknotebridgenew-3.10.5/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/snapi_py_client/configuration.py` & `stocknotebridgenew-3.10.5/snapi_py_client/configuration.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/snapi_py_client/rest.py` & `stocknotebridgenew-3.10.5/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/snapi_py_client/snapi_bridge.py` & `stocknotebridgenew-3.10.5/snapi_py_client/snapi_bridge.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-3.10.4/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-3.10.5/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 3.10.4
+Version: 3.10.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

