# Comparing `tmp/pyobjc-framework-AppleScriptKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-AppleScriptKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AppleScriptKit-9.1b1.tar", last modified: Sun Mar 26 11:14:15 2023, max compression
+gzip compressed data, was "pyobjc-framework-AppleScriptKit-9.2.tar", last modified: Wed Jun  7 00:05:56 2023, max compression
```

## Comparing `pyobjc-framework-AppleScriptKit-9.1b1.tar` & `pyobjc-framework-AppleScriptKit-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.748393 pyobjc-framework-AppleScriptKit-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppleScriptKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.725206 pyobjc-framework-AppleScriptKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.737736 pyobjc-framework-AppleScriptKit-9.1b1/Lib/AppleScriptKit/
--rw-r--r--   0 ronald     (501) staff       (20)      722 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/AppleScriptKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/AppleScriptKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.740808 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2131 2023-03-26 11:14:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      839 2023-03-26 11:14:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:18.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:14:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:14:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1920 2023-03-26 11:14:15.748057 pyobjc-framework-AppleScriptKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.741774 pyobjc-framework-AppleScriptKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      504 2022-04-11 08:03:15.000000 pyobjc-framework-AppleScriptKit-9.1b1/PyObjCTest/test_applescriptkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-AppleScriptKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.743012 pyobjc-framework-AppleScriptKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      213 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/AppleScriptKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:15.747406 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     1099 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1118 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1100 2021-03-21 10:08:22.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1014 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1014 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1103 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1100 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1119 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppleScriptKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:15.748500 pyobjc-framework-AppleScriptKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      645 2023-03-25 14:20:30.000000 pyobjc-framework-AppleScriptKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.414627 pyobjc-framework-AppleScriptKit-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppleScriptKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.380595 pyobjc-framework-AppleScriptKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.386685 pyobjc-framework-AppleScriptKit-9.2/Lib/AppleScriptKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      722 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/AppleScriptKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/AppleScriptKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.389859 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2129 2023-06-07 00:05:56.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      854 2023-06-07 00:05:56.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:56.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:18.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:56.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:05:56.000000 pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1918 2023-06-07 00:05:56.412506 pyobjc-framework-AppleScriptKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.390893 pyobjc-framework-AppleScriptKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      504 2022-04-11 08:03:15.000000 pyobjc-framework-AppleScriptKit-9.2/PyObjCTest/test_applescriptkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-AppleScriptKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.392346 pyobjc-framework-AppleScriptKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      213 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/AppleScriptKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:56.409807 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     1099 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1118 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1100 2021-03-21 10:08:22.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1014 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1014 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1103 2020-11-30 18:45:14.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1100 2021-07-30 09:00:37.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1119 2022-02-24 08:47:16.000000 pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppleScriptKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AppleScriptKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:56.415201 pyobjc-framework-AppleScriptKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      727 2023-05-29 10:07:45.000000 pyobjc-framework-AppleScriptKit-9.2/setup.py
```

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/LICENSE.txt` & `pyobjc-framework-AppleScriptKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/Lib/AppleScriptKit/__init__.py` & `pyobjc-framework-AppleScriptKit-9.2/Lib/AppleScriptKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/PKG-INFO` & `pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppleScriptKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppleScriptKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppleScriptKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/Lib/pyobjc_framework_AppleScriptKit.egg-info/SOURCES.txt` & `pyobjc-framework-AppleScriptKit-9.2/Lib/pyobjc_framework_AppleScriptKit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AppleScriptKit/__init__.py
 Lib/AppleScriptKit/_metadata.py
 Lib/pyobjc_framework_AppleScriptKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_AppleScriptKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AppleScriptKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AppleScriptKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/PKG-INFO` & `pyobjc-framework-AppleScriptKit-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppleScriptKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppleScriptKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppleScriptKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AppleScriptKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppleScriptKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AppleScriptKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

