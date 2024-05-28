# Comparing `tmp/pyobjc-framework-LinkPresentation-9.1b1.tar.gz` & `tmp/pyobjc-framework-LinkPresentation-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LinkPresentation-9.1b1.tar", last modified: Sun Mar 26 11:28:08 2023, max compression
+gzip compressed data, was "pyobjc-framework-LinkPresentation-9.2.tar", last modified: Wed Jun  7 00:18:37 2023, max compression
```

## Comparing `pyobjc-framework-LinkPresentation-9.1b1.tar` & `pyobjc-framework-LinkPresentation-9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.932053 pyobjc-framework-LinkPresentation-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.909463 pyobjc-framework-LinkPresentation-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.914031 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/
--rw-r--r--   0 ronald     (501) staff       (20)      744 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2045 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.916965 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      947 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LinkPresentation-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:28:08.931744 pyobjc-framework-LinkPresentation-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.920094 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_linkpresentation.py
--rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lperror.py
--rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lplinkmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      823 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lpmetadataprovider.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.921636 pyobjc-framework-LinkPresentation-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      896 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/LinkPresentation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.931161 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10808 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10871 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10929 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9843 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10123 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10809 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10872 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10930 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LinkPresentation-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:08.932164 pyobjc-framework-LinkPresentation-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      763 2023-03-25 14:20:31.000000 pyobjc-framework-LinkPresentation-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:37.018888 pyobjc-framework-LinkPresentation-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:36.993422 pyobjc-framework-LinkPresentation-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:36.999188 pyobjc-framework-LinkPresentation-9.2/Lib/LinkPresentation/
+-rw-r--r--   0 ronald     (501) staff       (20)      744 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.2/Lib/LinkPresentation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2045 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.2/Lib/LinkPresentation/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:37.002948 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2134 2023-06-07 00:18:36.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      962 2023-06-07 00:18:36.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:36.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:18:36.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:18:36.000000 pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LinkPresentation-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1923 2023-06-07 00:18:37.018504 pyobjc-framework-LinkPresentation-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:37.009959 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_linkpresentation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_lperror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_lplinkmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      823 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_lpmetadataprovider.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:37.012042 pyobjc-framework-LinkPresentation-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.2/metadata/LinkPresentation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:37.017810 pyobjc-framework-LinkPresentation-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10808 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10871 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10929 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9843 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10123 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10809 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10872 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10930 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LinkPresentation-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-LinkPresentation-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:37.018999 pyobjc-framework-LinkPresentation-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      845 2023-05-29 10:07:46.000000 pyobjc-framework-LinkPresentation-9.2/setup.py
```

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/__init__.py` & `pyobjc-framework-LinkPresentation-9.2/Lib/LinkPresentation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/_metadata.py` & `pyobjc-framework-LinkPresentation-9.2/Lib/LinkPresentation/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO` & `pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LinkPresentation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LinkPresentation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LinkPresentation
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt` & `pyobjc-framework-LinkPresentation-9.2/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/LinkPresentation/__init__.py
 Lib/LinkPresentation/_metadata.py
 Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO
 Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt
 Lib/pyobjc_framework_LinkPresentation.egg-info/dependency_links.txt
 Lib/pyobjc_framework_LinkPresentation.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/License.txt` & `pyobjc-framework-LinkPresentation-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/PKG-INFO` & `pyobjc-framework-LinkPresentation-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LinkPresentation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LinkPresentation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LinkPresentation
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lplinkmetadata.py` & `pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_lplinkmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lpmetadataprovider.py` & `pyobjc-framework-LinkPresentation-9.2/PyObjCTest/test_lpmetadataprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/LinkPresentation.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/LinkPresentation.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1b1/pyobjc_setup.py` & `pyobjc-framework-LinkPresentation-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

