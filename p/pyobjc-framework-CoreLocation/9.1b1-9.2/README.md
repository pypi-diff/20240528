# Comparing `tmp/pyobjc-framework-CoreLocation-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreLocation-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreLocation-9.1b1.tar", last modified: Sun Mar 26 11:20:38 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreLocation-9.2.tar", last modified: Wed Jun  7 00:10:36 2023, max compression
```

## Comparing `pyobjc-framework-CoreLocation-9.1b1.tar` & `pyobjc-framework-CoreLocation-9.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.516967 pyobjc-framework-CoreLocation-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.436333 pyobjc-framework-CoreLocation-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.443967 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.444944 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)   200374 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/English.lproj/MainMenu.xib
--rw-r--r--   0 ronald     (501) staff       (20)      441 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/HTMLFormatString.html
--rw-r--r--   0 ronald     (501) staff       (20)      218 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)     4314 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/WhereIsMyMacAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      342 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreLocation-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.436947 pyobjc-framework-CoreLocation-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.450554 pyobjc-framework-CoreLocation-9.1b1/Lib/CoreLocation/
--rw-r--r--   0 ronald     (501) staff       (20)     1139 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/CoreLocation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    19239 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/CoreLocation/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.454222 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2277 2023-03-26 11:20:38.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1679 2023-03-26 11:20:38.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:20:38.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:46.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:20:38.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:20:38.000000 pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.457187 pyobjc-framework-CoreLocation-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1148 2021-10-18 19:38:40.000000 pyobjc-framework-CoreLocation-9.1b1/Modules/_CoreLocation.m
--rw-r--r--   0 ronald     (501) staff       (20)      291 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/Modules/_CoreLocation_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreLocation-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2066 2023-03-26 11:20:38.516543 pyobjc-framework-CoreLocation-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.482247 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      376 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clbeaconregion.py
--rw-r--r--   0 ronald     (501) staff       (20)      597 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clcircularregion.py
--rw-r--r--   0 ronald     (501) staff       (20)     2165 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      195 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clerrordomain.py
--rw-r--r--   0 ronald     (501) staff       (20)     1795 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clgeocoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clheading.py
--rw-r--r--   0 ronald     (501) staff       (20)     3211 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocation.py
--rw-r--r--   0 ronald     (501) staff       (20)     4500 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocationmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1073 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocationmanagerdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1303 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clregion.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_corelocation.py
--rw-r--r--   0 ronald     (501) staff       (20)      289 2021-10-18 19:38:40.000000 pyobjc-framework-CoreLocation-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.491412 pyobjc-framework-CoreLocation-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     4268 2021-07-31 12:28:11.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/CoreLocation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:38.515331 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    81944 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    82347 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85353 2022-10-19 09:49:10.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85413 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53134 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    70525 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76471 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6981 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    19168 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25604 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81945 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    82348 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85354 2022-10-19 09:49:10.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85414 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:20:38.517100 pyobjc-framework-CoreLocation-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1295 2023-03-25 14:20:30.000000 pyobjc-framework-CoreLocation-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.239332 pyobjc-framework-CoreLocation-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.166011 pyobjc-framework-CoreLocation-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.175031 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.179447 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)   200374 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/English.lproj/MainMenu.xib
+-rw-r--r--   0 ronald     (501) staff       (20)      441 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/HTMLFormatString.html
+-rw-r--r--   0 ronald     (501) staff       (20)      218 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     4314 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/WhereIsMyMacAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      342 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreLocation-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.166757 pyobjc-framework-CoreLocation-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.182255 pyobjc-framework-CoreLocation-9.2/Lib/CoreLocation/
+-rw-r--r--   0 ronald     (501) staff       (20)     1139 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Lib/CoreLocation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19239 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.2/Lib/CoreLocation/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.186451 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2275 2023-06-07 00:10:36.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1694 2023-06-07 00:10:36.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:10:36.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:46.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:10:36.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:10:36.000000 pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.188950 pyobjc-framework-CoreLocation-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1148 2021-10-18 19:38:40.000000 pyobjc-framework-CoreLocation-9.2/Modules/_CoreLocation.m
+-rw-r--r--   0 ronald     (501) staff       (20)      291 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/Modules/_CoreLocation_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreLocation-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2064 2023-06-07 00:10:36.238925 pyobjc-framework-CoreLocation-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.207476 pyobjc-framework-CoreLocation-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      376 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clbeaconregion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      597 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clcircularregion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2165 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      195 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clerrordomain.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1795 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clgeocoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clheading.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3211 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4651 2023-05-04 11:00:07.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocationmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1073 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocationmanagerdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1303 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clregion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_corelocation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2021-10-18 19:38:40.000000 pyobjc-framework-CoreLocation-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.209335 pyobjc-framework-CoreLocation-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     4268 2021-07-31 12:28:11.000000 pyobjc-framework-CoreLocation-9.2/metadata/CoreLocation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:36.237595 pyobjc-framework-CoreLocation-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    81944 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    82347 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85353 2022-10-19 09:49:10.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85413 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53134 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    70525 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76471 2021-03-21 10:08:22.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6981 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    19168 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25604 2020-11-30 18:45:14.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81945 2022-01-02 11:04:26.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    82348 2022-02-24 08:47:16.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85354 2022-10-19 09:49:10.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85414 2023-02-19 10:50:35.000000 pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreLocation-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreLocation-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:10:36.239598 pyobjc-framework-CoreLocation-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1366 2023-05-29 10:07:45.000000 pyobjc-framework-CoreLocation-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/English.lproj/MainMenu.xib` & `pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/English.lproj/MainMenu.xib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Examples/WhereIsMyMac/WhereIsMyMacAppDelegate.py` & `pyobjc-framework-CoreLocation-9.2/Examples/WhereIsMyMac/WhereIsMyMacAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/LICENSE.txt` & `pyobjc-framework-CoreLocation-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Lib/CoreLocation/__init__.py` & `pyobjc-framework-CoreLocation-9.2/Lib/CoreLocation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Lib/CoreLocation/_metadata.py` & `pyobjc-framework-CoreLocation-9.2/Lib/CoreLocation/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/PKG-INFO` & `pyobjc-framework-CoreLocation-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreLocation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreLocation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreLocation
 Platform: MacOS X (>=10.6)
