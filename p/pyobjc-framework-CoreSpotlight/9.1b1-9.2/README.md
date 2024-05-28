# Comparing `tmp/pyobjc-framework-CoreSpotlight-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreSpotlight-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreSpotlight-9.1b1.tar", last modified: Sun Mar 26 11:22:09 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreSpotlight-9.2.tar", last modified: Wed Jun  7 00:12:10 2023, max compression
```

## Comparing `pyobjc-framework-CoreSpotlight-9.1b1.tar` & `pyobjc-framework-CoreSpotlight-9.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.820069 pyobjc-framework-CoreSpotlight-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.760006 pyobjc-framework-CoreSpotlight-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.764294 pyobjc-framework-CoreSpotlight-9.1b1/Lib/CoreSpotlight/
--rw-r--r--   0 ronald     (501) staff       (20)      779 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/CoreSpotlight/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    10785 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/CoreSpotlight/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.771363 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2124 2023-03-26 11:22:09.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1193 2023-03-26 11:22:09.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:22:09.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:54.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:22:09.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:22:09.000000 pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreSpotlight-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.779871 pyobjc-framework-CoreSpotlight-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1156 2021-10-18 19:38:40.000000 pyobjc-framework-CoreSpotlight-9.1b1/Modules/_CoreSpotlight.m
--rw-r--r--   0 ronald     (501) staff       (20)      231 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.1b1/Modules/_CoreSpotlight_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreSpotlight-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreSpotlight-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-03-26 11:22:09.819653 pyobjc-framework-CoreSpotlight-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.792957 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      434 2022-04-11 08:03:15.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_corespotlight.py
--rw-r--r--   0 ronald     (501) staff       (20)      426 2021-06-10 09:09:03.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_csimportextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     3612 2022-07-30 15:06:02.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableindex.py
--rw-r--r--   0 ronald     (501) staff       (20)      449 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1541 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableitemattributeset.py
--rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableitemset_messaging.py
--rw-r--r--   0 ronald     (501) staff       (20)     1367 2022-06-15 11:57:00.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      392 2022-06-15 11:57:00.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssuggestion.py
--rw-r--r--   0 ronald     (501) staff       (20)      602 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_csuserquery.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.795251 pyobjc-framework-CoreSpotlight-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     8072 2022-06-25 20:05:31.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/CoreSpotlight.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:09.817988 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   150482 2021-07-30 09:00:37.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   150603 2022-02-24 08:47:16.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162223 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   147710 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   150483 2021-07-30 09:00:37.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   150604 2022-02-24 08:47:16.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162224 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreSpotlight-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:22:09.820172 pyobjc-framework-CoreSpotlight-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2023-03-25 14:20:31.000000 pyobjc-framework-CoreSpotlight-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.543112 pyobjc-framework-CoreSpotlight-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.501697 pyobjc-framework-CoreSpotlight-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.506939 pyobjc-framework-CoreSpotlight-9.2/Lib/CoreSpotlight/
+-rw-r--r--   0 ronald     (501) staff       (20)      779 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/CoreSpotlight/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10785 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/CoreSpotlight/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.510189 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-06-07 00:12:10.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1208 2023-06-07 00:12:10.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:12:10.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:54.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:12:10.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:12:10.000000 pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreSpotlight-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.515425 pyobjc-framework-CoreSpotlight-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1156 2021-10-18 19:38:40.000000 pyobjc-framework-CoreSpotlight-9.2/Modules/_CoreSpotlight.m
+-rw-r--r--   0 ronald     (501) staff       (20)      231 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.2/Modules/_CoreSpotlight_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreSpotlight-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreSpotlight-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-06-07 00:12:10.542447 pyobjc-framework-CoreSpotlight-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.523904 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      434 2022-04-11 08:03:15.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_corespotlight.py
+-rw-r--r--   0 ronald     (501) staff       (20)      426 2021-06-10 09:09:03.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_csimportextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3612 2022-07-30 15:06:02.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableindex.py
+-rw-r--r--   0 ronald     (501) staff       (20)      449 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1541 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableitemattributeset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableitemset_messaging.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1367 2022-06-15 11:57:00.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      392 2022-06-15 11:57:00.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssuggestion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_csuserquery.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.525773 pyobjc-framework-CoreSpotlight-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     8072 2022-06-25 20:05:31.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/CoreSpotlight.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:10.540668 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   150482 2021-07-30 09:00:37.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   150603 2022-02-24 08:47:16.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162223 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   147710 2021-03-21 10:08:22.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   150483 2021-07-30 09:00:37.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   150604 2022-02-24 08:47:16.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162224 2022-10-18 09:53:23.000000 pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreSpotlight-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreSpotlight-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:12:10.543208 pyobjc-framework-CoreSpotlight-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1245 2023-05-29 10:07:46.000000 pyobjc-framework-CoreSpotlight-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Lib/CoreSpotlight/__init__.py` & `pyobjc-framework-CoreSpotlight-9.2/Lib/CoreSpotlight/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Lib/CoreSpotlight/_metadata.py` & `pyobjc-framework-CoreSpotlight-9.2/Lib/CoreSpotlight/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/PKG-INFO` & `pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreSpotlight
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreSpotlight on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreSpotlight
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Lib/pyobjc_framework_CoreSpotlight.egg-info/SOURCES.txt` & `pyobjc-framework-CoreSpotlight-9.2/Lib/pyobjc_framework_CoreSpotlight.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreSpotlight/__init__.py
 Lib/CoreSpotlight/_metadata.py
 Lib/pyobjc_framework_CoreSpotlight.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreSpotlight.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreSpotlight.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreSpotlight.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/License.txt` & `pyobjc-framework-CoreSpotlight-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Modules/_CoreSpotlight.m` & `pyobjc-framework-CoreSpotlight-9.2/Modules/_CoreSpotlight.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreSpotlight-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreSpotlight-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PKG-INFO` & `pyobjc-framework-CoreSpotlight-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreSpotlight
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreSpotlight on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreSpotlight
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableindex.py` & `pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableindex.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableitemattributeset.py` & `pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableitemattributeset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchableitemset_messaging.py` & `pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchableitemset_messaging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_cssearchquery.py` & `pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_cssearchquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/PyObjCTest/test_csuserquery.py` & `pyobjc-framework-CoreSpotlight-9.2/PyObjCTest/test_csuserquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/CoreSpotlight.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/CoreSpotlight.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreSpotlight-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreSpotlight-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreSpotlight-9.1b1/setup.py` & `pyobjc-framework-CoreSpotlight-9.2/setup.py`

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
     name="pyobjc-framework-CoreSpotlight",
     description="Wrappers for the framework CoreSpotlight on macOS",
     min_os_level="10.13",
     packages=["CoreSpotlight"],
     ext_modules=[
```

