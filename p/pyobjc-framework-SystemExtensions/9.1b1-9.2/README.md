# Comparing `tmp/pyobjc-framework-SystemExtensions-9.1b1.tar.gz` & `tmp/pyobjc-framework-SystemExtensions-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SystemExtensions-9.1b1.tar", last modified: Sun Mar 26 11:42:47 2023, max compression
+gzip compressed data, was "pyobjc-framework-SystemExtensions-9.2.tar", last modified: Wed Jun  7 00:30:30 2023, max compression
```

## Comparing `pyobjc-framework-SystemExtensions-9.1b1.tar` & `pyobjc-framework-SystemExtensions-9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:47.001840 pyobjc-framework-SystemExtensions-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.968315 pyobjc-framework-SystemExtensions-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.979992 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/
--rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3219 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.988848 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      896 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:53.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemExtensions-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.991454 pyobjc-framework-SystemExtensions-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions.m
--rw-r--r--   0 ronald     (501) staff       (20)      298 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:42:47.001532 pyobjc-framework-SystemExtensions-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.993501 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3446 2022-06-25 20:07:35.000000 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/test_systemextensions.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.995272 pyobjc-framework-SystemExtensions-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      803 2021-10-25 15:33:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/SystemExtensions.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:47.000928 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10275 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10540 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8360 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8412 2021-03-21 10:08:23.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10276 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10541 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemExtensions-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:47.001936 pyobjc-framework-SystemExtensions-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1201 2023-03-25 14:20:32.000000 pyobjc-framework-SystemExtensions-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.529577 pyobjc-framework-SystemExtensions-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.506032 pyobjc-framework-SystemExtensions-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.511409 pyobjc-framework-SystemExtensions-9.2/Lib/SystemExtensions/
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/Lib/SystemExtensions/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3219 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.2/Lib/SystemExtensions/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.514707 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2134 2023-06-07 00:30:30.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      911 2023-06-07 00:30:30.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:30:30.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:53.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:30:30.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:30:30.000000 pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemExtensions-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.518027 pyobjc-framework-SystemExtensions-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-SystemExtensions-9.2/Modules/_SystemExtensions.m
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/Modules/_SystemExtensions_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemExtensions-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SystemExtensions-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1923 2023-06-07 00:30:30.529176 pyobjc-framework-SystemExtensions-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.522974 pyobjc-framework-SystemExtensions-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3446 2022-06-25 20:07:35.000000 pyobjc-framework-SystemExtensions-9.2/PyObjCTest/test_systemextensions.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.524453 pyobjc-framework-SystemExtensions-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2021-10-25 15:33:38.000000 pyobjc-framework-SystemExtensions-9.2/metadata/SystemExtensions.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:30.528428 pyobjc-framework-SystemExtensions-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10275 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10540 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8360 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8412 2021-03-21 10:08:23.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10276 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10541 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemExtensions-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SystemExtensions-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:30:30.529691 pyobjc-framework-SystemExtensions-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1272 2023-05-29 10:07:47.000000 pyobjc-framework-SystemExtensions-9.2/setup.py
```

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/__init__.py` & `pyobjc-framework-SystemExtensions-9.2/Lib/SystemExtensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/_metadata.py` & `pyobjc-framework-SystemExtensions-9.2/Lib/SystemExtensions/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO` & `pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemExtensions
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SystemExtensions on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemExtensions
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt` & `pyobjc-framework-SystemExtensions-9.2/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SystemExtensions/__init__.py
 Lib/SystemExtensions/_metadata.py
 Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO
 Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SystemExtensions.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SystemExtensions.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/License.txt` & `pyobjc-framework-SystemExtensions-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions.m` & `pyobjc-framework-SystemExtensions-9.2/Modules/_SystemExtensions.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SystemExtensions-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SystemExtensions-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/PKG-INFO` & `pyobjc-framework-SystemExtensions-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemExtensions
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SystemExtensions on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemExtensions
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/test_systemextensions.py` & `pyobjc-framework-SystemExtensions-9.2/PyObjCTest/test_systemextensions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/SystemExtensions.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/SystemExtensions.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SystemExtensions-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SystemExtensions-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1b1/setup.py` & `pyobjc-framework-SystemExtensions-9.2/setup.py`

 * *Files 8% similar despite different names*

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
     name="pyobjc-framework-SystemExtensions",
     description="Wrappers for the framework SystemExtensions on macOS",
     min_os_level="10.15",
     packages=["SystemExtensions"],
     ext_modules=[
```

