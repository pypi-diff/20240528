# Comparing `tmp/pyobjc-framework-MediaLibrary-9.1b1.tar.gz` & `tmp/pyobjc-framework-MediaLibrary-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MediaLibrary-9.1b1.tar", last modified: Sun Mar 26 11:28:53 2023, max compression
+gzip compressed data, was "pyobjc-framework-MediaLibrary-9.2.tar", last modified: Wed Jun  7 00:19:26 2023, max compression
```

## Comparing `pyobjc-framework-MediaLibrary-9.1b1.tar` & `pyobjc-framework-MediaLibrary-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.435812 pyobjc-framework-MediaLibrary-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.390357 pyobjc-framework-MediaLibrary-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.395507 pyobjc-framework-MediaLibrary-9.1b1/Lib/MediaLibrary/
--rw-r--r--   0 ronald     (501) staff       (20)      727 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/MediaLibrary/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5904 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/MediaLibrary/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.398259 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2144 2023-03-26 11:28:53.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      941 2023-03-26 11:28:53.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:53.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:18.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:28:53.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:28:53.000000 pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaLibrary-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1933 2023-03-26 11:28:53.435492 pyobjc-framework-MediaLibrary-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.406958 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_medialibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmediagroup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1908 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmedialibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmediaobject.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmediasource.py
--rw-r--r--   0 ronald     (501) staff       (20)    12243 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmediatypes.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.408700 pyobjc-framework-MediaLibrary-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1125 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/MediaLibrary.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:53.434733 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    24180 2021-07-30 09:00:38.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24291 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    23400 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24181 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21895 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24181 2021-07-30 09:00:38.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24292 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaLibrary-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:53.435917 pyobjc-framework-MediaLibrary-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      771 2023-03-25 14:20:31.000000 pyobjc-framework-MediaLibrary-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:26.007801 pyobjc-framework-MediaLibrary-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:25.970853 pyobjc-framework-MediaLibrary-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:25.975490 pyobjc-framework-MediaLibrary-9.2/Lib/MediaLibrary/
+-rw-r--r--   0 ronald     (501) staff       (20)      727 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/Lib/MediaLibrary/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5904 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.2/Lib/MediaLibrary/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:25.978746 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2142 2023-06-07 00:19:25.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      956 2023-06-07 00:19:25.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:25.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:18.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:19:25.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:19:25.000000 pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaLibrary-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1931 2023-06-07 00:19:26.007391 pyobjc-framework-MediaLibrary-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:25.987512 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_medialibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmediagroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1908 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmedialibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmediaobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmediasource.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12243 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmediatypes.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:25.989178 pyobjc-framework-MediaLibrary-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1125 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/metadata/MediaLibrary.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:26.006154 pyobjc-framework-MediaLibrary-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    24180 2021-07-30 09:00:38.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24291 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    23400 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24181 2021-03-21 10:08:23.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21895 2020-11-30 18:45:15.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24181 2021-07-30 09:00:38.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24292 2022-02-24 08:47:16.000000 pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaLibrary-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MediaLibrary-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:26.007893 pyobjc-framework-MediaLibrary-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      852 2023-05-29 10:07:46.000000 pyobjc-framework-MediaLibrary-9.2/setup.py
```

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/Lib/MediaLibrary/__init__.py` & `pyobjc-framework-MediaLibrary-9.2/Lib/MediaLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/Lib/MediaLibrary/_metadata.py` & `pyobjc-framework-MediaLibrary-9.2/Lib/MediaLibrary/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/PKG-INFO` & `pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaLibrary
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaLibrary on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaLibrary
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/Lib/pyobjc_framework_MediaLibrary.egg-info/SOURCES.txt` & `pyobjc-framework-MediaLibrary-9.2/Lib/pyobjc_framework_MediaLibrary.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MediaLibrary/__init__.py
 Lib/MediaLibrary/_metadata.py
 Lib/pyobjc_framework_MediaLibrary.egg-info/PKG-INFO
 Lib/pyobjc_framework_MediaLibrary.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MediaLibrary.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MediaLibrary.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/License.txt` & `pyobjc-framework-MediaLibrary-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/PKG-INFO` & `pyobjc-framework-MediaLibrary-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaLibrary
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaLibrary on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaLibrary
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmedialibrary.py` & `pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmedialibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/PyObjCTest/test_mlmediatypes.py` & `pyobjc-framework-MediaLibrary-9.2/PyObjCTest/test_mlmediatypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/MediaLibrary.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/MediaLibrary.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MediaLibrary-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MediaLibrary-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaLibrary-9.1b1/setup.py` & `pyobjc-framework-MediaLibrary-9.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "MediaLibrary" framework on macOS introduced in macOS 10.9.
 
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
     name="pyobjc-framework-MediaLibrary",
     description="Wrappers for the framework MediaLibrary on macOS",
     min_os_level="10.9",
     packages=["MediaLibrary"],
     version=VERSION,
```

