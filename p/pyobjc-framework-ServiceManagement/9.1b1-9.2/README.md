# Comparing `tmp/pyobjc-framework-ServiceManagement-9.1b1.tar.gz` & `tmp/pyobjc-framework-ServiceManagement-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ServiceManagement-9.1b1.tar", last modified: Sun Mar 26 11:40:01 2023, max compression
+gzip compressed data, was "pyobjc-framework-ServiceManagement-9.2.tar", last modified: Wed Jun  7 00:28:12 2023, max compression
```

## Comparing `pyobjc-framework-ServiceManagement-9.1b1.tar` & `pyobjc-framework-ServiceManagement-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.712081 pyobjc-framework-ServiceManagement-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ServiceManagement-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.644323 pyobjc-framework-ServiceManagement-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.651517 pyobjc-framework-ServiceManagement-9.1b1/Lib/ServiceManagement/
--rw-r--r--   0 ronald     (501) staff       (20)      762 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/ServiceManagement/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3570 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/ServiceManagement/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.666858 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2328 2023-03-26 11:40:01.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2023-03-26 11:40:01.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:40:01.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:38.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:40:01.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-03-26 11:40:01.000000 pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-03-26 11:40:01.711722 pyobjc-framework-ServiceManagement-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.698431 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3482 2022-04-11 08:03:15.000000 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_servicemanagement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1090 2022-06-25 20:05:13.000000 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_smappservice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1188 2022-06-15 11:57:00.000000 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_smerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      320 2021-03-21 10:08:23.000000 pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_smloginitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      294 2021-10-18 19:38:40.000000 pyobjc-framework-ServiceManagement-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.701996 pyobjc-framework-ServiceManagement-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/ServiceManagement.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:01.711043 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     3828 2021-07-30 09:00:38.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3847 2022-02-24 08:47:17.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7721 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3814 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-03-21 10:08:23.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3800 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3800 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3954 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-07-30 09:00:38.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3848 2022-02-24 08:47:17.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7722 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ServiceManagement-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:40:01.712189 pyobjc-framework-ServiceManagement-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      858 2023-03-25 14:20:32.000000 pyobjc-framework-ServiceManagement-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.469121 pyobjc-framework-ServiceManagement-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ServiceManagement-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.430041 pyobjc-framework-ServiceManagement-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.436862 pyobjc-framework-ServiceManagement-9.2/Lib/ServiceManagement/
+-rw-r--r--   0 ronald     (501) staff       (20)      762 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/Lib/ServiceManagement/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3570 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.2/Lib/ServiceManagement/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.444063 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2326 2023-06-07 00:28:12.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1071 2023-06-07 00:28:12.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:28:12.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:38.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:28:12.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-06-07 00:28:12.000000 pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2115 2023-06-07 00:28:12.468713 pyobjc-framework-ServiceManagement-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.447275 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3482 2022-04-11 08:03:15.000000 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_servicemanagement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1090 2022-06-25 20:05:13.000000 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_smappservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1188 2022-06-15 11:57:00.000000 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_smerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      320 2021-03-21 10:08:23.000000 pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_smloginitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2021-10-18 19:38:40.000000 pyobjc-framework-ServiceManagement-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.448778 pyobjc-framework-ServiceManagement-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1932 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/ServiceManagement.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:12.467376 pyobjc-framework-ServiceManagement-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     3828 2021-07-30 09:00:38.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3847 2022-02-24 08:47:17.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7721 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3814 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-03-21 10:08:23.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3800 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3800 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3954 2020-11-30 18:45:15.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-07-30 09:00:38.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3848 2022-02-24 08:47:17.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7722 2022-10-18 09:53:23.000000 pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ServiceManagement-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ServiceManagement-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:28:12.469216 pyobjc-framework-ServiceManagement-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      940 2023-05-29 10:07:47.000000 pyobjc-framework-ServiceManagement-9.2/setup.py
```

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/LICENSE.txt` & `pyobjc-framework-ServiceManagement-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/Lib/ServiceManagement/__init__.py` & `pyobjc-framework-ServiceManagement-9.2/Lib/ServiceManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/Lib/ServiceManagement/_metadata.py` & `pyobjc-framework-ServiceManagement-9.2/Lib/ServiceManagement/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/PKG-INFO` & `pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ServiceManagement
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ServiceManagement on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ServiceManagement
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/Lib/pyobjc_framework_ServiceManagement.egg-info/SOURCES.txt` & `pyobjc-framework-ServiceManagement-9.2/Lib/pyobjc_framework_ServiceManagement.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ServiceManagement/__init__.py
 Lib/ServiceManagement/_metadata.py
 Lib/pyobjc_framework_ServiceManagement.egg-info/PKG-INFO
 Lib/pyobjc_framework_ServiceManagement.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ServiceManagement.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ServiceManagement.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/PKG-INFO` & `pyobjc-framework-ServiceManagement-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ServiceManagement
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ServiceManagement on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ServiceManagement
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_servicemanagement.py` & `pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_servicemanagement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_smappservice.py` & `pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_smappservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/PyObjCTest/test_smerrors.py` & `pyobjc-framework-ServiceManagement-9.2/PyObjCTest/test_smerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/ServiceManagement.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/ServiceManagement.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ServiceManagement-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ServiceManagement-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ServiceManagement-9.1b1/setup.py` & `pyobjc-framework-ServiceManagement-9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 a this provides a secure and object-oriented interface from launchd.
 
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
     name="pyobjc-framework-ServiceManagement",
     description="Wrappers for the framework ServiceManagement on macOS",
     min_os_level="10.6",
     packages=["ServiceManagement"],
     version=VERSION,
```

