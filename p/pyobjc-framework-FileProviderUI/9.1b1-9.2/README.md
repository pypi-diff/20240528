# Comparing `tmp/pyobjc-framework-FileProviderUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-FileProviderUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-FileProviderUI-9.1b1.tar", last modified: Sun Mar 26 11:24:39 2023, max compression
+gzip compressed data, was "pyobjc-framework-FileProviderUI-9.2.tar", last modified: Wed Jun  7 00:14:51 2023, max compression
```

## Comparing `pyobjc-framework-FileProviderUI-9.1b1.tar` & `pyobjc-framework-FileProviderUI-9.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.412149 pyobjc-framework-FileProviderUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.383382 pyobjc-framework-FileProviderUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.388044 pyobjc-framework-FileProviderUI-9.1b1/Lib/FileProviderUI/
--rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/FileProviderUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1158 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/FileProviderUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.391443 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2128 2023-03-26 11:24:39.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      811 2023-03-26 11:24:39.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:39.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:10.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:24:39.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:24:39.000000 pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FileProviderUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1917 2023-03-26 11:24:39.411822 pyobjc-framework-FileProviderUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.404988 pyobjc-framework-FileProviderUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-FileProviderUI-9.1b1/PyObjCTest/test_fileproviderui.py
--rw-r--r--   0 ronald     (501) staff       (20)      799 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.1b1/PyObjCTest/test_fpuiactionextensioncontext.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.406562 pyobjc-framework-FileProviderUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/FileProviderUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:39.411071 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     3904 2021-07-30 09:00:38.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3978 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3678 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3905 2021-03-21 10:08:22.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3905 2021-07-30 09:00:38.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3979 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FileProviderUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:39.412247 pyobjc-framework-FileProviderUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      715 2023-03-25 14:20:31.000000 pyobjc-framework-FileProviderUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.678215 pyobjc-framework-FileProviderUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.655344 pyobjc-framework-FileProviderUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.660464 pyobjc-framework-FileProviderUI-9.2/Lib/FileProviderUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.2/Lib/FileProviderUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1158 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.2/Lib/FileProviderUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.663704 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2126 2023-06-07 00:14:51.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      826 2023-06-07 00:14:51.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:14:51.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:10.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:14:51.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:14:51.000000 pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FileProviderUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1915 2023-06-07 00:14:51.677839 pyobjc-framework-FileProviderUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.665536 pyobjc-framework-FileProviderUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FileProviderUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-FileProviderUI-9.2/PyObjCTest/test_fileproviderui.py
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.2/PyObjCTest/test_fpuiactionextensioncontext.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.672321 pyobjc-framework-FileProviderUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.2/metadata/FileProviderUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:51.677001 pyobjc-framework-FileProviderUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     3904 2021-07-30 09:00:38.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3978 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3678 2020-11-30 18:45:15.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3905 2021-03-21 10:08:22.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3905 2021-07-30 09:00:38.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3979 2022-02-24 08:47:16.000000 pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FileProviderUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-FileProviderUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:14:51.678330 pyobjc-framework-FileProviderUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      796 2023-05-29 10:07:46.000000 pyobjc-framework-FileProviderUI-9.2/setup.py
```

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/Lib/FileProviderUI/__init__.py` & `pyobjc-framework-FileProviderUI-9.2/Lib/FileProviderUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/Lib/FileProviderUI/_metadata.py` & `pyobjc-framework-FileProviderUI-9.2/Lib/FileProviderUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/PKG-INFO` & `pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FileProviderUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FileProviderUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FileProviderUI
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/Lib/pyobjc_framework_FileProviderUI.egg-info/SOURCES.txt` & `pyobjc-framework-FileProviderUI-9.2/Lib/pyobjc_framework_FileProviderUI.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/FileProviderUI/__init__.py
 Lib/FileProviderUI/_metadata.py
 Lib/pyobjc_framework_FileProviderUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_FileProviderUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_FileProviderUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_FileProviderUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/License.txt` & `pyobjc-framework-FileProviderUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/PKG-INFO` & `pyobjc-framework-FileProviderUI-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FileProviderUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FileProviderUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FileProviderUI
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/PyObjCTest/test_fpuiactionextensioncontext.py` & `pyobjc-framework-FileProviderUI-9.2/PyObjCTest/test_fpuiactionextensioncontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-FileProviderUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FileProviderUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-FileProviderUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

