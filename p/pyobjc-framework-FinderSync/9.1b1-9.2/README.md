# Comparing `tmp/pyobjc-framework-FinderSync-9.1b1.tar.gz` & `tmp/pyobjc-framework-FinderSync-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-FinderSync-9.1b1.tar", last modified: Sun Mar 26 11:24:43 2023, max compression
+gzip compressed data, was "pyobjc-framework-FinderSync-9.2.tar", last modified: Wed Jun  7 00:14:56 2023, max compression
```

## Comparing `pyobjc-framework-FinderSync-9.1b1.tar` & `pyobjc-framework-FinderSync-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.993073 pyobjc-framework-FinderSync-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FinderSync-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.968786 pyobjc-framework-FinderSync-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.974457 pyobjc-framework-FinderSync-9.1b1/Lib/FinderSync/
--rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/Lib/FinderSync/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3789 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.1b1/Lib/FinderSync/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.977211 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2138 2023-03-26 11:24:43.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      799 2023-03-26 11:24:43.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:43.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:11.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:24:43.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:24:43.000000 pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1927 2023-03-26 11:24:43.992589 pyobjc-framework-FinderSync-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.978269 pyobjc-framework-FinderSync-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2022-06-25 09:10:43.000000 pyobjc-framework-FinderSync-9.1b1/PyObjCTest/test_findersync.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-FinderSync-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.979861 pyobjc-framework-FinderSync-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1574 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/metadata/FinderSync.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:43.989995 pyobjc-framework-FinderSync-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10282 2021-07-30 09:00:38.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10344 2022-02-24 08:47:16.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10397 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5948 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10283 2021-03-21 10:08:22.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10283 2021-07-30 09:00:38.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10345 2022-02-24 08:47:16.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10398 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FinderSync-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:43.993183 pyobjc-framework-FinderSync-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      669 2023-03-25 14:20:31.000000 pyobjc-framework-FinderSync-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.646112 pyobjc-framework-FinderSync-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FinderSync-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.622462 pyobjc-framework-FinderSync-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.628481 pyobjc-framework-FinderSync-9.2/Lib/FinderSync/
+-rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/Lib/FinderSync/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3789 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.2/Lib/FinderSync/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.632183 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-06-07 00:14:56.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      814 2023-06-07 00:14:56.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:14:56.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:11.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:14:56.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:14:56.000000 pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-06-07 00:14:56.645563 pyobjc-framework-FinderSync-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.633549 pyobjc-framework-FinderSync-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2116 2022-06-25 09:10:43.000000 pyobjc-framework-FinderSync-9.2/PyObjCTest/test_findersync.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-FinderSync-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.634975 pyobjc-framework-FinderSync-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1574 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/metadata/FinderSync.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:56.644657 pyobjc-framework-FinderSync-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10282 2021-07-30 09:00:38.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10344 2022-02-24 08:47:16.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10397 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5948 2020-11-30 18:45:15.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10283 2021-03-21 10:08:22.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10283 2021-07-30 09:00:38.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10345 2022-02-24 08:47:16.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10398 2023-02-19 10:50:35.000000 pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FinderSync-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-FinderSync-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:14:56.646264 pyobjc-framework-FinderSync-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      750 2023-05-29 10:07:46.000000 pyobjc-framework-FinderSync-9.2/setup.py
```

### Comparing `pyobjc-framework-FinderSync-9.1b1/LICENSE.txt` & `pyobjc-framework-FinderSync-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/Lib/FinderSync/__init__.py` & `pyobjc-framework-FinderSync-9.2/Lib/FinderSync/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/Lib/FinderSync/_metadata.py` & `pyobjc-framework-FinderSync-9.2/Lib/FinderSync/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/PKG-INFO` & `pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FinderSync
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FinderSync on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FinderSync
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-FinderSync-9.1b1/Lib/pyobjc_framework_FinderSync.egg-info/SOURCES.txt` & `pyobjc-framework-FinderSync-9.2/Lib/pyobjc_framework_FinderSync.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/FinderSync/__init__.py
 Lib/FinderSync/_metadata.py
 Lib/pyobjc_framework_FinderSync.egg-info/PKG-INFO
 Lib/pyobjc_framework_FinderSync.egg-info/SOURCES.txt
 Lib/pyobjc_framework_FinderSync.egg-info/dependency_links.txt
 Lib/pyobjc_framework_FinderSync.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-FinderSync-9.1b1/PKG-INFO` & `pyobjc-framework-FinderSync-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FinderSync
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FinderSync on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FinderSync
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-FinderSync-9.1b1/PyObjCTest/test_findersync.py` & `pyobjc-framework-FinderSync-9.2/PyObjCTest/test_findersync.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/FinderSync.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/FinderSync.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-FinderSync-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FinderSync-9.1b1/pyobjc_setup.py` & `pyobjc-framework-FinderSync-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

