# Comparing `tmp/pyobjc-framework-MailKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-MailKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MailKit-9.1b1.tar", last modified: Sun Mar 26 11:28:27 2023, max compression
+gzip compressed data, was "pyobjc-framework-MailKit-9.2.tar", last modified: Wed Jun  7 00:18:57 2023, max compression
```

## Comparing `pyobjc-framework-MailKit-9.1b1.tar` & `pyobjc-framework-MailKit-9.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.099217 pyobjc-framework-MailKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.038573 pyobjc-framework-MailKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.060733 pyobjc-framework-MailKit-9.1b1/Lib/MailKit/
--rw-r--r--   0 ronald     (501) staff       (20)      671 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/Lib/MailKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9897 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/Lib/MailKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.066366 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2101 2023-03-26 11:28:27.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1488 2023-03-26 11:28:27.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:27.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:03:25.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:28:27.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:28:27.000000 pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MailKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1890 2023-03-26 11:28:27.098879 pyobjc-framework-MailKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.092407 pyobjc-framework-MailKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mailkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      167 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meaddressannotation.py
--rw-r--r--   0 ronald     (501) staff       (20)      786 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mecomposecontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1083 2022-06-25 20:09:57.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mecomposesession.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-06-25 20:14:37.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mecontentblocker.py
--rw-r--r--   0 ronald     (501) staff       (20)      161 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_medecodedmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)      279 2021-10-25 15:33:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_medecodedmessagebanner.py
--rw-r--r--   0 ronald     (501) staff       (20)      162 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meemailaddress.py
--rw-r--r--   0 ronald     (501) staff       (20)      359 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meencodedoutgoingmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)      188 2022-06-25 20:11:30.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meextension.py
--rw-r--r--   0 ronald     (501) staff       (20)      458 2021-10-26 11:32:35.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meextensionmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      179 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meextensionviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      719 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1403 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      175 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageactiondecision.py
--rw-r--r--   0 ronald     (501) staff       (20)      524 2022-06-25 20:16:48.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageactionhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-06-25 20:18:06.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagedecoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      875 2022-06-25 20:14:07.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      175 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageencodingresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      743 2022-06-25 20:13:28.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagesecurityhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2021-08-14 10:34:11.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagesecurityinformation.py
--rw-r--r--   0 ronald     (501) staff       (20)      159 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagesigner.py
--rw-r--r--   0 ronald     (501) staff       (20)      740 2021-09-09 08:49:25.000000 pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meoutgoingmessageencodingstatus.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.093783 pyobjc-framework-MailKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/metadata/MailKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:27.097282 pyobjc-framework-MailKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    50726 2022-01-02 11:04:26.000000 pyobjc-framework-MailKit-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51118 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    50727 2022-01-02 11:04:26.000000 pyobjc-framework-MailKit-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51119 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MailKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:27.099320 pyobjc-framework-MailKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      681 2023-03-25 14:20:31.000000 pyobjc-framework-MailKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.776423 pyobjc-framework-MailKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.705165 pyobjc-framework-MailKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.710218 pyobjc-framework-MailKit-9.2/Lib/MailKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      671 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/Lib/MailKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9897 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/Lib/MailKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.723595 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2099 2023-06-07 00:18:57.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1503 2023-06-07 00:18:57.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:57.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:03:25.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:18:57.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:18:57.000000 pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MailKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1888 2023-06-07 00:18:57.773094 pyobjc-framework-MailKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.755130 pyobjc-framework-MailKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_mailkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      167 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meaddressannotation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      786 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_mecomposecontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1083 2022-06-25 20:09:57.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_mecomposesession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-06-25 20:14:37.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_mecontentblocker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      161 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_medecodedmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      279 2021-10-25 15:33:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_medecodedmessagebanner.py
+-rw-r--r--   0 ronald     (501) staff       (20)      162 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meemailaddress.py
+-rw-r--r--   0 ronald     (501) staff       (20)      359 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meencodedoutgoingmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      188 2022-06-25 20:11:30.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)      458 2021-10-26 11:32:35.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meextensionmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      179 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meextensionviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      719 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1403 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      175 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageactiondecision.py
+-rw-r--r--   0 ronald     (501) staff       (20)      524 2022-06-25 20:16:48.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageactionhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-06-25 20:18:06.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagedecoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      875 2022-06-25 20:14:07.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      175 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageencodingresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      743 2022-06-25 20:13:28.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagesecurityhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2021-08-14 10:34:11.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagesecurityinformation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      159 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagesigner.py
+-rw-r--r--   0 ronald     (501) staff       (20)      740 2021-09-09 08:49:25.000000 pyobjc-framework-MailKit-9.2/PyObjCTest/test_meoutgoingmessageencodingstatus.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.756717 pyobjc-framework-MailKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/metadata/MailKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2021-07-30 09:00:38.000000 pyobjc-framework-MailKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:57.760657 pyobjc-framework-MailKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    50726 2022-01-02 11:04:26.000000 pyobjc-framework-MailKit-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51118 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    50727 2022-01-02 11:04:26.000000 pyobjc-framework-MailKit-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51119 2022-02-24 08:47:16.000000 pyobjc-framework-MailKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MailKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MailKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:57.776601 pyobjc-framework-MailKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      762 2023-05-29 10:07:46.000000 pyobjc-framework-MailKit-9.2/setup.py
```

### Comparing `pyobjc-framework-MailKit-9.1b1/Lib/MailKit/__init__.py` & `pyobjc-framework-MailKit-9.2/Lib/MailKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/Lib/MailKit/_metadata.py` & `pyobjc-framework-MailKit-9.2/Lib/MailKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/PKG-INFO` & `pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MailKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MailKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MailKit
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-MailKit-9.1b1/Lib/pyobjc_framework_MailKit.egg-info/SOURCES.txt` & `pyobjc-framework-MailKit-9.2/Lib/pyobjc_framework_MailKit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MailKit/__init__.py
 Lib/MailKit/_metadata.py
 Lib/pyobjc_framework_MailKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_MailKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MailKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MailKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MailKit-9.1b1/License.txt` & `pyobjc-framework-MailKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PKG-INFO` & `pyobjc-framework-MailKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MailKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MailKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MailKit
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mecomposecontext.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_mecomposecontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_mecomposesession.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_mecomposesession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessage.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageaction.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageactionhandler.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageactionhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessageencoder.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessageencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagesecurityhandler.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagesecurityhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_memessagesecurityinformation.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_memessagesecurityinformation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/PyObjCTest/test_meoutgoingmessageencodingstatus.py` & `pyobjc-framework-MailKit-9.2/PyObjCTest/test_meoutgoingmessageencodingstatus.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-MailKit-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MailKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-MailKit-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MailKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MailKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MailKit-9.1b1/setup.py` & `pyobjc-framework-MailKit-9.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "MailKit" framework on macOS.9.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MailKit",
     description="Wrappers for the framework MailKit on macOS",
     min_os_level="12.0",
     packages=["MailKit"],
     version=VERSION,
```

