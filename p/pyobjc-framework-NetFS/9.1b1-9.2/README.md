# Comparing `tmp/pyobjc-framework-NetFS-9.1b1.tar.gz` & `tmp/pyobjc-framework-NetFS-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-NetFS-9.1b1.tar", last modified: Sun Mar 26 11:31:35 2023, max compression
+gzip compressed data, was "pyobjc-framework-NetFS-9.2.tar", last modified: Wed Jun  7 00:21:53 2023, max compression
```

## Comparing `pyobjc-framework-NetFS-9.1b1.tar` & `pyobjc-framework-NetFS-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.945012 pyobjc-framework-NetFS-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.911834 pyobjc-framework-NetFS-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.917462 pyobjc-framework-NetFS-9.1b1/Lib/NetFS/
--rw-r--r--   0 ronald     (501) staff       (20)      715 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/Lib/NetFS/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4510 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.1b1/Lib/NetFS/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.925317 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2091 2023-03-26 11:31:35.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      766 2023-03-26 11:31:35.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:31:35.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:38.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:31:35.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        6 2023-03-26 11:31:35.000000 pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NetFS-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1880 2023-03-26 11:31:35.944606 pyobjc-framework-NetFS-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.933778 pyobjc-framework-NetFS-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4945 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.1b1/PyObjCTest/test_netfs.py
--rw-r--r--   0 ronald     (501) staff       (20)      509 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/PyObjCTest/test_netfsplugins.py
--rw-r--r--   0 ronald     (501) staff       (20)      321 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/PyObjCTest/test_netfsutil.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.935590 pyobjc-framework-NetFS-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3799 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/metadata/NetFS.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:35.943944 pyobjc-framework-NetFS-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     7045 2021-07-30 09:00:38.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7064 2022-02-24 08:47:16.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7293 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7046 2021-03-21 10:08:23.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7046 2021-07-30 09:00:38.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7065 2022-02-24 08:47:16.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7294 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NetFS-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:31:35.945139 pyobjc-framework-NetFS-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      648 2023-03-25 14:20:32.000000 pyobjc-framework-NetFS-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.086685 pyobjc-framework-NetFS-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.064159 pyobjc-framework-NetFS-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.069299 pyobjc-framework-NetFS-9.2/Lib/NetFS/
+-rw-r--r--   0 ronald     (501) staff       (20)      715 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/Lib/NetFS/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4510 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.2/Lib/NetFS/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.072616 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2089 2023-06-07 00:21:53.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2023-06-07 00:21:53.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:53.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:38.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:21:53.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        6 2023-06-07 00:21:53.000000 pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NetFS-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1878 2023-06-07 00:21:53.086326 pyobjc-framework-NetFS-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.075010 pyobjc-framework-NetFS-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4945 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.2/PyObjCTest/test_netfs.py
+-rw-r--r--   0 ronald     (501) staff       (20)      509 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/PyObjCTest/test_netfsplugins.py
+-rw-r--r--   0 ronald     (501) staff       (20)      321 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/PyObjCTest/test_netfsutil.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.076472 pyobjc-framework-NetFS-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3799 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/metadata/NetFS.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-NetFS-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:53.085648 pyobjc-framework-NetFS-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     7045 2021-07-30 09:00:38.000000 pyobjc-framework-NetFS-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7064 2022-02-24 08:47:16.000000 pyobjc-framework-NetFS-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7293 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7046 2021-03-21 10:08:23.000000 pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7046 2021-07-30 09:00:38.000000 pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7065 2022-02-24 08:47:16.000000 pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7294 2022-06-25 20:19:21.000000 pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NetFS-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-NetFS-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:53.086800 pyobjc-framework-NetFS-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      729 2023-05-29 10:07:46.000000 pyobjc-framework-NetFS-9.2/setup.py
```

### Comparing `pyobjc-framework-NetFS-9.1b1/Lib/NetFS/__init__.py` & `pyobjc-framework-NetFS-9.2/Lib/NetFS/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/Lib/NetFS/_metadata.py` & `pyobjc-framework-NetFS-9.2/Lib/NetFS/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/PKG-INFO` & `pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NetFS
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NetFS on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NetFS
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-NetFS-9.1b1/Lib/pyobjc_framework_NetFS.egg-info/SOURCES.txt` & `pyobjc-framework-NetFS-9.2/Lib/pyobjc_framework_NetFS.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/NetFS/__init__.py
 Lib/NetFS/_metadata.py
 Lib/pyobjc_framework_NetFS.egg-info/PKG-INFO
 Lib/pyobjc_framework_NetFS.egg-info/SOURCES.txt
 Lib/pyobjc_framework_NetFS.egg-info/dependency_links.txt
 Lib/pyobjc_framework_NetFS.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-NetFS-9.1b1/License.txt` & `pyobjc-framework-NetFS-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/PKG-INFO` & `pyobjc-framework-NetFS-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NetFS
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NetFS on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NetFS
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-NetFS-9.1b1/PyObjCTest/test_netfs.py` & `pyobjc-framework-NetFS-9.2/PyObjCTest/test_netfs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/NetFS.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/NetFS.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-NetFS-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/pyobjc_setup.py` & `pyobjc-framework-NetFS-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetFS-9.1b1/setup.py` & `pyobjc-framework-NetFS-9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
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
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-NetFS",
     description="Wrappers for the framework NetFS on macOS",
     min_os_level="10.6",
     packages=["NetFS"],
     version=VERSION,
```

