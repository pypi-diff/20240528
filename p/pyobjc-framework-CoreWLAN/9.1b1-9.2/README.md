# Comparing `tmp/pyobjc-framework-CoreWLAN-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreWLAN-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreWLAN-9.1b1.tar", last modified: Sun Mar 26 11:22:35 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreWLAN-9.2.tar", last modified: Wed Jun  7 00:12:37 2023, max compression
```

## Comparing `pyobjc-framework-CoreWLAN-9.1b1.tar` & `pyobjc-framework-CoreWLAN-9.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.104185 pyobjc-framework-CoreWLAN-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.037022 pyobjc-framework-CoreWLAN-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)      564 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.1b1/Examples/toggle-wlan.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.033301 pyobjc-framework-CoreWLAN-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.038525 pyobjc-framework-CoreWLAN-9.1b1/Lib/CoreWLAN/
--rw-r--r--   0 ronald     (501) staff       (20)     2879 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/CoreWLAN/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    18023 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/CoreWLAN/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.054069 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2103 2023-03-26 11:22:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1412 2023-03-26 11:22:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:22:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:56.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:22:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:22:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreWLAN-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.056933 pyobjc-framework-CoreWLAN-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-CoreWLAN-9.1b1/Modules/_CoreWLAN.m
--rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/Modules/_CoreWLAN_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreWLAN-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1892 2023-03-26 11:22:35.103873 pyobjc-framework-CoreWLAN-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.066870 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       31 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      452 2022-04-11 08:03:15.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlan.py
--rw-r--r--   0 ronald     (501) staff       (20)     2353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlanconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     9462 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlantypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     2031 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlanutil.py
--rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cw8021xprofile.py
--rw-r--r--   0 ronald     (501) staff       (20)      523 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwchannel.py
--rw-r--r--   0 ronald     (501) staff       (20)     2423 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     4813 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwinterface.py
--rw-r--r--   0 ronald     (501) staff       (20)      893 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwnetwork.py
--rw-r--r--   0 ronald     (501) staff       (20)      563 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwnetworkprofile.py
--rw-r--r--   0 ronald     (501) staff       (20)     1389 2022-06-25 09:09:38.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwwificlient.py
--rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwwirelessprofile.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.068197 pyobjc-framework-CoreWLAN-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     5554 2021-06-10 09:09:03.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/CoreWLAN.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:35.102454 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    44844 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45302 2022-02-24 08:47:16.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45828 2022-06-25 20:19:21.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45856 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43304 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44462 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44821 2021-03-21 10:08:22.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40040 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40040 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44845 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45303 2022-02-24 08:47:16.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45829 2022-06-25 20:19:21.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45857 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreWLAN-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:22:35.104432 pyobjc-framework-CoreWLAN-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1128 2023-03-25 14:20:31.000000 pyobjc-framework-CoreWLAN-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.603429 pyobjc-framework-CoreWLAN-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.544846 pyobjc-framework-CoreWLAN-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)      564 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.2/Examples/toggle-wlan.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.540191 pyobjc-framework-CoreWLAN-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.549856 pyobjc-framework-CoreWLAN-9.2/Lib/CoreWLAN/
+-rw-r--r--   0 ronald     (501) staff       (20)     2879 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/Lib/CoreWLAN/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18023 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.2/Lib/CoreWLAN/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.554067 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2101 2023-06-07 00:12:37.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1427 2023-06-07 00:12:37.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:12:37.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:56.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:12:37.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:12:37.000000 pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreWLAN-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.556568 pyobjc-framework-CoreWLAN-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-CoreWLAN-9.2/Modules/_CoreWLAN.m
+-rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/Modules/_CoreWLAN_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreWLAN-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1890 2023-06-07 00:12:37.602983 pyobjc-framework-CoreWLAN-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.565638 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       31 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      452 2022-04-11 08:03:15.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlan.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlanconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9462 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlantypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2031 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlanutil.py
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cw8021xprofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)      523 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwchannel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2423 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4813 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwinterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)      893 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwnetwork.py
+-rw-r--r--   0 ronald     (501) staff       (20)      563 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwnetworkprofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1389 2022-06-25 09:09:38.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwwificlient.py
+-rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwwirelessprofile.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.577643 pyobjc-framework-CoreWLAN-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     5554 2021-06-10 09:09:03.000000 pyobjc-framework-CoreWLAN-9.2/metadata/CoreWLAN.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:37.601553 pyobjc-framework-CoreWLAN-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    44844 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45302 2022-02-24 08:47:16.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45828 2022-06-25 20:19:21.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45856 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43304 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44462 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44821 2021-03-21 10:08:22.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40040 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40040 2020-11-30 18:45:14.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44845 2021-07-30 09:00:37.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45303 2022-02-24 08:47:16.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45829 2022-06-25 20:19:21.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45857 2023-02-19 10:50:35.000000 pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreWLAN-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreWLAN-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:12:37.603548 pyobjc-framework-CoreWLAN-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1199 2023-05-29 10:07:46.000000 pyobjc-framework-CoreWLAN-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Examples/toggle-wlan.py` & `pyobjc-framework-CoreWLAN-9.2/Examples/toggle-wlan.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Lib/CoreWLAN/__init__.py` & `pyobjc-framework-CoreWLAN-9.2/Lib/CoreWLAN/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Lib/CoreWLAN/_metadata.py` & `pyobjc-framework-CoreWLAN-9.2/Lib/CoreWLAN/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/PKG-INFO` & `pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreWLAN
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreWLAN on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreWLAN
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Lib/pyobjc_framework_CoreWLAN.egg-info/SOURCES.txt` & `pyobjc-framework-CoreWLAN-9.2/Lib/pyobjc_framework_CoreWLAN.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/toggle-wlan.py
 Lib/CoreWLAN/__init__.py
 Lib/CoreWLAN/_metadata.py
 Lib/pyobjc_framework_CoreWLAN.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreWLAN.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreWLAN.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/License.txt` & `pyobjc-framework-CoreWLAN-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Modules/_CoreWLAN.m` & `pyobjc-framework-CoreWLAN-9.2/Modules/_CoreWLAN.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreWLAN-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreWLAN-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PKG-INFO` & `pyobjc-framework-CoreWLAN-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreWLAN
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreWLAN on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreWLAN
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlanconstants.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlanconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlantypes.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlantypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_corewlanutil.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_corewlanutil.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cw8021xprofile.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cw8021xprofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwchannel.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwchannel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwconfiguration.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwinterface.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwinterface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwnetwork.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwnetwork.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwnetworkprofile.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwnetworkprofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/PyObjCTest/test_cwwificlient.py` & `pyobjc-framework-CoreWLAN-9.2/PyObjCTest/test_cwwificlient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/CoreWLAN.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/CoreWLAN.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-CoreWLAN-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreWLAN-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreWLAN-9.1b1/setup.py` & `pyobjc-framework-CoreWLAN-9.2/setup.py`

 * *Files 12% similar despite different names*

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
     name="pyobjc-framework-CoreWLAN",
     description="Wrappers for the framework CoreWLAN on macOS",
     min_os_level="10.6",
     packages=["CoreWLAN"],
     ext_modules=[
```

