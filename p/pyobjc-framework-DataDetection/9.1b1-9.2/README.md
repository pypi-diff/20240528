# Comparing `tmp/pyobjc-framework-DataDetection-9.1b1.tar.gz` & `tmp/pyobjc-framework-DataDetection-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DataDetection-9.1b1.tar", last modified: Sun Mar 26 11:23:02 2023, max compression
+gzip compressed data, was "pyobjc-framework-DataDetection-9.2.tar", last modified: Wed Jun  7 00:13:06 2023, max compression
```

## Comparing `pyobjc-framework-DataDetection-9.1b1.tar` & `pyobjc-framework-DataDetection-9.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.854588 pyobjc-framework-DataDetection-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.827666 pyobjc-framework-DataDetection-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.832262 pyobjc-framework-DataDetection-9.1b1/Lib/DataDetection/
--rw-r--r--   0 ronald     (501) staff       (20)      711 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/Lib/DataDetection/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      781 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.1b1/Lib/DataDetection/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.835609 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2123 2023-03-26 11:23:02.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      752 2023-03-26 11:23:02.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:02.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:08.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:02.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:23:02.000000 pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DataDetection-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1912 2023-03-26 11:23:02.854277 pyobjc-framework-DataDetection-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.836714 pyobjc-framework-DataDetection-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-DataDetection-9.1b1/PyObjCTest/test_datadetection.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.838155 pyobjc-framework-DataDetection-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/metadata/DataDetection.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:02.853471 pyobjc-framework-DataDetection-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    11244 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10649 2022-02-24 08:47:16.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10667 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11245 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10650 2022-02-24 08:47:16.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10668 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DataDetection-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:02.854698 pyobjc-framework-DataDetection-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      702 2023-03-25 14:20:31.000000 pyobjc-framework-DataDetection-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.647693 pyobjc-framework-DataDetection-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.626284 pyobjc-framework-DataDetection-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.631393 pyobjc-framework-DataDetection-9.2/Lib/DataDetection/
+-rw-r--r--   0 ronald     (501) staff       (20)      711 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/Lib/DataDetection/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.2/Lib/DataDetection/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.635169 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2121 2023-06-07 00:13:06.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      767 2023-06-07 00:13:06.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:06.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:08.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:06.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:13:06.000000 pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DataDetection-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1910 2023-06-07 00:13:06.647287 pyobjc-framework-DataDetection-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.636477 pyobjc-framework-DataDetection-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-DataDetection-9.2/PyObjCTest/test_datadetection.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.637794 pyobjc-framework-DataDetection-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/metadata/DataDetection.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:06.646417 pyobjc-framework-DataDetection-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    11244 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10649 2022-02-24 08:47:16.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10667 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11245 2021-07-30 09:00:37.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10650 2022-02-24 08:47:16.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10668 2023-02-19 10:50:35.000000 pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DataDetection-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DataDetection-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:06.647823 pyobjc-framework-DataDetection-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2023-05-29 10:07:46.000000 pyobjc-framework-DataDetection-9.2/setup.py
```

### Comparing `pyobjc-framework-DataDetection-9.1b1/Lib/DataDetection/__init__.py` & `pyobjc-framework-DataDetection-9.2/Lib/DataDetection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/Lib/DataDetection/_metadata.py` & `pyobjc-framework-DataDetection-9.2/Lib/DataDetection/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/PKG-INFO` & `pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DataDetection
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DataDetection on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DataDetection
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-DataDetection-9.1b1/Lib/pyobjc_framework_DataDetection.egg-info/SOURCES.txt` & `pyobjc-framework-DataDetection-9.2/Lib/pyobjc_framework_DataDetection.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/DataDetection/__init__.py
 Lib/DataDetection/_metadata.py
 Lib/pyobjc_framework_DataDetection.egg-info/PKG-INFO
 Lib/pyobjc_framework_DataDetection.egg-info/SOURCES.txt
 Lib/pyobjc_framework_DataDetection.egg-info/dependency_links.txt
 Lib/pyobjc_framework_DataDetection.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-DataDetection-9.1b1/License.txt` & `pyobjc-framework-DataDetection-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/PKG-INFO` & `pyobjc-framework-DataDetection-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DataDetection
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DataDetection on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DataDetection
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-DataDetection-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DataDetection-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DataDetection-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

