# Comparing `tmp/pyobjc-framework-ScreenCaptureKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-ScreenCaptureKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ScreenCaptureKit-9.1b1.tar", last modified: Sun Mar 26 11:38:05 2023, max compression
+gzip compressed data, was "pyobjc-framework-ScreenCaptureKit-9.2.tar", last modified: Wed Jun  7 00:26:42 2023, max compression
```

## Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1.tar` & `pyobjc-framework-ScreenCaptureKit-9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.202176 pyobjc-framework-ScreenCaptureKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.119252 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.125177 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/ScreenCaptureKit/
--rw-r--r--   0 ronald     (501) staff       (20)      786 2022-02-24 21:31:41.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/ScreenCaptureKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7934 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/ScreenCaptureKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.128648 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2135 2023-03-26 11:38:05.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      987 2023-03-26 11:38:05.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:38:05.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-02-24 08:56:10.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       53 2023-03-26 11:38:05.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:38:05.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.131787 pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-02-24 21:31:43.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/_ScreenCaptureKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      255 2022-02-24 15:45:54.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/_ScreenCaptureKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1924 2023-03-26 11:38:05.201723 pyobjc-framework-ScreenCaptureKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.166395 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-02-24 15:34:53.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1920 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 14:28:01.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_screencaputurekit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1930 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scshareablecontent.py
--rw-r--r--   0 ronald     (501) staff       (20)     4109 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scstream.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.170252 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1989 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/ScreenCaptureKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:05.200710 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    29952 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33044 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33503 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29953 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33045 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33504 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:38:05.202268 pyobjc-framework-ScreenCaptureKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1170 2023-03-25 14:20:32.000000 pyobjc-framework-ScreenCaptureKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.904214 pyobjc-framework-ScreenCaptureKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.876622 pyobjc-framework-ScreenCaptureKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.881982 pyobjc-framework-ScreenCaptureKit-9.2/Lib/ScreenCaptureKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      786 2022-02-24 21:31:41.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/ScreenCaptureKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7934 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/ScreenCaptureKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.885450 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2133 2023-06-07 00:26:42.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1002 2023-06-07 00:26:42.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:26:42.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-02-24 08:56:10.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       49 2023-06-07 00:26:42.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:26:42.000000 pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.892021 pyobjc-framework-ScreenCaptureKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-02-24 21:31:43.000000 pyobjc-framework-ScreenCaptureKit-9.2/Modules/_ScreenCaptureKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      255 2022-02-24 15:45:54.000000 pyobjc-framework-ScreenCaptureKit-9.2/Modules/_ScreenCaptureKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenCaptureKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ScreenCaptureKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1922 2023-06-07 00:26:42.903791 pyobjc-framework-ScreenCaptureKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.896188 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-02-24 15:34:53.000000 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1920 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 14:28:01.000000 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_screencaputurekit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1930 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scshareablecontent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4109 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scstream.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.897502 pyobjc-framework-ScreenCaptureKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1989 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/ScreenCaptureKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:42.903015 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    29952 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33044 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33503 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29953 2022-02-24 08:48:43.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33045 2022-10-19 09:49:10.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33504 2022-12-16 16:43:02.000000 pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenCaptureKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ScreenCaptureKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:26:42.904347 pyobjc-framework-ScreenCaptureKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1241 2023-05-29 10:07:47.000000 pyobjc-framework-ScreenCaptureKit-9.2/setup.py
```

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/ScreenCaptureKit/__init__.py` & `pyobjc-framework-ScreenCaptureKit-9.2/Lib/ScreenCaptureKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/ScreenCaptureKit/_metadata.py` & `pyobjc-framework-ScreenCaptureKit-9.2/Lib/ScreenCaptureKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/PKG-INFO` & `pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenCaptureKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenCaptureKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenCaptureKit
 Platform: MacOS X (>=12.3)
```

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/SOURCES.txt` & `pyobjc-framework-ScreenCaptureKit-9.2/Lib/pyobjc_framework_ScreenCaptureKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ScreenCaptureKit/__init__.py
 Lib/ScreenCaptureKit/_metadata.py
 Lib/pyobjc_framework_ScreenCaptureKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_ScreenCaptureKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ScreenCaptureKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ScreenCaptureKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/License.txt` & `pyobjc-framework-ScreenCaptureKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/_ScreenCaptureKit.m` & `pyobjc-framework-ScreenCaptureKit-9.2/Modules/_ScreenCaptureKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ScreenCaptureKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ScreenCaptureKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/PKG-INFO` & `pyobjc-framework-ScreenCaptureKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenCaptureKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenCaptureKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenCaptureKit
 Platform: MacOS X (>=12.3)
```

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scerror.py` & `pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scshareablecontent.py` & `pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scshareablecontent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/PyObjCTest/test_scstream.py` & `pyobjc-framework-ScreenCaptureKit-9.2/PyObjCTest/test_scstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/ScreenCaptureKit.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/ScreenCaptureKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-ScreenCaptureKit-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ScreenCaptureKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenCaptureKit-9.1b1/setup.py` & `pyobjc-framework-ScreenCaptureKit-9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 Wrappers for the "ScreenCaptureKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-
-from pyobjc_setup import setup, Extension
 import os
+import sys
+
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup, Extension  # noqa: E402
 
-VERSION = "9.1b1"
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-ScreenCaptureKit",
     description="Wrappers for the framework ScreenCaptureKit on macOS",
     min_os_level="12.3",
     packages=["ScreenCaptureKit"],
     ext_modules=[
```

