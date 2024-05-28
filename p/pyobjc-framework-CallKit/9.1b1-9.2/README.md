# Comparing `tmp/pyobjc-framework-CallKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-CallKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CallKit-9.1b1.tar", last modified: Sun Mar 26 11:16:27 2023, max compression
+gzip compressed data, was "pyobjc-framework-CallKit-9.2.tar", last modified: Wed Jun  7 00:07:34 2023, max compression
```

## Comparing `pyobjc-framework-CallKit-9.1b1.tar` & `pyobjc-framework-CallKit-9.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.521731 pyobjc-framework-CallKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.420725 pyobjc-framework-CallKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.427510 pyobjc-framework-CallKit-9.1b1/Lib/CallKit/
--rw-r--r--   0 ronald     (501) staff       (20)      681 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/Lib/CallKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    13401 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.1b1/Lib/CallKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.437393 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-03-26 11:16:27.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1142 2023-03-26 11:16:27.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:27.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:19.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:16:27.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:16:27.000000 pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CallKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2023-03-26 11:16:27.521059 pyobjc-framework-CallKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.458581 pyobjc-framework-CallKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_callkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      352 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcall.py
--rw-r--r--   0 ronald     (501) staff       (20)      506 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcallcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      221 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcalldirectory.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-06-25 20:15:59.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcallobserver.py
--rw-r--r--   0 ronald     (501) staff       (20)      832 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcallupdate.py
--rw-r--r--   0 ronald     (501) staff       (20)     2766 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      482 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxhandle.py
--rw-r--r--   0 ronald     (501) staff       (20)      444 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxplaydtmfcallaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      821 2022-06-25 20:11:59.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      499 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxproviderconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      273 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxsetheldcallaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2021-07-31 10:33:36.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxsetmutedcallaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      265 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxstartcallaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      191 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxtransaction.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.462326 pyobjc-framework-CallKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      303 2021-07-31 10:37:50.000000 pyobjc-framework-CallKit-9.1b1/metadata/CallKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:27.487836 pyobjc-framework-CallKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    60320 2021-07-30 09:00:37.000000 pyobjc-framework-CallKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60854 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    59346 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60321 2021-07-30 09:00:37.000000 pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60855 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CallKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:16:27.521825 pyobjc-framework-CallKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      657 2023-03-25 14:20:30.000000 pyobjc-framework-CallKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.737219 pyobjc-framework-CallKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.693841 pyobjc-framework-CallKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.698368 pyobjc-framework-CallKit-9.2/Lib/CallKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      681 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/Lib/CallKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13401 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.2/Lib/CallKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.701928 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-06-07 00:07:34.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1157 2023-06-07 00:07:34.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:34.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:19.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:07:34.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:07:34.000000 pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CallKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:07:34.736803 pyobjc-framework-CallKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.717758 pyobjc-framework-CallKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_callkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      352 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcall.py
+-rw-r--r--   0 ronald     (501) staff       (20)      506 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcallcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      221 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcalldirectory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-06-25 20:15:59.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcallobserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      832 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcallupdate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2766 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      482 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxhandle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      444 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxplaydtmfcallaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      821 2022-06-25 20:11:59.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      499 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxproviderconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      273 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxsetheldcallaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2021-07-31 10:33:36.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxsetmutedcallaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      265 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxstartcallaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      191 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxtransaction.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.719299 pyobjc-framework-CallKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      303 2021-07-31 10:37:50.000000 pyobjc-framework-CallKit-9.2/metadata/CallKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:34.735341 pyobjc-framework-CallKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    60320 2021-07-30 09:00:37.000000 pyobjc-framework-CallKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60854 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    59346 2021-03-21 10:08:22.000000 pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60321 2021-07-30 09:00:37.000000 pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60855 2022-02-24 08:47:16.000000 pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CallKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CallKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:34.737316 pyobjc-framework-CallKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      738 2023-05-29 10:07:45.000000 pyobjc-framework-CallKit-9.2/setup.py
```

### Comparing `pyobjc-framework-CallKit-9.1b1/Lib/CallKit/__init__.py` & `pyobjc-framework-CallKit-9.2/Lib/CallKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/Lib/CallKit/_metadata.py` & `pyobjc-framework-CallKit-9.2/Lib/CallKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/PKG-INFO` & `pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CallKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CallKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CallKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-CallKit-9.1b1/Lib/pyobjc_framework_CallKit.egg-info/SOURCES.txt` & `pyobjc-framework-CallKit-9.2/Lib/pyobjc_framework_CallKit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CallKit/__init__.py
 Lib/CallKit/_metadata.py
 Lib/pyobjc_framework_CallKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_CallKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CallKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CallKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CallKit-9.1b1/License.txt` & `pyobjc-framework-CallKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/PKG-INFO` & `pyobjc-framework-CallKit-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CallKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CallKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CallKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxcallupdate.py` & `pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxcallupdate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxerror.py` & `pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/PyObjCTest/test_cxprovider.py` & `pyobjc-framework-CallKit-9.2/PyObjCTest/test_cxprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CallKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CallKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CallKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CallKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CallKit-9.1b1/setup.py` & `pyobjc-framework-CallKit-9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "CallKit" framework on macOS.
 
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
     name="pyobjc-framework-CallKit",
     description="Wrappers for the framework CallKit on macOS",
     min_os_level="10.16",
     packages=["CallKit"],
     version=VERSION,
```

