# Comparing `tmp/pyobjc-framework-CoreBluetooth-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreBluetooth-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreBluetooth-9.1b1.tar", last modified: Sun Mar 26 11:20:00 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreBluetooth-9.2.tar", last modified: Wed Jun  7 00:10:05 2023, max compression
```

## Comparing `pyobjc-framework-CoreBluetooth-9.1b1.tar` & `pyobjc-framework-CoreBluetooth-9.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.334667 pyobjc-framework-CoreBluetooth-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreBluetooth-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.118310 pyobjc-framework-CoreBluetooth-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.182077 pyobjc-framework-CoreBluetooth-9.1b1/Lib/CoreBluetooth/
--rw-r--r--   0 ronald     (501) staff       (20)      797 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/CoreBluetooth/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    18277 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/CoreBluetooth/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.270831 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2150 2023-03-26 11:20:00.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1385 2023-03-26 11:20:00.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:20:00.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:43.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:20:00.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:20:00.000000 pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.276999 pyobjc-framework-CoreBluetooth-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1122 2021-10-18 19:38:40.000000 pyobjc-framework-CoreBluetooth-9.1b1/Modules/_CoreBluetooth.m
--rw-r--r--   0 ronald     (501) staff       (20)      530 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/Modules/_CoreBluetooth_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreBluetooth-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreBluetooth-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1939 2023-03-26 11:20:00.334197 pyobjc-framework-CoreBluetooth-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.297171 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      917 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbadvertisementdata.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbattrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcentral.py
--rw-r--r--   0 ronald     (501) staff       (20)     2143 2022-06-26 21:30:09.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcentralmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     2110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcentralmanagerconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     2117 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcharacteristic.py
--rw-r--r--   0 ronald     (501) staff       (20)      345 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     3032 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cberror.py
--rw-r--r--   0 ronald     (501) staff       (20)      841 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbmananager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1483 2022-06-25 09:08:12.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheral.py
--rw-r--r--   0 ronald     (501) staff       (20)     3589 2022-06-26 21:30:09.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheralmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      643 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheralmanagerconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      610 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbservice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1880 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbuuid.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_corebluetooth.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-CoreBluetooth-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.305060 pyobjc-framework-CoreBluetooth-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     4470 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/CoreBluetooth.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       37 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:00.332962 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    62548 2021-07-30 09:00:37.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    56244 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    62042 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    62539 2021-03-21 10:08:22.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    62549 2021-07-30 09:00:37.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63306 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreBluetooth-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:20:00.334756 pyobjc-framework-CoreBluetooth-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2023-03-25 14:20:30.000000 pyobjc-framework-CoreBluetooth-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.423833 pyobjc-framework-CoreBluetooth-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreBluetooth-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.364102 pyobjc-framework-CoreBluetooth-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.373557 pyobjc-framework-CoreBluetooth-9.2/Lib/CoreBluetooth/
+-rw-r--r--   0 ronald     (501) staff       (20)      797 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/CoreBluetooth/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18277 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/CoreBluetooth/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.377359 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2148 2023-06-07 00:10:05.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1400 2023-06-07 00:10:05.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:10:05.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:43.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:10:05.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:10:05.000000 pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.391400 pyobjc-framework-CoreBluetooth-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1122 2021-10-18 19:38:40.000000 pyobjc-framework-CoreBluetooth-9.2/Modules/_CoreBluetooth.m
+-rw-r--r--   0 ronald     (501) staff       (20)      530 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/Modules/_CoreBluetooth_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreBluetooth-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreBluetooth-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1937 2023-06-07 00:10:05.423457 pyobjc-framework-CoreBluetooth-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.412615 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      917 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbadvertisementdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbattrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcentral.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2143 2022-06-26 21:30:09.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcentralmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcentralmanagerconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcharacteristic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      345 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3032 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cberror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      841 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbmananager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1483 2022-06-25 09:08:12.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheral.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3589 2022-06-26 21:30:09.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheralmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      643 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheralmanagerconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      610 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1880 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbuuid.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_corebluetooth.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-CoreBluetooth-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.413735 pyobjc-framework-CoreBluetooth-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     4470 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/CoreBluetooth.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       37 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:05.422357 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    62548 2021-07-30 09:00:37.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    56244 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    62042 2020-11-30 18:45:14.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    62539 2021-03-21 10:08:22.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    62549 2021-07-30 09:00:37.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63306 2022-02-24 08:47:16.000000 pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreBluetooth-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreBluetooth-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:10:05.423942 pyobjc-framework-CoreBluetooth-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1245 2023-05-29 10:07:45.000000 pyobjc-framework-CoreBluetooth-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/LICENSE.txt` & `pyobjc-framework-CoreBluetooth-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Lib/CoreBluetooth/__init__.py` & `pyobjc-framework-CoreBluetooth-9.2/Lib/CoreBluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Lib/CoreBluetooth/_metadata.py` & `pyobjc-framework-CoreBluetooth-9.2/Lib/CoreBluetooth/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/PKG-INFO` & `pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreBluetooth
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreBluetooth on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreBluetooth
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Lib/pyobjc_framework_CoreBluetooth.egg-info/SOURCES.txt` & `pyobjc-framework-CoreBluetooth-9.2/Lib/pyobjc_framework_CoreBluetooth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreBluetooth/__init__.py
 Lib/CoreBluetooth/_metadata.py
 Lib/pyobjc_framework_CoreBluetooth.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreBluetooth.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreBluetooth.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreBluetooth.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Modules/_CoreBluetooth.m` & `pyobjc-framework-CoreBluetooth-9.2/Modules/_CoreBluetooth.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Modules/_CoreBluetooth_protocols.m` & `pyobjc-framework-CoreBluetooth-9.2/Modules/_CoreBluetooth_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreBluetooth-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreBluetooth-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PKG-INFO` & `pyobjc-framework-CoreBluetooth-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreBluetooth
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreBluetooth on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreBluetooth
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbadvertisementdata.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbadvertisementdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcentralmanager.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcentralmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcentralmanagerconstants.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcentralmanagerconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbcharacteristic.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbcharacteristic.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cberror.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cberror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbmananager.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbmananager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheral.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheral.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheralmanager.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheralmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbperipheralmanagerconstants.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbperipheralmanagerconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbservice.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/PyObjCTest/test_cbuuid.py` & `pyobjc-framework-CoreBluetooth-9.2/PyObjCTest/test_cbuuid.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/CoreBluetooth.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/CoreBluetooth.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreBluetooth-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreBluetooth-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreBluetooth-9.1b1/setup.py` & `pyobjc-framework-CoreBluetooth-9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,22 @@
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
     name="pyobjc-framework-CoreBluetooth",
     description="Wrappers for the framework CoreBluetooth on macOS",
     min_os_level="10.10",
     packages=["CoreBluetooth"],
     ext_modules=[
```

