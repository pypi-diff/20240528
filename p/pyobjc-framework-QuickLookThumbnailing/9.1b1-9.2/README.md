# Comparing `tmp/pyobjc-framework-QuickLookThumbnailing-9.1b1.tar.gz` & `tmp/pyobjc-framework-QuickLookThumbnailing-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-QuickLookThumbnailing-9.1b1.tar", last modified: Sun Mar 26 11:36:31 2023, max compression
+gzip compressed data, was "pyobjc-framework-QuickLookThumbnailing-9.2.tar", last modified: Wed Jun  7 00:25:31 2023, max compression
```

## Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1.tar` & `pyobjc-framework-QuickLookThumbnailing-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.227806 pyobjc-framework-QuickLookThumbnailing-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.187801 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.194742 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/QuickLookThumbnailing/
--rw-r--r--   0 ronald     (501) staff       (20)      779 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/QuickLookThumbnailing/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4629 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/QuickLookThumbnailing/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.200024 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2156 2023-03-26 11:36:31.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1080 2023-03-26 11:36:31.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:36:31.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:36:31.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       22 2023-03-26 11:36:31.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1945 2023-03-26 11:36:31.227339 pyobjc-framework-QuickLookThumbnailing-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.215176 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      650 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     1118 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailgenerationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      811 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailgenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)      383 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailreply.py
--rw-r--r--   0 ronald     (501) staff       (20)      514 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailrepresentation.py
--rw-r--r--   0 ronald     (501) staff       (20)      226 2022-04-11 08:03:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_quicklookthumbnailing.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.217398 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2501 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/QuickLookThumbnailing.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:31.226082 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16535 2021-07-30 09:00:38.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16993 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    13226 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14769 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16536 2021-07-30 09:00:38.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16994 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:36:31.227907 pyobjc-framework-QuickLookThumbnailing-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      783 2023-03-25 14:20:32.000000 pyobjc-framework-QuickLookThumbnailing-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.253977 pyobjc-framework-QuickLookThumbnailing-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.228924 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.234087 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/QuickLookThumbnailing/
+-rw-r--r--   0 ronald     (501) staff       (20)      779 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/QuickLookThumbnailing/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4629 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/QuickLookThumbnailing/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.237291 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2154 2023-06-07 00:25:31.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1095 2023-06-07 00:25:31.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:25:31.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:25:31.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       22 2023-06-07 00:25:31.000000 pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-QuickLookThumbnailing-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1943 2023-06-07 00:25:31.253580 pyobjc-framework-QuickLookThumbnailing-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.245898 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      650 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1118 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailgenerationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      811 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailgenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      383 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailreply.py
+-rw-r--r--   0 ronald     (501) staff       (20)      514 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailrepresentation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      226 2022-04-11 08:03:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_quicklookthumbnailing.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.247469 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2501 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/QuickLookThumbnailing.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:31.252410 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16535 2021-07-30 09:00:38.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16993 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    13226 2020-11-30 18:45:15.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14769 2021-03-21 10:08:23.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16536 2021-07-30 09:00:38.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16994 2023-02-19 10:50:35.000000 pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-QuickLookThumbnailing-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-QuickLookThumbnailing-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:25:31.254087 pyobjc-framework-QuickLookThumbnailing-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      865 2023-05-29 10:07:47.000000 pyobjc-framework-QuickLookThumbnailing-9.2/setup.py
```

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/QuickLookThumbnailing/__init__.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/Lib/QuickLookThumbnailing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/QuickLookThumbnailing/_metadata.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/Lib/QuickLookThumbnailing/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/PKG-INFO` & `pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-QuickLookThumbnailing
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework QuickLookThumbnailing on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,QuickLookThumbnailing
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/SOURCES.txt` & `pyobjc-framework-QuickLookThumbnailing-9.2/Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/QuickLookThumbnailing/__init__.py
 Lib/QuickLookThumbnailing/_metadata.py
 Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/PKG-INFO
 Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/SOURCES.txt
 Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/dependency_links.txt
 Lib/pyobjc_framework_QuickLookThumbnailing.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/License.txt` & `pyobjc-framework-QuickLookThumbnailing-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PKG-INFO` & `pyobjc-framework-QuickLookThumbnailing-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-QuickLookThumbnailing
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework QuickLookThumbnailing on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,QuickLookThumbnailing
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailerrors.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailgenerationrequest.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailgenerationrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailgenerator.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailgenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailreply.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailreply.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/PyObjCTest/test_qlthumbnailrepresentation.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/PyObjCTest/test_qlthumbnailrepresentation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/QuickLookThumbnailing.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/QuickLookThumbnailing.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-QuickLookThumbnailing-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/pyobjc_setup.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-QuickLookThumbnailing-9.1b1/setup.py` & `pyobjc-framework-QuickLookThumbnailing-9.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-QuickLookThumbnailing",
     description="Wrappers for the framework QuickLookThumbnailing on macOS",
     min_os_level="10.15",
     packages=["QuickLookThumbnailing"],
     version=VERSION,
```

