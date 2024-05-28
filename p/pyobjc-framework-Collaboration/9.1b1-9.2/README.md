# Comparing `tmp/pyobjc-framework-Collaboration-9.1b1.tar.gz` & `tmp/pyobjc-framework-Collaboration-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Collaboration-9.1b1.tar", last modified: Sun Mar 26 11:18:27 2023, max compression
+gzip compressed data, was "pyobjc-framework-Collaboration-9.2.tar", last modified: Wed Jun  7 00:08:57 2023, max compression
```

## Comparing `pyobjc-framework-Collaboration-9.1b1.tar` & `pyobjc-framework-Collaboration-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.587240 pyobjc-framework-Collaboration-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Collaboration-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.554454 pyobjc-framework-Collaboration-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.560436 pyobjc-framework-Collaboration-9.1b1/Lib/Collaboration/
--rw-r--r--   0 ronald     (501) staff       (20)      717 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/Lib/Collaboration/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2618 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.1b1/Lib/Collaboration/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.563435 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2284 2023-03-26 11:18:27.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      928 2023-03-26 11:18:27.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:18:27.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:35.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:18:27.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:18:27.000000 pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2073 2023-03-26 11:18:27.586478 pyobjc-framework-Collaboration-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.570730 pyobjc-framework-Collaboration-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      695 2021-03-21 10:08:22.000000 pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_cbidentity.py
--rw-r--r--   0 ronald     (501) staff       (20)      992 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_cbidentitypicker.py
--rw-r--r--   0 ronald     (501) staff       (20)      769 2022-04-11 08:03:15.000000 pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_collaboration.py
--rw-r--r--   0 ronald     (501) staff       (20)      290 2021-10-18 19:38:40.000000 pyobjc-framework-Collaboration-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.573083 pyobjc-framework-Collaboration-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3053 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/Collaboration.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:27.585487 pyobjc-framework-Collaboration-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16164 2021-07-30 09:00:37.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16183 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10917 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16165 2021-03-21 10:08:22.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10817 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10817 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10906 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16165 2021-07-30 09:00:37.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16184 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Collaboration-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:18:27.587368 pyobjc-framework-Collaboration-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      814 2023-03-25 14:20:30.000000 pyobjc-framework-Collaboration-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.235235 pyobjc-framework-Collaboration-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Collaboration-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.204668 pyobjc-framework-Collaboration-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.210564 pyobjc-framework-Collaboration-9.2/Lib/Collaboration/
+-rw-r--r--   0 ronald     (501) staff       (20)      717 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/Lib/Collaboration/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2618 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.2/Lib/Collaboration/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.213814 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2282 2023-06-07 00:08:57.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      943 2023-06-07 00:08:57.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:08:57.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:35.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:08:57.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:08:57.000000 pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2071 2023-06-07 00:08:57.234829 pyobjc-framework-Collaboration-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.219113 pyobjc-framework-Collaboration-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2021-03-21 10:08:22.000000 pyobjc-framework-Collaboration-9.2/PyObjCTest/test_cbidentity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      992 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/PyObjCTest/test_cbidentitypicker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      769 2022-04-11 08:03:15.000000 pyobjc-framework-Collaboration-9.2/PyObjCTest/test_collaboration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      290 2021-10-18 19:38:40.000000 pyobjc-framework-Collaboration-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.221090 pyobjc-framework-Collaboration-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3053 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/Collaboration.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:08:57.233827 pyobjc-framework-Collaboration-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16164 2021-07-30 09:00:37.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16183 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10917 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16165 2021-03-21 10:08:22.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10817 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10817 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10906 2020-11-30 18:45:14.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16165 2021-07-30 09:00:37.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16184 2022-02-24 08:47:16.000000 pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Collaboration-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Collaboration-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:08:57.235338 pyobjc-framework-Collaboration-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2023-05-29 10:07:45.000000 pyobjc-framework-Collaboration-9.2/setup.py
```

### Comparing `pyobjc-framework-Collaboration-9.1b1/LICENSE.txt` & `pyobjc-framework-Collaboration-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/Lib/Collaboration/__init__.py` & `pyobjc-framework-Collaboration-9.2/Lib/Collaboration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/Lib/Collaboration/_metadata.py` & `pyobjc-framework-Collaboration-9.2/Lib/Collaboration/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/PKG-INFO` & `pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Collaboration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Collaboration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Collaboration
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-Collaboration-9.1b1/Lib/pyobjc_framework_Collaboration.egg-info/SOURCES.txt` & `pyobjc-framework-Collaboration-9.2/Lib/pyobjc_framework_Collaboration.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Collaboration/__init__.py
 Lib/Collaboration/_metadata.py
 Lib/pyobjc_framework_Collaboration.egg-info/PKG-INFO
 Lib/pyobjc_framework_Collaboration.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Collaboration.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Collaboration.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Collaboration-9.1b1/PKG-INFO` & `pyobjc-framework-Collaboration-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Collaboration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Collaboration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Collaboration
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_cbidentity.py` & `pyobjc-framework-Collaboration-9.2/PyObjCTest/test_cbidentity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_cbidentitypicker.py` & `pyobjc-framework-Collaboration-9.2/PyObjCTest/test_cbidentitypicker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/PyObjCTest/test_collaboration.py` & `pyobjc-framework-Collaboration-9.2/PyObjCTest/test_collaboration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/Collaboration.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/Collaboration.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Collaboration-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Collaboration-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Collaboration-9.1b1/setup.py` & `pyobjc-framework-Collaboration-9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 user interface elements for selecting identities.
 
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
     name="pyobjc-framework-Collaboration",
     description="Wrappers for the framework Collaboration on macOS",
     min_os_level="10.5",
     packages=["Collaboration"],
     version=VERSION,
```

