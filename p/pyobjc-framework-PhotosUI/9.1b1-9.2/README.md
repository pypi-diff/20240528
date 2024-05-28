# Comparing `tmp/pyobjc-framework-PhotosUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-PhotosUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PhotosUI-9.1b1.tar", last modified: Sun Mar 26 11:34:04 2023, max compression
+gzip compressed data, was "pyobjc-framework-PhotosUI-9.2.tar", last modified: Wed Jun  7 00:23:45 2023, max compression
```

## Comparing `pyobjc-framework-PhotosUI-9.1b1.tar` & `pyobjc-framework-PhotosUI-9.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:04.039958 pyobjc-framework-PhotosUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:03.975108 pyobjc-framework-PhotosUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:03.984581 pyobjc-framework-PhotosUI-9.1b1/Lib/PhotosUI/
--rw-r--r--   0 ronald     (501) staff       (20)      972 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/PhotosUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9139 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/PhotosUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:03.987461 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2104 2023-03-26 11:34:03.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1274 2023-03-26 11:34:03.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:34:03.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:49.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:34:03.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:34:03.000000 pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PhotosUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:03.989463 pyobjc-framework-PhotosUI-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      778 2021-10-18 19:38:40.000000 pyobjc-framework-PhotosUI-9.1b1/Modules/_PhotosUI.m
--rw-r--r--   0 ronald     (501) staff       (20)     1112 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.1b1/Modules/_PhotosUI_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PhotosUI-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-PhotosUI-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1893 2023-03-26 11:34:04.039303 pyobjc-framework-PhotosUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:04.004150 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      980 2022-06-25 20:12:10.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phcontenteditingcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2096 2022-06-25 20:05:12.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phlivephotoview.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_photosui.py
--rw-r--r--   0 ronald     (501) staff       (20)     1022 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_photosuitypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1224 2022-06-25 20:10:25.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phpicker.py
--rw-r--r--   0 ronald     (501) staff       (20)      347 2022-10-18 09:53:24.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojectextensionContext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1153 2022-06-25 20:07:10.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojectextensioncontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2088 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojectinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojecttypedescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      350 2022-06-25 20:13:50.000000 pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojecttypedescriptiondatasource.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:04.005714 pyobjc-framework-PhotosUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     5525 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/PhotosUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:04.037112 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    43176 2021-07-30 09:00:38.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43473 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    59673 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41431 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42760 2021-03-21 10:08:23.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43177 2021-07-30 09:00:38.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43474 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    59674 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PhotosUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:34:04.040092 pyobjc-framework-PhotosUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1129 2023-03-25 14:20:32.000000 pyobjc-framework-PhotosUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.475240 pyobjc-framework-PhotosUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.430219 pyobjc-framework-PhotosUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.434963 pyobjc-framework-PhotosUI-9.2/Lib/PhotosUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      972 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.2/Lib/PhotosUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9139 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.2/Lib/PhotosUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.438377 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2102 2023-06-07 00:23:45.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1289 2023-06-07 00:23:45.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:23:45.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:49.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:23:45.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:23:45.000000 pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PhotosUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.443460 pyobjc-framework-PhotosUI-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      778 2021-10-18 19:38:40.000000 pyobjc-framework-PhotosUI-9.2/Modules/_PhotosUI.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1112 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.2/Modules/_PhotosUI_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-PhotosUI-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-PhotosUI-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1891 2023-06-07 00:23:45.474841 pyobjc-framework-PhotosUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.451580 pyobjc-framework-PhotosUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      980 2022-06-25 20:12:10.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phcontenteditingcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2096 2022-06-25 20:05:12.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phlivephotoview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_photosui.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1022 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_photosuitypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1224 2022-06-25 20:10:25.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phpicker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      347 2022-10-18 09:53:24.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojectextensionContext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1153 2022-06-25 20:07:10.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojectextensioncontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2088 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojectinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojecttypedescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      350 2022-06-25 20:13:50.000000 pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojecttypedescriptiondatasource.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.464426 pyobjc-framework-PhotosUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     5525 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.2/metadata/PhotosUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:45.473469 pyobjc-framework-PhotosUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    43176 2021-07-30 09:00:38.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43473 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    59673 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41431 2020-11-30 18:45:15.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42760 2021-03-21 10:08:23.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43177 2021-07-30 09:00:38.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43474 2022-02-24 08:47:16.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    59674 2022-06-15 11:57:00.000000 pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PhotosUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PhotosUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:23:45.475334 pyobjc-framework-PhotosUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1200 2023-05-29 10:07:47.000000 pyobjc-framework-PhotosUI-9.2/setup.py
```

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Lib/PhotosUI/__init__.py` & `pyobjc-framework-PhotosUI-9.2/Lib/PhotosUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Lib/PhotosUI/_metadata.py` & `pyobjc-framework-PhotosUI-9.2/Lib/PhotosUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/PKG-INFO` & `pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PhotosUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PhotosUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PhotosUI
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Lib/pyobjc_framework_PhotosUI.egg-info/SOURCES.txt` & `pyobjc-framework-PhotosUI-9.2/Lib/pyobjc_framework_PhotosUI.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PhotosUI/__init__.py
 Lib/PhotosUI/_metadata.py
 Lib/pyobjc_framework_PhotosUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_PhotosUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PhotosUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PhotosUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PhotosUI-9.1b1/License.txt` & `pyobjc-framework-PhotosUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Modules/_PhotosUI.m` & `pyobjc-framework-PhotosUI-9.2/Modules/_PhotosUI.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Modules/_PhotosUI_protocols.m` & `pyobjc-framework-PhotosUI-9.2/Modules/_PhotosUI_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-PhotosUI-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-PhotosUI-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PKG-INFO` & `pyobjc-framework-PhotosUI-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PhotosUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PhotosUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PhotosUI
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phcontenteditingcontroller.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phcontenteditingcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phlivephotoview.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phlivephotoview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_photosuitypes.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_photosuitypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phpicker.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phpicker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojectextensioncontroller.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojectextensioncontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/PyObjCTest/test_phprojectinfo.py` & `pyobjc-framework-PhotosUI-9.2/PyObjCTest/test_phprojectinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/PhotosUI.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/PhotosUI.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-PhotosUI-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PhotosUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PhotosUI-9.1b1/setup.py` & `pyobjc-framework-PhotosUI-9.2/setup.py`

 * *Files 4% similar despite different names*

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
     name="pyobjc-framework-PhotosUI",
     description="Wrappers for the framework PhotosUI on macOS",
     min_os_level="10.11",
     packages=["PhotosUI"],
     ext_modules=[
```

