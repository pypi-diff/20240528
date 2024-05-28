# Comparing `tmp/pyobjc-framework-AppTrackingTransparency-9.1b1.tar.gz` & `tmp/pyobjc-framework-AppTrackingTransparency-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AppTrackingTransparency-9.1b1.tar", last modified: Sun Mar 26 11:14:09 2023, max compression
+gzip compressed data, was "pyobjc-framework-AppTrackingTransparency-9.2.tar", last modified: Wed Jun  7 00:05:51 2023, max compression
```

## Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1.tar` & `pyobjc-framework-AppTrackingTransparency-9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.121356 pyobjc-framework-AppTrackingTransparency-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.092882 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.105263 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/AppTrackingTransparency/
--rw-r--r--   0 ronald     (501) staff       (20)      807 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/AppTrackingTransparency/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1425 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/AppTrackingTransparency/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.108451 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2164 2023-03-26 11:14:09.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      922 2023-03-26 11:14:09.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:09.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:14.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:14:09.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       24 2023-03-26 11:14:09.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1953 2023-03-26 11:14:09.120688 pyobjc-framework-AppTrackingTransparency-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.110103 pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      549 2022-04-11 08:03:15.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/test_apptrackingtransparency.py
--rw-r--r--   0 ronald     (501) staff       (20)     1023 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/test_attrackingmanager.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.111104 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      305 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/AppTrackingTransparency.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       62 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:09.119789 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     2592 2021-07-30 09:00:37.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2680 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2788 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2593 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2593 2021-07-30 09:00:37.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2681 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2789 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:09.121576 pyobjc-framework-AppTrackingTransparency-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      721 2023-03-25 14:20:30.000000 pyobjc-framework-AppTrackingTransparency-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.740261 pyobjc-framework-AppTrackingTransparency-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.718883 pyobjc-framework-AppTrackingTransparency-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.723465 pyobjc-framework-AppTrackingTransparency-9.2/Lib/AppTrackingTransparency/
+-rw-r--r--   0 ronald     (501) staff       (20)      807 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/AppTrackingTransparency/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1425 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/AppTrackingTransparency/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.726899 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2162 2023-06-07 00:05:51.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      937 2023-06-07 00:05:51.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:51.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:14.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:51.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       24 2023-06-07 00:05:51.000000 pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AppTrackingTransparency-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1951 2023-06-07 00:05:51.739898 pyobjc-framework-AppTrackingTransparency-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.728432 pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      549 2022-04-11 08:03:15.000000 pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/test_apptrackingtransparency.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1023 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/test_attrackingmanager.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.729757 pyobjc-framework-AppTrackingTransparency-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/AppTrackingTransparency.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       62 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:51.738979 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     2592 2021-07-30 09:00:37.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2680 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2788 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2593 2021-03-21 10:08:22.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2593 2021-07-30 09:00:37.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2681 2022-02-24 08:47:16.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2789 2023-02-19 10:50:34.000000 pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AppTrackingTransparency-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AppTrackingTransparency-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:51.740380 pyobjc-framework-AppTrackingTransparency-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      802 2023-05-29 10:07:45.000000 pyobjc-framework-AppTrackingTransparency-9.2/setup.py
```

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/AppTrackingTransparency/__init__.py` & `pyobjc-framework-AppTrackingTransparency-9.2/Lib/AppTrackingTransparency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/AppTrackingTransparency/_metadata.py` & `pyobjc-framework-AppTrackingTransparency-9.2/Lib/AppTrackingTransparency/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/PKG-INFO` & `pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppTrackingTransparency
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppTrackingTransparency on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppTrackingTransparency
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/SOURCES.txt` & `pyobjc-framework-AppTrackingTransparency-9.2/Lib/pyobjc_framework_AppTrackingTransparency.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AppTrackingTransparency/__init__.py
 Lib/AppTrackingTransparency/_metadata.py
 Lib/pyobjc_framework_AppTrackingTransparency.egg-info/PKG-INFO
 Lib/pyobjc_framework_AppTrackingTransparency.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AppTrackingTransparency.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AppTrackingTransparency.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/License.txt` & `pyobjc-framework-AppTrackingTransparency-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/PKG-INFO` & `pyobjc-framework-AppTrackingTransparency-9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AppTrackingTransparency
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AppTrackingTransparency on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AppTrackingTransparency
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/test_apptrackingtransparency.py` & `pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/test_apptrackingtransparency.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/PyObjCTest/test_attrackingmanager.py` & `pyobjc-framework-AppTrackingTransparency-9.2/PyObjCTest/test_attrackingmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-AppTrackingTransparency-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AppTrackingTransparency-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AppTrackingTransparency-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

