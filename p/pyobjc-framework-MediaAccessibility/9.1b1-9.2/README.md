# Comparing `tmp/pyobjc-framework-MediaAccessibility-9.1b1.tar.gz` & `tmp/pyobjc-framework-MediaAccessibility-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MediaAccessibility-9.1b1.tar", last modified: Sun Mar 26 11:28:48 2023, max compression
+gzip compressed data, was "pyobjc-framework-MediaAccessibility-9.2.tar", last modified: Wed Jun  7 00:19:20 2023, max compression
```

## Comparing `pyobjc-framework-MediaAccessibility-9.1b1.tar` & `pyobjc-framework-MediaAccessibility-9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.674206 pyobjc-framework-MediaAccessibility-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.641317 pyobjc-framework-MediaAccessibility-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.649579 pyobjc-framework-MediaAccessibility-9.1b1/Lib/MediaAccessibility/
--rw-r--r--   0 ronald     (501) staff       (20)      741 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/MediaAccessibility/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5911 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/MediaAccessibility/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.654364 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2155 2023-03-26 11:28:48.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1084 2023-03-26 11:28:48.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:48.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:26.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:28:48.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:28:48.000000 pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaAccessibility-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1944 2023-03-26 11:28:48.673799 pyobjc-framework-MediaAccessibility-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.665125 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      829 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_maaudiblemedia.py
--rw-r--r--   0 ronald     (501) staff       (20)     5124 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_macaptionappearance.py
--rw-r--r--   0 ronald     (501) staff       (20)      725 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_maimagecaptioning.py
--rw-r--r--   0 ronald     (501) staff       (20)      414 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_mavideoaccommodations.py
--rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_mediaaccessibility.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.667543 pyobjc-framework-MediaAccessibility-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2190 2022-04-11 15:02:41.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/MediaAccessibility.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:48.673217 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     7475 2021-07-30 09:00:38.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7793 2022-02-24 08:47:16.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8451 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6268 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7478 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7476 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5815 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7476 2021-07-30 09:00:38.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7794 2022-02-24 08:47:16.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8452 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaAccessibility-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:48.674306 pyobjc-framework-MediaAccessibility-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      712 2023-03-25 14:20:31.000000 pyobjc-framework-MediaAccessibility-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.997850 pyobjc-framework-MediaAccessibility-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.957762 pyobjc-framework-MediaAccessibility-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.962648 pyobjc-framework-MediaAccessibility-9.2/Lib/MediaAccessibility/
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/MediaAccessibility/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5911 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/MediaAccessibility/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.966414 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2153 2023-06-07 00:19:20.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1099 2023-06-07 00:19:20.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:20.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:26.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:19:20.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-06-07 00:19:20.000000 pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaAccessibility-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1942 2023-06-07 00:19:20.997355 pyobjc-framework-MediaAccessibility-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.974316 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_maaudiblemedia.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5124 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_macaptionappearance.py
+-rw-r--r--   0 ronald     (501) staff       (20)      725 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_maimagecaptioning.py
+-rw-r--r--   0 ronald     (501) staff       (20)      414 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_mavideoaccommodations.py
+-rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_mediaaccessibility.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.976155 pyobjc-framework-MediaAccessibility-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2190 2022-04-11 15:02:41.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/MediaAccessibility.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:20.996173 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     7475 2021-07-30 09:00:38.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7793 2022-02-24 08:47:16.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8451 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6268 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7478 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7476 2021-03-21 10:08:23.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5815 2020-11-30 18:45:15.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7476 2021-07-30 09:00:38.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7794 2022-02-24 08:47:16.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8452 2023-02-19 10:50:35.000000 pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaAccessibility-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MediaAccessibility-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:20.997957 pyobjc-framework-MediaAccessibility-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      793 2023-05-29 10:07:46.000000 pyobjc-framework-MediaAccessibility-9.2/setup.py
```

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/Lib/MediaAccessibility/__init__.py` & `pyobjc-framework-MediaAccessibility-9.2/Lib/MediaAccessibility/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/Lib/MediaAccessibility/_metadata.py` & `pyobjc-framework-MediaAccessibility-9.2/Lib/MediaAccessibility/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/PKG-INFO` & `pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaAccessibility
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaAccessibility on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaAccessibility
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/Lib/pyobjc_framework_MediaAccessibility.egg-info/SOURCES.txt` & `pyobjc-framework-MediaAccessibility-9.2/Lib/pyobjc_framework_MediaAccessibility.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MediaAccessibility/__init__.py
 Lib/MediaAccessibility/_metadata.py
 Lib/pyobjc_framework_MediaAccessibility.egg-info/PKG-INFO
 Lib/pyobjc_framework_MediaAccessibility.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MediaAccessibility.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MediaAccessibility.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/License.txt` & `pyobjc-framework-MediaAccessibility-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/PKG-INFO` & `pyobjc-framework-MediaAccessibility-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaAccessibility
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaAccessibility on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaAccessibility
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_maaudiblemedia.py` & `pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_maaudiblemedia.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_macaptionappearance.py` & `pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_macaptionappearance.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/PyObjCTest/test_maimagecaptioning.py` & `pyobjc-framework-MediaAccessibility-9.2/PyObjCTest/test_maimagecaptioning.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/MediaAccessibility.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/MediaAccessibility.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-MediaAccessibility-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaAccessibility-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MediaAccessibility-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