@@ -26,17 +26,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for framework 'CoreLocation' on macOS 10.6. This framework provides
 an interface for dealing with the physical location of a machine, which allows
 for geo-aware applications.
 
 These wrappers don't include documentation, please check Apple's documentation
```

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Lib/pyobjc_framework_CoreLocation.egg-info/SOURCES.txt` & `pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/WhereIsMyMac/HTMLFormatString.html
 Examples/WhereIsMyMac/ReadMe.txt
 Examples/WhereIsMyMac/WhereIsMyMacAppDelegate.py
 Examples/WhereIsMyMac/main.py
 Examples/WhereIsMyMac/setup.py
 Examples/WhereIsMyMac/English.lproj/MainMenu.xib
```

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Modules/_CoreLocation.m` & `pyobjc-framework-CoreLocation-9.2/Modules/_CoreLocation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreLocation-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreLocation-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PKG-INFO` & `pyobjc-framework-CoreLocation-9.2/Lib/pyobjc_framework_CoreLocation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreLocation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreLocation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreLocation
 Platform: MacOS X (>=10.6)
@@ -26,14 +26,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for framework 'CoreLocation' on macOS 10.6. This framework provides
 an interface for dealing with the physical location of a machine, which allows
 for geo-aware applications.
 
 These wrappers don't include documentation, please check Apple's documentation
```

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clcircularregion.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clcircularregion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clerror.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clgeocoder.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clgeocoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocation.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocationmanager.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocationmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,21 +69,26 @@
         self.assertResultIsBOOL(CoreLocation.CLLocationManager.locationServicesEnabled)
         self.assertResultIsBOOL(
             CoreLocation.CLLocationManager.pausesLocationUpdatesAutomatically
         )
         self.assertArgIsBOOL(
             CoreLocation.CLLocationManager.setPausesLocationUpdatesAutomatically_, 0
         )
+        self.assertResultIsBOOL(CoreLocation.CLLocationManager.headingAvailable)
+
+    @min_os_level("10.12")
+    def testMethods10_12(self):
+        # Documentation claims there APIs are available on 10.11, in practice they aren't
+
         self.assertResultIsBOOL(
             CoreLocation.CLLocationManager.allowsBackgroundLocationUpdates
         )
         self.assertArgIsBOOL(
             CoreLocation.CLLocationManager.setAllowsBackgroundLocationUpdates_, 0
         )
-        self.assertResultIsBOOL(CoreLocation.CLLocationManager.headingAvailable)
 
     @min_os_level("10.15")
     def testMethods10_15(self):
         self.assertResultIsBOOL(CoreLocation.CLLocationManager.isRangingAvailable)
 
     @min_os_level("11.0")
     def testMethods11_0(self):
```

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_cllocationmanagerdelegate.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_cllocationmanagerdelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/PyObjCTest/test_clregion.py` & `pyobjc-framework-CoreLocation-9.2/PyObjCTest/test_clregion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/CoreLocation.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/CoreLocation.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-CoreLocation-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreLocation-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreLocation-9.1b1/setup.py` & `pyobjc-framework-CoreLocation-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
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
     name="pyobjc-framework-CoreLocation",
     description="Wrappers for the framework CoreLocation on macOS",
     min_os_level="10.6",
     packages=["CoreLocation"],
     ext_modules=[
```

