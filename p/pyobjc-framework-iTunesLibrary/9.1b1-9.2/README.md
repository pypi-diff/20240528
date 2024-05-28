# Comparing `tmp/pyobjc-framework-iTunesLibrary-9.1b1.tar.gz` & `tmp/pyobjc-framework-iTunesLibrary-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-iTunesLibrary-9.1b1.tar", last modified: Sun Mar 26 11:44:33 2023, max compression
+gzip compressed data, was "pyobjc-framework-iTunesLibrary-9.2.tar", last modified: Wed Jun  7 00:32:21 2023, max compression
```

## Comparing `pyobjc-framework-iTunesLibrary-9.1b1.tar` & `pyobjc-framework-iTunesLibrary-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:33.010287 pyobjc-framework-iTunesLibrary-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:32.983535 pyobjc-framework-iTunesLibrary-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:32.987246 pyobjc-framework-iTunesLibrary-9.1b1/Lib/iTunesLibrary/
--rw-r--r--   0 ronald     (501) staff       (20)      960 2021-03-21 10:08:23.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/iTunesLibrary/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9455 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/iTunesLibrary/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:32.991753 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2190 2023-03-26 11:44:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1053 2023-03-26 11:44:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:44:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:04.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:44:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:44:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-iTunesLibrary-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1979 2023-03-26 11:44:33.009935 pyobjc-framework-iTunesLibrary-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:33.000533 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibalbum.py
--rw-r--r--   0 ronald     (501) staff       (20)      215 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibartist.py
--rw-r--r--   0 ronald     (501) staff       (20)      844 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibartwork.py
--rw-r--r--   0 ronald     (501) staff       (20)      704 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibmediaentity.py
--rw-r--r--   0 ronald     (501) staff       (20)     9128 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibmediaitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      343 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibmediaitemvideoinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     3786 2021-06-10 09:09:03.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibplaylist.py
--rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_ituneslibrary.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:33.001806 pyobjc-framework-iTunesLibrary-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    12073 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/iTunesLibrary.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:33.008980 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    52826 2021-07-30 09:00:38.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53331 2022-02-24 08:47:17.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53969 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52327 2021-03-21 10:08:23.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52827 2021-07-30 09:00:38.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53332 2022-02-24 08:47:17.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53970 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-iTunesLibrary-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:44:33.010394 pyobjc-framework-iTunesLibrary-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      747 2023-03-25 14:20:32.000000 pyobjc-framework-iTunesLibrary-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.540730 pyobjc-framework-iTunesLibrary-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.459876 pyobjc-framework-iTunesLibrary-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.464717 pyobjc-framework-iTunesLibrary-9.2/Lib/iTunesLibrary/
+-rw-r--r--   0 ronald     (501) staff       (20)      960 2021-03-21 10:08:23.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/iTunesLibrary/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9455 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/iTunesLibrary/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.472442 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2188 2023-06-07 00:32:21.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1068 2023-06-07 00:32:21.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:32:21.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:04.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:32:21.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:32:21.000000 pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-iTunesLibrary-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1977 2023-06-07 00:32:21.537274 pyobjc-framework-iTunesLibrary-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.478675 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibalbum.py
+-rw-r--r--   0 ronald     (501) staff       (20)      215 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibartist.py
+-rw-r--r--   0 ronald     (501) staff       (20)      844 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibartwork.py
+-rw-r--r--   0 ronald     (501) staff       (20)      704 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibmediaentity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9128 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibmediaitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      343 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibmediaitemvideoinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3786 2021-06-10 09:09:03.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibplaylist.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_ituneslibrary.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.480083 pyobjc-framework-iTunesLibrary-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    12073 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/iTunesLibrary.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:15.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:21.533611 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    52826 2021-07-30 09:00:38.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53331 2022-02-24 08:47:17.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53969 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52327 2021-03-21 10:08:23.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52827 2021-07-30 09:00:38.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53332 2022-02-24 08:47:17.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53970 2022-10-18 09:53:24.000000 pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-iTunesLibrary-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-iTunesLibrary-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:32:21.541005 pyobjc-framework-iTunesLibrary-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2023-05-29 10:07:47.000000 pyobjc-framework-iTunesLibrary-9.2/setup.py
```

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/Lib/iTunesLibrary/__init__.py` & `pyobjc-framework-iTunesLibrary-9.2/Lib/iTunesLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/Lib/iTunesLibrary/_metadata.py` & `pyobjc-framework-iTunesLibrary-9.2/Lib/iTunesLibrary/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/PKG-INFO` & `pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-iTunesLibrary
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework iTunesLibrary on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,iTunesLibrary
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/Lib/pyobjc_framework_iTunesLibrary.egg-info/SOURCES.txt` & `pyobjc-framework-iTunesLibrary-9.2/Lib/pyobjc_framework_iTunesLibrary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/iTunesLibrary/__init__.py
 Lib/iTunesLibrary/_metadata.py
 Lib/pyobjc_framework_iTunesLibrary.egg-info/PKG-INFO
 Lib/pyobjc_framework_iTunesLibrary.egg-info/SOURCES.txt
 Lib/pyobjc_framework_iTunesLibrary.egg-info/dependency_links.txt
 Lib/pyobjc_framework_iTunesLibrary.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/License.txt` & `pyobjc-framework-iTunesLibrary-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PKG-INFO` & `pyobjc-framework-iTunesLibrary-9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-iTunesLibrary
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework iTunesLibrary on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,iTunesLibrary
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibartwork.py` & `pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibartwork.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibmediaentity.py` & `pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibmediaentity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibmediaitem.py` & `pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibmediaitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibplaylist.py` & `pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibplaylist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/PyObjCTest/test_itlibrary.py` & `pyobjc-framework-iTunesLibrary-9.2/PyObjCTest/test_itlibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/iTunesLibrary.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/iTunesLibrary.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-iTunesLibrary-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/pyobjc_setup.py` & `pyobjc-framework-iTunesLibrary-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-iTunesLibrary-9.1b1/setup.py` & `pyobjc-framework-iTunesLibrary-9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 
 Note that using the library requires a signed application bundle.
 """
 
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-iTunesLibrary",
     description="Wrappers for the framework iTunesLibrary on macOS",
     min_os_level="10.6",
     packages=["iTunesLibrary"],
     version=VERSION,
```

