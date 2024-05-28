# Comparing `tmp/pyobjc-framework-ClassKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-ClassKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ClassKit-9.1b1.tar", last modified: Sun Mar 26 11:16:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-ClassKit-9.2.tar", last modified: Wed Jun  7 00:07:39 2023, max compression
```

## Comparing `pyobjc-framework-ClassKit-9.1b1.tar` & `pyobjc-framework-ClassKit-9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.099151 pyobjc-framework-ClassKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.025815 pyobjc-framework-ClassKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.033967 pyobjc-framework-ClassKit-9.1b1/Lib/ClassKit/
--rw-r--r--   0 ronald     (501) staff       (20)      729 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/Lib/ClassKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7764 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/Lib/ClassKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.050468 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2104 2023-03-26 11:16:34.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1043 2023-03-26 11:16:34.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:33.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:19.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:16:33.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:16:33.000000 pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ClassKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.056604 pyobjc-framework-ClassKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      754 2021-10-18 19:38:40.000000 pyobjc-framework-ClassKit-9.1b1/Modules/_ClassKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      326 2021-10-18 19:38:40.000000 pyobjc-framework-ClassKit-9.1b1/Modules/_ClassKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-ClassKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ClassKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1893 2023-03-26 11:16:34.098524 pyobjc-framework-ClassKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.076173 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_classkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      189 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsactivity.py
--rw-r--r--   0 ronald     (501) staff       (20)      643 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsbinaryitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2420 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clscontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      473 2022-06-25 20:14:41.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clscontextprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      618 2022-06-25 20:13:05.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsdatastore.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsdeeplinks.py
--rw-r--r--   0 ronald     (501) staff       (20)     1646 2021-11-16 10:40:07.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsdefines.py
--rw-r--r--   0 ronald     (501) staff       (20)      652 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsprogressreportingcapability.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.078483 pyobjc-framework-ClassKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1399 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/metadata/ClassKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:34.086397 pyobjc-framework-ClassKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    39272 2022-01-02 11:04:26.000000 pyobjc-framework-ClassKit-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    39495 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    37224 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    39273 2022-01-02 11:04:26.000000 pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    39496 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ClassKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:16:34.099317 pyobjc-framework-ClassKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1128 2023-03-25 14:20:30.000000 pyobjc-framework-ClassKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.861463 pyobjc-framework-ClassKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.818662 pyobjc-framework-ClassKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.823586 pyobjc-framework-ClassKit-9.2/Lib/ClassKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      729 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/Lib/ClassKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7764 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/Lib/ClassKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.826729 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2102 2023-06-07 00:07:39.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1058 2023-06-07 00:07:39.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:39.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:19.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:07:39.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:07:39.000000 pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ClassKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.830137 pyobjc-framework-ClassKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2021-10-18 19:38:40.000000 pyobjc-framework-ClassKit-9.2/Modules/_ClassKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      326 2021-10-18 19:38:40.000000 pyobjc-framework-ClassKit-9.2/Modules/_ClassKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-ClassKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ClassKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1891 2023-06-07 00:07:39.861047 pyobjc-framework-ClassKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.844087 pyobjc-framework-ClassKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_classkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      189 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsactivity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      643 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsbinaryitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2420 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clscontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2022-06-25 20:14:41.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clscontextprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      618 2022-06-25 20:13:05.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsdatastore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsdeeplinks.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1646 2021-11-16 10:40:07.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsdefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)      652 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsprogressreportingcapability.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.852955 pyobjc-framework-ClassKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1399 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/metadata/ClassKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:39.859813 pyobjc-framework-ClassKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    39272 2022-01-02 11:04:26.000000 pyobjc-framework-ClassKit-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    39495 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    37224 2021-03-21 10:08:22.000000 pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    39273 2022-01-02 11:04:26.000000 pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    39496 2022-02-24 08:47:16.000000 pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ClassKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ClassKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:39.861560 pyobjc-framework-ClassKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1199 2023-05-29 10:07:45.000000 pyobjc-framework-ClassKit-9.2/setup.py
```

### Comparing `pyobjc-framework-ClassKit-9.1b1/Lib/ClassKit/__init__.py` & `pyobjc-framework-ClassKit-9.2/Lib/ClassKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/Lib/ClassKit/_metadata.py` & `pyobjc-framework-ClassKit-9.2/Lib/ClassKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/PKG-INFO` & `pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ClassKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ClassKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ClassKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ClassKit-9.1b1/Lib/pyobjc_framework_ClassKit.egg-info/SOURCES.txt` & `pyobjc-framework-ClassKit-9.2/Lib/pyobjc_framework_ClassKit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ClassKit/__init__.py
 Lib/ClassKit/_metadata.py
 Lib/pyobjc_framework_ClassKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_ClassKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ClassKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ClassKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ClassKit-9.1b1/License.txt` & `pyobjc-framework-ClassKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/Modules/_ClassKit.m` & `pyobjc-framework-ClassKit-9.2/Modules/_ClassKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ClassKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ClassKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ClassKit-9.1b1/PKG-INFO` & `pyobjc-framework-ClassKit-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ClassKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ClassKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ClassKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsbinaryitem.py` & `pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsbinaryitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clscontext.py` & `pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clscontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsdatastore.py` & `pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsdatastore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsdefines.py` & `pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsdefines.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/PyObjCTest/test_clsprogressreportingcapability.py` & `pyobjc-framework-ClassKit-9.2/PyObjCTest/test_clsprogressreportingcapability.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/ClassKit.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/ClassKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ClassKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ClassKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ClassKit-9.1b1/setup.py` & `pyobjc-framework-ClassKit-9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import setup, Extension
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-ClassKit",
     description="Wrappers for the framework ClassKit on macOS",
     min_os_level="10.16",
     packages=["ClassKit"],
     ext_modules=[
```

