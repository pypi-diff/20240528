# Comparing `tmp/pyobjc-framework-ExecutionPolicy-9.1b1.tar.gz` & `tmp/pyobjc-framework-ExecutionPolicy-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ExecutionPolicy-9.1b1.tar", last modified: Sun Mar 26 11:23:46 2023, max compression
+gzip compressed data, was "pyobjc-framework-ExecutionPolicy-9.2.tar", last modified: Wed Jun  7 00:13:54 2023, max compression
```

## Comparing `pyobjc-framework-ExecutionPolicy-9.1b1.tar` & `pyobjc-framework-ExecutionPolicy-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.382851 pyobjc-framework-ExecutionPolicy-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.352627 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.357263 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/ExecutionPolicy/
--rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/ExecutionPolicy/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1500 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/ExecutionPolicy/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.367445 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2148 2023-03-26 11:23:46.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      901 2023-03-26 11:23:46.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:46.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:03.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:46.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:23:46.000000 pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExecutionPolicy-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1937 2023-03-26 11:23:46.382460 pyobjc-framework-ExecutionPolicy-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.375267 pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      799 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/test_epdevelopertool.py
--rw-r--r--   0 ronald     (501) staff       (20)      328 2021-03-21 10:08:22.000000 pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/test_eperrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/test_executionpolicy.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.376505 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/ExecutionPolicy.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:46.381529 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     3038 2021-07-30 09:00:37.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3149 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3257 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2782 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3039 2021-03-21 10:08:22.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3039 2021-07-30 09:00:37.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3150 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3258 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExecutionPolicy-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:46.382953 pyobjc-framework-ExecutionPolicy-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      705 2023-03-25 14:20:31.000000 pyobjc-framework-ExecutionPolicy-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.041846 pyobjc-framework-ExecutionPolicy-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.018662 pyobjc-framework-ExecutionPolicy-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.023337 pyobjc-framework-ExecutionPolicy-9.2/Lib/ExecutionPolicy/
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/ExecutionPolicy/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1500 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/ExecutionPolicy/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.026986 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2146 2023-06-07 00:13:54.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      916 2023-06-07 00:13:54.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:53.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:03.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:53.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:13:53.000000 pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExecutionPolicy-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1935 2023-06-07 00:13:54.041482 pyobjc-framework-ExecutionPolicy-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.030436 pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/test_epdevelopertool.py
+-rw-r--r--   0 ronald     (501) staff       (20)      328 2021-03-21 10:08:22.000000 pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/test_eperrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/test_executionpolicy.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.034905 pyobjc-framework-ExecutionPolicy-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/ExecutionPolicy.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:54.040836 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     3038 2021-07-30 09:00:37.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3149 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3257 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2782 2020-11-30 18:45:14.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3039 2021-03-21 10:08:22.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3039 2021-07-30 09:00:37.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3150 2022-02-24 08:47:16.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3258 2023-02-19 10:50:35.000000 pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExecutionPolicy-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ExecutionPolicy-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:54.041955 pyobjc-framework-ExecutionPolicy-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      787 2023-05-29 10:07:46.000000 pyobjc-framework-ExecutionPolicy-9.2/setup.py
```

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/Lib/ExecutionPolicy/__init__.py` & `pyobjc-framework-ExecutionPolicy-9.2/Lib/ExecutionPolicy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/Lib/ExecutionPolicy/_metadata.py` & `pyobjc-framework-ExecutionPolicy-9.2/Lib/ExecutionPolicy/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/PKG-INFO` & `pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExecutionPolicy
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExecutionPolicy on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExecutionPolicy
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/Lib/pyobjc_framework_ExecutionPolicy.egg-info/SOURCES.txt` & `pyobjc-framework-ExecutionPolicy-9.2/Lib/pyobjc_framework_ExecutionPolicy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ExecutionPolicy/__init__.py
 Lib/ExecutionPolicy/_metadata.py
 Lib/pyobjc_framework_ExecutionPolicy.egg-info/PKG-INFO
 Lib/pyobjc_framework_ExecutionPolicy.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ExecutionPolicy.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ExecutionPolicy.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/License.txt` & `pyobjc-framework-ExecutionPolicy-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/PKG-INFO` & `pyobjc-framework-ExecutionPolicy-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExecutionPolicy
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExecutionPolicy on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExecutionPolicy
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/PyObjCTest/test_epdevelopertool.py` & `pyobjc-framework-ExecutionPolicy-9.2/PyObjCTest/test_epdevelopertool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/ExecutionPolicy.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/ExecutionPolicy.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-ExecutionPolicy-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ExecutionPolicy-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExecutionPolicy-9.1b1/setup.py` & `pyobjc-framework-ExecutionPolicy-9.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
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
     name="pyobjc-framework-ExecutionPolicy",
     description="Wrappers for the framework ExecutionPolicy on macOS",
     min_os_level="10.15",
     packages=["ExecutionPolicy"],
     version=VERSION,
```

