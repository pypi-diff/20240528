# Comparing `tmp/pyobjc-framework-ImageCaptureCore-9.1b1.tar.gz` & `tmp/pyobjc-framework-ImageCaptureCore-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ImageCaptureCore-9.1b1.tar", last modified: Sun Mar 26 11:26:49 2023, max compression
+gzip compressed data, was "pyobjc-framework-ImageCaptureCore-9.2.tar", last modified: Wed Jun  7 00:17:08 2023, max compression
```

## Comparing `pyobjc-framework-ImageCaptureCore-9.1b1.tar` & `pyobjc-framework-ImageCaptureCore-9.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:49.007347 pyobjc-framework-ImageCaptureCore-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ImageCaptureCore-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.939847 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.947956 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/ImageCaptureCore/
--rw-r--r--   0 ronald     (501) staff       (20)      789 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/ImageCaptureCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    34189 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/ImageCaptureCore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.951727 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2161 2023-03-26 11:26:48.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1253 2023-03-26 11:26:48.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:26:48.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:18.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:26:48.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:26:48.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.954285 pyobjc-framework-ImageCaptureCore-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Modules/_ImageCaptureCore.m
--rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Modules/_ImageCaptureCore_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ImageCaptureCore-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1950 2023-03-26 11:26:49.006784 pyobjc-framework-ImageCaptureCore-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.986033 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5854 2022-06-26 20:28:13.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccameradevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1263 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccamerafile.py
--rw-r--r--   0 ronald     (501) staff       (20)     1622 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccameraitem.py
--rw-r--r--   0 ronald     (501) staff       (20)    19285 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccommonconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     4700 2022-06-26 20:28:03.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      877 2022-06-25 20:11:12.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icdevicebrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)      257 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icscannerbanddata.py
--rw-r--r--   0 ronald     (501) staff       (20)      637 2022-06-25 20:16:50.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icscannerdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_imagecapurecore.py
--rw-r--r--   0 ronald     (501) staff       (20)    10203 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_isscannerfunctionalunits.py
--rw-r--r--   0 ronald     (501) staff       (20)      293 2021-10-18 19:38:40.000000 pyobjc-framework-ImageCaptureCore-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.987634 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    13314 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/ImageCaptureCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      100 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:48.999468 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   127156 2021-07-30 09:00:38.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   128392 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    94151 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.11.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   118363 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   126046 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   127157 2021-07-30 09:00:38.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   128393 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ImageCaptureCore-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:26:49.007461 pyobjc-framework-ImageCaptureCore-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1199 2023-03-25 14:20:31.000000 pyobjc-framework-ImageCaptureCore-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.993816 pyobjc-framework-ImageCaptureCore-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ImageCaptureCore-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.935795 pyobjc-framework-ImageCaptureCore-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.941585 pyobjc-framework-ImageCaptureCore-9.2/Lib/ImageCaptureCore/
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/ImageCaptureCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    34189 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/ImageCaptureCore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.945310 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2159 2023-06-07 00:17:08.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1268 2023-06-07 00:17:08.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:08.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:18.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:17:08.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:17:08.000000 pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.948937 pyobjc-framework-ImageCaptureCore-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-ImageCaptureCore-9.2/Modules/_ImageCaptureCore.m
+-rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/Modules/_ImageCaptureCore_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ImageCaptureCore-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ImageCaptureCore-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1948 2023-06-07 00:17:08.993359 pyobjc-framework-ImageCaptureCore-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.968621 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5854 2023-05-04 11:00:07.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccameradevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1263 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccamerafile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1622 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccameraitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19285 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccommonconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4720 2023-05-04 11:00:07.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      877 2022-06-25 20:11:12.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icdevicebrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      257 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icscannerbanddata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      637 2022-06-25 20:16:50.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icscannerdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_imagecapurecore.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10203 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_isscannerfunctionalunits.py
+-rw-r--r--   0 ronald     (501) staff       (20)      293 2021-10-18 19:38:40.000000 pyobjc-framework-ImageCaptureCore-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.970549 pyobjc-framework-ImageCaptureCore-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    13314 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/ImageCaptureCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      100 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:08.991824 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   127156 2021-07-30 09:00:38.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   128392 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    94151 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.11.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   118363 2020-11-30 18:45:15.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   126046 2021-03-21 10:08:22.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   127157 2021-07-30 09:00:38.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   128393 2022-02-24 08:47:16.000000 pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ImageCaptureCore-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ImageCaptureCore-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:08.993926 pyobjc-framework-ImageCaptureCore-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1270 2023-05-29 10:07:46.000000 pyobjc-framework-ImageCaptureCore-9.2/setup.py
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/LICENSE.txt` & `pyobjc-framework-ImageCaptureCore-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Lib/ImageCaptureCore/__init__.py` & `pyobjc-framework-ImageCaptureCore-9.2/Lib/ImageCaptureCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Lib/ImageCaptureCore/_metadata.py` & `pyobjc-framework-ImageCaptureCore-9.2/Lib/ImageCaptureCore/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/PKG-INFO` & `pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ImageCaptureCore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ImageCaptureCore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ImageCaptureCore
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Lib/pyobjc_framework_ImageCaptureCore.egg-info/SOURCES.txt` & `pyobjc-framework-ImageCaptureCore-9.2/Lib/pyobjc_framework_ImageCaptureCore.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ImageCaptureCore/__init__.py
 Lib/ImageCaptureCore/_metadata.py
 Lib/pyobjc_framework_ImageCaptureCore.egg-info/PKG-INFO
 Lib/pyobjc_framework_ImageCaptureCore.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ImageCaptureCore.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ImageCaptureCore.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Modules/_ImageCaptureCore.m` & `pyobjc-framework-ImageCaptureCore-9.2/Modules/_ImageCaptureCore.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Modules/_ImageCaptureCore_protocols.m` & `pyobjc-framework-ImageCaptureCore-9.2/Modules/_ImageCaptureCore_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ImageCaptureCore-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ImageCaptureCore-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PKG-INFO` & `pyobjc-framework-ImageCaptureCore-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ImageCaptureCore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ImageCaptureCore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ImageCaptureCore
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccameradevice.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccameradevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         )
         self.assertArgIsSEL(
             ImageCaptureCore.ICCameraDevice.requestSendPTPCommand_outData_sendCommandDelegate_didSendCommandSelector_contextInfo_,
             3,
             b"v@:@@@@^v",
         )
 
