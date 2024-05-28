# Comparing `tmp/pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1.tar.gz` & `tmp/pyobjc-framework-AutomaticAssessmentConfiguration-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1.tar", last modified: Sun Mar 26 11:15:18 2023, max compression
+gzip compressed data, was "pyobjc-framework-AutomaticAssessmentConfiguration-9.2.tar", last modified: Wed Jun  7 00:06:42 2023, max compression
```

## Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1.tar` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:18.005315 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.905435 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.911560 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/AutomaticAssessmentConfiguration/
--rw-r--r--   0 ronald     (501) staff       (20)      920 2021-03-21 10:08:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/AutomaticAssessmentConfiguration/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     6335 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/AutomaticAssessmentConfiguration/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.935371 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2200 2023-03-26 11:15:17.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1376 2023-03-26 11:15:17.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:15:17.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:15:17.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       33 2023-03-26 11:15:17.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.941084 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1213 2021-10-18 19:38:40.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/_AutomaticAssessmentConfiguration.m
--rw-r--r--   0 ronald     (501) staff       (20)      333 2021-10-18 19:38:40.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/_AutomaticAssessmentConfiguration_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1989 2023-03-26 11:15:18.004963 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.947215 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      694 2021-10-25 15:33:38.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentapplication.py
--rw-r--r--   0 ronald     (501) staff       (20)      345 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      524 2021-10-25 15:33:38.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentparticipantconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      508 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      626 2022-06-25 20:10:06.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentsessiondelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      557 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2022-04-11 08:03:15.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_automaticassessmentconfiguration.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:17.948586 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1337 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/AutomaticAssessmentConfiguration.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       80 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:18.003812 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    18262 2021-07-30 09:00:37.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18779 2022-02-24 08:47:16.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18953 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11392 2021-03-21 10:08:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18263 2021-07-30 09:00:37.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18780 2022-02-24 08:47:16.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18954 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:15:18.005414 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1343 2023-03-25 14:20:30.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.456110 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.406231 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.412901 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/AutomaticAssessmentConfiguration/
+-rw-r--r--   0 ronald     (501) staff       (20)      920 2021-03-21 10:08:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/AutomaticAssessmentConfiguration/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6335 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/AutomaticAssessmentConfiguration/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.416564 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2198 2023-06-07 00:06:42.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1391 2023-06-07 00:06:42.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:42.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:06:42.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       33 2023-06-07 00:06:42.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.421233 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1213 2021-10-18 19:38:40.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/_AutomaticAssessmentConfiguration.m
+-rw-r--r--   0 ronald     (501) staff       (20)      333 2021-10-18 19:38:40.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/_AutomaticAssessmentConfiguration_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1987 2023-06-07 00:06:42.452290 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.439526 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      694 2021-10-25 15:33:38.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentapplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)      345 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      524 2021-10-25 15:33:38.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentparticipantconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      508 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2022-06-25 20:10:06.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentsessiondelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      557 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2022-04-11 08:03:15.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_automaticassessmentconfiguration.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.441404 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1337 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/AutomaticAssessmentConfiguration.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       80 2020-11-30 18:45:14.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:42.451088 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    18262 2021-07-30 09:00:37.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18779 2022-02-24 08:47:16.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18953 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11392 2021-03-21 10:08:22.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18263 2021-07-30 09:00:37.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18780 2022-02-24 08:47:16.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18954 2022-10-18 09:53:23.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:42.456237 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1415 2023-05-29 10:07:45.000000 pyobjc-framework-AutomaticAssessmentConfiguration-9.2/setup.py
```

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/AutomaticAssessmentConfiguration/__init__.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/AutomaticAssessmentConfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/AutomaticAssessmentConfiguration/_metadata.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/AutomaticAssessmentConfiguration/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/PKG-INFO` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AutomaticAssessmentConfiguration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AutomaticAssessmentConfiguration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AutomaticAssessmentConfiguration
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/SOURCES.txt` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AutomaticAssessmentConfiguration/__init__.py
 Lib/AutomaticAssessmentConfiguration/_metadata.py
 Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/PKG-INFO
 Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AutomaticAssessmentConfiguration.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/License.txt` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/_AutomaticAssessmentConfiguration.m` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/_AutomaticAssessmentConfiguration.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PKG-INFO` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AutomaticAssessmentConfiguration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AutomaticAssessmentConfiguration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AutomaticAssessmentConfiguration
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentapplication.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentapplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentparticipantconfiguration.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentparticipantconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeassessmentsessiondelegate.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeassessmentsessiondelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/PyObjCTest/test_aeerrors.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/PyObjCTest/test_aeerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/AutomaticAssessmentConfiguration.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/AutomaticAssessmentConfiguration.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AutomaticAssessmentConfiguration-9.1b1/setup.py` & `pyobjc-framework-AutomaticAssessmentConfiguration-9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
-from pyobjc_setup import setup, Extension
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-AutomaticAssessmentConfiguration",
     description="Wrappers for the framework AutomaticAssessmentConfiguration on macOS",
     min_os_level="10.15",
     packages=["AutomaticAssessmentConfiguration"],
     ext_modules=[
```

