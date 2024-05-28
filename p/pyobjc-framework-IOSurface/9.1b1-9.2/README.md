# Comparing `tmp/pyobjc-framework-IOSurface-9.1b1.tar.gz` & `tmp/pyobjc-framework-IOSurface-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-IOSurface-9.1b1.tar", last modified: Sun Mar 26 11:26:44 2023, max compression
+gzip compressed data, was "pyobjc-framework-IOSurface-9.2.tar", last modified: Wed Jun  7 00:17:03 2023, max compression
```

## Comparing `pyobjc-framework-IOSurface-9.1b1.tar` & `pyobjc-framework-IOSurface-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.291262 pyobjc-framework-IOSurface-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.261523 pyobjc-framework-IOSurface-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.271174 pyobjc-framework-IOSurface-9.1b1/Lib/IOSurface/
--rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.1b1/Lib/IOSurface/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     8780 2023-03-25 15:03:24.000000 pyobjc-framework-IOSurface-9.1b1/Lib/IOSurface/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.274711 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2107 2023-03-26 11:26:44.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      843 2023-03-26 11:26:44.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:26:44.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:17.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:26:44.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:26:44.000000 pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-IOSurface-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1896 2023-03-26 11:26:44.290938 pyobjc-framework-IOSurface-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.277339 pyobjc-framework-IOSurface-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-IOSurface-9.1b1/PyObjCTest/test_iosurface.py
--rw-r--r--   0 ronald     (501) staff       (20)     8902 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.1b1/PyObjCTest/test_iosurfaceapi.py
--rw-r--r--   0 ronald     (501) staff       (20)     2943 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.1b1/PyObjCTest/test_iosurfaceobjc.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.283043 pyobjc-framework-IOSurface-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    12425 2023-03-25 15:03:24.000000 pyobjc-framework-IOSurface-9.1b1/metadata/IOSurface.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:44.289823 pyobjc-framework-IOSurface-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    15682 2021-07-30 09:00:38.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16022 2022-02-24 08:47:16.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16538 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10243 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    15500 2021-03-21 10:08:22.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    15683 2021-07-30 09:00:38.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16023 2022-02-24 08:47:16.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16539 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOSurface-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:26:44.291430 pyobjc-framework-IOSurface-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      664 2023-03-25 14:20:31.000000 pyobjc-framework-IOSurface-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.932313 pyobjc-framework-IOSurface-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.908910 pyobjc-framework-IOSurface-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.913945 pyobjc-framework-IOSurface-9.2/Lib/IOSurface/
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.2/Lib/IOSurface/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8858 2023-05-27 09:46:33.000000 pyobjc-framework-IOSurface-9.2/Lib/IOSurface/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.917099 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-06-07 00:17:03.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      858 2023-06-07 00:17:03.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:03.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:17.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:17:03.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:17:03.000000 pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-IOSurface-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-06-07 00:17:03.931910 pyobjc-framework-IOSurface-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.919609 pyobjc-framework-IOSurface-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-IOSurface-9.2/PyObjCTest/test_iosurface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8902 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.2/PyObjCTest/test_iosurfaceapi.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2943 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.2/PyObjCTest/test_iosurfaceobjc.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.920949 pyobjc-framework-IOSurface-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    12516 2023-05-27 09:46:33.000000 pyobjc-framework-IOSurface-9.2/metadata/IOSurface.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:03.930724 pyobjc-framework-IOSurface-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    15682 2021-07-30 09:00:38.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16022 2022-02-24 08:47:16.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16538 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10243 2020-11-30 18:45:15.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    15500 2021-03-21 10:08:22.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    15683 2021-07-30 09:00:38.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16023 2022-02-24 08:47:16.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16539 2022-06-15 11:57:00.000000 pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOSurface-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-IOSurface-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:03.932590 pyobjc-framework-IOSurface-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2023-05-29 10:07:46.000000 pyobjc-framework-IOSurface-9.2/setup.py
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/Lib/IOSurface/__init__.py` & `pyobjc-framework-IOSurface-9.2/Lib/IOSurface/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/Lib/IOSurface/_metadata.py` & `pyobjc-framework-IOSurface-9.2/Lib/IOSurface/_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:48:11 2023
+# Last update: Sat May 20 12:12:16 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -124,15 +124,19 @@
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "IOSurfaceGetElementHeightOfPlane": (b"Q^{__IOSurface=}Q",),
     "IOSurfaceGetBytesPerElement": (b"Q^{__IOSurface=}",),
     "IOSurfaceGetPropertyAlignment": (b"Q^{__CFString=}",),
     "IOSurfaceGetNameOfComponentOfPlane": (b"i^{__IOSurface=}QQ",),
-    "IOSurfaceSetPurgeable": (b"i^{__IOSurface=}I^I",),
+    "IOSurfaceSetPurgeable": (
+        b"i^{__IOSurface=}I^I",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "IOSurfaceUnlock": (
         b"i^{__IOSurface=}I^I",
         "",
         {"arguments": {2: {"type_modifier": "N"}}},
     ),
     "IOSurfaceGetPropertyMaximum": (b"Q^{__CFString=}",),
     "IOSurfaceGetWidthOfPlane": (b"Q^{__IOSurface=}Q",),
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/PKG-INFO` & `pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOSurface
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOSurface on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOSurface
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/Lib/pyobjc_framework_IOSurface.egg-info/SOURCES.txt` & `pyobjc-framework-IOSurface-9.2/Lib/pyobjc_framework_IOSurface.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/IOSurface/__init__.py
 Lib/IOSurface/_metadata.py
 Lib/pyobjc_framework_IOSurface.egg-info/PKG-INFO
 Lib/pyobjc_framework_IOSurface.egg-info/SOURCES.txt
 Lib/pyobjc_framework_IOSurface.egg-info/dependency_links.txt
 Lib/pyobjc_framework_IOSurface.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/License.txt` & `pyobjc-framework-IOSurface-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/PKG-INFO` & `pyobjc-framework-IOSurface-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOSurface
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOSurface on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOSurface
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/PyObjCTest/test_iosurfaceapi.py` & `pyobjc-framework-IOSurface-9.2/PyObjCTest/test_iosurfaceapi.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/PyObjCTest/test_iosurfaceobjc.py` & `pyobjc-framework-IOSurface-9.2/PyObjCTest/test_iosurfaceobjc.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/IOSurface.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/IOSurface.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,19 @@
       "retval": { "c_array_of_variable_length": true }
      }
     ]
    }
   },
   "formal_protocols": {},
   "functions": {
+   "IOSurfaceSetPurgeable": {
+    "args": {
+     "2": { "type_modifier": "o" }
+    }
+   },
    "IOSurfaceGetNumberOfComponentsOfPlane": {
     "args": {
      "0": { "typestr": "^{__IOSurface=}" },
      "1": { "typestr": "I" }
     },
     "retval": { "typestr": "I" }
    },
```

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-IOSurface-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/pyobjc_setup.py` & `pyobjc-framework-IOSurface-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOSurface-9.1b1/setup.py` & `pyobjc-framework-IOSurface-9.2/setup.py`

 * *Files 24% similar despite different names*

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
     name="pyobjc-framework-IOSurface",
     description="Wrappers for the framework IOSurface on macOS",
     min_os_level="10.6",
     packages=["IOSurface"],
     version=VERSION,
```

