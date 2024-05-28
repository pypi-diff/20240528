# Comparing `tmp/pyobjc-framework-PassKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-PassKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PassKit-9.1b1.tar", last modified: Sun Mar 26 11:33:13 2023, max compression
+gzip compressed data, was "pyobjc-framework-PassKit-9.2.tar", last modified: Wed Jun  7 00:23:06 2023, max compression
```

## Comparing `pyobjc-framework-PassKit-9.1b1.tar` & `pyobjc-framework-PassKit-9.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:13.072664 pyobjc-framework-PassKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.842781 pyobjc-framework-PassKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.895395 pyobjc-framework-PassKit-9.1b1/Lib/PassKit/
--rw-r--r--   0 ronald     (501) staff       (20)      719 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/Lib/PassKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    40400 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.1b1/Lib/PassKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.898811 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-03-26 11:33:12.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1837 2023-03-26 11:33:12.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:33:12.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:02.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:33:12.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:33:12.000000 pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PassKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.902004 pyobjc-framework-PassKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      748 2021-10-18 19:38:40.000000 pyobjc-framework-PassKit-9.1b1/Modules/_PassKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      553 2021-10-18 19:38:40.000000 pyobjc-framework-PassKit-9.1b1/Modules/_PassKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-PassKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2023-03-26 11:33:13.072171 pyobjc-framework-PassKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.971717 pyobjc-framework-PassKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1424 2022-10-18 09:53:24.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_PKAddShareablePassConfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_passkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      664 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkaddpaymentpassrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      557 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkbarcodeeventmetadatarequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     5396 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2022-06-25 20:08:29.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkdisbursementauthorizationcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      384 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkdisbursementrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     2480 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      909 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkissuerprovisioningextensionstatus.py
--rw-r--r--   0 ronald     (501) staff       (20)      464 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpass.py
--rw-r--r--   0 ronald     (501) staff       (20)     3943 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpasslibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)     3828 2022-06-25 09:21:12.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      538 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     3587 2022-06-25 09:21:14.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationviewcontrollerdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1047 2022-06-25 20:11:41.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentinformationeventextension.py
--rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentmethod.py
--rw-r--r--   0 ronald     (501) staff       (20)      615 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentpass.py
--rw-r--r--   0 ronald     (501) staff       (20)     1997 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      367 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentsummaryitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      679 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pksecureelementpass.py
--rw-r--r--   0 ronald     (501) staff       (20)      688 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pksuicapassproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)      367 2021-04-09 09:35:36.000000 pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pktransitpassproperties.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:12.977735 pyobjc-framework-PassKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2166 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.1b1/metadata/PassKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:13.068924 pyobjc-framework-PassKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   165269 2021-10-26 11:32:35.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   166733 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   221369 2022-10-18 09:53:23.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   228521 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   143322 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-11.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   165271 2021-10-26 11:32:35.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   166734 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   221370 2022-10-18 09:53:23.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   228522 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PassKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:33:13.072784 pyobjc-framework-PassKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1119 2023-03-25 14:20:32.000000 pyobjc-framework-PassKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.921690 pyobjc-framework-PassKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.822174 pyobjc-framework-PassKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.832676 pyobjc-framework-PassKit-9.2/Lib/PassKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      719 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/Lib/PassKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    40400 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.2/Lib/PassKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.846136 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-06-07 00:23:06.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1852 2023-06-07 00:23:06.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:23:06.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:02.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:23:06.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:23:06.000000 pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PassKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.857951 pyobjc-framework-PassKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      748 2021-10-18 19:38:40.000000 pyobjc-framework-PassKit-9.2/Modules/_PassKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      553 2021-10-18 19:38:40.000000 pyobjc-framework-PassKit-9.2/Modules/_PassKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-PassKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:23:06.921093 pyobjc-framework-PassKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.896263 pyobjc-framework-PassKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1424 2022-10-18 09:53:24.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_PKAddShareablePassConfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_passkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      664 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkaddpaymentpassrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      557 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkbarcodeeventmetadatarequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5396 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2022-06-25 20:08:29.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkdisbursementauthorizationcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      384 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkdisbursementrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2480 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      909 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkissuerprovisioningextensionstatus.py
+-rw-r--r--   0 ronald     (501) staff       (20)      464 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3943 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpasslibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3828 2022-06-25 09:21:12.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      538 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3587 2022-06-25 09:21:14.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationviewcontrollerdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1047 2022-06-25 20:11:41.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentinformationeventextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentmethod.py
+-rw-r--r--   0 ronald     (501) staff       (20)      615 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentpass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1997 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      367 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentsummaryitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      679 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pksecureelementpass.py
+-rw-r--r--   0 ronald     (501) staff       (20)      688 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pksuicapassproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      367 2021-04-09 09:35:36.000000 pyobjc-framework-PassKit-9.2/PyObjCTest/test_pktransitpassproperties.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.898422 pyobjc-framework-PassKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2166 2022-06-15 11:57:00.000000 pyobjc-framework-PassKit-9.2/metadata/PassKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:06.917185 pyobjc-framework-PassKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   165269 2021-10-26 11:32:35.000000 pyobjc-framework-PassKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   166733 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   221369 2022-10-18 09:53:23.000000 pyobjc-framework-PassKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   228521 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   143322 2021-03-21 10:08:23.000000 pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-11.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   165271 2021-10-26 11:32:35.000000 pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   166734 2022-02-24 08:47:16.000000 pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   221370 2022-10-18 09:53:23.000000 pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   228522 2023-02-19 10:50:35.000000 pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PassKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PassKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:23:06.921797 pyobjc-framework-PassKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1190 2023-05-29 10:07:47.000000 pyobjc-framework-PassKit-9.2/setup.py
```

### Comparing `pyobjc-framework-PassKit-9.1b1/Lib/PassKit/__init__.py` & `pyobjc-framework-PassKit-9.2/Lib/PassKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Lib/PassKit/_metadata.py` & `pyobjc-framework-PassKit-9.2/Lib/PassKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/PKG-INFO` & `pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PassKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PassKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PassKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-PassKit-9.1b1/Lib/pyobjc_framework_PassKit.egg-info/SOURCES.txt` & `pyobjc-framework-PassKit-9.2/Lib/pyobjc_framework_PassKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PassKit/__init__.py
 Lib/PassKit/_metadata.py
 Lib/pyobjc_framework_PassKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_PassKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PassKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PassKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PassKit-9.1b1/License.txt` & `pyobjc-framework-PassKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Modules/_PassKit.m` & `pyobjc-framework-PassKit-9.2/Modules/_PassKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Modules/_PassKit_protocols.m` & `pyobjc-framework-PassKit-9.2/Modules/_PassKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-PassKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-PassKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-PassKit-9.1b1/PKG-INFO` & `pyobjc-framework-PassKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PassKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PassKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PassKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_PKAddShareablePassConfiguration.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_PKAddShareablePassConfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkaddpaymentpassrequest.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkaddpaymentpassrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkbarcodeeventmetadatarequest.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkbarcodeeventmetadatarequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkconstants.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkerror.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkissuerprovisioningextensionstatus.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkissuerprovisioningextensionstatus.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpasslibrary.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpasslibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationcontroller.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationviewcontroller.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentauthorizationviewcontrollerdelegate.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentauthorizationviewcontrollerdelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentinformationeventextension.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentinformationeventextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentmethod.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentmethod.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentpass.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentpass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pkpaymentrequest.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pkpaymentrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pksecureelementpass.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pksecureelementpass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/PyObjCTest/test_pksuicapassproperties.py` & `pyobjc-framework-PassKit-9.2/PyObjCTest/test_pksuicapassproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/PassKit.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/PassKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-11.0.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-11.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-PassKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PassKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PassKit-9.1b1/setup.py` & `pyobjc-framework-PassKit-9.2/setup.py`

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
 
-from pyobjc_setup import setup, Extension
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-PassKit",
     description="Wrappers for the framework PassKit on macOS",
     min_os_level="10.16",
     packages=["PassKit"],
     ext_modules=[
```

