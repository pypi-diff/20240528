# Comparing `tmp/pyobjc-framework-DictionaryServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-DictionaryServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DictionaryServices-9.1b1.tar", last modified: Sun Mar 26 11:23:11 2023, max compression
+gzip compressed data, was "pyobjc-framework-DictionaryServices-9.2.tar", last modified: Wed Jun  7 00:13:16 2023, max compression
```

## Comparing `pyobjc-framework-DictionaryServices-9.1b1.tar` & `pyobjc-framework-DictionaryServices-9.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:11.960977 pyobjc-framework-DictionaryServices-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DictionaryServices-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:11.949346 pyobjc-framework-DictionaryServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:11.953237 pyobjc-framework-DictionaryServices-9.1b1/Lib/DictionaryServices/
--rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/DictionaryServices/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:11.957019 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     1981 2023-03-26 11:23:11.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      531 2023-03-26 11:23:11.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:11.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:08.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:23:11.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:23:11.000000 pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1770 2023-03-26 11:23:11.959516 pyobjc-framework-DictionaryServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:11.958719 pyobjc-framework-DictionaryServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1028 2022-04-11 08:03:15.000000 pyobjc-framework-DictionaryServices-9.1b1/PyObjCTest/test_dictionaryservices.py
--rw-r--r--   0 ronald     (501) staff       (20)      295 2021-10-18 19:38:40.000000 pyobjc-framework-DictionaryServices-9.1b1/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DictionaryServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:11.961107 pyobjc-framework-DictionaryServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      541 2023-03-25 14:20:31.000000 pyobjc-framework-DictionaryServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:16.310221 pyobjc-framework-DictionaryServices-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DictionaryServices-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:16.300136 pyobjc-framework-DictionaryServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:16.304517 pyobjc-framework-DictionaryServices-9.2/Lib/DictionaryServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.2/Lib/DictionaryServices/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:16.307945 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     1979 2023-06-07 00:13:16.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      546 2023-06-07 00:13:16.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:16.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:08.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:13:16.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-06-07 00:13:16.000000 pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1768 2023-06-07 00:13:16.309820 pyobjc-framework-DictionaryServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:16.309107 pyobjc-framework-DictionaryServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-DictionaryServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1028 2022-04-11 08:03:15.000000 pyobjc-framework-DictionaryServices-9.2/PyObjCTest/test_dictionaryservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)      295 2021-10-18 19:38:40.000000 pyobjc-framework-DictionaryServices-9.2/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DictionaryServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DictionaryServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:16.310343 pyobjc-framework-DictionaryServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      623 2023-05-29 10:07:46.000000 pyobjc-framework-DictionaryServices-9.2/setup.py
```

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/LICENSE.txt` & `pyobjc-framework-DictionaryServices-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/Lib/DictionaryServices/__init__.py` & `pyobjc-framework-DictionaryServices-9.2/Lib/DictionaryServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/PKG-INFO` & `pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DictionaryServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DictionaryServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DictionaryServices
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/Lib/pyobjc_framework_DictionaryServices.egg-info/SOURCES.txt` & `pyobjc-framework-DictionaryServices-9.2/Lib/pyobjc_framework_DictionaryServices.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/DictionaryServices/__init__.py
 Lib/pyobjc_framework_DictionaryServices.egg-info/PKG-INFO
 Lib/pyobjc_framework_DictionaryServices.egg-info/SOURCES.txt
 Lib/pyobjc_framework_DictionaryServices.egg-info/dependency_links.txt
 Lib/pyobjc_framework_DictionaryServices.egg-info/not-zip-safe
 Lib/pyobjc_framework_DictionaryServices.egg-info/requires.txt
```

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/PKG-INFO` & `pyobjc-framework-DictionaryServices-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DictionaryServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DictionaryServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DictionaryServices
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/PyObjCTest/test_dictionaryservices.py` & `pyobjc-framework-DictionaryServices-9.2/PyObjCTest/test_dictionaryservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DictionaryServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DictionaryServices-9.1b1/setup.py` & `pyobjc-framework-DictionaryServices-9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """
 Deprecated wrappers for the "DictionaryServices" framework on macOS 10.5 or later.
 
 Use package "CoreServices" instead.
 """
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-DictionaryServices",
     description="Wrappers for the framework DictionaryServices on macOS",
     min_os_level="10.5",
     packages=["DictionaryServices"],
     version=VERSION,
```

