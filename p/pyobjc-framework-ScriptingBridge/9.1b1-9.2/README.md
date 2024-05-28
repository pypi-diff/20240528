# Comparing `tmp/pyobjc-framework-ScriptingBridge-9.1b1.tar.gz` & `tmp/pyobjc-framework-ScriptingBridge-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ScriptingBridge-9.1b1.tar", last modified: Sun Mar 26 11:38:50 2023, max compression
+gzip compressed data, was "pyobjc-framework-ScriptingBridge-9.2.tar", last modified: Wed Jun  7 00:27:18 2023, max compression
```

## Comparing `pyobjc-framework-ScriptingBridge-9.1b1.tar` & `pyobjc-framework-ScriptingBridge-9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.176154 pyobjc-framework-ScriptingBridge-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.111317 pyobjc-framework-ScriptingBridge-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)      238 2022-01-02 11:04:26.000000 pyobjc-framework-ScriptingBridge-9.1b1/Examples/iTunesCurrentTrack.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScriptingBridge-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.090058 pyobjc-framework-ScriptingBridge-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.112948 pyobjc-framework-ScriptingBridge-9.1b1/Lib/ScriptingBridge/
--rw-r--r--   0 ronald     (501) staff       (20)     1026 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/ScriptingBridge/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1342 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/ScriptingBridge/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.115970 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2481 2023-03-26 11:38:50.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1052 2023-03-26 11:38:50.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:38:50.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:31.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:38:50.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:38:50.000000 pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.132357 pyobjc-framework-ScriptingBridge-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1134 2021-10-18 19:38:40.000000 pyobjc-framework-ScriptingBridge-9.1b1/Modules/_ScriptingBridge.m
--rw-r--r--   0 ronald     (501) staff       (20)      362 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/Modules/_ScriptingBridge_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ScriptingBridge-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2270 2023-03-26 11:38:50.175813 pyobjc-framework-ScriptingBridge-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.139792 pyobjc-framework-ScriptingBridge-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      777 2022-06-25 20:12:31.000000 pyobjc-framework-ScriptingBridge-9.1b1/PyObjCTest/test_scriptingbridge.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-ScriptingBridge-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.158408 pyobjc-framework-ScriptingBridge-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1694 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/ScriptingBridge.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:50.174914 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    12112 2021-07-30 09:00:38.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12131 2022-02-24 08:47:17.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12149 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12113 2021-03-21 10:08:23.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11351 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11351 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11393 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12113 2021-07-30 09:00:38.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12132 2022-02-24 08:47:17.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12150 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScriptingBridge-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:38:50.176252 pyobjc-framework-ScriptingBridge-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1514 2023-03-25 14:20:32.000000 pyobjc-framework-ScriptingBridge-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.570828 pyobjc-framework-ScriptingBridge-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.545362 pyobjc-framework-ScriptingBridge-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2022-01-02 11:04:26.000000 pyobjc-framework-ScriptingBridge-9.2/Examples/iTunesCurrentTrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScriptingBridge-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.539610 pyobjc-framework-ScriptingBridge-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.547025 pyobjc-framework-ScriptingBridge-9.2/Lib/ScriptingBridge/
+-rw-r--r--   0 ronald     (501) staff       (20)     1026 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/ScriptingBridge/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1342 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/ScriptingBridge/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.550797 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2479 2023-06-07 00:27:18.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1067 2023-06-07 00:27:18.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:18.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:31.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:27:18.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:27:18.000000 pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.558169 pyobjc-framework-ScriptingBridge-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1134 2021-10-18 19:38:40.000000 pyobjc-framework-ScriptingBridge-9.2/Modules/_ScriptingBridge.m
+-rw-r--r--   0 ronald     (501) staff       (20)      362 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/Modules/_ScriptingBridge_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ScriptingBridge-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2268 2023-06-07 00:27:18.570461 pyobjc-framework-ScriptingBridge-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.559778 pyobjc-framework-ScriptingBridge-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2022-06-25 20:12:31.000000 pyobjc-framework-ScriptingBridge-9.2/PyObjCTest/test_scriptingbridge.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-ScriptingBridge-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.561450 pyobjc-framework-ScriptingBridge-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1694 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/ScriptingBridge.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:18.569586 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    12112 2021-07-30 09:00:38.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12131 2022-02-24 08:47:17.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12149 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12113 2021-03-21 10:08:23.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11351 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11351 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11393 2020-11-30 18:45:15.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12113 2021-07-30 09:00:38.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12132 2022-02-24 08:47:17.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12150 2023-02-19 10:50:35.000000 pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScriptingBridge-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ScriptingBridge-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:18.571100 pyobjc-framework-ScriptingBridge-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1585 2023-05-29 10:07:47.000000 pyobjc-framework-ScriptingBridge-9.2/setup.py
```

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/LICENSE.txt` & `pyobjc-framework-ScriptingBridge-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Lib/ScriptingBridge/__init__.py` & `pyobjc-framework-ScriptingBridge-9.2/Lib/ScriptingBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Lib/ScriptingBridge/_metadata.py` & `pyobjc-framework-ScriptingBridge-9.2/Lib/ScriptingBridge/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/PKG-INFO` & `pyobjc-framework-ScriptingBridge-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScriptingBridge
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScriptingBridge on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScriptingBridge
 Platform: MacOS X (>=10.5)
@@ -26,17 +26,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "ScriptingBrige" framework on macOS 10.5 or later. This
 framework provides an easy way to use the scripting functionality of
 applications ("AppleScript") from Cocoa applications.
 
 The functionality of this framework is comparable to that off "appscript",
```

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Lib/pyobjc_framework_ScriptingBridge.egg-info/SOURCES.txt` & `pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/iTunesCurrentTrack.py
 Lib/ScriptingBridge/__init__.py
 Lib/ScriptingBridge/_metadata.py
 Lib/pyobjc_framework_ScriptingBridge.egg-info/PKG-INFO
 Lib/pyobjc_framework_ScriptingBridge.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ScriptingBridge.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Modules/_ScriptingBridge.m` & `pyobjc-framework-ScriptingBridge-9.2/Modules/_ScriptingBridge.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ScriptingBridge-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ScriptingBridge-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/PKG-INFO` & `pyobjc-framework-ScriptingBridge-9.2/Lib/pyobjc_framework_ScriptingBridge.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScriptingBridge
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScriptingBridge on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScriptingBridge
 Platform: MacOS X (>=10.5)
@@ -26,14 +26,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "ScriptingBrige" framework on macOS 10.5 or later. This
 framework provides an easy way to use the scripting functionality of
 applications ("AppleScript") from Cocoa applications.
 
 The functionality of this framework is comparable to that off "appscript",
```

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/PyObjCTest/test_scriptingbridge.py` & `pyobjc-framework-ScriptingBridge-9.2/PyObjCTest/test_scriptingbridge.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/ScriptingBridge.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/ScriptingBridge.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-ScriptingBridge-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ScriptingBridge-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScriptingBridge-9.1b1/setup.py` & `pyobjc-framework-ScriptingBridge-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 
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
     name="pyobjc-framework-ScriptingBridge",
     description="Wrappers for the framework ScriptingBridge on macOS",
     min_os_level="10.5",
     packages=["ScriptingBridge"],
     ext_modules=[
```