-    @min_os_level("10.10")
+    @min_os_level("10.12")
     def test_methods10_10(self):
         self.assertResultIsBOOL(ImageCaptureCore.ICCameraDevice.iCloudPhotosEnabled)
 
     @min_os_level("10.15")
     def test_methods10_15(self):
         self.assertResultIsBOOL(ImageCaptureCore.ICCameraDevice.isEjectable)
         self.assertArgIsBlock(
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccamerafile.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccamerafile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccameraitem.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccameraitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_iccommonconstants.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_iccommonconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icdevice.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import ImageCaptureCore
-from PyObjCTools.TestSupport import TestCase, min_os_level, expectedFailure
+from PyObjCTools.TestSupport import (
+    TestCase,
+    min_os_level,
+    max_os_level,
+)
 
 
 class TestICDevice(TestCase):
     def test_typed_enum(self):
         self.assertIsTypedEnum(ImageCaptureCore.ICDeviceCapability, str)
         self.assertIsTypedEnum(ImageCaptureCore.ICDeviceLocationOptions, str)
         self.assertIsTypedEnum(ImageCaptureCore.ICDeviceStatus, str)
@@ -71,15 +75,15 @@
 
         self.assertArgIsSEL(
             ImageCaptureCore.ICDevice.requestSendMessage_outData_maxReturnedDataSize_sendMessageDelegate_didSendMessageSelector_contextInfo_,  # noqa: B950
             4,
             b"v@:I@@^v",
         )
 
-    @expectedFailure
+    @max_os_level("10.14")
     def testMethods_removed_in_10_15(self):
         self.assertResultIsBOOL(ImageCaptureCore.ICDevice.isShared)
 
     @min_os_level("10.15")
     def testMethods10_15(self):
         self.assertArgIsBlock(
             ImageCaptureCore.ICDevice.requestOpenSessionWithOptions_completion_,
```

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icdevicebrowser.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icdevicebrowser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_icscannerdevice.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_icscannerdevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/PyObjCTest/test_isscannerfunctionalunits.py` & `pyobjc-framework-ImageCaptureCore-9.2/PyObjCTest/test_isscannerfunctionalunits.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/ImageCaptureCore.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/ImageCaptureCore.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.11.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.11.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ImageCaptureCore-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ImageCaptureCore-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ImageCaptureCore-9.1b1/setup.py` & `pyobjc-framework-ImageCaptureCore-9.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-ImageCaptureCore",
     description="Wrappers for the framework ImageCaptureCore on macOS",
     min_os_level="10.6",
     packages=["ImageCaptureCore"],
     ext_modules=[
```

