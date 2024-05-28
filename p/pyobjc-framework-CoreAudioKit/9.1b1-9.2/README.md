# Comparing `tmp/pyobjc-framework-CoreAudioKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreAudioKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreAudioKit-9.1b1.tar", last modified: Sun Mar 26 11:19:38 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreAudioKit-9.2.tar", last modified: Wed Jun  7 00:09:49 2023, max compression
```

## Comparing `pyobjc-framework-CoreAudioKit-9.1b1.tar` & `pyobjc-framework-CoreAudioKit-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.705790 pyobjc-framework-CoreAudioKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.598741 pyobjc-framework-CoreAudioKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.645573 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/
--rw-r--r--   0 ronald     (501) staff       (20)      740 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2363 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.655877 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1015 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:41.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       83 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreAudioKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.671203 pyobjc-framework-CoreAudioKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      835 2021-10-18 19:38:40.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      192 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-03-26 11:19:38.705281 pyobjc-framework-CoreAudioKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.690986 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      222 2022-06-25 20:07:08.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_aucustomviewpersistentdata.py
--rw-r--r--   0 ronald     (501) staff       (20)      649 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_augenericview.py
--rw-r--r--   0 ronald     (501) staff       (20)      596 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_auviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_canetworkbrowserwindowcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_coreaudiokit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.693392 pyobjc-framework-CoreAudioKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1456 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/CoreAudioKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.703688 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     9033 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8821 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9111 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreAudioKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:19:38.705903 pyobjc-framework-CoreAudioKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1369 2023-03-25 14:20:30.000000 pyobjc-framework-CoreAudioKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.588263 pyobjc-framework-CoreAudioKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.552405 pyobjc-framework-CoreAudioKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.557325 pyobjc-framework-CoreAudioKit-9.2/Lib/CoreAudioKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      740 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/CoreAudioKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2363 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/CoreAudioKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.560437 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2108 2023-06-07 00:09:49.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1030 2023-06-07 00:09:49.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:09:49.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:41.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       77 2023-06-07 00:09:49.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:09:49.000000 pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreAudioKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.562645 pyobjc-framework-CoreAudioKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2021-10-18 19:38:40.000000 pyobjc-framework-CoreAudioKit-9.2/Modules/_CoreAudioKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      192 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/Modules/_CoreAudioKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreAudioKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreAudioKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1897 2023-06-07 00:09:49.587723 pyobjc-framework-CoreAudioKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.570770 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      222 2022-06-25 20:07:08.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_aucustomviewpersistentdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      649 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_augenericview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      596 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_auviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_canetworkbrowserwindowcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_coreaudiokit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.572295 pyobjc-framework-CoreAudioKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1456 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/CoreAudioKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:49.576871 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     9033 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8821 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9111 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreAudioKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreAudioKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:09:49.588365 pyobjc-framework-CoreAudioKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1341 2023-05-29 10:07:45.000000 pyobjc-framework-CoreAudioKit-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/__init__.py` & `pyobjc-framework-CoreAudioKit-9.2/Lib/CoreAudioKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/_metadata.py` & `pyobjc-framework-CoreAudioKit-9.2/Lib/CoreAudioKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO` & `pyobjc-framework-CoreAudioKit-9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreAudioKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreAudioKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreAudioKit
 Platform: MacOS X
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
 
 
 Wrappers for the "CoreAudioKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt` & `pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreAudioKit/__init__.py
 Lib/CoreAudioKit/_metadata.py
 Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreAudioKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreAudioKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/License.txt` & `pyobjc-framework-CoreAudioKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit.m` & `pyobjc-framework-CoreAudioKit-9.2/Modules/_CoreAudioKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreAudioKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreAudioKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/PKG-INFO` & `pyobjc-framework-CoreAudioKit-9.2/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreAudioKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreAudioKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreAudioKit
 Platform: MacOS X
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
 
 
 Wrappers for the "CoreAudioKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_augenericview.py` & `pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_augenericview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_auviewcontroller.py` & `pyobjc-framework-CoreAudioKit-9.2/PyObjCTest/test_auviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/CoreAudioKit.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/CoreAudioKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreAudioKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreAudioKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1b1/setup.py` & `pyobjc-framework-CoreAudioKit-9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 #
 # Distutils doesn't understand '.mm' as an extension
 #
-import distutils.unixccompiler
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
 
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
-distutils.unixccompiler.UnixCCompiler.src_extensions.append(".mm")
 
 setup(
     name="pyobjc-framework-CoreAudioKit",
     description="Wrappers for the framework CoreAudioKit on macOS",
     packages=["CoreAudioKit"],
     ext_modules=[
         Extension(
```

