# Comparing `tmp/pyobjc-framework-FSEvents-9.1b1.tar.gz` & `tmp/pyobjc-framework-FSEvents-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-FSEvents-9.1b1.tar", last modified: Sun Mar 26 11:24:15 2023, max compression
+gzip compressed data, was "pyobjc-framework-FSEvents-9.2.tar", last modified: Wed Jun  7 00:14:26 2023, max compression
```

## Comparing `pyobjc-framework-FSEvents-9.1b1.tar` & `pyobjc-framework-FSEvents-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.514602 pyobjc-framework-FSEvents-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.488466 pyobjc-framework-FSEvents-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)     8978 2021-07-30 09:00:37.000000 pyobjc-framework-FSEvents-9.1b1/Examples/watcher.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FSEvents-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.484219 pyobjc-framework-FSEvents-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.490422 pyobjc-framework-FSEvents-9.1b1/Lib/FSEvents/
--rw-r--r--   0 ronald     (501) staff       (20)      742 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.1b1/Lib/FSEvents/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3929 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.1b1/Lib/FSEvents/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.498555 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2263 2023-03-26 11:24:15.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      825 2023-03-26 11:24:15.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:15.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:05.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:24:15.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:24:15.000000 pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.500728 pyobjc-framework-FSEvents-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    10765 2021-10-18 19:38:40.000000 pyobjc-framework-FSEvents-9.1b1/Modules/_callbacks.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-FSEvents-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-FSEvents-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2052 2023-03-26 11:24:15.514276 pyobjc-framework-FSEvents-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.501977 pyobjc-framework-FSEvents-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7802 2022-04-11 08:03:15.000000 pyobjc-framework-FSEvents-9.1b1/PyObjCTest/test_fsevents.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.508066 pyobjc-framework-FSEvents-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     5957 2021-07-31 13:47:06.000000 pyobjc-framework-FSEvents-9.1b1/metadata/CoreServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:15.513314 pyobjc-framework-FSEvents-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10783 2021-08-04 10:01:04.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10802 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8292 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8875 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8948 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10784 2021-08-04 10:01:04.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10803 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FSEvents-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:15.514706 pyobjc-framework-FSEvents-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      974 2023-03-25 14:20:31.000000 pyobjc-framework-FSEvents-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.574374 pyobjc-framework-FSEvents-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.553074 pyobjc-framework-FSEvents-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)     8978 2021-07-30 09:00:37.000000 pyobjc-framework-FSEvents-9.2/Examples/watcher.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-FSEvents-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.548631 pyobjc-framework-FSEvents-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.554982 pyobjc-framework-FSEvents-9.2/Lib/FSEvents/
+-rw-r--r--   0 ronald     (501) staff       (20)      742 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.2/Lib/FSEvents/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3929 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.2/Lib/FSEvents/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.559236 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2261 2023-06-07 00:14:26.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      840 2023-06-07 00:14:26.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:14:26.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:05.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:14:26.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:14:26.000000 pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.561077 pyobjc-framework-FSEvents-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    10765 2021-10-18 19:38:40.000000 pyobjc-framework-FSEvents-9.2/Modules/_callbacks.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-FSEvents-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-FSEvents-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2050 2023-06-07 00:14:26.573979 pyobjc-framework-FSEvents-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.562801 pyobjc-framework-FSEvents-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7802 2022-04-11 08:03:15.000000 pyobjc-framework-FSEvents-9.2/PyObjCTest/test_fsevents.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.568002 pyobjc-framework-FSEvents-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     5957 2021-07-31 13:47:06.000000 pyobjc-framework-FSEvents-9.2/metadata/CoreServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:14.000000 pyobjc-framework-FSEvents-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:14:26.573235 pyobjc-framework-FSEvents-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10783 2021-08-04 10:01:04.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10802 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8292 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8875 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8948 2021-03-21 10:08:22.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10784 2021-08-04 10:01:04.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10803 2022-02-24 08:47:16.000000 pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-FSEvents-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-FSEvents-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:14:26.574490 pyobjc-framework-FSEvents-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2023-05-29 10:07:46.000000 pyobjc-framework-FSEvents-9.2/setup.py
```

### Comparing `pyobjc-framework-FSEvents-9.1b1/Examples/watcher.py` & `pyobjc-framework-FSEvents-9.2/Examples/watcher.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/LICENSE.txt` & `pyobjc-framework-FSEvents-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/Lib/FSEvents/__init__.py` & `pyobjc-framework-FSEvents-9.2/Lib/FSEvents/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/Lib/FSEvents/_metadata.py` & `pyobjc-framework-FSEvents-9.2/Lib/FSEvents/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/PKG-INFO` & `pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FSEvents
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FSEvents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FSEvents
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-FSEvents-9.1b1/Lib/pyobjc_framework_FSEvents.egg-info/SOURCES.txt` & `pyobjc-framework-FSEvents-9.2/Lib/pyobjc_framework_FSEvents.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/watcher.py
 Lib/FSEvents/__init__.py
 Lib/FSEvents/_metadata.py
 Lib/pyobjc_framework_FSEvents.egg-info/PKG-INFO
 Lib/pyobjc_framework_FSEvents.egg-info/SOURCES.txt
 Lib/pyobjc_framework_FSEvents.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-FSEvents-9.1b1/Modules/_callbacks.m` & `pyobjc-framework-FSEvents-9.2/Modules/_callbacks.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-FSEvents-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-FSEvents-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-FSEvents-9.1b1/PKG-INFO` & `pyobjc-framework-FSEvents-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-FSEvents
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework FSEvents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,FSEvents
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-FSEvents-9.1b1/PyObjCTest/test_fsevents.py` & `pyobjc-framework-FSEvents-9.2/PyObjCTest/test_fsevents.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/CoreServices.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/CoreServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-FSEvents-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/pyobjc_setup.py` & `pyobjc-framework-FSEvents-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-FSEvents-9.1b1/setup.py` & `pyobjc-framework-FSEvents-9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 program is not running al the time.
 
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
     name="pyobjc-framework-FSEvents",
     description="Wrappers for the framework FSEvents on macOS",
     min_os_level="10.5",
     packages=["FSEvents"],
     ext_modules=[
```

