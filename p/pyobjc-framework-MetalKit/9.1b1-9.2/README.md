# Comparing `tmp/pyobjc-framework-MetalKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-MetalKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MetalKit-9.1b1.tar", last modified: Sun Mar 26 11:29:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-MetalKit-9.2.tar", last modified: Wed Jun  7 00:20:19 2023, max compression
```

## Comparing `pyobjc-framework-MetalKit-9.1b1.tar` & `pyobjc-framework-MetalKit-9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.367658 pyobjc-framework-MetalKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.327203 pyobjc-framework-MetalKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.331336 pyobjc-framework-MetalKit-9.1b1/Lib/MetalKit/
--rw-r--r--   0 ronald     (501) staff       (20)      729 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/Lib/MetalKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9452 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.1b1/Lib/MetalKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.334095 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2104 2023-03-26 11:29:41.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1017 2023-03-26 11:29:41.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:29:41.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:31.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       79 2023-03-26 11:29:41.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:29:41.000000 pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.336449 pyobjc-framework-MetalKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      811 2021-10-18 19:38:40.000000 pyobjc-framework-MetalKit-9.1b1/Modules/_MetalKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/Modules/_MetalKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MetalKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1893 2023-03-26 11:29:41.367053 pyobjc-framework-MetalKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.343523 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_metalkit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1146 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtkmodel.py
--rw-r--r--   0 ronald     (501) staff       (20)     4619 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtktextureloader.py
--rw-r--r--   0 ronald     (501) staff       (20)     1310 2022-06-25 20:10:33.000000 pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtkview.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.344937 pyobjc-framework-MetalKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     5756 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.1b1/metadata/MetalKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:41.365508 pyobjc-framework-MetalKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    41395 2021-07-30 09:00:38.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41414 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42519 2022-06-15 11:57:00.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43464 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    39518 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41396 2021-03-21 10:08:23.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41396 2021-07-30 09:00:38.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41415 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42520 2022-06-15 11:57:00.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43465 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:29:41.367762 pyobjc-framework-MetalKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1198 2023-03-25 14:20:31.000000 pyobjc-framework-MetalKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.241412 pyobjc-framework-MetalKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.194948 pyobjc-framework-MetalKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.200321 pyobjc-framework-MetalKit-9.2/Lib/MetalKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      729 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/Lib/MetalKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9452 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.2/Lib/MetalKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.203488 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2102 2023-06-07 00:20:19.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1032 2023-06-07 00:20:19.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:20:19.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:31.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       73 2023-06-07 00:20:19.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:20:19.000000 pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.209919 pyobjc-framework-MetalKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      811 2021-10-18 19:38:40.000000 pyobjc-framework-MetalKit-9.2/Modules/_MetalKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/Modules/_MetalKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MetalKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1891 2023-06-07 00:20:19.240815 pyobjc-framework-MetalKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.224289 pyobjc-framework-MetalKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-MetalKit-9.2/PyObjCTest/test_metalkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1146 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtkmodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4619 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtktextureloader.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1310 2022-06-25 20:10:33.000000 pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtkview.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.226351 pyobjc-framework-MetalKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     5756 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.2/metadata/MetalKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:19.239421 pyobjc-framework-MetalKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    41395 2021-07-30 09:00:38.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41414 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42519 2022-06-15 11:57:00.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43464 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    39518 2020-11-30 18:45:15.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41396 2021-03-21 10:08:23.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41396 2021-07-30 09:00:38.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41415 2022-02-24 08:47:16.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42520 2022-06-15 11:57:00.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43465 2023-02-19 10:50:35.000000 pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MetalKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:20:19.241513 pyobjc-framework-MetalKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1268 2023-05-29 10:07:46.000000 pyobjc-framework-MetalKit-9.2/setup.py
```

### Comparing `pyobjc-framework-MetalKit-9.1b1/Lib/MetalKit/__init__.py` & `pyobjc-framework-MetalKit-9.2/Lib/MetalKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/Lib/MetalKit/_metadata.py` & `pyobjc-framework-MetalKit-9.2/Lib/MetalKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/PKG-INFO` & `pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalKit
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-MetalKit-9.1b1/Lib/pyobjc_framework_MetalKit.egg-info/SOURCES.txt` & `pyobjc-framework-MetalKit-9.2/Lib/pyobjc_framework_MetalKit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MetalKit/__init__.py
 Lib/MetalKit/_metadata.py
 Lib/pyobjc_framework_MetalKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_MetalKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MetalKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MetalKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MetalKit-9.1b1/License.txt` & `pyobjc-framework-MetalKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/Modules/_MetalKit.m` & `pyobjc-framework-MetalKit-9.2/Modules/_MetalKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MetalKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MetalKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MetalKit-9.1b1/PKG-INFO` & `pyobjc-framework-MetalKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalKit
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtkmodel.py` & `pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtkmodel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtktextureloader.py` & `pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtktextureloader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/PyObjCTest/test_mtkview.py` & `pyobjc-framework-MetalKit-9.2/PyObjCTest/test_mtkview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/MetalKit.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/MetalKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-MetalKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MetalKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalKit-9.1b1/setup.py` & `pyobjc-framework-MetalKit-9.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Wrappers for the "MetalKit" framework on macOS.
 
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
     name="pyobjc-framework-MetalKit",
     description="Wrappers for the framework MetalKit on macOS",
     min_os_level="10.11",
     packages=["MetalKit"],
     ext_modules=[
```

