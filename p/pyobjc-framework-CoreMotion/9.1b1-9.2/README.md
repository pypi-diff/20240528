# Comparing `tmp/pyobjc-framework-CoreMotion-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreMotion-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreMotion-9.1b1.tar", last modified: Sun Mar 26 11:21:44 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreMotion-9.2.tar", last modified: Wed Jun  7 00:11:44 2023, max compression
```

## Comparing `pyobjc-framework-CoreMotion-9.1b1.tar` & `pyobjc-framework-CoreMotion-9.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.202708 pyobjc-framework-CoreMotion-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.158491 pyobjc-framework-CoreMotion-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.162753 pyobjc-framework-CoreMotion-9.1b1/Lib/CoreMotion/
--rw-r--r--   0 ronald     (501) staff       (20)      772 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/CoreMotion/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    18954 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/CoreMotion/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.165928 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2112 2023-03-26 11:21:44.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1333 2023-03-26 11:21:44.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:21:44.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:54.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:21:44.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:21:44.000000 pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMotion-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.168388 pyobjc-framework-CoreMotion-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      766 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/Modules/_CoreMotion.m
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/Modules/_CoreMotion_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMotion-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreMotion-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1901 2023-03-26 11:21:44.202235 pyobjc-framework-CoreMotion-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.182363 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmaccelerometer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmattitude.py
--rw-r--r--   0 ronald     (501) staff       (20)      515 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmauthorization.py
--rw-r--r--   0 ronald     (501) staff       (20)     1102 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmdevicemotion.py
--rw-r--r--   0 ronald     (501) staff       (20)     1032 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      232 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmerrordomain.py
--rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmfalldetectionevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmgyro.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmmagnetometer.py
--rw-r--r--   0 ronald     (501) staff       (20)      448 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmmotionactivity.py
--rw-r--r--   0 ronald     (501) staff       (20)     1308 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmpedometer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1074 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmwatersubmersiondata.py
--rw-r--r--   0 ronald     (501) staff       (20)      439 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmwatersubmersionmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_coremotion.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.183660 pyobjc-framework-CoreMotion-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1489 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/CoreMotion.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:44.200564 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    67097 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68718 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81475 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    50635 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    59284 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    67098 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68719 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81476 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMotion-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:21:44.202821 pyobjc-framework-CoreMotion-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1089 2023-03-25 14:20:31.000000 pyobjc-framework-CoreMotion-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.224620 pyobjc-framework-CoreMotion-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.165339 pyobjc-framework-CoreMotion-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.170112 pyobjc-framework-CoreMotion-9.2/Lib/CoreMotion/
+-rw-r--r--   0 ronald     (501) staff       (20)      772 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/Lib/CoreMotion/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18954 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/Lib/CoreMotion/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.177354 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-06-07 00:11:44.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1348 2023-06-07 00:11:44.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:11:44.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:54.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:11:44.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:11:44.000000 pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMotion-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.180328 pyobjc-framework-CoreMotion-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      766 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/Modules/_CoreMotion.m
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/Modules/_CoreMotion_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMotion-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreMotion-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-06-07 00:11:44.224203 pyobjc-framework-CoreMotion-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.204342 pyobjc-framework-CoreMotion-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmaccelerometer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmattitude.py
+-rw-r--r--   0 ronald     (501) staff       (20)      515 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmauthorization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1102 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmdevicemotion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1032 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      232 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmerrordomain.py
+-rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmfalldetectionevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmgyro.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmmagnetometer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      448 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmmotionactivity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1308 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmpedometer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1074 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmwatersubmersiondata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      439 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmwatersubmersionmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_coremotion.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.207314 pyobjc-framework-CoreMotion-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1489 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.2/metadata/CoreMotion.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:44.222967 pyobjc-framework-CoreMotion-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    67097 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68718 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81475 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    50635 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    59284 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    67098 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68719 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81476 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMotion-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreMotion-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:11:44.224732 pyobjc-framework-CoreMotion-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1160 2023-05-29 10:07:46.000000 pyobjc-framework-CoreMotion-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Lib/CoreMotion/__init__.py` & `pyobjc-framework-CoreMotion-9.2/Lib/CoreMotion/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Lib/CoreMotion/_metadata.py` & `pyobjc-framework-CoreMotion-9.2/Lib/CoreMotion/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/PKG-INFO` & `pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMotion
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMotion on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMotion
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Lib/pyobjc_framework_CoreMotion.egg-info/SOURCES.txt` & `pyobjc-framework-CoreMotion-9.2/Lib/pyobjc_framework_CoreMotion.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreMotion/__init__.py
 Lib/CoreMotion/_metadata.py
 Lib/pyobjc_framework_CoreMotion.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreMotion.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreMotion.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreMotion.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreMotion-9.1b1/License.txt` & `pyobjc-framework-CoreMotion-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Modules/_CoreMotion.m` & `pyobjc-framework-CoreMotion-9.2/Modules/_CoreMotion.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreMotion-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreMotion-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PKG-INFO` & `pyobjc-framework-CoreMotion-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMotion
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMotion on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMotion
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmattitude.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmattitude.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmauthorization.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmauthorization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmdevicemotion.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmdevicemotion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmerror.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmfalldetectionevent.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmfalldetectionevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmpedometer.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmpedometer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/PyObjCTest/test_cmwatersubmersiondata.py` & `pyobjc-framework-CoreMotion-9.2/PyObjCTest/test_cmwatersubmersiondata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/CoreMotion.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/CoreMotion.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreMotion-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreMotion-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMotion-9.1b1/setup.py` & `pyobjc-framework-CoreMotion-9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import setup, Extension
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-CoreMotion",
     description="Wrappers for the framework CoreMotion on macOS",
     min_os_level="10.15",
     packages=["CoreMotion"],
     ext_modules=[
```
