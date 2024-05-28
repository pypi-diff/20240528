# Comparing `tmp/pyobjc-framework-Social-9.1b1.tar.gz` & `tmp/pyobjc-framework-Social-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Social-9.1b1.tar", last modified: Sun Mar 26 11:41:01 2023, max compression
+gzip compressed data, was "pyobjc-framework-Social-9.2.tar", last modified: Wed Jun  7 00:29:01 2023, max compression
```

## Comparing `pyobjc-framework-Social-9.1b1.tar` & `pyobjc-framework-Social-9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.113775 pyobjc-framework-Social-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Social-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.071956 pyobjc-framework-Social-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.091156 pyobjc-framework-Social-9.1b1/Lib/Social/
--rw-r--r--   0 ronald     (501) staff       (20)      684 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/Lib/Social/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1487 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.1b1/Lib/Social/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.094456 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     1946 2023-03-26 11:41:01.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      841 2023-03-26 11:41:01.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:41:00.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:39.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:41:00.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:41:00.000000 pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1735 2023-03-26 11:41:01.113430 pyobjc-framework-Social-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.101773 pyobjc-framework-Social-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      268 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.1b1/PyObjCTest/test_slcomposeserviceviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      671 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.1b1/PyObjCTest/test_slrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.1b1/PyObjCTest/test_slservicetypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Social-9.1b1/PyObjCTest/test_social.py
--rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-Social-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.103254 pyobjc-framework-Social-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/metadata/Social.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:01.112750 pyobjc-framework-Social-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     8860 2021-07-30 09:00:38.000000 pyobjc-framework-Social-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8927 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8669 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8861 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3718 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8861 2021-07-30 09:00:38.000000 pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8928 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Social-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:41:01.113878 pyobjc-framework-Social-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      477 2023-03-25 14:20:32.000000 pyobjc-framework-Social-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.510825 pyobjc-framework-Social-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Social-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.485474 pyobjc-framework-Social-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.491342 pyobjc-framework-Social-9.2/Lib/Social/
+-rw-r--r--   0 ronald     (501) staff       (20)      684 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/Lib/Social/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1487 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.2/Lib/Social/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.494621 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     1944 2023-06-07 00:29:01.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      856 2023-06-07 00:29:01.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:29:01.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:39.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:29:01.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:29:01.000000 pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1733 2023-06-07 00:29:01.510443 pyobjc-framework-Social-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.502540 pyobjc-framework-Social-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      268 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.2/PyObjCTest/test_slcomposeserviceviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      671 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.2/PyObjCTest/test_slrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.2/PyObjCTest/test_slservicetypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Social-9.2/PyObjCTest/test_social.py
+-rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-Social-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.504331 pyobjc-framework-Social-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/metadata/Social.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:01.509767 pyobjc-framework-Social-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     8860 2021-07-30 09:00:38.000000 pyobjc-framework-Social-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8927 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8669 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8861 2021-03-21 10:08:23.000000 pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3718 2020-11-30 18:45:15.000000 pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8861 2021-07-30 09:00:38.000000 pyobjc-framework-Social-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8928 2022-02-24 08:47:17.000000 pyobjc-framework-Social-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Social-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Social-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:29:01.510947 pyobjc-framework-Social-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      559 2023-05-29 10:07:47.000000 pyobjc-framework-Social-9.2/setup.py
```

### Comparing `pyobjc-framework-Social-9.1b1/LICENSE.txt` & `pyobjc-framework-Social-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/Lib/Social/__init__.py` & `pyobjc-framework-Social-9.2/Lib/Social/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/Lib/Social/_metadata.py` & `pyobjc-framework-Social-9.2/Lib/Social/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/PKG-INFO` & `pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Social
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Social on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Social
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-Social-9.1b1/Lib/pyobjc_framework_Social.egg-info/SOURCES.txt` & `pyobjc-framework-Social-9.2/Lib/pyobjc_framework_Social.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Social/__init__.py
 Lib/Social/_metadata.py
 Lib/pyobjc_framework_Social.egg-info/PKG-INFO
 Lib/pyobjc_framework_Social.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Social.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Social.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Social-9.1b1/PKG-INFO` & `pyobjc-framework-Social-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Social
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Social on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Social
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-Social-9.1b1/PyObjCTest/test_slrequest.py` & `pyobjc-framework-Social-9.2/PyObjCTest/test_slrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/PyObjCTest/test_slservicetypes.py` & `pyobjc-framework-Social-9.2/PyObjCTest/test_slservicetypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/Social.fwinfo` & `pyobjc-framework-Social-9.2/metadata/Social.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Social-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Social-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Social-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

