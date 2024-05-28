# Comparing `tmp/pyobjc-framework-FileProvider-9.1b1.tar.gz` & `tmp/pyobjc-framework-FileProvider-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-FileProvider-9.1b1.tar", last modified: Sun Mar 26 11:24:27 2023, max compression
+gzip compressed data, was "pyobjc-framework-FileProvider-9.2.tar", last modified: Wed Jun  7 00:14:38 2023, max compression
```

## Comparing `pyobjc-framework-FileProvider-9.1b1.tar` & `pyobjc-framework-FileProvider-9.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.365588 pyobjc-framework-FileProvider-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.290154 pyobjc-framework-FileProvider-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.304127 pyobjc-framework-FileProvider-9.1b1/Lib/FileProvider/
--rw-r--r--   0 ronald     (501) staff       (20)      792 2021-03-21 10:08:22.000000 pyobjc-framework-FileProvider-9.1b1/Lib/FileProvider/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    55500 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.1b1/Lib/FileProvider/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.308521 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2120 2023-03-26 11:24:27.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1498 2023-03-26 11:24:27.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:27.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:09.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:24:27.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:24:27.000000 pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FileProvider-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.311217 pyobjc-framework-FileProvider-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      778 2021-10-18 19:38:40.000000 pyobjc-framework-FileProvider-9.1b1/Modules/_FileProvider.m
--rw-r--r--   0 ronald     (501) staff       (20)     1460 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.1b1/Modules/_FileProvider_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-FileProvider-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1909 2023-03-26 11:24:27.365011 pyobjc-framework-FileProvider-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.323272 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_fileprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     2160 2021-07-30 09:00:37.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovideractions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1155 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderdomain.py
--rw-r--r--   0 ronald     (501) staff       (20)     2102 2022-06-25 09:10:08.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderenumerating.py
--rw-r--r--   0 ronald     (501) staff       (20)     1867 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidererror.py
--rw-r--r--   0 ronald     (501) staff       (20)     1418 2021-03-21 10:08:22.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     5593 2022-06-25 09:10:28.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovideritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      394 2022-06-25 20:07:33.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovideritemdecoration.py
--rw-r--r--   0 ronald     (501) staff       (20)     4890 2022-06-25 09:10:18.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidermanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     9056 2022-06-25 09:10:26.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderreplicatedextension.py
--rw-r--r--   0 ronald     (501) staff       (20)      543 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1029 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderservice.py
--rw-r--r--   0 ronald     (501) staff       (20)     3050 2022-06-25 09:10:15.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidertesting.py
--rw-r--r--   0 ronald     (501) staff       (20)      661 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderthumbnailing.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.336246 pyobjc-framework-FileProvider-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    20156 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.1b1/metadata/FileProvider.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:27.363494 pyobjc-framework-FileProvider-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    94606 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97524 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103738 2022-06-25 20:05:31.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   104586 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    71565 2021-04-09 08:47:51.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    94607 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97525 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103739 2022-06-25 20:05:31.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   104587 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FileProvider-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:27.365702 pyobjc-framework-FileProvider-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1107 2023-03-25 14:20:31.000000 pyobjc-framework-FileProvider-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.951148 pyobjc-framework-FileProvider-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.867950 pyobjc-framework-FileProvider-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.877379 pyobjc-framework-FileProvider-9.2/Lib/FileProvider/
+-rw-r--r--   0 ronald     (501) staff       (20)      792 2021-03-21 10:08:22.000000 pyobjc-framework-FileProvider-9.2/Lib/FileProvider/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    55500 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.2/Lib/FileProvider/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.881785 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2118 2023-06-07 00:14:38.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1513 2023-06-07 00:14:38.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:14:38.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:09.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:14:38.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:14:38.000000 pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FileProvider-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.885043 pyobjc-framework-FileProvider-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      778 2021-10-18 19:38:40.000000 pyobjc-framework-FileProvider-9.2/Modules/_FileProvider.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1460 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.2/Modules/_FileProvider_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-FileProvider-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1907 2023-06-07 00:14:38.950289 pyobjc-framework-FileProvider-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.918709 pyobjc-framework-FileProvider-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_fileprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2160 2021-07-30 09:00:37.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovideractions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1155 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderdomain.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2102 2022-06-25 09:10:08.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderenumerating.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1867 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidererror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1418 2021-03-21 10:08:22.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5593 2022-06-25 09:10:28.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovideritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      394 2022-06-25 20:07:33.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovideritemdecoration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4890 2022-06-25 09:10:18.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidermanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9056 2022-06-25 09:10:26.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderreplicatedextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)      543 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1029 2022-06-23 11:03:28.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3050 2022-06-25 09:10:15.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidertesting.py
+-rw-r--r--   0 ronald     (501) staff       (20)      661 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderthumbnailing.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.922279 pyobjc-framework-FileProvider-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    20156 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.2/metadata/FileProvider.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-FileProvider-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:38.948113 pyobjc-framework-FileProvider-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    94606 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97524 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103738 2022-06-25 20:05:31.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   104586 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    71565 2021-04-09 08:47:51.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    94607 2021-07-30 09:00:38.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97525 2022-02-24 08:47:16.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103739 2022-06-25 20:05:31.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   104587 2023-02-19 10:50:35.000000 pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FileProvider-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-FileProvider-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:14:38.951259 pyobjc-framework-FileProvider-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1178 2023-05-29 10:07:46.000000 pyobjc-framework-FileProvider-9.2/setup.py
```

### Comparing `pyobjc-framework-FileProvider-9.1b1/Lib/FileProvider/__init__.py` & `pyobjc-framework-FileProvider-9.2/Lib/FileProvider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Lib/FileProvider/_metadata.py` & `pyobjc-framework-FileProvider-9.2/Lib/FileProvider/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/PKG-INFO` & `pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FileProvider
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FileProvider on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FileProvider
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-FileProvider-9.1b1/Lib/pyobjc_framework_FileProvider.egg-info/SOURCES.txt` & `pyobjc-framework-FileProvider-9.2/Lib/pyobjc_framework_FileProvider.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/FileProvider/__init__.py
 Lib/FileProvider/_metadata.py
 Lib/pyobjc_framework_FileProvider.egg-info/PKG-INFO
 Lib/pyobjc_framework_FileProvider.egg-info/SOURCES.txt
 Lib/pyobjc_framework_FileProvider.egg-info/dependency_links.txt
 Lib/pyobjc_framework_FileProvider.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-FileProvider-9.1b1/License.txt` & `pyobjc-framework-FileProvider-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Modules/_FileProvider.m` & `pyobjc-framework-FileProvider-9.2/Modules/_FileProvider.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Modules/_FileProvider_protocols.m` & `pyobjc-framework-FileProvider-9.2/Modules/_FileProvider_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-FileProvider-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-FileProvider-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-FileProvider-9.1b1/PKG-INFO` & `pyobjc-framework-FileProvider-9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FileProvider
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FileProvider on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FileProvider
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovideractions.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovideractions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderdomain.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderdomain.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderenumerating.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderenumerating.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidererror.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidererror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderextension.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovideritem.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovideritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidermanager.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidermanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderreplicatedextension.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderreplicatedextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderrequest.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderservice.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileprovidertesting.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileprovidertesting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/PyObjCTest/test_nsfileproviderthumbnailing.py` & `pyobjc-framework-FileProvider-9.2/PyObjCTest/test_nsfileproviderthumbnailing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/FileProvider.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/FileProvider.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-FileProvider-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/pyobjc_setup.py` & `pyobjc-framework-FileProvider-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProvider-9.1b1/setup.py` & `pyobjc-framework-FileProvider-9.2/setup.py`

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
     name="pyobjc-framework-FileProvider",
     description="Wrappers for the framework FileProvider on macOS",
     min_os_level="10.15",
     packages=["FileProvider"],
     ext_modules=[
```

