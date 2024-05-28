# Comparing `tmp/pyobjc-framework-PushKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-PushKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PushKit-9.1b1.tar", last modified: Sun Mar 26 11:34:37 2023, max compression
+gzip compressed data, was "pyobjc-framework-PushKit-9.2.tar", last modified: Wed Jun  7 00:24:11 2023, max compression
```

## Comparing `pyobjc-framework-PushKit-9.1b1.tar` & `pyobjc-framework-PushKit-9.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.929846 pyobjc-framework-PushKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.862272 pyobjc-framework-PushKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.887810 pyobjc-framework-PushKit-9.1b1/Lib/PushKit/
--rw-r--r--   0 ronald     (501) staff       (20)      700 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/Lib/PushKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2118 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.1b1/Lib/PushKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.906785 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-03-26 11:34:37.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      951 2023-03-26 11:34:37.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:34:37.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:52.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:34:37.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:34:37.000000 pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PushKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.914699 pyobjc-framework-PushKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-PushKit-9.1b1/Modules/_PushKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      228 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/Modules/_PushKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-PushKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-03-26 11:34:37.929448 pyobjc-framework-PushKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.918168 pyobjc-framework-PushKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      181 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.1b1/PyObjCTest/test_pkdefines.py
--rw-r--r--   0 ronald     (501) staff       (20)      205 2021-03-21 10:08:23.000000 pyobjc-framework-PushKit-9.1b1/PyObjCTest/test_pkpushcredentials.py
--rw-r--r--   0 ronald     (501) staff       (20)      815 2022-06-25 20:11:53.000000 pyobjc-framework-PushKit-9.1b1/PyObjCTest/test_pkpushregistry.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-PushKit-9.1b1/PyObjCTest/test_pushkit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.919348 pyobjc-framework-PushKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      635 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.1b1/metadata/PushKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:37.928449 pyobjc-framework-PushKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     7295 2021-07-30 09:00:38.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7314 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7365 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7120 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7296 2021-03-21 10:08:23.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7296 2021-07-30 09:00:38.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7315 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7366 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PushKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:34:37.929951 pyobjc-framework-PushKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1136 2023-03-25 14:20:32.000000 pyobjc-framework-PushKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.534063 pyobjc-framework-PushKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.509570 pyobjc-framework-PushKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.514443 pyobjc-framework-PushKit-9.2/Lib/PushKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      700 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/Lib/PushKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2118 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.2/Lib/PushKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.517959 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-06-07 00:24:11.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      966 2023-06-07 00:24:11.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:24:11.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:52.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:24:11.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:24:11.000000 pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PushKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.522204 pyobjc-framework-PushKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-PushKit-9.2/Modules/_PushKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      228 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/Modules/_PushKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-PushKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-06-07 00:24:11.533636 pyobjc-framework-PushKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.525944 pyobjc-framework-PushKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      181 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.2/PyObjCTest/test_pkdefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)      205 2021-03-21 10:08:23.000000 pyobjc-framework-PushKit-9.2/PyObjCTest/test_pkpushcredentials.py
+-rw-r--r--   0 ronald     (501) staff       (20)      815 2022-06-25 20:11:53.000000 pyobjc-framework-PushKit-9.2/PyObjCTest/test_pkpushregistry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-PushKit-9.2/PyObjCTest/test_pushkit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.527227 pyobjc-framework-PushKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      635 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.2/metadata/PushKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:11.532788 pyobjc-framework-PushKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     7295 2021-07-30 09:00:38.000000 pyobjc-framework-PushKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7314 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7365 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7120 2020-11-30 18:45:15.000000 pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7296 2021-03-21 10:08:23.000000 pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7296 2021-07-30 09:00:38.000000 pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7315 2022-02-24 08:47:16.000000 pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7366 2023-02-19 10:50:35.000000 pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PushKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PushKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:24:11.534198 pyobjc-framework-PushKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1207 2023-05-29 10:07:47.000000 pyobjc-framework-PushKit-9.2/setup.py
```

### Comparing `pyobjc-framework-PushKit-9.1b1/Lib/PushKit/__init__.py` & `pyobjc-framework-PushKit-9.2/Lib/PushKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/Lib/PushKit/_metadata.py` & `pyobjc-framework-PushKit-9.2/Lib/PushKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/PKG-INFO` & `pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PushKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PushKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PushKit
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-PushKit-9.1b1/Lib/pyobjc_framework_PushKit.egg-info/SOURCES.txt` & `pyobjc-framework-PushKit-9.2/Lib/pyobjc_framework_PushKit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PushKit/__init__.py
 Lib/PushKit/_metadata.py
 Lib/pyobjc_framework_PushKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_PushKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PushKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PushKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PushKit-9.1b1/License.txt` & `pyobjc-framework-PushKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/Modules/_PushKit.m` & `pyobjc-framework-PushKit-9.2/Modules/_PushKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-PushKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-PushKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-PushKit-9.1b1/PKG-INFO` & `pyobjc-framework-PushKit-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PushKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PushKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PushKit
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-PushKit-9.1b1/PyObjCTest/test_pkpushregistry.py` & `pyobjc-framework-PushKit-9.2/PyObjCTest/test_pkpushregistry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/PushKit.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/PushKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-PushKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PushKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PushKit-9.1b1/setup.py` & `pyobjc-framework-PushKit-9.2/setup.py`

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
     name="pyobjc-framework-PushKit",
     description="Wrappers for the framework PushKit on macOS",
     min_os_level="10.15",
     packages=["PushKit"],
     ext_modules=[
```

