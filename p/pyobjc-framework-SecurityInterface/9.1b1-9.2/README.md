# Comparing `tmp/pyobjc-framework-SecurityInterface-9.1b1.tar.gz` & `tmp/pyobjc-framework-SecurityInterface-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SecurityInterface-9.1b1.tar", last modified: Sun Mar 26 11:39:40 2023, max compression
+gzip compressed data, was "pyobjc-framework-SecurityInterface-9.2.tar", last modified: Wed Jun  7 00:27:56 2023, max compression
```

## Comparing `pyobjc-framework-SecurityInterface-9.1b1.tar` & `pyobjc-framework-SecurityInterface-9.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.637298 pyobjc-framework-SecurityInterface-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.582800 pyobjc-framework-SecurityInterface-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.590700 pyobjc-framework-SecurityInterface-9.1b1/Lib/SecurityInterface/
--rw-r--r--   0 ronald     (501) staff       (20)      837 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/SecurityInterface/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     8542 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/SecurityInterface/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.594049 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2130 2023-03-26 11:39:40.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1243 2023-03-26 11:39:40.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:39:40.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:36.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       82 2023-03-26 11:39:40.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-03-26 11:39:40.000000 pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SecurityInterface-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.599639 pyobjc-framework-SecurityInterface-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     5759 2023-02-19 10:50:35.000000 pyobjc-framework-SecurityInterface-9.1b1/Modules/_SecurityInterface.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SecurityInterface-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SecurityInterface-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1919 2023-03-26 11:39:40.636645 pyobjc-framework-SecurityInterface-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.609956 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_securityinterface.py
--rw-r--r--   0 ronald     (501) staff       (20)     1504 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfauthorizationpluginview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1440 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfauthorizationview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1726 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfcertificatepanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      470 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfcertificatetrustpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1466 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfcertificateview.py
--rw-r--r--   0 ronald     (501) staff       (20)      904 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfchooseidentitypanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfchooseidentitytablecellview.py
--rw-r--r--   0 ronald     (501) staff       (20)      481 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfkeychainsavepanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      488 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfkeychainsettingspanel.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.611602 pyobjc-framework-SecurityInterface-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3684 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/SecurityInterface.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      527 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:40.625765 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    36151 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36170 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36165 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36162 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36152 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36171 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SecurityInterface-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:39:40.637449 pyobjc-framework-SecurityInterface-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1061 2023-03-25 14:20:32.000000 pyobjc-framework-SecurityInterface-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.380850 pyobjc-framework-SecurityInterface-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.332425 pyobjc-framework-SecurityInterface-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.337928 pyobjc-framework-SecurityInterface-9.2/Lib/SecurityInterface/
+-rw-r--r--   0 ronald     (501) staff       (20)      837 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/Lib/SecurityInterface/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8542 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.2/Lib/SecurityInterface/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.345108 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2128 2023-06-07 00:27:56.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1258 2023-06-07 00:27:56.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:56.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:36.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       76 2023-06-07 00:27:56.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-06-07 00:27:56.000000 pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SecurityInterface-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.346979 pyobjc-framework-SecurityInterface-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     5759 2023-02-19 10:50:35.000000 pyobjc-framework-SecurityInterface-9.2/Modules/_SecurityInterface.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SecurityInterface-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SecurityInterface-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1917 2023-06-07 00:27:56.375033 pyobjc-framework-SecurityInterface-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.364383 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_securityinterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1504 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfauthorizationpluginview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1440 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfauthorizationview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1726 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfcertificatepanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      470 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfcertificatetrustpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1466 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfcertificateview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      904 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfchooseidentitypanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfchooseidentitytablecellview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      481 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfkeychainsavepanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      488 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfkeychainsettingspanel.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.366447 pyobjc-framework-SecurityInterface-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3684 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/metadata/SecurityInterface.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      527 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:56.373656 pyobjc-framework-SecurityInterface-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    36151 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36170 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36165 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36162 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36152 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36171 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SecurityInterface-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SecurityInterface-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:56.380991 pyobjc-framework-SecurityInterface-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1143 2023-05-29 10:07:47.000000 pyobjc-framework-SecurityInterface-9.2/setup.py
```

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Lib/SecurityInterface/__init__.py` & `pyobjc-framework-SecurityInterface-9.2/Lib/SecurityInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Lib/SecurityInterface/_metadata.py` & `pyobjc-framework-SecurityInterface-9.2/Lib/SecurityInterface/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/PKG-INFO` & `pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SecurityInterface
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SecurityInterface on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SecurityInterface
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Lib/pyobjc_framework_SecurityInterface.egg-info/SOURCES.txt` & `pyobjc-framework-SecurityInterface-9.2/Lib/pyobjc_framework_SecurityInterface.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SecurityInterface/__init__.py
 Lib/SecurityInterface/_metadata.py
 Lib/pyobjc_framework_SecurityInterface.egg-info/PKG-INFO
 Lib/pyobjc_framework_SecurityInterface.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SecurityInterface.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SecurityInterface.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/License.txt` & `pyobjc-framework-SecurityInterface-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Modules/_SecurityInterface.m` & `pyobjc-framework-SecurityInterface-9.2/Modules/_SecurityInterface.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SecurityInterface-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SecurityInterface-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PKG-INFO` & `pyobjc-framework-SecurityInterface-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SecurityInterface
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SecurityInterface on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SecurityInterface
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfauthorizationpluginview.py` & `pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfauthorizationpluginview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfauthorizationview.py` & `pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfauthorizationview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfcertificatepanel.py` & `pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfcertificatepanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfcertificateview.py` & `pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfcertificateview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/PyObjCTest/test_sfchooseidentitypanel.py` & `pyobjc-framework-SecurityInterface-9.2/PyObjCTest/test_sfchooseidentitypanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/SecurityInterface.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/SecurityInterface.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/metadata.ini` & `pyobjc-framework-SecurityInterface-9.2/metadata/metadata.ini`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SecurityInterface-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SecurityInterface-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityInterface-9.1b1/setup.py` & `pyobjc-framework-SecurityInterface-9.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-from pyobjc_setup import Extension, setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-SecurityInterface",
     description="Wrappers for the framework SecurityInterface on macOS",
     packages=["SecurityInterface"],
     ext_modules=[
         Extension(
```

