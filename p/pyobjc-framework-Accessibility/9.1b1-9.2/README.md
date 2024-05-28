# Comparing `tmp/pyobjc-framework-Accessibility-9.1b1.tar.gz` & `tmp/pyobjc-framework-Accessibility-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Accessibility-9.1b1.tar", last modified: Sun Mar 26 11:13:16 2023, max compression
+gzip compressed data, was "pyobjc-framework-Accessibility-9.2.tar", last modified: Wed Jun  7 00:05:10 2023, max compression
```

## Comparing `pyobjc-framework-Accessibility-9.1b1.tar` & `pyobjc-framework-Accessibility-9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.500497 pyobjc-framework-Accessibility-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.429692 pyobjc-framework-Accessibility-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.435500 pyobjc-framework-Accessibility-9.1b1/Lib/Accessibility/
--rw-r--r--   0 ronald     (501) staff       (20)      963 2021-10-29 07:58:20.000000 pyobjc-framework-Accessibility-9.1b1/Lib/Accessibility/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5812 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/Accessibility/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.454138 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2124 2023-03-26 11:13:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      962 2023-03-26 11:13:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:13:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:12.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:13:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:13:16.000000 pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Accessibility-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.471826 pyobjc-framework-Accessibility-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1099 2021-10-18 19:38:40.000000 pyobjc-framework-Accessibility-9.1b1/Modules/_Accessibility.m
--rw-r--r--   0 ronald     (501) staff       (20)      605 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.1b1/Modules/_Accessibility_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-Accessibility-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Accessibility-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-03-26 11:13:16.500167 pyobjc-framework-Accessibility-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.492279 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_accessibility.py
--rw-r--r--   0 ronald     (501) staff       (20)     2473 2022-06-25 20:17:28.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_axaudiograph.py
--rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-25 20:09:06.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_axbraillemap.py
--rw-r--r--   0 ronald     (501) staff       (20)      480 2022-06-25 20:09:02.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_axcustomcontent.py
--rw-r--r--   0 ronald     (501) staff       (20)      175 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_cxcolorutilities.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.494382 pyobjc-framework-Accessibility-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      282 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/metadata/Accessibility.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:16.498718 pyobjc-framework-Accessibility-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    43361 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43401 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5433 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43361 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43402 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Accessibility-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:13:16.500599 pyobjc-framework-Accessibility-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1242 2023-03-25 14:20:30.000000 pyobjc-framework-Accessibility-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.888676 pyobjc-framework-Accessibility-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.846393 pyobjc-framework-Accessibility-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.852993 pyobjc-framework-Accessibility-9.2/Lib/Accessibility/
+-rw-r--r--   0 ronald     (501) staff       (20)      963 2021-10-29 07:58:20.000000 pyobjc-framework-Accessibility-9.2/Lib/Accessibility/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5812 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.2/Lib/Accessibility/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.856668 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-06-07 00:05:10.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      977 2023-06-07 00:05:10.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:10.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:12.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:05:10.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:05:10.000000 pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Accessibility-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.862982 pyobjc-framework-Accessibility-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1099 2021-10-18 19:38:40.000000 pyobjc-framework-Accessibility-9.2/Modules/_Accessibility.m
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.2/Modules/_Accessibility_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-Accessibility-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-Accessibility-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-06-07 00:05:10.888257 pyobjc-framework-Accessibility-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.868663 pyobjc-framework-Accessibility-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/test_accessibility.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2473 2022-06-25 20:17:28.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/test_axaudiograph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-25 20:09:06.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/test_axbraillemap.py
+-rw-r--r--   0 ronald     (501) staff       (20)      480 2022-06-25 20:09:02.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/test_axcustomcontent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      175 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/PyObjCTest/test_cxcolorutilities.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.881694 pyobjc-framework-Accessibility-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/metadata/Accessibility.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:10.887057 pyobjc-framework-Accessibility-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    43361 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43401 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5433 2021-03-21 10:08:22.000000 pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43361 2022-01-02 11:04:26.000000 pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43402 2022-02-24 08:47:16.000000 pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Accessibility-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Accessibility-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:10.888768 pyobjc-framework-Accessibility-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1314 2023-05-29 10:07:45.000000 pyobjc-framework-Accessibility-9.2/setup.py
```

### Comparing `pyobjc-framework-Accessibility-9.1b1/Lib/Accessibility/__init__.py` & `pyobjc-framework-Accessibility-9.2/Lib/Accessibility/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Lib/Accessibility/_metadata.py` & `pyobjc-framework-Accessibility-9.2/Lib/Accessibility/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/PKG-INFO` & `pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Accessibility
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Accessibility on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Accessibility
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-Accessibility-9.1b1/Lib/pyobjc_framework_Accessibility.egg-info/SOURCES.txt` & `pyobjc-framework-Accessibility-9.2/Lib/pyobjc_framework_Accessibility.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Accessibility/__init__.py
 Lib/Accessibility/_metadata.py
 Lib/pyobjc_framework_Accessibility.egg-info/PKG-INFO
 Lib/pyobjc_framework_Accessibility.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Accessibility.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Accessibility.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Accessibility-9.1b1/License.txt` & `pyobjc-framework-Accessibility-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Modules/_Accessibility.m` & `pyobjc-framework-Accessibility-9.2/Modules/_Accessibility.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Modules/_Accessibility_protocols.m` & `pyobjc-framework-Accessibility-9.2/Modules/_Accessibility_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Accessibility-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Accessibility-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Accessibility-9.1b1/PKG-INFO` & `pyobjc-framework-Accessibility-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Accessibility
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Accessibility on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Accessibility
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_axaudiograph.py` & `pyobjc-framework-Accessibility-9.2/PyObjCTest/test_axaudiograph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/PyObjCTest/test_axbraillemap.py` & `pyobjc-framework-Accessibility-9.2/PyObjCTest/test_axbraillemap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-Accessibility-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Accessibility-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Accessibility-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Accessibility-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accessibility-9.1b1/setup.py` & `pyobjc-framework-Accessibility-9.2/setup.py`

 * *Files 12% similar despite different names*

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
     name="pyobjc-framework-Accessibility",
     description="Wrappers for the framework Accessibility on macOS",
     min_os_level="10.16",
     packages=["Accessibility"],
     ext_modules=[
```

