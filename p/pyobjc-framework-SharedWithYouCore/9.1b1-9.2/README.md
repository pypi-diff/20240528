# Comparing `tmp/pyobjc-framework-SharedWithYouCore-9.1b1.tar.gz` & `tmp/pyobjc-framework-SharedWithYouCore-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SharedWithYouCore-9.1b1.tar", last modified: Sun Mar 26 11:40:26 2023, max compression
+gzip compressed data, was "pyobjc-framework-SharedWithYouCore-9.2.tar", last modified: Wed Jun  7 00:28:32 2023, max compression
```

## Comparing `pyobjc-framework-SharedWithYouCore-9.1b1.tar` & `pyobjc-framework-SharedWithYouCore-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.532592 pyobjc-framework-SharedWithYouCore-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.503198 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.508091 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/SharedWithYouCore/
--rw-r--r--   0 ronald     (501) staff       (20)      837 2022-06-26 19:31:07.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/SharedWithYouCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1658 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/SharedWithYouCore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.511337 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2139 2023-03-26 11:40:26.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      986 2023-03-26 11:40:26.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:40:26.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-26 10:45:07.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:40:26.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-03-26 11:40:26.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.514047 pyobjc-framework-SharedWithYouCore-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1180 2022-06-26 19:30:42.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Modules/_SharedWithYouCore.m
--rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-26 19:28:04.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Modules/_SharedWithYouCore_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SharedWithYouCore-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1928 2023-03-26 11:40:26.532156 pyobjc-framework-SharedWithYouCore-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.527564 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      407 2022-06-26 19:33:07.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_sharedwithyoucore.py
--rw-r--r--   0 ronald     (501) staff       (20)      201 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_swaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      232 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_swcollaborationactionhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      299 2022-06-26 19:34:16.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_swcollaborationmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_swcollaborationoption.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2022-06-26 21:30:12.000000 pyobjc-framework-SharedWithYouCore-9.1b1/PyObjCTest/test_swcollaborationoptionsgroup.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.529429 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      468 2022-06-26 21:30:15.000000 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/SharedWithYouCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       50 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:26.531247 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    31323 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31324 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SharedWithYouCore-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:40:26.532703 pyobjc-framework-SharedWithYouCore-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1233 2023-03-25 14:20:32.000000 pyobjc-framework-SharedWithYouCore-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.895821 pyobjc-framework-SharedWithYouCore-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.868757 pyobjc-framework-SharedWithYouCore-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.874602 pyobjc-framework-SharedWithYouCore-9.2/Lib/SharedWithYouCore/
+-rw-r--r--   0 ronald     (501) staff       (20)      837 2022-06-26 19:31:07.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/SharedWithYouCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1658 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/SharedWithYouCore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.878165 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2137 2023-06-07 00:28:32.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1001 2023-06-07 00:28:32.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:28:32.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-26 10:45:07.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:28:32.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-06-07 00:28:32.000000 pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.881385 pyobjc-framework-SharedWithYouCore-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1180 2022-06-26 19:30:42.000000 pyobjc-framework-SharedWithYouCore-9.2/Modules/_SharedWithYouCore.m
+-rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-26 19:28:04.000000 pyobjc-framework-SharedWithYouCore-9.2/Modules/_SharedWithYouCore_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SharedWithYouCore-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SharedWithYouCore-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1926 2023-06-07 00:28:32.895444 pyobjc-framework-SharedWithYouCore-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.890626 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      407 2022-06-26 19:33:07.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_sharedwithyoucore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_swaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      232 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_swcollaborationactionhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      299 2022-06-26 19:34:16.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_swcollaborationmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_swcollaborationoption.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2022-06-26 21:30:12.000000 pyobjc-framework-SharedWithYouCore-9.2/PyObjCTest/test_swcollaborationoptionsgroup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.892452 pyobjc-framework-SharedWithYouCore-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      468 2022-06-26 21:30:15.000000 pyobjc-framework-SharedWithYouCore-9.2/metadata/SharedWithYouCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYouCore-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:32.894590 pyobjc-framework-SharedWithYouCore-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    31323 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31324 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYouCore-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SharedWithYouCore-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SharedWithYouCore-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:28:32.895938 pyobjc-framework-SharedWithYouCore-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1304 2023-05-29 10:07:47.000000 pyobjc-framework-SharedWithYouCore-9.2/setup.py
```

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Lib/SharedWithYouCore/__init__.py` & `pyobjc-framework-SharedWithYouCore-9.2/Lib/SharedWithYouCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Lib/SharedWithYouCore/_metadata.py` & `pyobjc-framework-SharedWithYouCore-9.2/Lib/SharedWithYouCore/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/PKG-INFO` & `pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SharedWithYouCore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SharedWithYouCore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SharedWithYouCore
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Lib/pyobjc_framework_SharedWithYouCore.egg-info/SOURCES.txt` & `pyobjc-framework-SharedWithYouCore-9.2/Lib/pyobjc_framework_SharedWithYouCore.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SharedWithYouCore/__init__.py
 Lib/SharedWithYouCore/_metadata.py
 Lib/pyobjc_framework_SharedWithYouCore.egg-info/PKG-INFO
 Lib/pyobjc_framework_SharedWithYouCore.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SharedWithYouCore.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SharedWithYouCore.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/License.txt` & `pyobjc-framework-SharedWithYouCore-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Modules/_SharedWithYouCore.m` & `pyobjc-framework-SharedWithYouCore-9.2/Modules/_SharedWithYouCore.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SharedWithYouCore-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SharedWithYouCore-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/PKG-INFO` & `pyobjc-framework-SharedWithYouCore-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SharedWithYouCore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SharedWithYouCore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SharedWithYouCore
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-SharedWithYouCore-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-SharedWithYouCore-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SharedWithYouCore-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYouCore-9.1b1/setup.py` & `pyobjc-framework-SharedWithYouCore-9.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-SharedWithYouCore",
     description="Wrappers for the framework SharedWithYouCore on macOS",
     min_os_level="13.0",
     packages=["SharedWithYouCore"],
     ext_modules=[
```

