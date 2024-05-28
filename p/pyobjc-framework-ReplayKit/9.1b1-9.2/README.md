# Comparing `tmp/pyobjc-framework-ReplayKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-ReplayKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ReplayKit-9.1b1.tar", last modified: Sun Mar 26 11:36:38 2023, max compression
+gzip compressed data, was "pyobjc-framework-ReplayKit-9.2.tar", last modified: Wed Jun  7 00:25:36 2023, max compression
```

## Comparing `pyobjc-framework-ReplayKit-9.1b1.tar` & `pyobjc-framework-ReplayKit-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.214496 pyobjc-framework-ReplayKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.154511 pyobjc-framework-ReplayKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.162837 pyobjc-framework-ReplayKit-9.1b1/Lib/ReplayKit/
--rw-r--r--   0 ronald     (501) staff       (20)      739 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/ReplayKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    11894 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/ReplayKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.169222 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2108 2023-03-26 11:36:38.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      956 2023-03-26 11:36:38.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:36:38.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:08.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:36:38.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:36:38.000000 pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ReplayKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.174126 pyobjc-framework-ReplayKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      760 2021-10-18 19:38:40.000000 pyobjc-framework-ReplayKit-9.1b1/Modules/_ReplayKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      606 2021-10-18 19:38:40.000000 pyobjc-framework-ReplayKit-9.1b1/Modules/_ReplayKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ReplayKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ReplayKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1897 2023-03-26 11:36:38.214008 pyobjc-framework-ReplayKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.189828 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_replaykit.py
--rw-r--r--   0 ronald     (501) staff       (20)      929 2022-06-25 20:09:30.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpbroadcast.py
--rw-r--r--   0 ronald     (501) staff       (20)      676 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpbroadcastextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     3260 2023-03-03 17:21:59.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rperror.py
--rw-r--r--   0 ronald     (501) staff       (20)      223 2022-06-25 20:13:02.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rppreviewviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2047 2022-06-25 09:24:28.000000 pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpscreenrecorder.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.194354 pyobjc-framework-ReplayKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1514 2021-06-10 09:09:03.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/ReplayKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:36:38.205499 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    29317 2021-07-30 09:00:38.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29538 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27468 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29318 2021-07-30 09:00:38.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29539 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ReplayKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:36:38.214609 pyobjc-framework-ReplayKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1137 2023-03-25 14:20:32.000000 pyobjc-framework-ReplayKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.372052 pyobjc-framework-ReplayKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.344347 pyobjc-framework-ReplayKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.349061 pyobjc-framework-ReplayKit-9.2/Lib/ReplayKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      739 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/Lib/ReplayKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11894 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.2/Lib/ReplayKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.352533 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-06-07 00:25:36.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      971 2023-06-07 00:25:36.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:25:36.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:08.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:25:36.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:25:36.000000 pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ReplayKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.355287 pyobjc-framework-ReplayKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      760 2021-10-18 19:38:40.000000 pyobjc-framework-ReplayKit-9.2/Modules/_ReplayKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      606 2021-10-18 19:38:40.000000 pyobjc-framework-ReplayKit-9.2/Modules/_ReplayKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ReplayKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ReplayKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1895 2023-06-07 00:25:36.371672 pyobjc-framework-ReplayKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.364143 pyobjc-framework-ReplayKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_replaykit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      929 2022-06-25 20:09:30.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpbroadcast.py
+-rw-r--r--   0 ronald     (501) staff       (20)      676 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpbroadcastextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3260 2023-03-03 17:21:59.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rperror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      223 2022-06-25 20:13:02.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rppreviewviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2047 2022-06-25 09:24:28.000000 pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpscreenrecorder.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.365732 pyobjc-framework-ReplayKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1514 2021-06-10 09:09:03.000000 pyobjc-framework-ReplayKit-9.2/metadata/ReplayKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:25:36.370881 pyobjc-framework-ReplayKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    29317 2021-07-30 09:00:38.000000 pyobjc-framework-ReplayKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29538 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27468 2021-03-21 10:08:23.000000 pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29318 2021-07-30 09:00:38.000000 pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29539 2022-02-24 08:47:17.000000 pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ReplayKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ReplayKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:25:36.372187 pyobjc-framework-ReplayKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1208 2023-05-29 10:07:47.000000 pyobjc-framework-ReplayKit-9.2/setup.py
```

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Lib/ReplayKit/__init__.py` & `pyobjc-framework-ReplayKit-9.2/Lib/ReplayKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Lib/ReplayKit/_metadata.py` & `pyobjc-framework-ReplayKit-9.2/Lib/ReplayKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/PKG-INFO` & `pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ReplayKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ReplayKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ReplayKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Lib/pyobjc_framework_ReplayKit.egg-info/SOURCES.txt` & `pyobjc-framework-ReplayKit-9.2/Lib/pyobjc_framework_ReplayKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ReplayKit/__init__.py
 Lib/ReplayKit/_metadata.py
 Lib/pyobjc_framework_ReplayKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_ReplayKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ReplayKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ReplayKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ReplayKit-9.1b1/License.txt` & `pyobjc-framework-ReplayKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Modules/_ReplayKit.m` & `pyobjc-framework-ReplayKit-9.2/Modules/_ReplayKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Modules/_ReplayKit_protocols.m` & `pyobjc-framework-ReplayKit-9.2/Modules/_ReplayKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ReplayKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ReplayKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ReplayKit-9.1b1/PKG-INFO` & `pyobjc-framework-ReplayKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ReplayKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ReplayKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ReplayKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpbroadcast.py` & `pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpbroadcast.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpbroadcastextension.py` & `pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpbroadcastextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rperror.py` & `pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rperror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/PyObjCTest/test_rpscreenrecorder.py` & `pyobjc-framework-ReplayKit-9.2/PyObjCTest/test_rpscreenrecorder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/ReplayKit.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/ReplayKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ReplayKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ReplayKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ReplayKit-9.1b1/setup.py` & `pyobjc-framework-ReplayKit-9.2/setup.py`

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
     name="pyobjc-framework-ReplayKit",
     description="Wrappers for the framework ReplayKit on macOS",
     min_os_level="10.16",
     packages=["ReplayKit"],
     ext_modules=[
```

