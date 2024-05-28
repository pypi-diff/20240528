# Comparing `tmp/pyobjc-framework-KernelManagement-9.1b1.tar.gz` & `tmp/pyobjc-framework-KernelManagement-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-KernelManagement-9.1b1.tar", last modified: Sun Mar 26 11:27:55 2023, max compression
+gzip compressed data, was "pyobjc-framework-KernelManagement-9.2.tar", last modified: Wed Jun  7 00:18:22 2023, max compression
```

## Comparing `pyobjc-framework-KernelManagement-9.1b1.tar` & `pyobjc-framework-KernelManagement-9.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.669878 pyobjc-framework-KernelManagement-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.653249 pyobjc-framework-KernelManagement-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.657387 pyobjc-framework-KernelManagement-9.1b1/Lib/KernelManagement/
--rw-r--r--   0 ronald     (501) staff       (20)      744 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/KernelManagement/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1436 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/KernelManagement/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.661245 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:27:55.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      752 2023-03-26 11:27:55.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:55.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:49.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:27:55.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:27:55.000000 pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-KernelManagement-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:27:55.669521 pyobjc-framework-KernelManagement-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.664085 pyobjc-framework-KernelManagement-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      540 2022-04-11 08:03:15.000000 pyobjc-framework-KernelManagement-9.1b1/PyObjCTest/test_kernelmanagement.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.665528 pyobjc-framework-KernelManagement-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      835 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/KernelManagement.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:55.668892 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)      765 2021-07-30 09:00:38.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      784 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2894 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      766 2021-07-30 09:00:38.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      785 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-KernelManagement-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:55.669974 pyobjc-framework-KernelManagement-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      693 2023-03-25 14:20:31.000000 pyobjc-framework-KernelManagement-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.026956 pyobjc-framework-KernelManagement-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.010925 pyobjc-framework-KernelManagement-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.015894 pyobjc-framework-KernelManagement-9.2/Lib/KernelManagement/
+-rw-r--r--   0 ronald     (501) staff       (20)      744 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/Lib/KernelManagement/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1436 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.2/Lib/KernelManagement/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.019790 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2134 2023-06-07 00:18:22.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      767 2023-06-07 00:18:22.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:21.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:49.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:18:21.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:18:21.000000 pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-KernelManagement-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1923 2023-06-07 00:18:22.026516 pyobjc-framework-KernelManagement-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.020724 pyobjc-framework-KernelManagement-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      540 2022-04-11 08:03:15.000000 pyobjc-framework-KernelManagement-9.2/PyObjCTest/test_kernelmanagement.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.021896 pyobjc-framework-KernelManagement-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/metadata/KernelManagement.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:22.025792 pyobjc-framework-KernelManagement-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)      765 2021-07-30 09:00:38.000000 pyobjc-framework-KernelManagement-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2894 2021-03-21 10:08:22.000000 pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      766 2021-07-30 09:00:38.000000 pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      785 2022-02-24 08:47:16.000000 pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-KernelManagement-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-KernelManagement-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:22.027059 pyobjc-framework-KernelManagement-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      775 2023-05-29 10:07:46.000000 pyobjc-framework-KernelManagement-9.2/setup.py
```

### Comparing `pyobjc-framework-KernelManagement-9.1b1/Lib/KernelManagement/__init__.py` & `pyobjc-framework-KernelManagement-9.2/Lib/KernelManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/Lib/KernelManagement/_metadata.py` & `pyobjc-framework-KernelManagement-9.2/Lib/KernelManagement/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/PKG-INFO` & `pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-KernelManagement
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework KernelManagement on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,KernelManagement
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-KernelManagement-9.1b1/Lib/pyobjc_framework_KernelManagement.egg-info/SOURCES.txt` & `pyobjc-framework-KernelManagement-9.2/Lib/pyobjc_framework_KernelManagement.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/KernelManagement/__init__.py
 Lib/KernelManagement/_metadata.py
 Lib/pyobjc_framework_KernelManagement.egg-info/PKG-INFO
 Lib/pyobjc_framework_KernelManagement.egg-info/SOURCES.txt
 Lib/pyobjc_framework_KernelManagement.egg-info/dependency_links.txt
 Lib/pyobjc_framework_KernelManagement.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-KernelManagement-9.1b1/License.txt` & `pyobjc-framework-KernelManagement-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/PKG-INFO` & `pyobjc-framework-KernelManagement-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-KernelManagement
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework KernelManagement on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,KernelManagement
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-KernelManagement-9.1b1/PyObjCTest/test_kernelmanagement.py` & `pyobjc-framework-KernelManagement-9.2/PyObjCTest/test_kernelmanagement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/KernelManagement.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/KernelManagement.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-KernelManagement-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-KernelManagement-9.1b1/pyobjc_setup.py` & `pyobjc-framework-KernelManagement-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

