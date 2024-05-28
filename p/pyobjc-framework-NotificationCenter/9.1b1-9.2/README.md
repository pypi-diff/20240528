# Comparing `tmp/pyobjc-framework-NotificationCenter-9.1b1.tar.gz` & `tmp/pyobjc-framework-NotificationCenter-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-NotificationCenter-9.1b1.tar", last modified: Sun Mar 26 11:32:16 2023, max compression
+gzip compressed data, was "pyobjc-framework-NotificationCenter-9.2.tar", last modified: Wed Jun  7 00:22:24 2023, max compression
```

## Comparing `pyobjc-framework-NotificationCenter-9.1b1.tar` & `pyobjc-framework-NotificationCenter-9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.722327 pyobjc-framework-NotificationCenter-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.648444 pyobjc-framework-NotificationCenter-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.669368 pyobjc-framework-NotificationCenter-9.1b1/Lib/NotificationCenter/
--rw-r--r--   0 ronald     (501) staff       (20)      847 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/NotificationCenter/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4955 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/NotificationCenter/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.672459 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2144 2023-03-26 11:32:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2023-03-26 11:32:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:32:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:42.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:32:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:32:16.000000 pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NotificationCenter-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.675718 pyobjc-framework-NotificationCenter-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1152 2021-10-18 19:38:40.000000 pyobjc-framework-NotificationCenter-9.1b1/Modules/_NotificationCenter.m
--rw-r--r--   0 ronald     (501) staff       (20)      526 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.1b1/Modules/_NotificationCenter_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-NotificationCenter-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-NotificationCenter-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1933 2023-03-26 11:32:16.721649 pyobjc-framework-NotificationCenter-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.683342 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      436 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2843 2022-06-25 09:20:45.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetlistviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1588 2022-06-25 09:20:22.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetproviding.py
--rw-r--r--   0 ronald     (501) staff       (20)      637 2022-06-25 09:20:37.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetsearchviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_notificationcenter.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.703871 pyobjc-framework-NotificationCenter-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3724 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/NotificationCenter.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:16.719971 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16439 2021-07-30 09:00:38.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16505 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16439 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16440 2021-07-30 09:00:38.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16506 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NotificationCenter-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:32:16.722483 pyobjc-framework-NotificationCenter-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1219 2023-03-25 14:20:32.000000 pyobjc-framework-NotificationCenter-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.327678 pyobjc-framework-NotificationCenter-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.301084 pyobjc-framework-NotificationCenter-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.305812 pyobjc-framework-NotificationCenter-9.2/Lib/NotificationCenter/
+-rw-r--r--   0 ronald     (501) staff       (20)      847 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.2/Lib/NotificationCenter/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4955 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.2/Lib/NotificationCenter/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.309069 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2142 2023-06-07 00:22:24.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1071 2023-06-07 00:22:24.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:22:24.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:42.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:22:24.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-06-07 00:22:24.000000 pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NotificationCenter-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.311560 pyobjc-framework-NotificationCenter-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1152 2021-10-18 19:38:40.000000 pyobjc-framework-NotificationCenter-9.2/Modules/_NotificationCenter.m
+-rw-r--r--   0 ronald     (501) staff       (20)      526 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.2/Modules/_NotificationCenter_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-NotificationCenter-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-NotificationCenter-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1931 2023-06-07 00:22:24.326949 pyobjc-framework-NotificationCenter-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.319237 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      436 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2843 2022-06-25 09:20:45.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetlistviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1588 2022-06-25 09:20:22.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetproviding.py
+-rw-r--r--   0 ronald     (501) staff       (20)      637 2022-06-25 09:20:37.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetsearchviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_notificationcenter.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.320472 pyobjc-framework-NotificationCenter-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3724 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.2/metadata/NotificationCenter.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-NotificationCenter-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:24.325905 pyobjc-framework-NotificationCenter-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16439 2021-07-30 09:00:38.000000 pyobjc-framework-NotificationCenter-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16505 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16439 2021-03-21 10:08:23.000000 pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16440 2021-07-30 09:00:38.000000 pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16506 2022-02-24 08:47:16.000000 pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NotificationCenter-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-NotificationCenter-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:22:24.327808 pyobjc-framework-NotificationCenter-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1290 2023-05-29 10:07:46.000000 pyobjc-framework-NotificationCenter-9.2/setup.py
```

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Lib/NotificationCenter/__init__.py` & `pyobjc-framework-NotificationCenter-9.2/Lib/NotificationCenter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Lib/NotificationCenter/_metadata.py` & `pyobjc-framework-NotificationCenter-9.2/Lib/NotificationCenter/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/PKG-INFO` & `pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NotificationCenter
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NotificationCenter on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NotificationCenter
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Lib/pyobjc_framework_NotificationCenter.egg-info/SOURCES.txt` & `pyobjc-framework-NotificationCenter-9.2/Lib/pyobjc_framework_NotificationCenter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/NotificationCenter/__init__.py
 Lib/NotificationCenter/_metadata.py
 Lib/pyobjc_framework_NotificationCenter.egg-info/PKG-INFO
 Lib/pyobjc_framework_NotificationCenter.egg-info/SOURCES.txt
 Lib/pyobjc_framework_NotificationCenter.egg-info/dependency_links.txt
 Lib/pyobjc_framework_NotificationCenter.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/License.txt` & `pyobjc-framework-NotificationCenter-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Modules/_NotificationCenter.m` & `pyobjc-framework-NotificationCenter-9.2/Modules/_NotificationCenter.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Modules/_NotificationCenter_protocols.m` & `pyobjc-framework-NotificationCenter-9.2/Modules/_NotificationCenter_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-NotificationCenter-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-NotificationCenter-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/PKG-INFO` & `pyobjc-framework-NotificationCenter-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NotificationCenter
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NotificationCenter on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NotificationCenter
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetlistviewcontroller.py` & `pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetlistviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetproviding.py` & `pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetproviding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/PyObjCTest/test_ncwidgetsearchviewcontroller.py` & `pyobjc-framework-NotificationCenter-9.2/PyObjCTest/test_ncwidgetsearchviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/NotificationCenter.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/NotificationCenter.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-NotificationCenter-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/pyobjc_setup.py` & `pyobjc-framework-NotificationCenter-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NotificationCenter-9.1b1/setup.py` & `pyobjc-framework-NotificationCenter-9.2/setup.py`

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
     name="pyobjc-framework-NotificationCenter",
     description="Wrappers for the framework NotificationCenter on macOS",
     min_os_level="10.10",
     packages=["NotificationCenter"],
     ext_modules=[
```

