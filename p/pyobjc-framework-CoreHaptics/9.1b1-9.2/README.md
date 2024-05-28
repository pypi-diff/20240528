# Comparing `tmp/pyobjc-framework-CoreHaptics-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreHaptics-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreHaptics-9.1b1.tar", last modified: Sun Mar 26 11:20:33 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreHaptics-9.2.tar", last modified: Wed Jun  7 00:10:31 2023, max compression
```

## Comparing `pyobjc-framework-CoreHaptics-9.1b1.tar` & `pyobjc-framework-CoreHaptics-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.864446 pyobjc-framework-CoreHaptics-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.830242 pyobjc-framework-CoreHaptics-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.835050 pyobjc-framework-CoreHaptics-9.1b1/Lib/CoreHaptics/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/CoreHaptics/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    14300 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/CoreHaptics/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.838233 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-03-26 11:20:33.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1055 2023-03-26 11:20:33.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:20:33.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:45.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:20:33.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:20:33.000000 pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreHaptics-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-03-26 11:20:33.863760 pyobjc-framework-CoreHaptics-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.848627 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1721 2022-06-25 09:08:41.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticdevicecapability.py
--rw-r--r--   0 ronald     (501) staff       (20)     4953 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticengine.py
--rw-r--r--   0 ronald     (501) staff       (20)     2052 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     2624 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticparameter.py
--rw-r--r--   0 ronald     (501) staff       (20)     2330 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticpattern.py
--rw-r--r--   0 ronald     (501) staff       (20)     4679 2022-06-25 09:08:38.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticpatternplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_corehaptics.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.849874 pyobjc-framework-CoreHaptics-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     8784 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/CoreHaptics.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:33.862297 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    41875 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42061 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44100 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40345 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41575 2021-03-21 10:08:22.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41876 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42062 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44101 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreHaptics-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:20:33.864561 pyobjc-framework-CoreHaptics-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      673 2023-03-25 14:20:30.000000 pyobjc-framework-CoreHaptics-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.147547 pyobjc-framework-CoreHaptics-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.106197 pyobjc-framework-CoreHaptics-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.110771 pyobjc-framework-CoreHaptics-9.2/Lib/CoreHaptics/
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.2/Lib/CoreHaptics/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14300 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/Lib/CoreHaptics/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.115139 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-06-07 00:10:31.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1070 2023-06-07 00:10:31.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:10:31.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:45.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:10:31.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:10:31.000000 pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreHaptics-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-06-07 00:10:31.147136 pyobjc-framework-CoreHaptics-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.125434 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1721 2022-06-25 09:08:41.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticdevicecapability.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4953 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticengine.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2052 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2624 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticparameter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2330 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticpattern.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4679 2022-06-25 09:08:38.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticpatternplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_corehaptics.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.126642 pyobjc-framework-CoreHaptics-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     8784 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/metadata/CoreHaptics.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:31.145799 pyobjc-framework-CoreHaptics-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    41875 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42061 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44100 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40345 2020-11-30 18:45:14.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41575 2021-03-21 10:08:22.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41876 2021-07-30 09:00:37.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42062 2022-02-24 08:47:16.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44101 2022-06-15 11:57:00.000000 pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreHaptics-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreHaptics-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:10:31.147647 pyobjc-framework-CoreHaptics-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2023-05-29 10:07:45.000000 pyobjc-framework-CoreHaptics-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/Lib/CoreHaptics/__init__.py` & `pyobjc-framework-CoreHaptics-9.2/Lib/CoreHaptics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/Lib/CoreHaptics/_metadata.py` & `pyobjc-framework-CoreHaptics-9.2/Lib/CoreHaptics/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/PKG-INFO` & `pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreHaptics
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreHaptics on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreHaptics
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/Lib/pyobjc_framework_CoreHaptics.egg-info/SOURCES.txt` & `pyobjc-framework-CoreHaptics-9.2/Lib/pyobjc_framework_CoreHaptics.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreHaptics/__init__.py
 Lib/CoreHaptics/_metadata.py
 Lib/pyobjc_framework_CoreHaptics.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreHaptics.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreHaptics.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreHaptics.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/License.txt` & `pyobjc-framework-CoreHaptics-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PKG-INFO` & `pyobjc-framework-CoreHaptics-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreHaptics
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreHaptics on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreHaptics
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticdevicecapability.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticdevicecapability.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticengine.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticengine.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticerror.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticevent.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticparameter.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticparameter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticpattern.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticpattern.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/PyObjCTest/test_chhapticpatternplayer.py` & `pyobjc-framework-CoreHaptics-9.2/PyObjCTest/test_chhapticpatternplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/CoreHaptics.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/CoreHaptics.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreHaptics-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreHaptics-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreHaptics-9.1b1/setup.py` & `pyobjc-framework-CoreHaptics-9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "CoreHaptics" framework on macOS.
 
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
     name="pyobjc-framework-CoreHaptics",
     description="Wrappers for the framework CoreHaptics on macOS",
     min_os_level="10.15",
     packages=["CoreHaptics"],
     version=VERSION,
```

