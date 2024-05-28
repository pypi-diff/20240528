# Comparing `tmp/pyobjc-framework-IOBluetoothUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-IOBluetoothUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-IOBluetoothUI-9.1b1.tar", last modified: Sun Mar 26 11:26:39 2023, max compression
+gzip compressed data, was "pyobjc-framework-IOBluetoothUI-9.2.tar", last modified: Wed Jun  7 00:16:58 2023, max compression
```

## Comparing `pyobjc-framework-IOBluetoothUI-9.1b1.tar` & `pyobjc-framework-IOBluetoothUI-9.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.814761 pyobjc-framework-IOBluetoothUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.798734 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.803017 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/IOBluetoothUI/
--rw-r--r--   0 ronald     (501) staff       (20)      711 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/IOBluetoothUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3517 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/IOBluetoothUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.806446 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-03-26 11:26:39.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      867 2023-03-26 11:26:39.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:26:39.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:45:29.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       55 2023-03-26 11:26:39.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:26:39.000000 pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-03-26 11:26:39.814344 pyobjc-framework-IOBluetoothUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.810873 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      276 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothobjectpushuicontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothpairingcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      658 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothpasskeydisplay.py
--rw-r--r--   0 ronald     (501) staff       (20)      720 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothservicebrowsercontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      743 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothui.py
--rw-r--r--   0 ronald     (501) staff       (20)     1449 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothuiuserlib.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.812048 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3444 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/IOBluetoothUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:39.813485 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    31462 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31463 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOBluetoothUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:26:39.816476 pyobjc-framework-IOBluetoothUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      741 2023-03-25 14:20:31.000000 pyobjc-framework-IOBluetoothUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.936818 pyobjc-framework-IOBluetoothUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.917907 pyobjc-framework-IOBluetoothUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.922338 pyobjc-framework-IOBluetoothUI-9.2/Lib/IOBluetoothUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      711 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/IOBluetoothUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3517 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/IOBluetoothUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.925530 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2112 2023-06-07 00:16:58.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      882 2023-06-07 00:16:58.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:16:58.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:45:29.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       51 2023-06-07 00:16:58.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:16:58.000000 pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1901 2023-06-07 00:16:58.936445 pyobjc-framework-IOBluetoothUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.929411 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      276 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothobjectpushuicontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothpairingcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      658 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothpasskeydisplay.py
+-rw-r--r--   0 ronald     (501) staff       (20)      720 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothservicebrowsercontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      743 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothui.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1449 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothuiuserlib.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.930669 pyobjc-framework-IOBluetoothUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3444 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/metadata/IOBluetoothUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:58.935533 pyobjc-framework-IOBluetoothUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    31462 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31463 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetoothUI-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOBluetoothUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-IOBluetoothUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:16:58.936924 pyobjc-framework-IOBluetoothUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      823 2023-05-29 10:07:46.000000 pyobjc-framework-IOBluetoothUI-9.2/setup.py
```

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/Lib/IOBluetoothUI/__init__.py` & `pyobjc-framework-IOBluetoothUI-9.2/Lib/IOBluetoothUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/Lib/IOBluetoothUI/_metadata.py` & `pyobjc-framework-IOBluetoothUI-9.2/Lib/IOBluetoothUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/PKG-INFO` & `pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOBluetoothUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOBluetoothUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOBluetoothUI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/Lib/pyobjc_framework_IOBluetoothUI.egg-info/SOURCES.txt` & `pyobjc-framework-IOBluetoothUI-9.2/Lib/pyobjc_framework_IOBluetoothUI.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/IOBluetoothUI/__init__.py
 Lib/IOBluetoothUI/_metadata.py
 Lib/pyobjc_framework_IOBluetoothUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_IOBluetoothUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_IOBluetoothUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_IOBluetoothUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/License.txt` & `pyobjc-framework-IOBluetoothUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/PKG-INFO` & `pyobjc-framework-IOBluetoothUI-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOBluetoothUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOBluetoothUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOBluetoothUI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothpasskeydisplay.py` & `pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothpasskeydisplay.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothservicebrowsercontroller.py` & `pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothservicebrowsercontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothui.py` & `pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothui.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/PyObjCTest/test_iobluetoothuiuserlib.py` & `pyobjc-framework-IOBluetoothUI-9.2/PyObjCTest/test_iobluetoothuiuserlib.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/metadata/IOBluetoothUI.fwinfo` & `pyobjc-framework-IOBluetoothUI-9.2/metadata/IOBluetoothUI.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-IOBluetoothUI-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-IOBluetoothUI-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-IOBluetoothUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetoothUI-9.1b1/setup.py` & `pyobjc-framework-IOBluetoothUI-9.2/setup.py`

 * *Files 9% similar despite different names*

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
     name="pyobjc-framework-IOBluetoothUI",
     description="Wrappers for the framework IOBluetoothUI on macOS",
     packages=["IOBluetoothUI"],
     version=VERSION,
     install_requires=[
```

