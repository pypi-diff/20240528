# Comparing `tmp/pygrl-0.0.2.tar.gz` & `tmp/pygrl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrl-0.0.2.tar", last modified: Mon May 27 10:38:14 2024, max compression
+gzip compressed data, was "pygrl-0.0.3.tar", last modified: Tue May 28 02:58:34 2024, max compression
```

## Comparing `pygrl-0.0.2.tar` & `pygrl-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-27 07:20:34.000000 pygrl-0.0.2/LICENSE
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2559 2024-05-27 10:38:14.924838 pygrl-0.0.2/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1989 2024-05-27 10:35:53.000000 pygrl-0.0.2/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/pygrl/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1497 2024-05-27 10:34:31.000000 pygrl-0.0.2/pygrl/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      133 2024-05-27 09:32:59.000000 pygrl-0.0.2/pygrl/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    11703 2024-05-27 10:17:36.000000 pygrl-0.0.2/pygrl/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2139 2024-05-27 10:13:10.000000 pygrl-0.0.2/pygrl/storage.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/pygrl.egg-info/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2559 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      217 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        6 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-27 10:38:14.924838 pygrl-0.0.2/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      869 2024-05-27 10:38:10.000000 pygrl-0.0.2/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-28 02:58:34.211444 pygrl-0.0.3/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-27 07:20:34.000000 pygrl-0.0.3/LICENSE
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4198 2024-05-28 02:58:34.211444 pygrl-0.0.3/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3628 2024-05-28 02:51:05.000000 pygrl-0.0.3/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-28 02:58:34.211444 pygrl-0.0.3/pygrl/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1533 2024-05-28 01:32:30.000000 pygrl-0.0.3/pygrl/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      133 2024-05-27 09:32:59.000000 pygrl-0.0.3/pygrl/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     8093 2024-05-28 02:54:15.000000 pygrl-0.0.3/pygrl/main.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-28 02:58:34.211444 pygrl-0.0.3/pygrl/storage/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1384 2024-05-28 02:14:48.000000 pygrl-0.0.3/pygrl/storage/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      746 2024-05-28 02:31:16.000000 pygrl-0.0.3/pygrl/storage/basic_storage.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4862 2024-05-28 02:30:38.000000 pygrl-0.0.3/pygrl/storage/sqlite3_storage.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1446 2024-05-28 02:13:54.000000 pygrl-0.0.3/pygrl/storage/storage.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-28 02:58:34.211444 pygrl-0.0.3/pygrl.egg-info/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4198 2024-05-28 02:58:34.000000 pygrl-0.0.3/pygrl.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      315 2024-05-28 02:58:34.000000 pygrl-0.0.3/pygrl.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-28 02:58:34.000000 pygrl-0.0.3/pygrl.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        6 2024-05-28 02:58:34.000000 pygrl-0.0.3/pygrl.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-28 02:58:34.211444 pygrl-0.0.3/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      879 2024-05-28 02:36:15.000000 pygrl-0.0.3/setup.py
```

### Comparing `pygrl-0.0.2/LICENSE` & `pygrl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.2/pygrl/__init__.py` & `pygrl-0.0.3/pygrl/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 __title__ = "pygrl"
 __author__ = "Jonah Whaler"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2024 Jonah Whaler"
 
 from .main import GeneralRateLimiter, GeneralRateLimiter_with_Lock
-from .storage import BasicStorage, Storage
+from .storage import BasicStorage, Storage, SQLite3_Storage
 from .custom_exception import ExceededRateLimitError
 
 __all__ = [
     "GeneralRateLimiter",
     "GeneralRateLimiter_with_Lock",
-    "BasicStorage", "Storage",
+    "BasicStorage", "Storage", "SQLite3_Storage",
     "ExceededRateLimitError"
 ]
```

### Comparing `pygrl-0.0.2/setup.py` & `pygrl-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Another Python package aim to offer "Rate Limiting" functionality for general use cases.'
 
 # python3 setup.py sdist bdist_wheel
-# twine upload --skip-existing dist/*
+# twine upload --skip-existing dist/* --verbose
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 setup(
     name='pygrl',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

