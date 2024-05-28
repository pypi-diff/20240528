# Comparing `tmp/pyobjc-framework-UserNotifications-9.1b1.tar.gz` & `tmp/pyobjc-framework-UserNotifications-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-UserNotifications-9.1b1.tar", last modified: Sun Mar 26 11:43:07 2023, max compression
+gzip compressed data, was "pyobjc-framework-UserNotifications-9.2.tar", last modified: Wed Jun  7 00:30:52 2023, max compression
```

## Comparing `pyobjc-framework-UserNotifications-9.1b1.tar` & `pyobjc-framework-UserNotifications-9.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.536504 pyobjc-framework-UserNotifications-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.454976 pyobjc-framework-UserNotifications-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.472340 pyobjc-framework-UserNotifications-9.1b1/Lib/UserNotifications/
--rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/UserNotifications/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    10088 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/UserNotifications/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.475158 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2140 2023-03-26 11:43:07.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1351 2023-03-26 11:43:07.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:07.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:55.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:43:07.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-03-26 11:43:07.000000 pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-UserNotifications-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.477907 pyobjc-framework-UserNotifications-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1180 2021-10-18 19:38:40.000000 pyobjc-framework-UserNotifications-9.1b1/Modules/_UserNotifications.m
--rw-r--r--   0 ronald     (501) staff       (20)      329 2021-10-18 19:38:40.000000 pyobjc-framework-UserNotifications-9.1b1/Modules/_UserNotifications_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotifications-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-UserNotifications-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1929 2023-03-26 11:43:07.535792 pyobjc-framework-UserNotifications-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.511726 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1318 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      731 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      859 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)      857 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationcategory.py
--rw-r--r--   0 ronald     (501) staff       (20)      992 2022-06-25 20:08:44.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationcontent.py
--rw-r--r--   0 ronald     (501) staff       (20)      374 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      353 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationserviceextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     1593 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationsettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      707 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationtrigger.py
--rw-r--r--   0 ronald     (501) staff       (20)     4218 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unusernotificationcenter.py
--rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_usernotifications.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.513227 pyobjc-framework-UserNotifications-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     7492 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/UserNotifications.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:07.533784 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    64482 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63724 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    66140 2022-07-30 15:06:02.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    55278 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    64483 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63725 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    66141 2022-07-30 15:06:02.000000 pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-UserNotifications-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:07.536619 pyobjc-framework-UserNotifications-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1210 2023-03-25 14:20:32.000000 pyobjc-framework-UserNotifications-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.382304 pyobjc-framework-UserNotifications-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.317681 pyobjc-framework-UserNotifications-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.323236 pyobjc-framework-UserNotifications-9.2/Lib/UserNotifications/
+-rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.2/Lib/UserNotifications/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10088 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.2/Lib/UserNotifications/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.326427 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2138 2023-06-07 00:30:52.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1366 2023-06-07 00:30:52.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:30:52.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:55.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:30:52.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-06-07 00:30:52.000000 pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-UserNotifications-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.329322 pyobjc-framework-UserNotifications-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1180 2021-10-18 19:38:40.000000 pyobjc-framework-UserNotifications-9.2/Modules/_UserNotifications.m
+-rw-r--r--   0 ronald     (501) staff       (20)      329 2021-10-18 19:38:40.000000 pyobjc-framework-UserNotifications-9.2/Modules/_UserNotifications_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotifications-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-UserNotifications-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1927 2023-06-07 00:30:52.381902 pyobjc-framework-UserNotifications-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.369630 pyobjc-framework-UserNotifications-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      731 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      859 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)      857 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationcategory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      992 2022-06-25 20:08:44.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationcontent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      374 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      353 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationserviceextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1593 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationsettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      707 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationtrigger.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4218 2022-07-08 16:02:54.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unusernotificationcenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      218 2022-04-11 08:03:15.000000 pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_usernotifications.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.370965 pyobjc-framework-UserNotifications-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     7492 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.2/metadata/UserNotifications.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:15.000000 pyobjc-framework-UserNotifications-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:30:52.380159 pyobjc-framework-UserNotifications-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    64482 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63724 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    66140 2022-07-30 15:06:02.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    55278 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    64483 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63725 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    66141 2022-07-30 15:06:02.000000 pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-UserNotifications-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-UserNotifications-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:30:52.382401 pyobjc-framework-UserNotifications-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1281 2023-05-29 10:07:47.000000 pyobjc-framework-UserNotifications-9.2/setup.py
```

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Lib/UserNotifications/__init__.py` & `pyobjc-framework-UserNotifications-9.2/Lib/UserNotifications/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Lib/UserNotifications/_metadata.py` & `pyobjc-framework-UserNotifications-9.2/Lib/UserNotifications/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/PKG-INFO` & `pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-UserNotifications
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework UserNotifications on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,UserNotifications
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Lib/pyobjc_framework_UserNotifications.egg-info/SOURCES.txt` & `pyobjc-framework-UserNotifications-9.2/Lib/pyobjc_framework_UserNotifications.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/UserNotifications/__init__.py
 Lib/UserNotifications/_metadata.py
 Lib/pyobjc_framework_UserNotifications.egg-info/PKG-INFO
 Lib/pyobjc_framework_UserNotifications.egg-info/SOURCES.txt
 Lib/pyobjc_framework_UserNotifications.egg-info/dependency_links.txt
 Lib/pyobjc_framework_UserNotifications.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-UserNotifications-9.1b1/License.txt` & `pyobjc-framework-UserNotifications-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Modules/_UserNotifications.m` & `pyobjc-framework-UserNotifications-9.2/Modules/_UserNotifications.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-UserNotifications-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-UserNotifications-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PKG-INFO` & `pyobjc-framework-UserNotifications-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-UserNotifications
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework UserNotifications on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,UserNotifications
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unerror.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationaction.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationattachment.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationattachment.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationcategory.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationcategory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationcontent.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationcontent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationsettings.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationsettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unnotificationtrigger.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unnotificationtrigger.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/PyObjCTest/test_unusernotificationcenter.py` & `pyobjc-framework-UserNotifications-9.2/PyObjCTest/test_unusernotificationcenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/UserNotifications.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/UserNotifications.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-UserNotifications-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/pyobjc_setup.py` & `pyobjc-framework-UserNotifications-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotifications-9.1b1/setup.py` & `pyobjc-framework-UserNotifications-9.2/setup.py`

 * *Files 6% similar despite different names*

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
     name="pyobjc-framework-UserNotifications",
     description="Wrappers for the framework UserNotifications on macOS",
     min_os_level="10.14",
     packages=["UserNotifications"],
     ext_modules=[
```

