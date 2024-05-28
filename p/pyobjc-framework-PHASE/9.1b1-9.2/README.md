# Comparing `tmp/pyobjc-framework-PHASE-9.1b1.tar.gz` & `tmp/pyobjc-framework-PHASE-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PHASE-9.1b1.tar", last modified: Sun Mar 26 11:33:06 2023, max compression
+gzip compressed data, was "pyobjc-framework-PHASE-9.2.tar", last modified: Wed Jun  7 00:23:01 2023, max compression
```

## Comparing `pyobjc-framework-PHASE-9.1b1.tar` & `pyobjc-framework-PHASE-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.563449 pyobjc-framework-PHASE-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.475452 pyobjc-framework-PHASE-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.495920 pyobjc-framework-PHASE-9.1b1/Lib/PHASE/
--rw-r--r--   0 ronald     (501) staff       (20)      671 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/Lib/PHASE/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    12515 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/Lib/PHASE/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.501347 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2091 2023-03-26 11:33:06.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      975 2023-03-26 11:33:06.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:33:06.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:48:52.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:33:06.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        6 2023-03-26 11:33:06.000000 pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1880 2023-03-26 11:33:06.560595 pyobjc-framework-PHASE-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.555318 pyobjc-framework-PHASE-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      849 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phase.py
--rw-r--r--   0 ronald     (501) staff       (20)      858 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseassetregistry.py
--rw-r--r--   0 ronald     (501) staff       (20)      182 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseducker.py
--rw-r--r--   0 ronald     (501) staff       (20)      265 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseengine.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseenvelope.py
--rw-r--r--   0 ronald     (501) staff       (20)     1238 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseenventnodes.py
--rw-r--r--   0 ronald     (501) staff       (20)      238 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasegroup.py
--rw-r--r--   0 ronald     (501) staff       (20)      643 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasematerial.py
--rw-r--r--   0 ronald     (501) staff       (20)      257 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasemedium.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasemixer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1047 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseobject.py
--rw-r--r--   0 ronald     (501) staff       (20)      842 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasesoundevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      741 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasespatialpipeline.py
--rw-r--r--   0 ronald     (501) staff       (20)     6685 2023-03-03 17:21:59.000000 pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasetypes.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.556601 pyobjc-framework-PHASE-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2013 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/metadata/PHASE.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       26 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:06.558331 pyobjc-framework-PHASE-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   139542 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   139543 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PHASE-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:33:06.564033 pyobjc-framework-PHASE-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      735 2023-03-25 14:20:32.000000 pyobjc-framework-PHASE-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.908422 pyobjc-framework-PHASE-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.879516 pyobjc-framework-PHASE-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.884173 pyobjc-framework-PHASE-9.2/Lib/PHASE/
+-rw-r--r--   0 ronald     (501) staff       (20)      671 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/Lib/PHASE/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12515 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/Lib/PHASE/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.889600 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2089 2023-06-07 00:23:01.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      990 2023-06-07 00:23:01.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:23:01.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:48:52.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:23:01.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        6 2023-06-07 00:23:01.000000 pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1878 2023-06-07 00:23:01.908008 pyobjc-framework-PHASE-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.900318 pyobjc-framework-PHASE-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      849 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phase.py
+-rw-r--r--   0 ronald     (501) staff       (20)      858 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseassetregistry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      182 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseducker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      265 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseengine.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseenvelope.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1238 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseenventnodes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasegroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      643 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasematerial.py
+-rw-r--r--   0 ronald     (501) staff       (20)      257 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasemedium.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasemixer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1047 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      842 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasesoundevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasespatialpipeline.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6685 2023-03-03 17:21:59.000000 pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasetypes.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.903285 pyobjc-framework-PHASE-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2013 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/metadata/PHASE.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:01.905907 pyobjc-framework-PHASE-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   139542 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   139543 2023-02-19 10:50:35.000000 pyobjc-framework-PHASE-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PHASE-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PHASE-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:23:01.908515 pyobjc-framework-PHASE-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      817 2023-05-29 10:07:46.000000 pyobjc-framework-PHASE-9.2/setup.py
```

### Comparing `pyobjc-framework-PHASE-9.1b1/Lib/PHASE/__init__.py` & `pyobjc-framework-PHASE-9.2/Lib/PHASE/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/Lib/PHASE/_metadata.py` & `pyobjc-framework-PHASE-9.2/Lib/PHASE/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/PKG-INFO` & `pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PHASE
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PHASE on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PHASE
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-PHASE-9.1b1/Lib/pyobjc_framework_PHASE.egg-info/SOURCES.txt` & `pyobjc-framework-PHASE-9.2/Lib/pyobjc_framework_PHASE.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PHASE/__init__.py
 Lib/PHASE/_metadata.py
 Lib/pyobjc_framework_PHASE.egg-info/PKG-INFO
 Lib/pyobjc_framework_PHASE.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PHASE.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PHASE.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PHASE-9.1b1/License.txt` & `pyobjc-framework-PHASE-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PKG-INFO` & `pyobjc-framework-PHASE-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PHASE
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PHASE on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PHASE
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phase.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseassetregistry.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseassetregistry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseenventnodes.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseenventnodes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasematerial.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasematerial.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phaseobject.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phaseobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasesoundevent.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasesoundevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasespatialpipeline.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasespatialpipeline.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/PyObjCTest/test_phasetypes.py` & `pyobjc-framework-PHASE-9.2/PyObjCTest/test_phasetypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/metadata/PHASE.fwinfo` & `pyobjc-framework-PHASE-9.2/metadata/PHASE.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-PHASE-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-PHASE-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PHASE-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PHASE-9.1b1/setup.py` & `pyobjc-framework-PHASE-9.2/setup.py`

 * *Files 14% similar despite different names*

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
     name="pyobjc-framework-PHASE",
     description="Wrappers for the framework PHASE on macOS",
     min_os_level="12.0",
     packages=["PHASE"],
     version=VERSION,
```

