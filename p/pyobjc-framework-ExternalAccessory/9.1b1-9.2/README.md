# Comparing `tmp/pyobjc-framework-ExternalAccessory-9.1b1.tar.gz` & `tmp/pyobjc-framework-ExternalAccessory-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ExternalAccessory-9.1b1.tar", last modified: Sun Mar 26 11:24:03 2023, max compression
+gzip compressed data, was "pyobjc-framework-ExternalAccessory-9.2.tar", last modified: Wed Jun  7 00:14:14 2023, max compression
```

## Comparing `pyobjc-framework-ExternalAccessory-9.1b1.tar` & `pyobjc-framework-ExternalAccessory-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.838102 pyobjc-framework-ExternalAccessory-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.812461 pyobjc-framework-ExternalAccessory-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.817559 pyobjc-framework-ExternalAccessory-9.1b1/Lib/ExternalAccessory/
--rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/ExternalAccessory/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3747 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/ExternalAccessory/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.820519 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2140 2023-03-26 11:24:03.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1014 2023-03-26 11:24:03.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:03.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:04.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:24:03.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-03-26 11:24:03.000000 pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExternalAccessory-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.823221 pyobjc-framework-ExternalAccessory-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1146 2021-10-18 19:38:40.000000 pyobjc-framework-ExternalAccessory-9.1b1/Modules/_ExternalAccessory.m
--rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/Modules/_ExternalAccessory_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ExternalAccessory-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ExternalAccessory-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1929 2023-03-26 11:24:03.837781 pyobjc-framework-ExternalAccessory-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.830769 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1234 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eaaccessorymanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      659 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eawifiunconfiguredaccessory.py
--rw-r--r--   0 ronald     (501) staff       (20)     1601 2022-06-25 20:16:29.000000 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eawifiunconfiguredaccessorybrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_externalaccessory.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.832191 pyobjc-framework-ExternalAccessory-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2067 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/ExternalAccessory.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:03.836864 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    17914 2021-07-30 09:00:37.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18216 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    17915 2021-03-21 10:08:22.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    17915 2021-07-30 09:00:37.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    18217 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExternalAccessory-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:03.838213 pyobjc-framework-ExternalAccessory-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1210 2023-03-25 14:20:31.000000 pyobjc-framework-ExternalAccessory-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.566540 pyobjc-framework-ExternalAccessory-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.538934 pyobjc-framework-ExternalAccessory-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.544548 pyobjc-framework-ExternalAccessory-9.2/Lib/ExternalAccessory/
+-rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/ExternalAccessory/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3747 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/ExternalAccessory/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.548141 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2138 2023-06-07 00:14:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1029 2023-06-07 00:14:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:14:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:04.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:14:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-06-07 00:14:14.000000 pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExternalAccessory-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.550881 pyobjc-framework-ExternalAccessory-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1146 2021-10-18 19:38:40.000000 pyobjc-framework-ExternalAccessory-9.2/Modules/_ExternalAccessory.m
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/Modules/_ExternalAccessory_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ExternalAccessory-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ExternalAccessory-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1927 2023-06-07 00:14:14.566129 pyobjc-framework-ExternalAccessory-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.558357 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1234 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eaaccessorymanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eawifiunconfiguredaccessory.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1601 2022-06-25 20:16:29.000000 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eawifiunconfiguredaccessorybrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_externalaccessory.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.560279 pyobjc-framework-ExternalAccessory-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2067 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/ExternalAccessory.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:14.565092 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    17914 2021-07-30 09:00:37.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18216 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    17915 2021-03-21 10:08:22.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    17915 2021-07-30 09:00:37.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    18217 2022-02-24 08:47:16.000000 pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExternalAccessory-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ExternalAccessory-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:14:14.566654 pyobjc-framework-ExternalAccessory-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1281 2023-05-29 10:07:46.000000 pyobjc-framework-ExternalAccessory-9.2/setup.py
```

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Lib/ExternalAccessory/__init__.py` & `pyobjc-framework-ExternalAccessory-9.2/Lib/ExternalAccessory/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Lib/ExternalAccessory/_metadata.py` & `pyobjc-framework-ExternalAccessory-9.2/Lib/ExternalAccessory/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/PKG-INFO` & `pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExternalAccessory
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExternalAccessory on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExternalAccessory
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Lib/pyobjc_framework_ExternalAccessory.egg-info/SOURCES.txt` & `pyobjc-framework-ExternalAccessory-9.2/Lib/pyobjc_framework_ExternalAccessory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ExternalAccessory/__init__.py
 Lib/ExternalAccessory/_metadata.py
 Lib/pyobjc_framework_ExternalAccessory.egg-info/PKG-INFO
 Lib/pyobjc_framework_ExternalAccessory.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ExternalAccessory.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ExternalAccessory.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/License.txt` & `pyobjc-framework-ExternalAccessory-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Modules/_ExternalAccessory.m` & `pyobjc-framework-ExternalAccessory-9.2/Modules/_ExternalAccessory.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ExternalAccessory-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ExternalAccessory-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/PKG-INFO` & `pyobjc-framework-ExternalAccessory-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExternalAccessory
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExternalAccessory on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExternalAccessory
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eaaccessorymanager.py` & `pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eaaccessorymanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eawifiunconfiguredaccessory.py` & `pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eawifiunconfiguredaccessory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/PyObjCTest/test_eawifiunconfiguredaccessorybrowser.py` & `pyobjc-framework-ExternalAccessory-9.2/PyObjCTest/test_eawifiunconfiguredaccessorybrowser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/ExternalAccessory.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/ExternalAccessory.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ExternalAccessory-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ExternalAccessory-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExternalAccessory-9.1b1/setup.py` & `pyobjc-framework-ExternalAccessory-9.2/setup.py`

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
     name="pyobjc-framework-ExternalAccessory",
     description="Wrappers for the framework ExternalAccessory on macOS",
     min_os_level="10.13",
     packages=["ExternalAccessory"],
     ext_modules=[
```
