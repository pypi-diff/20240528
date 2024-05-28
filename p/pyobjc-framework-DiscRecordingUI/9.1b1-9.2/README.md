# Comparing `tmp/pyobjc-framework-DiscRecordingUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-DiscRecordingUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DiscRecordingUI-9.1b1.tar", last modified: Sun Mar 26 11:23:28 2023, max compression
+gzip compressed data, was "pyobjc-framework-DiscRecordingUI-9.2.tar", last modified: Wed Jun  7 00:13:33 2023, max compression
```

## Comparing `pyobjc-framework-DiscRecordingUI-9.1b1.tar` & `pyobjc-framework-DiscRecordingUI-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.283856 pyobjc-framework-DiscRecordingUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.254258 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.260454 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/DiscRecordingUI/
--rw-r--r--   0 ronald     (501) staff       (20)      772 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/DiscRecordingUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9509 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/DiscRecordingUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.264007 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-03-26 11:23:28.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1033 2023-03-26 11:23:28.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:28.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:01.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       87 2023-03-26 11:23:28.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:23:28.000000 pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiscRecordingUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-03-26 11:23:28.283439 pyobjc-framework-DiscRecordingUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.275107 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_discrecordingui.py
--rw-r--r--   0 ronald     (501) staff       (20)      272 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_discrecordinguiresources.py
--rw-r--r--   0 ronald     (501) staff       (20)      883 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drburnprogresspanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     2659 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drburnsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      486 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drburnsetuppanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      661 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_dreraseprogresspanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     2234 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drerasesession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1092 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drsetuppanel.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.277130 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1968 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/DiscRecordingUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:28.282708 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    26902 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26921 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26898 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26903 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26903 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26922 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiscRecordingUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:28.283957 pyobjc-framework-DiscRecordingUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      740 2023-03-25 14:20:31.000000 pyobjc-framework-DiscRecordingUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.614915 pyobjc-framework-DiscRecordingUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.588801 pyobjc-framework-DiscRecordingUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.593622 pyobjc-framework-DiscRecordingUI-9.2/Lib/DiscRecordingUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      772 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/DiscRecordingUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9509 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/DiscRecordingUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.597542 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2120 2023-06-07 00:13:33.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1048 2023-06-07 00:13:33.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:33.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:01.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       81 2023-06-07 00:13:33.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:13:33.000000 pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiscRecordingUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1909 2023-06-07 00:13:33.614376 pyobjc-framework-DiscRecordingUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.606002 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_discrecordingui.py
+-rw-r--r--   0 ronald     (501) staff       (20)      272 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_discrecordinguiresources.py
+-rw-r--r--   0 ronald     (501) staff       (20)      883 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drburnprogresspanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2659 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drburnsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      486 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drburnsetuppanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      661 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_dreraseprogresspanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2234 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drerasesession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1092 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drsetuppanel.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.607451 pyobjc-framework-DiscRecordingUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1968 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/DiscRecordingUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:33.613369 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    26902 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26921 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26898 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26903 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26903 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26922 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiscRecordingUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DiscRecordingUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:33.615042 pyobjc-framework-DiscRecordingUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      821 2023-05-29 10:07:46.000000 pyobjc-framework-DiscRecordingUI-9.2/setup.py
```

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/Lib/DiscRecordingUI/__init__.py` & `pyobjc-framework-DiscRecordingUI-9.2/Lib/DiscRecordingUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/Lib/DiscRecordingUI/_metadata.py` & `pyobjc-framework-DiscRecordingUI-9.2/Lib/DiscRecordingUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/PKG-INFO` & `pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiscRecordingUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiscRecordingUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiscRecordingUI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/Lib/pyobjc_framework_DiscRecordingUI.egg-info/SOURCES.txt` & `pyobjc-framework-DiscRecordingUI-9.2/Lib/pyobjc_framework_DiscRecordingUI.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/DiscRecordingUI/__init__.py
 Lib/DiscRecordingUI/_metadata.py
 Lib/pyobjc_framework_DiscRecordingUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_DiscRecordingUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_DiscRecordingUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_DiscRecordingUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/License.txt` & `pyobjc-framework-DiscRecordingUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PKG-INFO` & `pyobjc-framework-DiscRecordingUI-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiscRecordingUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiscRecordingUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiscRecordingUI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drburnprogresspanel.py` & `pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drburnprogresspanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drburnsession.py` & `pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drburnsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_dreraseprogresspanel.py` & `pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_dreraseprogresspanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drerasesession.py` & `pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drerasesession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/PyObjCTest/test_drsetuppanel.py` & `pyobjc-framework-DiscRecordingUI-9.2/PyObjCTest/test_drsetuppanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/DiscRecordingUI.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/DiscRecordingUI.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-DiscRecordingUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DiscRecordingUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecordingUI-9.1b1/setup.py` & `pyobjc-framework-DiscRecordingUI-9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "DiscRecordingUI" framework on macOS.
 
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
     name="pyobjc-framework-DiscRecordingUI",
     description="Wrappers for the framework DiscRecordingUI on macOS",
     packages=["DiscRecordingUI"],
     version=VERSION,
     install_requires=[
```

