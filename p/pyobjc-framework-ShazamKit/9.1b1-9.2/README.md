# Comparing `tmp/pyobjc-framework-ShazamKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-ShazamKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ShazamKit-9.1b1.tar", last modified: Sun Mar 26 11:40:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-ShazamKit-9.2.tar", last modified: Wed Jun  7 00:28:44 2023, max compression
```

## Comparing `pyobjc-framework-ShazamKit-9.1b1.tar` & `pyobjc-framework-ShazamKit-9.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.241081 pyobjc-framework-ShazamKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.149328 pyobjc-framework-ShazamKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.173220 pyobjc-framework-ShazamKit-9.1b1/Lib/ShazamKit/
--rw-r--r--   0 ronald     (501) staff       (20)      722 2021-09-09 08:50:47.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/ShazamKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4296 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/ShazamKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.178997 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2107 2023-03-26 11:40:41.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1193 2023-03-26 11:40:41.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:40:41.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-06-10 10:16:28.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:40:41.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:40:41.000000 pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ShazamKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.182759 pyobjc-framework-ShazamKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      818 2021-10-18 19:38:40.000000 pyobjc-framework-ShazamKit-9.1b1/Modules/_ShazamKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      295 2021-09-09 08:14:29.000000 pyobjc-framework-ShazamKit-9.1b1/Modules/_ShazamKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ShazamKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1896 2023-03-26 11:40:41.240486 pyobjc-framework-ShazamKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.225447 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shazamkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      242 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shcatalog.py
--rw-r--r--   0 ronald     (501) staff       (20)      866 2021-09-09 08:49:25.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shcustomcatalog.py
--rw-r--r--   0 ronald     (501) staff       (20)      833 2022-06-15 11:57:00.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_sherror.py
--rw-r--r--   0 ronald     (501) staff       (20)      238 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shmatch.py
--rw-r--r--   0 ronald     (501) staff       (20)      340 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shmatchedmediatiem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1590 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shmediaitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      360 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shmedialibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:07:29.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      387 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shsignature.py
--rw-r--r--   0 ronald     (501) staff       (20)      667 2022-06-15 11:57:00.000000 pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shsignaturegenerator.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.228282 pyobjc-framework-ShazamKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1513 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/ShazamKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:41.238877 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    22458 2021-07-30 09:00:38.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22521 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27357 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27357 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22459 2021-07-30 09:00:38.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22522 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27358 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27358 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ShazamKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:40:41.241234 pyobjc-framework-ShazamKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1102 2023-03-25 14:20:32.000000 pyobjc-framework-ShazamKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.969609 pyobjc-framework-ShazamKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.921043 pyobjc-framework-ShazamKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.926911 pyobjc-framework-ShazamKit-9.2/Lib/ShazamKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      722 2021-09-09 08:50:47.000000 pyobjc-framework-ShazamKit-9.2/Lib/ShazamKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4296 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.2/Lib/ShazamKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.933035 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-06-07 00:28:44.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1208 2023-06-07 00:28:44.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:28:44.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-06-10 10:16:28.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:28:44.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:28:44.000000 pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ShazamKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.936466 pyobjc-framework-ShazamKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      818 2021-10-18 19:38:40.000000 pyobjc-framework-ShazamKit-9.2/Modules/_ShazamKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      295 2021-09-09 08:14:29.000000 pyobjc-framework-ShazamKit-9.2/Modules/_ShazamKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ShazamKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-06-07 00:28:44.969069 pyobjc-framework-ShazamKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.950021 pyobjc-framework-ShazamKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shazamkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      242 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shcatalog.py
+-rw-r--r--   0 ronald     (501) staff       (20)      866 2021-09-09 08:49:25.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shcustomcatalog.py
+-rw-r--r--   0 ronald     (501) staff       (20)      833 2022-06-15 11:57:00.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_sherror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shmatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)      340 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shmatchedmediatiem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1590 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shmediaitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      360 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shmedialibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:07:29.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      387 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shsignature.py
+-rw-r--r--   0 ronald     (501) staff       (20)      667 2022-06-15 11:57:00.000000 pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shsignaturegenerator.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.952077 pyobjc-framework-ShazamKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1513 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.2/metadata/ShazamKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2021-06-10 09:09:03.000000 pyobjc-framework-ShazamKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:44.962664 pyobjc-framework-ShazamKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    22458 2021-07-30 09:00:38.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22521 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27357 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27357 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22459 2021-07-30 09:00:38.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22522 2022-02-24 08:47:17.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27358 2022-06-25 20:19:21.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27358 2023-02-19 10:50:35.000000 pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ShazamKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ShazamKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:28:44.969723 pyobjc-framework-ShazamKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2023-05-29 10:07:47.000000 pyobjc-framework-ShazamKit-9.2/setup.py
```

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Lib/ShazamKit/__init__.py` & `pyobjc-framework-ShazamKit-9.2/Lib/ShazamKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Lib/ShazamKit/_metadata.py` & `pyobjc-framework-ShazamKit-9.2/Lib/ShazamKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/PKG-INFO` & `pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ShazamKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ShazamKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ShazamKit
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Lib/pyobjc_framework_ShazamKit.egg-info/SOURCES.txt` & `pyobjc-framework-ShazamKit-9.2/Lib/pyobjc_framework_ShazamKit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ShazamKit/__init__.py
 Lib/ShazamKit/_metadata.py
 Lib/pyobjc_framework_ShazamKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_ShazamKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ShazamKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ShazamKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ShazamKit-9.1b1/License.txt` & `pyobjc-framework-ShazamKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Modules/_ShazamKit.m` & `pyobjc-framework-ShazamKit-9.2/Modules/_ShazamKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ShazamKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ShazamKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ShazamKit-9.1b1/PKG-INFO` & `pyobjc-framework-ShazamKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ShazamKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ShazamKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ShazamKit
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shcustomcatalog.py` & `pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shcustomcatalog.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_sherror.py` & `pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_sherror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shmediaitem.py` & `pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shmediaitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/PyObjCTest/test_shsignaturegenerator.py` & `pyobjc-framework-ShazamKit-9.2/PyObjCTest/test_shsignaturegenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/ShazamKit.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/ShazamKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-ShazamKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ShazamKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ShazamKit-9.1b1/setup.py` & `pyobjc-framework-ShazamKit-9.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
-from pyobjc_setup import setup, Extension
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-ShazamKit",
     description="Wrappers for the framework ShazamKit on macOS",
     min_os_level="12.0",
     packages=["ShazamKit"],
     ext_modules=[
```
