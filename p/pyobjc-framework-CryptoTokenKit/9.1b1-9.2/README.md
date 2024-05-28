# Comparing `tmp/pyobjc-framework-CryptoTokenKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-CryptoTokenKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CryptoTokenKit-9.1b1.tar", last modified: Sun Mar 26 11:22:46 2023, max compression
+gzip compressed data, was "pyobjc-framework-CryptoTokenKit-9.2.tar", last modified: Wed Jun  7 00:12:49 2023, max compression
```

## Comparing `pyobjc-framework-CryptoTokenKit-9.1b1.tar` & `pyobjc-framework-CryptoTokenKit-9.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.695391 pyobjc-framework-CryptoTokenKit-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CryptoTokenKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.636704 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.647532 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/CryptoTokenKit/
--rw-r--r--   0 ronald     (501) staff       (20)      789 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/CryptoTokenKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    14725 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/CryptoTokenKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.653323 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2154 2023-03-26 11:22:46.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1184 2023-03-26 11:22:46.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:22:46.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:57.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:22:46.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:22:46.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.657126 pyobjc-framework-CryptoTokenKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1162 2021-10-18 19:38:40.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Modules/_CryptoTokenKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Modules/_CryptoTokenKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CryptoTokenKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1943 2023-03-26 11:22:46.694991 pyobjc-framework-CryptoTokenKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.664634 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_cryptotokenkit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1140 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tkerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     5340 2022-06-25 09:09:54.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcard.py
--rw-r--r--   0 ronald     (501) staff       (20)     1027 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcardatr.py
--rw-r--r--   0 ronald     (501) staff       (20)      619 2022-06-25 20:16:56.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcardtoken.py
--rw-r--r--   0 ronald     (501) staff       (20)     3054 2022-06-25 20:18:13.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktoken.py
--rw-r--r--   0 ronald     (501) staff       (20)      412 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktokenconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     1110 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktokenkeychainitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      598 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktokenwatcher.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-CryptoTokenKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.665851 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     9154 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/CryptoTokenKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:46.685768 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    83136 2021-07-30 09:00:37.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    83622 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    15058 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    78229 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81151 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    83137 2021-07-30 09:00:37.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    83623 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CryptoTokenKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:22:46.695505 pyobjc-framework-CryptoTokenKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1183 2023-03-25 14:20:31.000000 pyobjc-framework-CryptoTokenKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.701392 pyobjc-framework-CryptoTokenKit-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CryptoTokenKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.642784 pyobjc-framework-CryptoTokenKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.648849 pyobjc-framework-CryptoTokenKit-9.2/Lib/CryptoTokenKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/CryptoTokenKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14725 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/CryptoTokenKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.652085 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2152 2023-06-07 00:12:49.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1199 2023-06-07 00:12:49.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:12:49.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:57.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:12:49.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:12:49.000000 pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.654701 pyobjc-framework-CryptoTokenKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1162 2021-10-18 19:38:40.000000 pyobjc-framework-CryptoTokenKit-9.2/Modules/_CryptoTokenKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/Modules/_CryptoTokenKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CryptoTokenKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CryptoTokenKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1941 2023-06-07 00:12:49.700862 pyobjc-framework-CryptoTokenKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.673761 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_cryptotokenkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1140 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tkerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5340 2022-06-25 09:09:54.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcard.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1027 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcardatr.py
+-rw-r--r--   0 ronald     (501) staff       (20)      619 2022-06-25 20:16:56.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcardtoken.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3054 2022-06-25 20:18:13.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktoken.py
+-rw-r--r--   0 ronald     (501) staff       (20)      412 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktokenconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1110 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktokenkeychainitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktokenwatcher.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-CryptoTokenKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.675358 pyobjc-framework-CryptoTokenKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     9154 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/CryptoTokenKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:49.699643 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    83136 2021-07-30 09:00:37.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    83622 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    15058 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    78229 2020-11-30 18:45:14.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81151 2021-03-21 10:08:22.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    83137 2021-07-30 09:00:37.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    83623 2022-02-24 08:47:16.000000 pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CryptoTokenKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CryptoTokenKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:12:49.701501 pyobjc-framework-CryptoTokenKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1254 2023-05-29 10:07:46.000000 pyobjc-framework-CryptoTokenKit-9.2/setup.py
```

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/LICENSE.txt` & `pyobjc-framework-CryptoTokenKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Lib/CryptoTokenKit/__init__.py` & `pyobjc-framework-CryptoTokenKit-9.2/Lib/CryptoTokenKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Lib/CryptoTokenKit/_metadata.py` & `pyobjc-framework-CryptoTokenKit-9.2/Lib/CryptoTokenKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/PKG-INFO` & `pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CryptoTokenKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CryptoTokenKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CryptoTokenKit
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Lib/pyobjc_framework_CryptoTokenKit.egg-info/SOURCES.txt` & `pyobjc-framework-CryptoTokenKit-9.2/Lib/pyobjc_framework_CryptoTokenKit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CryptoTokenKit/__init__.py
 Lib/CryptoTokenKit/_metadata.py
 Lib/pyobjc_framework_CryptoTokenKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_CryptoTokenKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CryptoTokenKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CryptoTokenKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Modules/_CryptoTokenKit.m` & `pyobjc-framework-CryptoTokenKit-9.2/Modules/_CryptoTokenKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Modules/_CryptoTokenKit_protocols.m` & `pyobjc-framework-CryptoTokenKit-9.2/Modules/_CryptoTokenKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CryptoTokenKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CryptoTokenKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PKG-INFO` & `pyobjc-framework-CryptoTokenKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CryptoTokenKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CryptoTokenKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CryptoTokenKit
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tkerror.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tkerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcard.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcard.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcardatr.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcardatr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tksmartcardtoken.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tksmartcardtoken.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktoken.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktoken.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktokenkeychainitem.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktokenkeychainitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/PyObjCTest/test_tktokenwatcher.py` & `pyobjc-framework-CryptoTokenKit-9.2/PyObjCTest/test_tktokenwatcher.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/CryptoTokenKit.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/CryptoTokenKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CryptoTokenKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CryptoTokenKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CryptoTokenKit-9.1b1/setup.py` & `pyobjc-framework-CryptoTokenKit-9.2/setup.py`

 * *Files 10% similar despite different names*

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
     name="pyobjc-framework-CryptoTokenKit",
     description="Wrappers for the framework CryptoTokenKit on macOS",
     min_os_level="10.10",
     packages=["CryptoTokenKit"],
     ext_modules=[
```

