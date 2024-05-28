# Comparing `tmp/pyobjc-framework-MediaToolbox-9.1b1.tar.gz` & `tmp/pyobjc-framework-MediaToolbox-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MediaToolbox-9.1b1.tar", last modified: Sun Mar 26 11:29:02 2023, max compression
+gzip compressed data, was "pyobjc-framework-MediaToolbox-9.2.tar", last modified: Wed Jun  7 00:19:36 2023, max compression
```

## Comparing `pyobjc-framework-MediaToolbox-9.1b1.tar` & `pyobjc-framework-MediaToolbox-9.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.302456 pyobjc-framework-MediaToolbox-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.274364 pyobjc-framework-MediaToolbox-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.280176 pyobjc-framework-MediaToolbox-9.1b1/Examples/ProcessingTap/
--rw-r--r--   0 ronald     (501) staff       (20)       93 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/Examples/ProcessingTap/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     2833 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/Examples/ProcessingTap/tap.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.274710 pyobjc-framework-MediaToolbox-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.282372 pyobjc-framework-MediaToolbox-9.1b1/Lib/MediaToolbox/
--rw-r--r--   0 ronald     (501) staff       (20)      857 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/MediaToolbox/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1675 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/MediaToolbox/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.285704 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-03-26 11:29:02.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1046 2023-03-26 11:29:02.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:29:02.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:27.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:29:02.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:29:02.000000 pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaToolbox-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.288083 pyobjc-framework-MediaToolbox-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    13726 2021-10-18 19:38:40.000000 pyobjc-framework-MediaToolbox-9.1b1/Modules/_MediaToolbox.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MediaToolbox-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MediaToolbox-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1908 2023-03-26 11:29:02.302127 pyobjc-framework-MediaToolbox-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.296473 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/test_mediatoolbox.py
--rw-r--r--   0 ronald     (501) staff       (20)     1345 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/test_mtaudioprocessingtap.py
--rw-r--r--   0 ronald     (501) staff       (20)      344 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/test_mtformatnames.py
--rw-r--r--   0 ronald     (501) staff       (20)      257 2022-10-18 09:53:24.000000 pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/test_mtprofessionalvideoWorkflow.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.298312 pyobjc-framework-MediaToolbox-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      910 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/MediaToolbox.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:02.301553 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     3106 2021-07-30 09:00:38.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3125 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3092 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3107 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3107 2021-07-30 09:00:38.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3126 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaToolbox-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:29:02.302575 pyobjc-framework-MediaToolbox-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      974 2023-03-25 14:20:31.000000 pyobjc-framework-MediaToolbox-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.190842 pyobjc-framework-MediaToolbox-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.153600 pyobjc-framework-MediaToolbox-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.159241 pyobjc-framework-MediaToolbox-9.2/Examples/ProcessingTap/
+-rw-r--r--   0 ronald     (501) staff       (20)       93 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/Examples/ProcessingTap/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     2833 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/Examples/ProcessingTap/tap.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.154118 pyobjc-framework-MediaToolbox-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.160385 pyobjc-framework-MediaToolbox-9.2/Lib/MediaToolbox/
+-rw-r--r--   0 ronald     (501) staff       (20)      857 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/Lib/MediaToolbox/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1675 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.2/Lib/MediaToolbox/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.164148 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-06-07 00:19:36.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1061 2023-06-07 00:19:36.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:36.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:27.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:19:36.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:19:36.000000 pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaToolbox-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.169563 pyobjc-framework-MediaToolbox-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    13726 2021-10-18 19:38:40.000000 pyobjc-framework-MediaToolbox-9.2/Modules/_MediaToolbox.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MediaToolbox-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MediaToolbox-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-06-07 00:19:36.190438 pyobjc-framework-MediaToolbox-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.173001 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/test_mediatoolbox.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1345 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/test_mtaudioprocessingtap.py
+-rw-r--r--   0 ronald     (501) staff       (20)      344 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/test_mtformatnames.py
+-rw-r--r--   0 ronald     (501) staff       (20)      257 2022-10-18 09:53:24.000000 pyobjc-framework-MediaToolbox-9.2/PyObjCTest/test_mtprofessionalvideoWorkflow.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.174930 pyobjc-framework-MediaToolbox-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      910 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/metadata/MediaToolbox.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:36.189374 pyobjc-framework-MediaToolbox-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     3106 2021-07-30 09:00:38.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3125 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3092 2020-11-30 18:45:15.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3107 2021-03-21 10:08:23.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3107 2021-07-30 09:00:38.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3126 2022-02-24 08:47:16.000000 pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaToolbox-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MediaToolbox-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:36.190940 pyobjc-framework-MediaToolbox-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1055 2023-05-29 10:07:46.000000 pyobjc-framework-MediaToolbox-9.2/setup.py
```

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Examples/ProcessingTap/tap.py` & `pyobjc-framework-MediaToolbox-9.2/Examples/ProcessingTap/tap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Lib/MediaToolbox/__init__.py` & `pyobjc-framework-MediaToolbox-9.2/Lib/MediaToolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Lib/MediaToolbox/_metadata.py` & `pyobjc-framework-MediaToolbox-9.2/Lib/MediaToolbox/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/PKG-INFO` & `pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaToolbox
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaToolbox on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaToolbox
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Lib/pyobjc_framework_MediaToolbox.egg-info/SOURCES.txt` & `pyobjc-framework-MediaToolbox-9.2/Lib/pyobjc_framework_MediaToolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/ProcessingTap/summary.txt
 Examples/ProcessingTap/tap.py
 Lib/MediaToolbox/__init__.py
 Lib/MediaToolbox/_metadata.py
 Lib/pyobjc_framework_MediaToolbox.egg-info/PKG-INFO
 Lib/pyobjc_framework_MediaToolbox.egg-info/SOURCES.txt
```

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/License.txt` & `pyobjc-framework-MediaToolbox-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Modules/_MediaToolbox.m` & `pyobjc-framework-MediaToolbox-9.2/Modules/_MediaToolbox.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MediaToolbox-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MediaToolbox-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/PKG-INFO` & `pyobjc-framework-MediaToolbox-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaToolbox
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaToolbox on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaToolbox
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/PyObjCTest/test_mtaudioprocessingtap.py` & `pyobjc-framework-MediaToolbox-9.2/PyObjCTest/test_mtaudioprocessingtap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/MediaToolbox.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/MediaToolbox.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MediaToolbox-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MediaToolbox-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaToolbox-9.1b1/setup.py` & `pyobjc-framework-MediaToolbox-9.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "MediaToolbox" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MediaToolbox",
     description="Wrappers for the framework MediaToolbox on macOS",
     min_os_level="10.9",
     packages=["MediaToolbox"],
     ext_modules=[
```

