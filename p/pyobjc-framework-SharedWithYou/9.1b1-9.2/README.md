# Comparing `tmp/pyobjc-framework-SharedWithYou-9.1b1.tar.gz` & `tmp/pyobjc-framework-SharedWithYou-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SharedWithYou-9.1b1.tar", last modified: Sun Mar 26 11:40:08 2023, max compression
+gzip compressed data, was "pyobjc-framework-SharedWithYou-9.2.tar", last modified: Wed Jun  7 00:28:17 2023, max compression
```

## Comparing `pyobjc-framework-SharedWithYou-9.1b1.tar` & `pyobjc-framework-SharedWithYou-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.286876 pyobjc-framework-SharedWithYou-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.227713 pyobjc-framework-SharedWithYou-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.236867 pyobjc-framework-SharedWithYou-9.1b1/Lib/SharedWithYou/
--rw-r--r--   0 ronald     (501) staff       (20)      815 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/SharedWithYou/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5637 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/SharedWithYou/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.244036 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2123 2023-03-26 11:40:08.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1043 2023-03-26 11:40:08.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:40:08.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-15 12:19:57.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       61 2023-03-26 11:40:08.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:40:08.000000 pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-SharedWithYou-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-SharedWithYou-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.248508 pyobjc-framework-SharedWithYou-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1156 2022-06-23 17:30:14.000000 pyobjc-framework-SharedWithYou-9.1b1/Modules/_SharedWithYou.m
--rw-r--r--   0 ronald     (501) staff       (20)      191 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.1b1/Modules/_SharedWithYou_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SharedWithYou-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SharedWithYou-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1912 2023-03-26 11:40:08.286395 pyobjc-framework-SharedWithYou-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.268927 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      195 2022-10-20 10:02:15.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_sharedwithyou.py
--rw-r--r--   0 ronald     (501) staff       (20)     1329 2022-06-24 08:28:52.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swattributionview.py
--rw-r--r--   0 ronald     (501) staff       (20)      727 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swcollaborationview.py
--rw-r--r--   0 ronald     (501) staff       (20)      523 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     1041 2022-10-20 21:08:30.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightcenter.py
--rw-r--r--   0 ronald     (501) staff       (20)      375 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightchangeevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      205 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      460 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightmembershipevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      566 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightpersistenceevent.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.271399 pyobjc-framework-SharedWithYou-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.1b1/metadata/SharedWithYou.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:40:08.275403 pyobjc-framework-SharedWithYou-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    35273 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35274 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SharedWithYou-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:40:08.286985 pyobjc-framework-SharedWithYou-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1209 2023-03-25 14:20:32.000000 pyobjc-framework-SharedWithYou-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.534164 pyobjc-framework-SharedWithYou-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.484133 pyobjc-framework-SharedWithYou-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.493275 pyobjc-framework-SharedWithYou-9.2/Lib/SharedWithYou/
+-rw-r--r--   0 ronald     (501) staff       (20)      815 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/Lib/SharedWithYou/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5637 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.2/Lib/SharedWithYou/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.497211 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2121 2023-06-07 00:28:17.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1058 2023-06-07 00:28:17.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:28:17.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-15 12:19:57.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       57 2023-06-07 00:28:17.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:28:17.000000 pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-SharedWithYou-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-SharedWithYou-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.500210 pyobjc-framework-SharedWithYou-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1156 2022-06-23 17:30:14.000000 pyobjc-framework-SharedWithYou-9.2/Modules/_SharedWithYou.m
+-rw-r--r--   0 ronald     (501) staff       (20)      191 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.2/Modules/_SharedWithYou_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SharedWithYou-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SharedWithYou-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1910 2023-06-07 00:28:17.533730 pyobjc-framework-SharedWithYou-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.520855 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      195 2022-10-20 10:02:15.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_sharedwithyou.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1329 2022-06-24 08:28:52.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swattributionview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      727 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swcollaborationview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      523 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1041 2022-10-20 21:08:30.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightcenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      375 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightchangeevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      205 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      460 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightmembershipevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      566 2022-06-26 10:16:33.000000 pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightpersistenceevent.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.523478 pyobjc-framework-SharedWithYou-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.2/metadata/SharedWithYou.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2022-06-15 11:57:00.000000 pyobjc-framework-SharedWithYou-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:28:17.526192 pyobjc-framework-SharedWithYou-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    35273 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35274 2022-10-18 09:53:23.000000 pyobjc-framework-SharedWithYou-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SharedWithYou-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SharedWithYou-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:28:17.534266 pyobjc-framework-SharedWithYou-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1280 2023-05-29 10:07:47.000000 pyobjc-framework-SharedWithYou-9.2/setup.py
```

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Lib/SharedWithYou/__init__.py` & `pyobjc-framework-SharedWithYou-9.2/Lib/SharedWithYou/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Lib/SharedWithYou/_metadata.py` & `pyobjc-framework-SharedWithYou-9.2/Lib/SharedWithYou/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/PKG-INFO` & `pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SharedWithYou
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SharedWithYou on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SharedWithYou
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Lib/pyobjc_framework_SharedWithYou.egg-info/SOURCES.txt` & `pyobjc-framework-SharedWithYou-9.2/Lib/pyobjc_framework_SharedWithYou.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SharedWithYou/__init__.py
 Lib/SharedWithYou/_metadata.py
 Lib/pyobjc_framework_SharedWithYou.egg-info/PKG-INFO
 Lib/pyobjc_framework_SharedWithYou.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SharedWithYou.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SharedWithYou.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/License.txt` & `pyobjc-framework-SharedWithYou-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Modules/_SharedWithYou.m` & `pyobjc-framework-SharedWithYou-9.2/Modules/_SharedWithYou.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SharedWithYou-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SharedWithYou-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PKG-INFO` & `pyobjc-framework-SharedWithYou-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SharedWithYou
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SharedWithYou on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SharedWithYou
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swattributionview.py` & `pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swattributionview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swcollaborationview.py` & `pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swcollaborationview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swerrors.py` & `pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightcenter.py` & `pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightcenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/PyObjCTest/test_swhighlightpersistenceevent.py` & `pyobjc-framework-SharedWithYou-9.2/PyObjCTest/test_swhighlightpersistenceevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-SharedWithYou-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-SharedWithYou-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SharedWithYou-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SharedWithYou-9.1b1/setup.py` & `pyobjc-framework-SharedWithYou-9.2/setup.py`

 * *Files 14% similar despite different names*

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
     name="pyobjc-framework-SharedWithYou",
     description="Wrappers for the framework SharedWithYou on macOS",
     min_os_level="13.0",
     packages=["SharedWithYou"],
     ext_modules=[
```

