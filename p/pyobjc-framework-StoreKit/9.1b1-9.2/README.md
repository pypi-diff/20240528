# Comparing `tmp/pyobjc-framework-StoreKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-StoreKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-StoreKit-9.1b1.tar", last modified: Sun Mar 26 11:42:03 2023, max compression
+gzip compressed data, was "pyobjc-framework-StoreKit-9.2.tar", last modified: Wed Jun  7 00:29:49 2023, max compression
```

## Comparing `pyobjc-framework-StoreKit-9.1b1.tar` & `pyobjc-framework-StoreKit-9.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.926461 pyobjc-framework-StoreKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.740007 pyobjc-framework-StoreKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.790957 pyobjc-framework-StoreKit-9.1b1/Lib/StoreKit/
--rw-r--r--   0 ronald     (501) staff       (20)      910 2023-02-19 10:50:35.000000 pyobjc-framework-StoreKit-9.1b1/Lib/StoreKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    20234 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/Lib/StoreKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.794919 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-03-26 11:42:03.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1573 2023-03-26 11:42:03.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:03.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:47.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:42:03.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:42:03.000000 pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-StoreKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.797648 pyobjc-framework-StoreKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-StoreKit-9.1b1/Modules/_StoreKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      855 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/Modules/_StoreKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-StoreKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-03-26 11:42:03.925921 pyobjc-framework-StoreKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.852484 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       23 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      634 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skarcadeservice.py
--rw-r--r--   0 ronald     (501) staff       (20)     2366 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skcloudservicecontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      646 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skdownload.py
--rw-r--r--   0 ronald     (501) staff       (20)     1222 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      359 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skpayment.py
--rw-r--r--   0 ronald     (501) staff       (20)      934 2022-06-25 20:09:26.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skpaymentqueue.py
--rw-r--r--   0 ronald     (501) staff       (20)      594 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skpaymenttransaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      830 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproduct.py
--rw-r--r--   0 ronald     (501) staff       (20)      670 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproductdiscount.py
--rw-r--r--   0 ronald     (501) staff       (20)      209 2022-06-25 20:15:13.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproductsrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1228 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproductstorepromotioncontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      505 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skreceiptrefreshrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      193 2022-06-25 20:17:44.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1282 2022-06-25 20:07:05.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skstoreproductviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      467 2022-06-25 20:15:25.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_storekit.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_storekitdefines.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.854591 pyobjc-framework-StoreKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1995 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/metadata/StoreKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:03.924177 pyobjc-framework-StoreKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    92110 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93297 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97685 2022-10-18 09:53:23.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97685 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27319 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    57040 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80138 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11824 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16193 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    92111 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93298 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97686 2022-10-18 09:53:23.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97686 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-StoreKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:03.926583 pyobjc-framework-StoreKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1142 2023-03-25 14:20:32.000000 pyobjc-framework-StoreKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.517529 pyobjc-framework-StoreKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.447723 pyobjc-framework-StoreKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.456972 pyobjc-framework-StoreKit-9.2/Lib/StoreKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      910 2023-02-19 10:50:35.000000 pyobjc-framework-StoreKit-9.2/Lib/StoreKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20234 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/Lib/StoreKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.461039 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2115 2023-06-07 00:29:49.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1588 2023-06-07 00:29:49.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:29:49.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:47.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:29:49.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:29:49.000000 pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-StoreKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.463844 pyobjc-framework-StoreKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-StoreKit-9.2/Modules/_StoreKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      855 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/Modules/_StoreKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-StoreKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1904 2023-06-07 00:29:49.516764 pyobjc-framework-StoreKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.496157 pyobjc-framework-StoreKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       23 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      634 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skarcadeservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2366 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skcloudservicecontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      646 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skdownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1222 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      359 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skpayment.py
+-rw-r--r--   0 ronald     (501) staff       (20)      934 2022-06-25 20:09:26.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skpaymentqueue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      594 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skpaymenttransaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      830 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproduct.py
+-rw-r--r--   0 ronald     (501) staff       (20)      670 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproductdiscount.py
+-rw-r--r--   0 ronald     (501) staff       (20)      209 2022-06-25 20:15:13.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproductsrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1228 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproductstorepromotioncontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      505 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skreceiptrefreshrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      193 2022-06-25 20:17:44.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1282 2022-06-25 20:07:05.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skstoreproductviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      467 2022-06-25 20:15:25.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_storekit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/PyObjCTest/test_storekitdefines.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.498566 pyobjc-framework-StoreKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1995 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/metadata/StoreKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:49.515369 pyobjc-framework-StoreKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    92110 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93297 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97685 2022-10-18 09:53:23.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97685 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27319 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    57040 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80138 2021-03-21 10:08:23.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11824 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16193 2020-11-30 18:45:15.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    92111 2021-07-30 09:00:38.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93298 2022-02-24 08:47:17.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97686 2022-10-18 09:53:23.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97686 2023-02-19 10:50:37.000000 pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-StoreKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-StoreKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:29:49.517626 pyobjc-framework-StoreKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1213 2023-05-29 10:07:47.000000 pyobjc-framework-StoreKit-9.2/setup.py
```

### Comparing `pyobjc-framework-StoreKit-9.1b1/Lib/StoreKit/__init__.py` & `pyobjc-framework-StoreKit-9.2/Lib/StoreKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Lib/StoreKit/_metadata.py` & `pyobjc-framework-StoreKit-9.2/Lib/StoreKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/PKG-INFO` & `pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-StoreKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework StoreKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,StoreKit
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-StoreKit-9.1b1/Lib/pyobjc_framework_StoreKit.egg-info/SOURCES.txt` & `pyobjc-framework-StoreKit-9.2/Lib/pyobjc_framework_StoreKit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/StoreKit/__init__.py
 Lib/StoreKit/_metadata.py
 Lib/pyobjc_framework_StoreKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_StoreKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_StoreKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_StoreKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-StoreKit-9.1b1/License.txt` & `pyobjc-framework-StoreKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Modules/_StoreKit.m` & `pyobjc-framework-StoreKit-9.2/Modules/_StoreKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Modules/_StoreKit_protocols.m` & `pyobjc-framework-StoreKit-9.2/Modules/_StoreKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-StoreKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-StoreKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-StoreKit-9.1b1/PKG-INFO` & `pyobjc-framework-StoreKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-StoreKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework StoreKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,StoreKit
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skarcadeservice.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skarcadeservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skcloudservicecontroller.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skcloudservicecontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skdownload.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skdownload.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skerror.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skpaymentqueue.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skpaymentqueue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skpaymenttransaction.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skpaymenttransaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproduct.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproduct.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproductdiscount.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproductdiscount.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skproductstorepromotioncontroller.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skproductstorepromotioncontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/PyObjCTest/test_skstoreproductviewcontroller.py` & `pyobjc-framework-StoreKit-9.2/PyObjCTest/test_skstoreproductviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/StoreKit.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/StoreKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-StoreKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-StoreKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-StoreKit-9.1b1/setup.py` & `pyobjc-framework-StoreKit-9.2/setup.py`

 * *Files 7% similar despite different names*

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
     name="pyobjc-framework-StoreKit",
     description="Wrappers for the framework StoreKit on macOS",
     min_os_level="10.7",
     packages=["StoreKit"],
     ext_modules=[
```

