# Comparing `tmp/pyobjc-framework-SystemConfiguration-9.1b1.tar.gz` & `tmp/pyobjc-framework-SystemConfiguration-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SystemConfiguration-9.1b1.tar", last modified: Sun Mar 26 11:42:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-SystemConfiguration-9.2.tar", last modified: Wed Jun  7 00:30:17 2023, max compression
```

## Comparing `pyobjc-framework-SystemConfiguration-9.1b1.tar` & `pyobjc-framework-SystemConfiguration-9.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.797946 pyobjc-framework-SystemConfiguration-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.729626 pyobjc-framework-SystemConfiguration-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.745677 pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/
--rw-r--r--   0 ronald     (501) staff       (20)      267 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1669 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/callbacks.py
--rw-r--r--   0 ronald     (501) staff       (20)     2170 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/interneton.py
--rw-r--r--   0 ronald     (501) staff       (20)      871 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/netcon.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.730646 pyobjc-framework-SystemConfiguration-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.747036 pyobjc-framework-SystemConfiguration-9.1b1/Lib/SystemConfiguration/
--rw-r--r--   0 ronald     (501) staff       (20)      993 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/SystemConfiguration/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    55428 2023-03-25 13:55:06.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/SystemConfiguration/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.751601 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2151 2023-03-26 11:42:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1930 2023-03-26 11:42:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:51.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:42:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       20 2023-03-26 11:42:34.000000 pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.753718 pyobjc-framework-SystemConfiguration-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    14176 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.1b1/Modules/_manual.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SystemConfiguration-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1940 2023-03-26 11:42:34.797484 pyobjc-framework-SystemConfiguration-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.764280 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      778 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_DHCPClientPreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)     4543 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1547 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreCopyDHCPInfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     1184 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreCopySpecific.py
--rw-r--r--   0 ronald     (501) staff       (20)     1930 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreKey.py
--rw-r--r--   0 ronald     (501) staff       (20)      485 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_captivenetwork.py
--rw-r--r--   0 ronald     (501) staff       (20)     2101 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetwork.py
--rw-r--r--   0 ronald     (501) staff       (20)    18901 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     5059 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     4551 2022-01-02 11:04:26.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkreachability.py
--rw-r--r--   0 ronald     (501) staff       (20)     3705 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)     1367 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferencespath.py
--rw-r--r--   0 ronald     (501) staff       (20)      756 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferencessetspecific.py
--rw-r--r--   0 ronald     (501) staff       (20)    26335 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scschemadefinitions.py
--rw-r--r--   0 ronald     (501) staff       (20)     2477 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_systemconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      519 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.766028 pyobjc-framework-SystemConfiguration-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    40387 2023-03-25 13:55:06.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/SystemConfiguration.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:34.795760 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    93136 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93385 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    95118 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    77156 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93137 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76068 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76238 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    77246 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93137 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    93386 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    95119 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:34.798052 pyobjc-framework-SystemConfiguration-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      873 2023-03-25 14:20:32.000000 pyobjc-framework-SystemConfiguration-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.760213 pyobjc-framework-SystemConfiguration-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.688154 pyobjc-framework-SystemConfiguration-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.698958 pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/
+-rw-r--r--   0 ronald     (501) staff       (20)      267 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1669 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/callbacks.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2170 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/interneton.py
+-rw-r--r--   0 ronald     (501) staff       (20)      871 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/netcon.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemConfiguration-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.688699 pyobjc-framework-SystemConfiguration-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.700866 pyobjc-framework-SystemConfiguration-9.2/Lib/SystemConfiguration/
+-rw-r--r--   0 ronald     (501) staff       (20)      993 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/SystemConfiguration/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    55428 2023-03-25 13:55:06.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/SystemConfiguration/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.712433 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2149 2023-06-07 00:30:17.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1945 2023-06-07 00:30:17.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:30:17.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:51.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:30:17.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       20 2023-06-07 00:30:17.000000 pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.715468 pyobjc-framework-SystemConfiguration-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    14176 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.2/Modules/_manual.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SystemConfiguration-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1938 2023-06-07 00:30:17.759801 pyobjc-framework-SystemConfiguration-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.736619 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      778 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_DHCPClientPreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4543 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1547 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreCopyDHCPInfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1184 2022-10-18 09:53:24.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreCopySpecific.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1930 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreKey.py
+-rw-r--r--   0 ronald     (501) staff       (20)      485 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_captivenetwork.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2101 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetwork.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18901 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5059 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4551 2022-01-02 11:04:26.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkreachability.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3705 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1367 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferencespath.py
+-rw-r--r--   0 ronald     (501) staff       (20)      756 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferencessetspecific.py
+-rw-r--r--   0 ronald     (501) staff       (20)    26335 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scschemadefinitions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2477 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_systemconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      519 2021-10-18 19:38:40.000000 pyobjc-framework-SystemConfiguration-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.738715 pyobjc-framework-SystemConfiguration-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    40387 2023-03-25 13:55:06.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/SystemConfiguration.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:15.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:17.758040 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    93136 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93385 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    95118 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    77156 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93137 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76068 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76238 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    77246 2021-03-21 10:08:23.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93137 2021-07-30 09:00:38.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    93386 2022-02-24 08:47:17.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    95119 2023-02-19 10:50:37.000000 pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemConfiguration-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SystemConfiguration-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:30:17.760307 pyobjc-framework-SystemConfiguration-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      955 2023-05-29 10:07:47.000000 pyobjc-framework-SystemConfiguration-9.2/setup.py
```

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/callbacks.py` & `pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/interneton.py` & `pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/interneton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Examples/CallbackDemo/netcon.py` & `pyobjc-framework-SystemConfiguration-9.2/Examples/CallbackDemo/netcon.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/LICENSE.txt` & `pyobjc-framework-SystemConfiguration-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Lib/SystemConfiguration/__init__.py` & `pyobjc-framework-SystemConfiguration-9.2/Lib/SystemConfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Lib/SystemConfiguration/_metadata.py` & `pyobjc-framework-SystemConfiguration-9.2/Lib/SystemConfiguration/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/PKG-INFO` & `pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemConfiguration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SystemConfiguration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemConfiguration
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Lib/pyobjc_framework_SystemConfiguration.egg-info/SOURCES.txt` & `pyobjc-framework-SystemConfiguration-9.2/Lib/pyobjc_framework_SystemConfiguration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/CallbackDemo/ReadMe.txt
 Examples/CallbackDemo/callbacks.py
 Examples/CallbackDemo/interneton.py
 Examples/CallbackDemo/netcon.py
 Lib/SystemConfiguration/__init__.py
 Lib/SystemConfiguration/_metadata.py
```

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Modules/_manual.m` & `pyobjc-framework-SystemConfiguration-9.2/Modules/_manual.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SystemConfiguration-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SystemConfiguration-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PKG-INFO` & `pyobjc-framework-SystemConfiguration-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemConfiguration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SystemConfiguration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemConfiguration
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_DHCPClientPreferences.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_DHCPClientPreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStore.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreCopyDHCPInfo.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreCopyDHCPInfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreCopySpecific.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreCopySpecific.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_SCDynamicStoreKey.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_SCDynamicStoreKey.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetwork.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetwork.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkconfiguration.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkconnection.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scnetworkreachability.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scnetworkreachability.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferences.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferencespath.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferencespath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scpreferencessetspecific.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scpreferencessetspecific.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_scschemadefinitions.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_scschemadefinitions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/PyObjCTest/test_systemconfiguration.py` & `pyobjc-framework-SystemConfiguration-9.2/PyObjCTest/test_systemconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/README.txt` & `pyobjc-framework-SystemConfiguration-9.2/README.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/SystemConfiguration.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/SystemConfiguration.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-SystemConfiguration-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SystemConfiguration-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemConfiguration-9.1b1/setup.py` & `pyobjc-framework-SystemConfiguration-9.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 Wrappers for framework 'SystemConfiguration'.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-from pyobjc_setup import Extension, setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-SystemConfiguration",
     description="Wrappers for the framework SystemConfiguration on macOS",
     packages=["SystemConfiguration"],
     ext_modules=[
         Extension(
```

