# Comparing `tmp/pyobjc-framework-MultipeerConnectivity-9.1b1.tar.gz` & `tmp/pyobjc-framework-MultipeerConnectivity-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MultipeerConnectivity-9.1b1.tar", last modified: Sun Mar 26 11:31:09 2023, max compression
+gzip compressed data, was "pyobjc-framework-MultipeerConnectivity-9.2.tar", last modified: Wed Jun  7 00:21:32 2023, max compression
```

## Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1.tar` & `pyobjc-framework-MultipeerConnectivity-9.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.788658 pyobjc-framework-MultipeerConnectivity-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.695232 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.712326 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/MultipeerConnectivity/
--rw-r--r--   0 ronald     (501) staff       (20)      923 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/MultipeerConnectivity/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7433 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/MultipeerConnectivity/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.727525 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2182 2023-03-26 11:31:09.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1222 2023-03-26 11:31:09.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:31:09.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:36.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:31:09.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       22 2023-03-26 11:31:09.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.732556 pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1170 2021-10-18 19:38:40.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/_MultipeerConnectivity.m
--rw-r--r--   0 ronald     (501) staff       (20)      717 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/_MultipeerConnectivity_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1971 2023-03-26 11:31:09.782538 pyobjc-framework-MultipeerConnectivity-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.769839 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      437 2022-06-26 21:30:10.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcadvertiserassistant.py
--rw-r--r--   0 ronald     (501) staff       (20)      831 2022-06-25 09:20:06.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcbrowserviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      661 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      933 2022-06-25 09:19:46.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcnearbyserviceadvertiser.py
--rw-r--r--   0 ronald     (501) staff       (20)      440 2022-06-26 19:58:21.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcnearbyservicebrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)      265 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcpeerid.py
--rw-r--r--   0 ronald     (501) staff       (20)     2465 2022-06-26 19:58:27.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      226 2022-04-11 08:03:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_multipeerconnectivity.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.772974 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2124 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/MultipeerConnectivity.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:09.779369 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    29901 2021-07-30 09:00:38.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30114 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28805 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29902 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29902 2021-07-30 09:00:38.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30115 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:31:09.788817 pyobjc-framework-MultipeerConnectivity-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1246 2023-03-25 14:20:32.000000 pyobjc-framework-MultipeerConnectivity-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.082483 pyobjc-framework-MultipeerConnectivity-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MultipeerConnectivity-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.027572 pyobjc-framework-MultipeerConnectivity-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.034049 pyobjc-framework-MultipeerConnectivity-9.2/Lib/MultipeerConnectivity/
+-rw-r--r--   0 ronald     (501) staff       (20)      923 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/MultipeerConnectivity/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7433 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/MultipeerConnectivity/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.037572 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2180 2023-06-07 00:21:32.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1237 2023-06-07 00:21:32.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:32.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:36.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:21:32.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       22 2023-06-07 00:21:32.000000 pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.043701 pyobjc-framework-MultipeerConnectivity-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1170 2021-10-18 19:38:40.000000 pyobjc-framework-MultipeerConnectivity-9.2/Modules/_MultipeerConnectivity.m
+-rw-r--r--   0 ronald     (501) staff       (20)      717 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.2/Modules/_MultipeerConnectivity_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MultipeerConnectivity-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MultipeerConnectivity-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1969 2023-06-07 00:21:32.075689 pyobjc-framework-MultipeerConnectivity-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.064083 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      437 2022-06-26 21:30:10.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcadvertiserassistant.py
+-rw-r--r--   0 ronald     (501) staff       (20)      831 2022-06-25 09:20:06.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcbrowserviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      661 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      933 2022-06-25 09:19:46.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcnearbyserviceadvertiser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      440 2022-06-26 19:58:21.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcnearbyservicebrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      265 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcpeerid.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2465 2022-06-26 19:58:27.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      226 2022-04-11 08:03:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_multipeerconnectivity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-MultipeerConnectivity-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.066356 pyobjc-framework-MultipeerConnectivity-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2124 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/MultipeerConnectivity.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:32.074483 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    29901 2021-07-30 09:00:38.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30114 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28805 2020-11-30 18:45:15.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29902 2021-03-21 10:08:23.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29902 2021-07-30 09:00:38.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30115 2022-02-24 08:47:16.000000 pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MultipeerConnectivity-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MultipeerConnectivity-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:32.082635 pyobjc-framework-MultipeerConnectivity-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1317 2023-05-29 10:07:46.000000 pyobjc-framework-MultipeerConnectivity-9.2/setup.py
```

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/LICENSE.txt` & `pyobjc-framework-MultipeerConnectivity-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/MultipeerConnectivity/__init__.py` & `pyobjc-framework-MultipeerConnectivity-9.2/Lib/MultipeerConnectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/MultipeerConnectivity/_metadata.py` & `pyobjc-framework-MultipeerConnectivity-9.2/Lib/MultipeerConnectivity/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/PKG-INFO` & `pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MultipeerConnectivity
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MultipeerConnectivity on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MultipeerConnectivity
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/SOURCES.txt` & `pyobjc-framework-MultipeerConnectivity-9.2/Lib/pyobjc_framework_MultipeerConnectivity.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MultipeerConnectivity/__init__.py
 Lib/MultipeerConnectivity/_metadata.py
 Lib/pyobjc_framework_MultipeerConnectivity.egg-info/PKG-INFO
 Lib/pyobjc_framework_MultipeerConnectivity.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MultipeerConnectivity.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MultipeerConnectivity.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/_MultipeerConnectivity.m` & `pyobjc-framework-MultipeerConnectivity-9.2/Modules/_MultipeerConnectivity.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/_MultipeerConnectivity_protocols.m` & `pyobjc-framework-MultipeerConnectivity-9.2/Modules/_MultipeerConnectivity_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MultipeerConnectivity-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MultipeerConnectivity-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/PKG-INFO` & `pyobjc-framework-MultipeerConnectivity-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MultipeerConnectivity
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MultipeerConnectivity on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MultipeerConnectivity
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcbrowserviewcontroller.py` & `pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcbrowserviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcerror.py` & `pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcnearbyserviceadvertiser.py` & `pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcnearbyserviceadvertiser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/PyObjCTest/test_mcsession.py` & `pyobjc-framework-MultipeerConnectivity-9.2/PyObjCTest/test_mcsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/MultipeerConnectivity.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/MultipeerConnectivity.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MultipeerConnectivity-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MultipeerConnectivity-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MultipeerConnectivity-9.1b1/setup.py` & `pyobjc-framework-MultipeerConnectivity-9.2/setup.py`

 * *Files 7% similar despite different names*

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
     name="pyobjc-framework-MultipeerConnectivity",
     description="Wrappers for the framework MultipeerConnectivity on macOS",
     min_os_level="10.10",
     packages=["MultipeerConnectivity"],
     ext_modules=[
```
