# Comparing `tmp/pyobjc-framework-ColorSync-9.1b1.tar.gz` & `tmp/pyobjc-framework-ColorSync-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ColorSync-9.1b1.tar", last modified: Sun Mar 26 11:18:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-ColorSync-9.2.tar", last modified: Wed Jun  7 00:09:02 2023, max compression
```

## Comparing `pyobjc-framework-ColorSync-9.1b1.tar` & `pyobjc-framework-ColorSync-9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.687783 pyobjc-framework-ColorSync-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.612831 pyobjc-framework-ColorSync-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.619336 pyobjc-framework-ColorSync-9.1b1/Lib/ColorSync/
--rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.1b1/Lib/ColorSync/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    17233 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.1b1/Lib/ColorSync/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.641245 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2127 2023-03-26 11:18:34.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      886 2023-03-26 11:18:34.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:18:34.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:36.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:18:34.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:18:34.000000 pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ColorSync-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1916 2023-03-26 11:18:34.686907 pyobjc-framework-ColorSync-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.645677 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsync.py
--rw-r--r--   0 ronald     (501) staff       (20)     1177 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsynccmm.py
--rw-r--r--   0 ronald     (501) staff       (20)     2903 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsyncdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)    10428 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsyncprofile.py
--rw-r--r--   0 ronald     (501) staff       (20)     6761 2021-10-29 07:58:20.000000 pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsynctransform.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.648023 pyobjc-framework-ColorSync-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    21177 2021-07-31 11:35:38.000000 pyobjc-framework-ColorSync-9.1b1/metadata/ColorSync.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:34.685334 pyobjc-framework-ColorSync-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    30398 2021-07-30 09:00:37.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30517 2022-02-24 08:47:16.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    32048 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29663 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30399 2021-07-30 09:00:37.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30518 2022-02-24 08:47:16.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    32049 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ColorSync-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:18:34.687976 pyobjc-framework-ColorSync-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      683 2023-03-25 14:20:30.000000 pyobjc-framework-ColorSync-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.223148 pyobjc-framework-ColorSync-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.195786 pyobjc-framework-ColorSync-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.201207 pyobjc-framework-ColorSync-9.2/Lib/ColorSync/
+-rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.2/Lib/ColorSync/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17233 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.2/Lib/ColorSync/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.204601 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2125 2023-06-07 00:09:02.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      901 2023-06-07 00:09:02.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:09:02.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:36.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:09:02.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:09:02.000000 pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ColorSync-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1914 2023-06-07 00:09:02.222779 pyobjc-framework-ColorSync-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.212403 pyobjc-framework-ColorSync-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsync.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1177 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsynccmm.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2903 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsyncdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10428 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsyncprofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6761 2021-10-29 07:58:20.000000 pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsynctransform.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.214763 pyobjc-framework-ColorSync-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    21177 2021-07-31 11:35:38.000000 pyobjc-framework-ColorSync-9.2/metadata/ColorSync.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-ColorSync-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:02.221895 pyobjc-framework-ColorSync-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    30398 2021-07-30 09:00:37.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30517 2022-02-24 08:47:16.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    32048 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29663 2021-03-21 10:08:22.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30399 2021-07-30 09:00:37.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30518 2022-02-24 08:47:16.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    32049 2022-10-18 09:53:23.000000 pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ColorSync-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ColorSync-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:09:02.223263 pyobjc-framework-ColorSync-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      765 2023-05-29 10:07:45.000000 pyobjc-framework-ColorSync-9.2/setup.py
```

### Comparing `pyobjc-framework-ColorSync-9.1b1/Lib/ColorSync/__init__.py` & `pyobjc-framework-ColorSync-9.2/Lib/ColorSync/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/Lib/ColorSync/_metadata.py` & `pyobjc-framework-ColorSync-9.2/Lib/ColorSync/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/PKG-INFO` & `pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ColorSync
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ColorSync on Mac OS X
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ColorSync
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-ColorSync-9.1b1/Lib/pyobjc_framework_ColorSync.egg-info/SOURCES.txt` & `pyobjc-framework-ColorSync-9.2/Lib/pyobjc_framework_ColorSync.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ColorSync/__init__.py
 Lib/ColorSync/_metadata.py
 Lib/pyobjc_framework_ColorSync.egg-info/PKG-INFO
 Lib/pyobjc_framework_ColorSync.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ColorSync.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ColorSync.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ColorSync-9.1b1/License.txt` & `pyobjc-framework-ColorSync-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/PKG-INFO` & `pyobjc-framework-ColorSync-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ColorSync
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ColorSync on Mac OS X
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ColorSync
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsynccmm.py` & `pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsynccmm.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsyncdevice.py` & `pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsyncdevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsyncprofile.py` & `pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsyncprofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/PyObjCTest/test_colorsynctransform.py` & `pyobjc-framework-ColorSync-9.2/PyObjCTest/test_colorsynctransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/ColorSync.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/ColorSync.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ColorSync-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ColorSync-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ColorSync-9.1b1/setup.py` & `pyobjc-framework-ColorSync-9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 Wrappers for the "ColorSync" framework on MacOSX 10.13 or later.
 
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
     name="pyobjc-framework-ColorSync",
     description="Wrappers for the framework ColorSync on Mac OS X",
     min_os_level="10.13",
     packages=["ColorSync"],
     version=VERSION,
```

