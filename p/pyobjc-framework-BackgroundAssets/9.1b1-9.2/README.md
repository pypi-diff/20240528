# Comparing `tmp/pyobjc-framework-BackgroundAssets-9.1b1.tar.gz` & `tmp/pyobjc-framework-BackgroundAssets-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-BackgroundAssets-9.1b1.tar", last modified: Sun Mar 26 11:15:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-BackgroundAssets-9.2.tar", last modified: Wed Jun  7 00:06:59 2023, max compression
```

## Comparing `pyobjc-framework-BackgroundAssets-9.1b1.tar` & `pyobjc-framework-BackgroundAssets-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.612367 pyobjc-framework-BackgroundAssets-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.564663 pyobjc-framework-BackgroundAssets-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.571413 pyobjc-framework-BackgroundAssets-9.1b1/Lib/BackgroundAssets/
--rw-r--r--   0 ronald     (501) staff       (20)      834 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/BackgroundAssets/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7112 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/BackgroundAssets/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.575096 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2135 2023-03-26 11:15:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      971 2023-03-26 11:15:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:15:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:10:11.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:15:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:15:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-BackgroundAssets-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-BackgroundAssets-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.577990 pyobjc-framework-BackgroundAssets-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.1b1/Modules/_BackgroundAssets.m
--rw-r--r--   0 ronald     (501) staff       (20)      371 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.1b1/Modules/_BackgroundAssets_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-BackgroundAssets-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1924 2023-03-26 11:15:41.610906 pyobjc-framework-BackgroundAssets-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.583182 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      215 2022-06-27 18:35:41.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_backgroundassets.py
--rw-r--r--   0 ronald     (501) staff       (20)     1058 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownload.py
--rw-r--r--   0 ronald     (501) staff       (20)      926 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownloaderextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     2518 2023-03-04 10:58:50.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownloadmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      360 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_baurldownload.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.590993 pyobjc-framework-BackgroundAssets-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      996 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/BackgroundAssets.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:41.609199 pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16344 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18992 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16345 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18993 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-BackgroundAssets-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:15:41.612563 pyobjc-framework-BackgroundAssets-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1224 2023-03-25 14:20:30.000000 pyobjc-framework-BackgroundAssets-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.584991 pyobjc-framework-BackgroundAssets-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.554021 pyobjc-framework-BackgroundAssets-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.559503 pyobjc-framework-BackgroundAssets-9.2/Lib/BackgroundAssets/
+-rw-r--r--   0 ronald     (501) staff       (20)      834 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/BackgroundAssets/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7112 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/BackgroundAssets/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.562754 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2133 2023-06-07 00:06:59.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      986 2023-06-07 00:06:59.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:59.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:10:11.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:06:59.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:06:59.000000 pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-BackgroundAssets-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-BackgroundAssets-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.569241 pyobjc-framework-BackgroundAssets-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.2/Modules/_BackgroundAssets.m
+-rw-r--r--   0 ronald     (501) staff       (20)      371 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.2/Modules/_BackgroundAssets_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-BackgroundAssets-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1922 2023-06-07 00:06:59.584583 pyobjc-framework-BackgroundAssets-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.576650 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      215 2022-06-27 18:35:41.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_backgroundassets.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1058 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)      926 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownloaderextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2518 2023-03-04 10:58:50.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownloadmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      360 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_baurldownload.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.578698 pyobjc-framework-BackgroundAssets-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      996 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/BackgroundAssets.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2022-06-23 11:03:27.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:59.583466 pyobjc-framework-BackgroundAssets-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16344 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18992 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16345 2022-10-18 09:53:23.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18993 2023-02-19 10:50:34.000000 pyobjc-framework-BackgroundAssets-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-BackgroundAssets-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-BackgroundAssets-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:59.585085 pyobjc-framework-BackgroundAssets-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1295 2023-05-29 10:07:45.000000 pyobjc-framework-BackgroundAssets-9.2/setup.py
```

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Lib/BackgroundAssets/__init__.py` & `pyobjc-framework-BackgroundAssets-9.2/Lib/BackgroundAssets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Lib/BackgroundAssets/_metadata.py` & `pyobjc-framework-BackgroundAssets-9.2/Lib/BackgroundAssets/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/PKG-INFO` & `pyobjc-framework-BackgroundAssets-9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-BackgroundAssets
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework BackgroundAssets on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,BackgroundAssets
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
 
 
 Wrappers for the "BackgroundAssets" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Lib/pyobjc_framework_BackgroundAssets.egg-info/SOURCES.txt` & `pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/BackgroundAssets/__init__.py
 Lib/BackgroundAssets/_metadata.py
 Lib/pyobjc_framework_BackgroundAssets.egg-info/PKG-INFO
 Lib/pyobjc_framework_BackgroundAssets.egg-info/SOURCES.txt
 Lib/pyobjc_framework_BackgroundAssets.egg-info/dependency_links.txt
 Lib/pyobjc_framework_BackgroundAssets.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/License.txt` & `pyobjc-framework-BackgroundAssets-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Modules/_BackgroundAssets.m` & `pyobjc-framework-BackgroundAssets-9.2/Modules/_BackgroundAssets.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-BackgroundAssets-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-BackgroundAssets-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/PKG-INFO` & `pyobjc-framework-BackgroundAssets-9.2/Lib/pyobjc_framework_BackgroundAssets.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-BackgroundAssets
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework BackgroundAssets on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,BackgroundAssets
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
 
 
 Wrappers for the "BackgroundAssets" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownload.py` & `pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownload.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownloaderextension.py` & `pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownloaderextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/PyObjCTest/test_badownloadmanager.py` & `pyobjc-framework-BackgroundAssets-9.2/PyObjCTest/test_badownloadmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/metadata/BackgroundAssets.fwinfo` & `pyobjc-framework-BackgroundAssets-9.2/metadata/BackgroundAssets.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-BackgroundAssets-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-BackgroundAssets-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-BackgroundAssets-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-BackgroundAssets-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/pyobjc_setup.py` & `pyobjc-framework-BackgroundAssets-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BackgroundAssets-9.1b1/setup.py` & `pyobjc-framework-BackgroundAssets-9.2/setup.py`

 * *Files 6% similar despite different names*

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
     name="pyobjc-framework-BackgroundAssets",
     description="Wrappers for the framework BackgroundAssets on macOS",
     min_os_level="13.0",
     packages=["BackgroundAssets"],
     ext_modules=[
```

