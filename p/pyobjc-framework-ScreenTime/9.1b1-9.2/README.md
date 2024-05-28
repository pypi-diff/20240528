# Comparing `tmp/pyobjc-framework-ScreenTime-9.1b1.tar.gz` & `tmp/pyobjc-framework-ScreenTime-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ScreenTime-9.1b1.tar", last modified: Sun Mar 26 11:38:43 2023, max compression
+gzip compressed data, was "pyobjc-framework-ScreenTime-9.2.tar", last modified: Wed Jun  7 00:27:13 2023, max compression
```

## Comparing `pyobjc-framework-ScreenTime-9.1b1.tar` & `pyobjc-framework-ScreenTime-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.710765 pyobjc-framework-ScreenTime-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.682444 pyobjc-framework-ScreenTime-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.690260 pyobjc-framework-ScreenTime-9.1b1/Lib/ScreenTime/
--rw-r--r--   0 ronald     (501) staff       (20)      702 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/ScreenTime/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1754 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/ScreenTime/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.693320 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2112 2023-03-26 11:38:43.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      871 2023-03-26 11:38:43.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:38:43.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:10.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:38:43.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:38:43.000000 pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScreenTime-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1901 2023-03-26 11:38:43.710316 pyobjc-framework-ScreenTime-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.696717 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/test_screentime.py
--rw-r--r--   0 ronald     (501) staff       (20)      259 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/test_stscreentimeconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/test_stwebhistory.py
--rw-r--r--   0 ronald     (501) staff       (20)     1007 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/test_stwebpagecontroller.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.700771 pyobjc-framework-ScreenTime-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/ScreenTime.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:43.709415 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     9039 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9058 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9076 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9039 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9040 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9059 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9077 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenTime-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:38:43.710979 pyobjc-framework-ScreenTime-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      669 2023-03-25 14:20:32.000000 pyobjc-framework-ScreenTime-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.564185 pyobjc-framework-ScreenTime-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.540995 pyobjc-framework-ScreenTime-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.545897 pyobjc-framework-ScreenTime-9.2/Lib/ScreenTime/
+-rw-r--r--   0 ronald     (501) staff       (20)      702 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/Lib/ScreenTime/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1754 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.2/Lib/ScreenTime/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.549295 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-06-07 00:27:13.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      886 2023-06-07 00:27:13.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:13.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:10.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:27:13.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:27:13.000000 pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScreenTime-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-06-07 00:27:13.563799 pyobjc-framework-ScreenTime-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.552814 pyobjc-framework-ScreenTime-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      204 2022-04-11 08:03:15.000000 pyobjc-framework-ScreenTime-9.2/PyObjCTest/test_screentime.py
+-rw-r--r--   0 ronald     (501) staff       (20)      259 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/PyObjCTest/test_stscreentimeconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.2/PyObjCTest/test_stwebhistory.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1007 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/PyObjCTest/test_stwebpagecontroller.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.554659 pyobjc-framework-ScreenTime-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/metadata/ScreenTime.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:13.563062 pyobjc-framework-ScreenTime-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     9039 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9058 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9076 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9039 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9040 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9059 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9077 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenTime-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ScreenTime-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:13.564293 pyobjc-framework-ScreenTime-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      751 2023-05-29 10:07:47.000000 pyobjc-framework-ScreenTime-9.2/setup.py
```

### Comparing `pyobjc-framework-ScreenTime-9.1b1/Lib/ScreenTime/__init__.py` & `pyobjc-framework-ScreenTime-9.2/Lib/ScreenTime/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/Lib/ScreenTime/_metadata.py` & `pyobjc-framework-ScreenTime-9.2/Lib/ScreenTime/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/PKG-INFO` & `pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenTime
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenTime on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenTime
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ScreenTime-9.1b1/Lib/pyobjc_framework_ScreenTime.egg-info/SOURCES.txt` & `pyobjc-framework-ScreenTime-9.2/Lib/pyobjc_framework_ScreenTime.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ScreenTime/__init__.py
 Lib/ScreenTime/_metadata.py
 Lib/pyobjc_framework_ScreenTime.egg-info/PKG-INFO
 Lib/pyobjc_framework_ScreenTime.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ScreenTime.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ScreenTime.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ScreenTime-9.1b1/License.txt` & `pyobjc-framework-ScreenTime-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/PKG-INFO` & `pyobjc-framework-ScreenTime-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenTime
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenTime on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenTime
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ScreenTime-9.1b1/PyObjCTest/test_stwebpagecontroller.py` & `pyobjc-framework-ScreenTime-9.2/PyObjCTest/test_stwebpagecontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-ScreenTime-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenTime-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ScreenTime-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

