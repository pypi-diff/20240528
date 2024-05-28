# Comparing `tmp/pyobjc-framework-SyncServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-SyncServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SyncServices-9.1b1.tar", last modified: Sun Mar 26 11:42:22 2023, max compression
+gzip compressed data, was "pyobjc-framework-SyncServices-9.2.tar", last modified: Wed Jun  7 00:30:05 2023, max compression
```

## Comparing `pyobjc-framework-SyncServices-9.1b1.tar` & `pyobjc-framework-SyncServices-9.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.952209 pyobjc-framework-SyncServices-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SyncServices-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.880321 pyobjc-framework-SyncServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.913830 pyobjc-framework-SyncServices-9.1b1/Lib/SyncServices/
--rw-r--r--   0 ronald     (501) staff       (20)      764 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/Lib/SyncServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    21303 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.1b1/Lib/SyncServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.917598 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2416 2023-03-26 11:42:22.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1272 2023-03-26 11:42:22.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:22.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:49.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       82 2023-03-26 11:42:22.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:42:22.000000 pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.920309 pyobjc-framework-SyncServices-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      801 2021-10-18 19:38:40.000000 pyobjc-framework-SyncServices-9.1b1/Modules/_SyncServices.m
--rw-r--r--   0 ronald     (501) staff       (20)      787 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/Modules/_SyncServices_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SyncServices-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SyncServices-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2205 2023-03-26 11:42:22.951868 pyobjc-framework-SyncServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.940152 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      978 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncchange.py
--rw-r--r--   0 ronald     (501) staff       (20)     1929 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncclient.py
--rw-r--r--   0 ronald     (501) staff       (20)      725 2023-03-03 17:21:59.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncconflictpropertytype.py
--rw-r--r--   0 ronald     (501) staff       (20)     1360 2022-06-25 20:16:04.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isynccoredata.py
--rw-r--r--   0 ronald     (501) staff       (20)      602 2022-06-25 20:07:24.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncfilter.py
--rw-r--r--   0 ronald     (501) staff       (20)      671 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      386 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncrecordsnapshot.py
--rw-r--r--   0 ronald     (501) staff       (20)     2138 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     8348 2022-06-25 09:26:49.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncsessiondriver.py
--rw-r--r--   0 ronald     (501) staff       (20)      841 2022-06-25 09:26:23.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_syncservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     1263 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_syncserviceserrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      289 2021-10-18 19:38:40.000000 pyobjc-framework-SyncServices-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.942060 pyobjc-framework-SyncServices-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    16768 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/metadata/SyncServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       84 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:22.950823 pyobjc-framework-SyncServices-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    61036 2021-07-30 09:00:38.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61149 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61037 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63721 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60929 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60997 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61037 2021-07-30 09:00:38.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61150 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SyncServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:22.952308 pyobjc-framework-SyncServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1490 2023-03-25 14:20:32.000000 pyobjc-framework-SyncServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.171046 pyobjc-framework-SyncServices-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SyncServices-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.114829 pyobjc-framework-SyncServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.123691 pyobjc-framework-SyncServices-9.2/Lib/SyncServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      764 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/Lib/SyncServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21303 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.2/Lib/SyncServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.127030 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2414 2023-06-07 00:30:05.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1287 2023-06-07 00:30:05.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:30:05.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:49.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       76 2023-06-07 00:30:05.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:30:05.000000 pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.129788 pyobjc-framework-SyncServices-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      801 2021-10-18 19:38:40.000000 pyobjc-framework-SyncServices-9.2/Modules/_SyncServices.m
+-rw-r--r--   0 ronald     (501) staff       (20)      787 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/Modules/_SyncServices_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SyncServices-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SyncServices-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2203 2023-06-07 00:30:05.170565 pyobjc-framework-SyncServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.150585 pyobjc-framework-SyncServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      978 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncchange.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1929 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncclient.py
+-rw-r--r--   0 ronald     (501) staff       (20)      725 2023-03-03 17:21:59.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncconflictpropertytype.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1360 2022-06-25 20:16:04.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isynccoredata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2022-06-25 20:07:24.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncfilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      671 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      386 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncrecordsnapshot.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2138 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8348 2022-06-25 09:26:49.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncsessiondriver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      841 2022-06-25 09:26:23.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_syncservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1263 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/PyObjCTest/test_syncserviceserrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2021-10-18 19:38:40.000000 pyobjc-framework-SyncServices-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.152895 pyobjc-framework-SyncServices-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    16768 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/metadata/SyncServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       84 2020-11-30 18:45:15.000000 pyobjc-framework-SyncServices-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:05.169422 pyobjc-framework-SyncServices-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    61036 2021-07-30 09:00:38.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61149 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61037 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63721 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60929 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60997 2021-03-21 10:08:23.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61037 2021-07-30 09:00:38.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61150 2022-02-24 08:47:17.000000 pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SyncServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SyncServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:30:05.171156 pyobjc-framework-SyncServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1561 2023-05-29 10:07:47.000000 pyobjc-framework-SyncServices-9.2/setup.py
```

### Comparing `pyobjc-framework-SyncServices-9.1b1/LICENSE.txt` & `pyobjc-framework-SyncServices-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Lib/SyncServices/__init__.py` & `pyobjc-framework-SyncServices-9.2/Lib/SyncServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Lib/SyncServices/_metadata.py` & `pyobjc-framework-SyncServices-9.2/Lib/SyncServices/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/PKG-INFO` & `pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SyncServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SyncServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SyncServices
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SyncServices-9.1b1/Lib/pyobjc_framework_SyncServices.egg-info/SOURCES.txt` & `pyobjc-framework-SyncServices-9.2/Lib/pyobjc_framework_SyncServices.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SyncServices/__init__.py
 Lib/SyncServices/_metadata.py
 Lib/pyobjc_framework_SyncServices.egg-info/PKG-INFO
 Lib/pyobjc_framework_SyncServices.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SyncServices.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SyncServices.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SyncServices-9.1b1/Modules/_SyncServices.m` & `pyobjc-framework-SyncServices-9.2/Modules/_SyncServices.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Modules/_SyncServices_protocols.m` & `pyobjc-framework-SyncServices-9.2/Modules/_SyncServices_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SyncServices-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SyncServices-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SyncServices-9.1b1/PKG-INFO` & `pyobjc-framework-SyncServices-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SyncServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SyncServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SyncServices
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncchange.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncchange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncclient.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncclient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncconflictpropertytype.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncconflictpropertytype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isynccoredata.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isynccoredata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncfilter.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncfilter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncmanager.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncsession.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_isyncsessiondriver.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_isyncsessiondriver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_syncservices.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_syncservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/PyObjCTest/test_syncserviceserrors.py` & `pyobjc-framework-SyncServices-9.2/PyObjCTest/test_syncserviceserrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/SyncServices.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/SyncServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SyncServices-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SyncServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SyncServices-9.1b1/setup.py` & `pyobjc-framework-SyncServices-9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 
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
     name="pyobjc-framework-SyncServices",
     description="Wrappers for the framework SyncServices on macOS",
     packages=["SyncServices"],
     ext_modules=[
         Extension(
```

