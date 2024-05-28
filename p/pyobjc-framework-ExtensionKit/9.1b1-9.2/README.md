# Comparing `tmp/pyobjc-framework-ExtensionKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-ExtensionKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ExtensionKit-9.1b1.tar", last modified: Sun Mar 26 11:23:50 2023, max compression
+gzip compressed data, was "pyobjc-framework-ExtensionKit-9.2.tar", last modified: Wed Jun  7 00:13:59 2023, max compression
```

## Comparing `pyobjc-framework-ExtensionKit-9.1b1.tar` & `pyobjc-framework-ExtensionKit-9.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.875460 pyobjc-framework-ExtensionKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.849491 pyobjc-framework-ExtensionKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.854061 pyobjc-framework-ExtensionKit-9.1b1/Lib/ExtensionKit/
--rw-r--r--   0 ronald     (501) staff       (20)      782 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/ExtensionKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1175 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/ExtensionKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.857490 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-03-26 11:23:50.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      869 2023-03-26 11:23:50.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:50.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:13:34.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:50.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:23:50.000000 pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-ExtensionKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-ExtensionKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.867818 pyobjc-framework-ExtensionKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      835 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/Modules/_ExtensionKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      294 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/Modules/_ExtensionKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ExtensionKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ExtensionKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1908 2023-03-26 11:23:50.875102 pyobjc-framework-ExtensionKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.871898 pyobjc-framework-ExtensionKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-10-18 09:53:24.000000 pyobjc-framework-ExtensionKit-9.1b1/PyObjCTest/test_exappExtensionbrowserviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      476 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.1b1/PyObjCTest/test_exhostviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/PyObjCTest/test_extensionkit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.873066 pyobjc-framework-ExtensionKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      445 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/metadata/ExtensionKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:50.874392 pyobjc-framework-ExtensionKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     3696 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3697 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExtensionKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:50.875566 pyobjc-framework-ExtensionKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1188 2023-03-25 14:20:31.000000 pyobjc-framework-ExtensionKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.012896 pyobjc-framework-ExtensionKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:58.991720 pyobjc-framework-ExtensionKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:58.996339 pyobjc-framework-ExtensionKit-9.2/Lib/ExtensionKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      782 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/Lib/ExtensionKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1175 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.2/Lib/ExtensionKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.000082 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-06-07 00:13:58.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      884 2023-06-07 00:13:58.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:58.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:13:34.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:58.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:13:58.000000 pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-ExtensionKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-ExtensionKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.002670 pyobjc-framework-ExtensionKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/Modules/_ExtensionKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/Modules/_ExtensionKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ExtensionKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ExtensionKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-06-07 00:13:59.012523 pyobjc-framework-ExtensionKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.005795 pyobjc-framework-ExtensionKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-10-18 09:53:24.000000 pyobjc-framework-ExtensionKit-9.2/PyObjCTest/test_exappExtensionbrowserviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      476 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.2/PyObjCTest/test_exhostviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/PyObjCTest/test_extensionkit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.010424 pyobjc-framework-ExtensionKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      445 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/metadata/ExtensionKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2022-06-23 11:03:28.000000 pyobjc-framework-ExtensionKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:59.011786 pyobjc-framework-ExtensionKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     3696 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3697 2022-10-18 09:53:23.000000 pyobjc-framework-ExtensionKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExtensionKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ExtensionKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:59.013012 pyobjc-framework-ExtensionKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1259 2023-05-29 10:07:46.000000 pyobjc-framework-ExtensionKit-9.2/setup.py
```

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Lib/ExtensionKit/__init__.py` & `pyobjc-framework-ExtensionKit-9.2/Lib/ExtensionKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Lib/ExtensionKit/_metadata.py` & `pyobjc-framework-ExtensionKit-9.2/Lib/ExtensionKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/PKG-INFO` & `pyobjc-framework-ExtensionKit-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExtensionKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExtensionKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExtensionKit
 Platform: MacOS X (>=13.0)
@@ -25,17 +25,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "ExtensionKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Lib/pyobjc_framework_ExtensionKit.egg-info/SOURCES.txt` & `pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ExtensionKit/__init__.py
 Lib/ExtensionKit/_metadata.py
 Lib/pyobjc_framework_ExtensionKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_ExtensionKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ExtensionKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ExtensionKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/License.txt` & `pyobjc-framework-ExtensionKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Modules/_ExtensionKit.m` & `pyobjc-framework-ExtensionKit-9.2/Modules/_ExtensionKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ExtensionKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ExtensionKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/PKG-INFO` & `pyobjc-framework-ExtensionKit-9.2/Lib/pyobjc_framework_ExtensionKit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExtensionKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExtensionKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExtensionKit
 Platform: MacOS X (>=13.0)
@@ -25,14 +25,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "ExtensionKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ExtensionKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ExtensionKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ExtensionKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExtensionKit-9.1b1/setup.py` & `pyobjc-framework-ExtensionKit-9.2/setup.py`

 * *Files 16% similar despite different names*

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
     name="pyobjc-framework-ExtensionKit",
     description="Wrappers for the framework ExtensionKit on macOS",
     min_os_level="13.0",
     packages=["ExtensionKit"],
     ext_modules=[
```

