# Comparing `tmp/pyobjc-framework-SafetyKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-SafetyKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SafetyKit-9.1b1.tar", last modified: Sun Mar 26 11:37:21 2023, max compression
+gzip compressed data, was "pyobjc-framework-SafetyKit-9.2.tar", last modified: Wed Jun  7 00:26:08 2023, max compression
```

## Comparing `pyobjc-framework-SafetyKit-9.1b1.tar` & `pyobjc-framework-SafetyKit-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.252297 pyobjc-framework-SafetyKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.190334 pyobjc-framework-SafetyKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.194867 pyobjc-framework-SafetyKit-9.1b1/Lib/SafetyKit/
--rw-r--r--   0 ronald     (501) staff       (20)      745 2022-10-21 10:39:53.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/SafetyKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3093 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/SafetyKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.198151 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2107 2023-03-26 11:37:21.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      881 2023-03-26 11:37:21.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:37:21.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-10-19 11:21:57.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:37:21.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:37:21.000000 pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.216531 pyobjc-framework-SafetyKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      761 2022-10-21 10:40:04.000000 pyobjc-framework-SafetyKit-9.1b1/Modules/_SafetyKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      248 2022-10-20 10:41:33.000000 pyobjc-framework-SafetyKit-9.1b1/Modules/_SafetyKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SafetyKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SafetyKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1896 2023-03-26 11:37:21.251807 pyobjc-framework-SafetyKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.245076 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      413 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_saauthorizationstatus.py
--rw-r--r--   0 ronald     (501) staff       (20)      364 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_sacrashdetectionevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      513 2022-10-20 21:08:30.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_sacrashdetectionmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1289 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_saemergencyresponsemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      479 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_saerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      183 2022-10-20 10:05:55.000000 pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_safetykit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.247537 pyobjc-framework-SafetyKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/metadata/SafetyKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:21.248795 pyobjc-framework-SafetyKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     8589 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8590 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SafetyKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:37:21.252420 pyobjc-framework-SafetyKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1205 2023-03-25 14:20:32.000000 pyobjc-framework-SafetyKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.706491 pyobjc-framework-SafetyKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.669437 pyobjc-framework-SafetyKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.674782 pyobjc-framework-SafetyKit-9.2/Lib/SafetyKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      745 2022-10-21 10:39:53.000000 pyobjc-framework-SafetyKit-9.2/Lib/SafetyKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3093 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/Lib/SafetyKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.678168 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-06-07 00:26:08.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2023-06-07 00:26:08.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:26:08.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-10-19 11:21:57.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:26:08.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:26:08.000000 pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.684551 pyobjc-framework-SafetyKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      761 2022-10-21 10:40:04.000000 pyobjc-framework-SafetyKit-9.2/Modules/_SafetyKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2022-10-20 10:41:33.000000 pyobjc-framework-SafetyKit-9.2/Modules/_SafetyKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SafetyKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SafetyKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-06-07 00:26:08.706066 pyobjc-framework-SafetyKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.689596 pyobjc-framework-SafetyKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      413 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_saauthorizationstatus.py
+-rw-r--r--   0 ronald     (501) staff       (20)      364 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_sacrashdetectionevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      513 2022-10-20 21:08:30.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_sacrashdetectionmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1289 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_saemergencyresponsemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      479 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_saerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      183 2022-10-20 10:05:55.000000 pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_safetykit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.702829 pyobjc-framework-SafetyKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/metadata/SafetyKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:08.704922 pyobjc-framework-SafetyKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     8589 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8590 2022-10-19 09:49:10.000000 pyobjc-framework-SafetyKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SafetyKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SafetyKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:26:08.706892 pyobjc-framework-SafetyKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1277 2023-05-29 10:07:47.000000 pyobjc-framework-SafetyKit-9.2/setup.py
```

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Lib/SafetyKit/__init__.py` & `pyobjc-framework-SafetyKit-9.2/Lib/SafetyKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Lib/SafetyKit/_metadata.py` & `pyobjc-framework-SafetyKit-9.2/Lib/SafetyKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/PKG-INFO` & `pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SafetyKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SafetyKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SafetyKit
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Lib/pyobjc_framework_SafetyKit.egg-info/SOURCES.txt` & `pyobjc-framework-SafetyKit-9.2/Lib/pyobjc_framework_SafetyKit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SafetyKit/__init__.py
 Lib/SafetyKit/_metadata.py
 Lib/pyobjc_framework_SafetyKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_SafetyKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SafetyKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SafetyKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SafetyKit-9.1b1/License.txt` & `pyobjc-framework-SafetyKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Modules/_SafetyKit.m` & `pyobjc-framework-SafetyKit-9.2/Modules/_SafetyKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SafetyKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SafetyKit-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-SafetyKit-9.1b1/PKG-INFO` & `pyobjc-framework-SafetyKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SafetyKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SafetyKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SafetyKit
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_sacrashdetectionmanager.py` & `pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_sacrashdetectionmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/PyObjCTest/test_saemergencyresponsemanager.py` & `pyobjc-framework-SafetyKit-9.2/PyObjCTest/test_saemergencyresponsemanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-SafetyKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-SafetyKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SafetyKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SafetyKit-9.1b1/setup.py` & `pyobjc-framework-SafetyKit-9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
-from pyobjc_setup import setup, Extension
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-SafetyKit",
     description="Wrappers for the framework SafetyKit on macOS",
     min_os_level="13.0",
     packages=["SafetyKit"],
     ext_modules=[
```

