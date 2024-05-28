# Comparing `tmp/pyobjc-framework-ThreadNetwork-9.1b1.tar.gz` & `tmp/pyobjc-framework-ThreadNetwork-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ThreadNetwork-9.1b1.tar", last modified: Sun Mar 26 11:42:58 2023, max compression
+gzip compressed data, was "pyobjc-framework-ThreadNetwork-9.2.tar", last modified: Wed Jun  7 00:30:42 2023, max compression
```

## Comparing `pyobjc-framework-ThreadNetwork-9.1b1.tar` & `pyobjc-framework-ThreadNetwork-9.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.482648 pyobjc-framework-ThreadNetwork-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.464649 pyobjc-framework-ThreadNetwork-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.469530 pyobjc-framework-ThreadNetwork-9.1b1/Lib/ThreadNetwork/
--rw-r--r--   0 ronald     (501) staff       (20)      736 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/ThreadNetwork/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3787 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/ThreadNetwork/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.473011 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2123 2023-03-26 11:42:58.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      654 2023-03-26 11:42:58.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:58.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-10-18 10:10:06.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:42:58.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:42:58.000000 pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-10-20 07:36:11.000000 pyobjc-framework-ThreadNetwork-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-10-20 07:36:11.000000 pyobjc-framework-ThreadNetwork-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1912 2023-03-26 11:42:58.482329 pyobjc-framework-ThreadNetwork-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.474463 pyobjc-framework-ThreadNetwork-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1128 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/PyObjCTest/test_thclient.py
--rw-r--r--   0 ronald     (501) staff       (20)      195 2022-10-20 10:07:07.000000 pyobjc-framework-ThreadNetwork-9.1b1/PyObjCTest/test_threadnetwork.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.476212 pyobjc-framework-ThreadNetwork-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/metadata/ThreadNetwork.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:58.481669 pyobjc-framework-ThreadNetwork-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10202 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10203 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ThreadNetwork-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:58.482752 pyobjc-framework-ThreadNetwork-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      703 2023-03-25 14:20:32.000000 pyobjc-framework-ThreadNetwork-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.565082 pyobjc-framework-ThreadNetwork-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.547041 pyobjc-framework-ThreadNetwork-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.552301 pyobjc-framework-ThreadNetwork-9.2/Lib/ThreadNetwork/
+-rw-r--r--   0 ronald     (501) staff       (20)      736 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/ThreadNetwork/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3787 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/ThreadNetwork/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.555513 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2121 2023-06-07 00:30:42.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      669 2023-06-07 00:30:42.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:30:42.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-10-18 10:10:06.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:30:42.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:30:42.000000 pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-10-20 07:36:11.000000 pyobjc-framework-ThreadNetwork-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-10-20 07:36:11.000000 pyobjc-framework-ThreadNetwork-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1910 2023-06-07 00:30:42.564718 pyobjc-framework-ThreadNetwork-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.557218 pyobjc-framework-ThreadNetwork-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1128 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/PyObjCTest/test_thclient.py
+-rw-r--r--   0 ronald     (501) staff       (20)      195 2022-10-20 10:07:07.000000 pyobjc-framework-ThreadNetwork-9.2/PyObjCTest/test_threadnetwork.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.558821 pyobjc-framework-ThreadNetwork-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/metadata/ThreadNetwork.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:42.563824 pyobjc-framework-ThreadNetwork-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10202 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10203 2022-10-18 09:53:23.000000 pyobjc-framework-ThreadNetwork-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ThreadNetwork-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ThreadNetwork-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:30:42.565237 pyobjc-framework-ThreadNetwork-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      785 2023-05-29 10:07:47.000000 pyobjc-framework-ThreadNetwork-9.2/setup.py
```

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/Lib/ThreadNetwork/__init__.py` & `pyobjc-framework-ThreadNetwork-9.2/Lib/ThreadNetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/Lib/ThreadNetwork/_metadata.py` & `pyobjc-framework-ThreadNetwork-9.2/Lib/ThreadNetwork/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/PKG-INFO` & `pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ThreadNetwork
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ThreadNetwork on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ThreadNetwork
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/Lib/pyobjc_framework_ThreadNetwork.egg-info/SOURCES.txt` & `pyobjc-framework-ThreadNetwork-9.2/Lib/pyobjc_framework_ThreadNetwork.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ThreadNetwork/__init__.py
 Lib/ThreadNetwork/_metadata.py
 Lib/pyobjc_framework_ThreadNetwork.egg-info/PKG-INFO
 Lib/pyobjc_framework_ThreadNetwork.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ThreadNetwork.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ThreadNetwork.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/License.txt` & `pyobjc-framework-ThreadNetwork-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/PKG-INFO` & `pyobjc-framework-ThreadNetwork-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ThreadNetwork
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ThreadNetwork on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ThreadNetwork
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/PyObjCTest/test_thclient.py` & `pyobjc-framework-ThreadNetwork-9.2/PyObjCTest/test_thclient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ThreadNetwork-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ThreadNetwork-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ThreadNetwork-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ThreadNetwork-9.1b1/setup.py` & `pyobjc-framework-ThreadNetwork-9.2/setup.py`

 * *Files 10% similar despite different names*

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
     name="pyobjc-framework-ThreadNetwork",
     description="Wrappers for the framework ThreadNetwork on macOS",
     min_os_level="13.0",
     packages=["ThreadNetwork"],
     version=VERSION,
```

