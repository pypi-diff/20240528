# Comparing `tmp/pyobjc-framework-MetalFX-9.1b1.tar.gz` & `tmp/pyobjc-framework-MetalFX-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MetalFX-9.1b1.tar", last modified: Sun Mar 26 11:29:30 2023, max compression
+gzip compressed data, was "pyobjc-framework-MetalFX-9.2.tar", last modified: Wed Jun  7 00:20:06 2023, max compression
```

## Comparing `pyobjc-framework-MetalFX-9.1b1.tar` & `pyobjc-framework-MetalFX-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.842680 pyobjc-framework-MetalFX-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.818924 pyobjc-framework-MetalFX-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.823644 pyobjc-framework-MetalFX-9.1b1/Lib/MetalFX/
--rw-r--r--   0 ronald     (501) staff       (20)      725 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.1b1/Lib/MetalFX/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     6663 2022-10-21 10:39:42.000000 pyobjc-framework-MetalFX-9.1b1/Lib/MetalFX/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.826684 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2099 2023-03-26 11:29:30.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      736 2023-03-26 11:29:30.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:29:30.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:16:27.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:29:30.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:29:30.000000 pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-MetalFX-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-MetalFX-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.829007 pyobjc-framework-MetalFX-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      805 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.1b1/Modules/_MetalFX.m
--rw-r--r--   0 ronald     (501) staff       (20)      437 2022-06-26 10:16:33.000000 pyobjc-framework-MetalFX-9.1b1/Modules/_MetalFX_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalFX-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MetalFX-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1888 2023-03-26 11:29:30.842357 pyobjc-framework-MetalFX-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.832044 pyobjc-framework-MetalFX-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      177 2022-06-26 10:16:33.000000 pyobjc-framework-MetalFX-9.1b1/PyObjCTest/test_metalfx.py
--rw-r--r--   0 ronald     (501) staff       (20)     2889 2022-10-20 21:08:30.000000 pyobjc-framework-MetalFX-9.1b1/PyObjCTest/test_mtlfxspatialscaler.py
--rw-r--r--   0 ronald     (501) staff       (20)     5347 2022-10-21 10:39:43.000000 pyobjc-framework-MetalFX-9.1b1/PyObjCTest/test_mtlfxtemporalscaler.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.837566 pyobjc-framework-MetalFX-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      346 2022-06-26 20:02:22.000000 pyobjc-framework-MetalFX-9.1b1/metadata/MetalFX.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:30.840995 pyobjc-framework-MetalFX-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    40148 2022-10-29 12:03:04.000000 pyobjc-framework-MetalFX-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40149 2022-10-29 12:03:04.000000 pyobjc-framework-MetalFX-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalFX-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:29:30.842785 pyobjc-framework-MetalFX-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1143 2023-03-25 14:20:31.000000 pyobjc-framework-MetalFX-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.472382 pyobjc-framework-MetalFX-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.426165 pyobjc-framework-MetalFX-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.431598 pyobjc-framework-MetalFX-9.2/Lib/MetalFX/
+-rw-r--r--   0 ronald     (501) staff       (20)      725 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.2/Lib/MetalFX/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6663 2022-10-21 10:39:42.000000 pyobjc-framework-MetalFX-9.2/Lib/MetalFX/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.435227 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2097 2023-06-07 00:20:06.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      751 2023-06-07 00:20:06.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:20:06.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:16:27.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:20:06.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:20:06.000000 pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-MetalFX-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-MetalFX-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.442286 pyobjc-framework-MetalFX-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      805 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.2/Modules/_MetalFX.m
+-rw-r--r--   0 ronald     (501) staff       (20)      437 2022-06-26 10:16:33.000000 pyobjc-framework-MetalFX-9.2/Modules/_MetalFX_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalFX-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MetalFX-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1886 2023-06-07 00:20:06.470736 pyobjc-framework-MetalFX-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.461645 pyobjc-framework-MetalFX-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      177 2022-06-26 10:16:33.000000 pyobjc-framework-MetalFX-9.2/PyObjCTest/test_metalfx.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2889 2022-10-20 21:08:30.000000 pyobjc-framework-MetalFX-9.2/PyObjCTest/test_mtlfxspatialscaler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5347 2022-10-21 10:39:43.000000 pyobjc-framework-MetalFX-9.2/PyObjCTest/test_mtlfxtemporalscaler.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.464861 pyobjc-framework-MetalFX-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      346 2022-06-26 20:02:22.000000 pyobjc-framework-MetalFX-9.2/metadata/MetalFX.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2022-06-23 11:03:28.000000 pyobjc-framework-MetalFX-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:06.468905 pyobjc-framework-MetalFX-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    40148 2022-10-29 12:03:04.000000 pyobjc-framework-MetalFX-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40149 2022-10-29 12:03:04.000000 pyobjc-framework-MetalFX-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalFX-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MetalFX-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:20:06.472492 pyobjc-framework-MetalFX-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1213 2023-05-29 10:07:46.000000 pyobjc-framework-MetalFX-9.2/setup.py
```

### Comparing `pyobjc-framework-MetalFX-9.1b1/Lib/MetalFX/__init__.py` & `pyobjc-framework-MetalFX-9.2/Lib/MetalFX/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/Lib/MetalFX/_metadata.py` & `pyobjc-framework-MetalFX-9.2/Lib/MetalFX/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/PKG-INFO` & `pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalFX
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalFX on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalFX
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-MetalFX-9.1b1/Lib/pyobjc_framework_MetalFX.egg-info/SOURCES.txt` & `pyobjc-framework-MetalFX-9.2/Lib/pyobjc_framework_MetalFX.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MetalFX/__init__.py
 Lib/MetalFX/_metadata.py
 Lib/pyobjc_framework_MetalFX.egg-info/PKG-INFO
 Lib/pyobjc_framework_MetalFX.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MetalFX.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MetalFX.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MetalFX-9.1b1/License.txt` & `pyobjc-framework-MetalFX-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/Modules/_MetalFX.m` & `pyobjc-framework-MetalFX-9.2/Modules/_MetalFX.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MetalFX-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MetalFX-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MetalFX-9.1b1/PKG-INFO` & `pyobjc-framework-MetalFX-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalFX
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalFX on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalFX
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-MetalFX-9.1b1/PyObjCTest/test_mtlfxspatialscaler.py` & `pyobjc-framework-MetalFX-9.2/PyObjCTest/test_mtlfxspatialscaler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/PyObjCTest/test_mtlfxtemporalscaler.py` & `pyobjc-framework-MetalFX-9.2/PyObjCTest/test_mtlfxtemporalscaler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MetalFX-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MetalFX-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MetalFX-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalFX-9.1b1/setup.py` & `pyobjc-framework-MetalFX-9.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Wrappers for the "MetalFX" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-
 import os
+import sys
+
+sys.path.insert(0, os.path.dirname(__file__))
+
 
-from pyobjc_setup import Extension, setup
+from pyobjc_setup import Extension, setup  # noqa: E402
 
-VERSION = "9.1b1"
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MetalFX",
     description="Wrappers for the framework MetalFX on macOS",
     min_os_level="13.0",
     packages=["MetalFX"],
     ext_modules=[
```

