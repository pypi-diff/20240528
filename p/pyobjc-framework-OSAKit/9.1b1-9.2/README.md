# Comparing `tmp/pyobjc-framework-OSAKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-OSAKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-OSAKit-9.1b1.tar", last modified: Sun Mar 26 11:32:36 2023, max compression
+gzip compressed data, was "pyobjc-framework-OSAKit-9.2.tar", last modified: Wed Jun  7 00:22:39 2023, max compression
```

## Comparing `pyobjc-framework-OSAKit-9.1b1.tar` & `pyobjc-framework-OSAKit-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.804845 pyobjc-framework-OSAKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.762590 pyobjc-framework-OSAKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.772720 pyobjc-framework-OSAKit-9.1b1/Lib/OSAKit/
--rw-r--r--   0 ronald     (501) staff       (20)      664 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/Lib/OSAKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4631 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.1b1/Lib/OSAKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.791738 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2086 2023-03-26 11:32:36.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      788 2023-03-26 11:32:36.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:32:36.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:44.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:32:36.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:32:36.000000 pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-OSAKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1875 2023-03-26 11:32:36.804491 pyobjc-framework-OSAKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.796795 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3775 2022-04-11 08:03:15.000000 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osakit.py
--rw-r--r--   0 ronald     (501) staff       (20)      813 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osalanguage.py
--rw-r--r--   0 ronald     (501) staff       (20)      392 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osascriptcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      691 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osascriptview.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.797982 pyobjc-framework-OSAKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3360 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/metadata/OSAKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:36.803669 pyobjc-framework-OSAKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    30517 2021-07-30 09:00:38.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30681 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30503 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30518 2021-03-21 10:08:23.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30518 2021-07-30 09:00:38.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30682 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-OSAKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:32:36.804949 pyobjc-framework-OSAKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      627 2023-03-25 14:20:32.000000 pyobjc-framework-OSAKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.461990 pyobjc-framework-OSAKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.437571 pyobjc-framework-OSAKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.442514 pyobjc-framework-OSAKit-9.2/Lib/OSAKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      664 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/Lib/OSAKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4631 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.2/Lib/OSAKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.445592 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2084 2023-06-07 00:22:39.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2023-06-07 00:22:39.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:22:39.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:44.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:22:39.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:22:39.000000 pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-OSAKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1873 2023-06-07 00:22:39.461550 pyobjc-framework-OSAKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.448941 pyobjc-framework-OSAKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3775 2022-04-11 08:03:15.000000 pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osakit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      813 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osalanguage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      392 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osascriptcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      691 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osascriptview.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.450147 pyobjc-framework-OSAKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3360 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/metadata/OSAKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:39.460271 pyobjc-framework-OSAKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    30517 2021-07-30 09:00:38.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30681 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30503 2020-11-30 18:45:15.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30518 2021-03-21 10:08:23.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30518 2021-07-30 09:00:38.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30682 2022-02-24 08:47:16.000000 pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-OSAKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-OSAKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:22:39.462104 pyobjc-framework-OSAKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      708 2023-05-29 10:07:46.000000 pyobjc-framework-OSAKit-9.2/setup.py
```

### Comparing `pyobjc-framework-OSAKit-9.1b1/Lib/OSAKit/__init__.py` & `pyobjc-framework-OSAKit-9.2/Lib/OSAKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/Lib/OSAKit/_metadata.py` & `pyobjc-framework-OSAKit-9.2/Lib/OSAKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/PKG-INFO` & `pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-OSAKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework OSAKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,OSAKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-OSAKit-9.1b1/Lib/pyobjc_framework_OSAKit.egg-info/SOURCES.txt` & `pyobjc-framework-OSAKit-9.2/Lib/pyobjc_framework_OSAKit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/OSAKit/__init__.py
 Lib/OSAKit/_metadata.py
 Lib/pyobjc_framework_OSAKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_OSAKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_OSAKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_OSAKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-OSAKit-9.1b1/License.txt` & `pyobjc-framework-OSAKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/PKG-INFO` & `pyobjc-framework-OSAKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-OSAKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework OSAKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,OSAKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osakit.py` & `pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osakit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osalanguage.py` & `pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osalanguage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/PyObjCTest/test_osascriptview.py` & `pyobjc-framework-OSAKit-9.2/PyObjCTest/test_osascriptview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/OSAKit.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/OSAKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-OSAKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OSAKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-OSAKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

