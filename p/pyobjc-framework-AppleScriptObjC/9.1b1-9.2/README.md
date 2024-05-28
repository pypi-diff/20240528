# Comparing `tmp/pyobjc-framework-AppleScriptObjC-9.1b1.tar.gz` & `tmp/pyobjc-framework-AppleScriptObjC-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AppleScriptObjC-9.1b1.tar", last modified: Sun Mar 26 11:14:22 2023, max compression
+gzip compressed data, was "pyobjc-framework-AppleScriptObjC-9.2.tar", last modified: Wed Jun  7 00:06:01 2023, max compression
```

## Comparing `pyobjc-framework-AppleScriptObjC-9.1b1.tar` & `pyobjc-framework-AppleScriptObjC-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.406443 pyobjc-framework-AppleScriptObjC-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppleScriptObjC-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.368296 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.375755 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/AppleScriptObjC/
--rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/AppleScriptObjC/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/AppleScriptObjC/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.379003 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2283 2023-03-26 11:14:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      849 2023-03-26 11:14:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:19.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:14:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:14:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2072 2023-03-26 11:14:22.406098 pyobjc-framework-AppleScriptObjC-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.381754 pyobjc-framework-AppleScriptObjC-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      462 2022-04-11 08:03:15.000000 pyobjc-framework-AppleScriptObjC-9.1b1/PyObjCTest/test_applescriptobjc.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-AppleScriptObjC-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.398970 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      213 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/AppleScriptObjC.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:22.405421 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)      976 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      995 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      977 2021-03-21 10:08:22.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      891 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      891 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      980 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      977 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      996 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppleScriptObjC-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:22.406559 pyobjc-framework-AppleScriptObjC-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      814 2023-03-25 14:20:30.000000 pyobjc-framework-AppleScriptObjC-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.173168 pyobjc-framework-AppleScriptObjC-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppleScriptObjC-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.151208 pyobjc-framework-AppleScriptObjC-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.157019 pyobjc-framework-AppleScriptObjC-9.2/Lib/AppleScriptObjC/
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/AppleScriptObjC/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/AppleScriptObjC/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.160140 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2281 2023-06-07 00:06:01.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      864 2023-06-07 00:06:01.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:01.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:19.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:06:01.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:06:01.000000 pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2070 2023-06-07 00:06:01.172804 pyobjc-framework-AppleScriptObjC-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.161296 pyobjc-framework-AppleScriptObjC-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      462 2022-04-11 08:03:15.000000 pyobjc-framework-AppleScriptObjC-9.2/PyObjCTest/test_applescriptobjc.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-AppleScriptObjC-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.162961 pyobjc-framework-AppleScriptObjC-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      213 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/AppleScriptObjC.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:01.172164 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)      976 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      995 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      977 2021-03-21 10:08:22.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      891 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      891 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      980 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      977 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      996 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppleScriptObjC-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AppleScriptObjC-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:01.173429 pyobjc-framework-AppleScriptObjC-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      895 2023-05-29 10:07:45.000000 pyobjc-framework-AppleScriptObjC-9.2/setup.py
```

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/LICENSE.txt` & `pyobjc-framework-AppleScriptObjC-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/Lib/AppleScriptObjC/__init__.py` & `pyobjc-framework-AppleScriptObjC-9.2/Lib/AppleScriptObjC/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/PKG-INFO` & `pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppleScriptObjC
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppleScriptObjC on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppleScriptObjC
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/Lib/pyobjc_framework_AppleScriptObjC.egg-info/SOURCES.txt` & `pyobjc-framework-AppleScriptObjC-9.2/Lib/pyobjc_framework_AppleScriptObjC.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AppleScriptObjC/__init__.py
 Lib/AppleScriptObjC/_metadata.py
 Lib/pyobjc_framework_AppleScriptObjC.egg-info/PKG-INFO
 Lib/pyobjc_framework_AppleScriptObjC.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AppleScriptObjC.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AppleScriptObjC.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/PKG-INFO` & `pyobjc-framework-AppleScriptObjC-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppleScriptObjC
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppleScriptObjC on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppleScriptObjC
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AppleScriptObjC-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AppleScriptObjC-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptObjC-9.1b1/setup.py` & `pyobjc-framework-AppleScriptObjC-9.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 based application bundles.
 
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
     name="pyobjc-framework-AppleScriptObjC",
     description="Wrappers for the framework AppleScriptObjC on macOS",
     min_os_level="10.6",
     packages=["AppleScriptObjC"],
     version=VERSION,
```

