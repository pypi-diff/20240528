# Comparing `tmp/pyobjc-framework-MetricKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-MetricKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MetricKit-9.1b1.tar", last modified: Sun Mar 26 11:30:31 2023, max compression
+gzip compressed data, was "pyobjc-framework-MetricKit-9.2.tar", last modified: Wed Jun  7 00:21:03 2023, max compression
```

## Comparing `pyobjc-framework-MetricKit-9.1b1.tar` & `pyobjc-framework-MetricKit-9.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.936531 pyobjc-framework-MetricKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.820361 pyobjc-framework-MetricKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.825250 pyobjc-framework-MetricKit-9.1b1/Lib/MetricKit/
--rw-r--r--   0 ronald     (501) staff       (20)      710 2021-08-04 10:00:42.000000 pyobjc-framework-MetricKit-9.1b1/Lib/MetricKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1271 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.1b1/Lib/MetricKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.828380 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2108 2023-03-26 11:30:31.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1244 2023-03-26 11:30:31.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:30:31.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:34:55.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:30:31.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:30:31.000000 pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetricKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.885373 pyobjc-framework-MetricKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      817 2021-10-18 19:38:40.000000 pyobjc-framework-MetricKit-9.1b1/Modules/_MetricKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      203 2021-10-18 19:38:40.000000 pyobjc-framework-MetricKit-9.1b1/Modules/_MetricKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetricKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MetricKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1897 2023-03-26 11:30:31.935623 pyobjc-framework-MetricKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.903631 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_metrickit.py
--rw-r--r--   0 ronald     (501) staff       (20)      151 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxaverage.py
--rw-r--r--   0 ronald     (501) staff       (20)      163 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxcallstacktree.py
--rw-r--r--   0 ronald     (501) staff       (20)      181 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxcpuexceptiondiagnostic.py
--rw-r--r--   0 ronald     (501) staff       (20)      155 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxcpumetrics.py
--rw-r--r--   0 ronald     (501) staff       (20)      167 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxcrashdiagnostic.py
--rw-r--r--   0 ronald     (501) staff       (20)      157 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxdiagnostic.py
--rw-r--r--   0 ronald     (501) staff       (20)      171 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxdiagnosticpayload.py
--rw-r--r--   0 ronald     (501) staff       (20)      193 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxdiskwriteexceptiondiagnostic.py
--rw-r--r--   0 ronald     (501) staff       (20)      165 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxhangdiagnostic.py
--rw-r--r--   0 ronald     (501) staff       (20)      191 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxhistogram.py
--rw-r--r--   0 ronald     (501) staff       (20)      153 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2022-06-25 20:14:31.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxmetricmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      521 2021-08-05 07:41:59.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxsignpost.py
--rw-r--r--   0 ronald     (501) staff       (20)     1017 2021-08-05 07:41:59.000000 pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxsignpost_private.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.920912 pyobjc-framework-MetricKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      415 2021-08-05 07:41:41.000000 pyobjc-framework-MetricKit-9.1b1/metadata/MetricKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:31.934054 pyobjc-framework-MetricKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    55575 2021-08-05 07:42:00.000000 pyobjc-framework-MetricKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    56013 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    55576 2021-08-05 07:42:00.000000 pyobjc-framework-MetricKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    56014 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetricKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:30:31.936659 pyobjc-framework-MetricKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1104 2023-03-25 14:20:31.000000 pyobjc-framework-MetricKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.350635 pyobjc-framework-MetricKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.288743 pyobjc-framework-MetricKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.297447 pyobjc-framework-MetricKit-9.2/Lib/MetricKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      710 2021-08-04 10:00:42.000000 pyobjc-framework-MetricKit-9.2/Lib/MetricKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1271 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.2/Lib/MetricKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.301168 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-06-07 00:21:03.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1259 2023-06-07 00:21:03.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:03.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:34:55.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:21:03.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:21:03.000000 pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetricKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.303821 pyobjc-framework-MetricKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      817 2021-10-18 19:38:40.000000 pyobjc-framework-MetricKit-9.2/Modules/_MetricKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2021-10-18 19:38:40.000000 pyobjc-framework-MetricKit-9.2/Modules/_MetricKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetricKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MetricKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1895 2023-06-07 00:21:03.350266 pyobjc-framework-MetricKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.314122 pyobjc-framework-MetricKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_metrickit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      151 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxaverage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      163 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxcallstacktree.py
+-rw-r--r--   0 ronald     (501) staff       (20)      181 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxcpuexceptiondiagnostic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      155 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxcpumetrics.py
+-rw-r--r--   0 ronald     (501) staff       (20)      167 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxcrashdiagnostic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      157 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxdiagnostic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      171 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxdiagnosticpayload.py
+-rw-r--r--   0 ronald     (501) staff       (20)      193 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxdiskwriteexceptiondiagnostic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      165 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxhangdiagnostic.py
+-rw-r--r--   0 ronald     (501) staff       (20)      191 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxhistogram.py
+-rw-r--r--   0 ronald     (501) staff       (20)      153 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2022-06-25 20:14:31.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxmetricmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      521 2021-08-05 07:41:59.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxsignpost.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1017 2021-08-05 07:41:59.000000 pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxsignpost_private.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.326739 pyobjc-framework-MetricKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      415 2021-08-05 07:41:41.000000 pyobjc-framework-MetricKit-9.2/metadata/MetricKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 09:00:38.000000 pyobjc-framework-MetricKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:03.349156 pyobjc-framework-MetricKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    55575 2021-08-05 07:42:00.000000 pyobjc-framework-MetricKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    56013 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    55576 2021-08-05 07:42:00.000000 pyobjc-framework-MetricKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    56014 2022-02-24 08:47:16.000000 pyobjc-framework-MetricKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetricKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MetricKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:03.350744 pyobjc-framework-MetricKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1175 2023-05-29 10:07:46.000000 pyobjc-framework-MetricKit-9.2/setup.py
```

### Comparing `pyobjc-framework-MetricKit-9.1b1/Lib/MetricKit/__init__.py` & `pyobjc-framework-MetricKit-9.2/Lib/MetricKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/Lib/MetricKit/_metadata.py` & `pyobjc-framework-MetricKit-9.2/Lib/MetricKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/PKG-INFO` & `pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetricKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetricKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetricKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-MetricKit-9.1b1/Lib/pyobjc_framework_MetricKit.egg-info/SOURCES.txt` & `pyobjc-framework-MetricKit-9.2/Lib/pyobjc_framework_MetricKit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MetricKit/__init__.py
 Lib/MetricKit/_metadata.py
 Lib/pyobjc_framework_MetricKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_MetricKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MetricKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MetricKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MetricKit-9.1b1/License.txt` & `pyobjc-framework-MetricKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/Modules/_MetricKit.m` & `pyobjc-framework-MetricKit-9.2/Modules/_MetricKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MetricKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MetricKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MetricKit-9.1b1/PKG-INFO` & `pyobjc-framework-MetricKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetricKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetricKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetricKit
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxsignpost.py` & `pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxsignpost.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/PyObjCTest/test_mxsignpost_private.py` & `pyobjc-framework-MetricKit-9.2/PyObjCTest/test_mxsignpost_private.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MetricKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MetricKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MetricKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MetricKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MetricKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetricKit-9.1b1/setup.py` & `pyobjc-framework-MetricKit-9.2/setup.py`

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
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MetricKit",
     description="Wrappers for the framework MetricKit on macOS",
     min_os_level="10.16",
     packages=["MetricKit"],
     ext_modules=[
```

