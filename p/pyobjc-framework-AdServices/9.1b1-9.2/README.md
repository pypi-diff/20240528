# Comparing `tmp/pyobjc-framework-AdServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-AdServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AdServices-9.1b1.tar", last modified: Sun Mar 26 11:13:39 2023, max compression
+gzip compressed data, was "pyobjc-framework-AdServices-9.2.tar", last modified: Wed Jun  7 00:05:29 2023, max compression
```

## Comparing `pyobjc-framework-AdServices-9.1b1.tar` & `pyobjc-framework-AdServices-9.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.200904 pyobjc-framework-AdServices-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.164056 pyobjc-framework-AdServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.170876 pyobjc-framework-AdServices-9.1b1/Lib/AdServices/
--rw-r--r--   0 ronald     (501) staff       (20)      702 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.1b1/Lib/AdServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      967 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.1b1/Lib/AdServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.182023 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2125 2023-03-26 11:13:39.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      754 2023-03-26 11:13:39.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:13:39.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-04-06 12:49:13.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:13:39.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:13:39.000000 pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AdServices-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1914 2023-03-26 11:13:39.200403 pyobjc-framework-AdServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.184841 pyobjc-framework-AdServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      520 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.1b1/PyObjCTest/test_aaatribution.py
--rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-AdServices-9.1b1/PyObjCTest/test_adservices.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.186860 pyobjc-framework-AdServices-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      580 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.1b1/metadata/AdServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:39.199111 pyobjc-framework-AdServices-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     1359 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1433 2022-02-24 08:47:16.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1513 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1360 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1434 2022-02-24 08:47:16.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1514 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AdServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:13:39.201012 pyobjc-framework-AdServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      682 2023-03-25 14:20:30.000000 pyobjc-framework-AdServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.036042 pyobjc-framework-AdServices-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.019150 pyobjc-framework-AdServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.023746 pyobjc-framework-AdServices-9.2/Lib/AdServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      702 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.2/Lib/AdServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      967 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.2/Lib/AdServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.027015 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2123 2023-06-07 00:05:29.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      769 2023-06-07 00:05:29.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:29.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-04-06 12:49:13.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:29.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:05:29.000000 pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AdServices-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1912 2023-06-07 00:05:29.035579 pyobjc-framework-AdServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.029315 pyobjc-framework-AdServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2021-03-21 10:08:22.000000 pyobjc-framework-AdServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      520 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.2/PyObjCTest/test_aaatribution.py
+-rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-AdServices-9.2/PyObjCTest/test_adservices.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.030409 pyobjc-framework-AdServices-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      580 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.2/metadata/AdServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:29.034433 pyobjc-framework-AdServices-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     1359 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1433 2022-02-24 08:47:16.000000 pyobjc-framework-AdServices-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1513 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1360 2021-07-30 09:00:37.000000 pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1434 2022-02-24 08:47:16.000000 pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1514 2023-02-19 10:50:34.000000 pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AdServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AdServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:29.036138 pyobjc-framework-AdServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      763 2023-05-29 10:07:45.000000 pyobjc-framework-AdServices-9.2/setup.py
```

### Comparing `pyobjc-framework-AdServices-9.1b1/Lib/AdServices/__init__.py` & `pyobjc-framework-AdServices-9.2/Lib/AdServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/Lib/AdServices/_metadata.py` & `pyobjc-framework-AdServices-9.2/Lib/AdServices/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/PKG-INFO` & `pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AdServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AdServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AdServices
 Platform: MacOS X (>=11.0)
```

### Comparing `pyobjc-framework-AdServices-9.1b1/Lib/pyobjc_framework_AdServices.egg-info/SOURCES.txt` & `pyobjc-framework-AdServices-9.2/Lib/pyobjc_framework_AdServices.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AdServices/__init__.py
 Lib/AdServices/_metadata.py
 Lib/pyobjc_framework_AdServices.egg-info/PKG-INFO
 Lib/pyobjc_framework_AdServices.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AdServices.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AdServices.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AdServices-9.1b1/License.txt` & `pyobjc-framework-AdServices-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/PKG-INFO` & `pyobjc-framework-AdServices-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AdServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AdServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AdServices
 Platform: MacOS X (>=11.0)
```

### Comparing `pyobjc-framework-AdServices-9.1b1/PyObjCTest/test_aaatribution.py` & `pyobjc-framework-AdServices-9.2/PyObjCTest/test_aaatribution.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/AdServices.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/AdServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-AdServices-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AdServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdServices-9.1b1/setup.py` & `pyobjc-framework-AdServices-9.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "AdServices" framework on macOS 11.1 or later.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-AdServices",
     description="Wrappers for the framework AdServices on macOS",
     min_os_level="11.0",
     packages=["AdServices"],
     version=VERSION,
```

