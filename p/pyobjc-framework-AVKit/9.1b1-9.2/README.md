# Comparing `tmp/pyobjc-framework-AVKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-AVKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AVKit-9.1b1.tar", last modified: Sun Mar 26 11:12:35 2023, max compression
+gzip compressed data, was "pyobjc-framework-AVKit-9.2.tar", last modified: Wed Jun  7 00:04:39 2023, max compression
```

## Comparing `pyobjc-framework-AVKit-9.1b1.tar` & `pyobjc-framework-AVKit-9.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.891023 pyobjc-framework-AVKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.735462 pyobjc-framework-AVKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.764269 pyobjc-framework-AVKit-9.1b1/Lib/AVKit/
--rw-r--r--   0 ronald     (501) staff       (20)      732 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/Lib/AVKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    12629 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.1b1/Lib/AVKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.780859 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-03-26 11:12:35.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1206 2023-03-26 11:12:35.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:12:35.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:06.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:12:35.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        6 2023-03-26 11:12:35.000000 pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AVKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.786589 pyobjc-framework-AVKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      759 2021-10-18 19:38:40.000000 pyobjc-framework-AVKit-9.1b1/Modules/_AVKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      865 2021-07-31 09:40:12.000000 pyobjc-framework-AVKit-9.1b1/Modules/_AVKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AVKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-AVKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-03-26 11:12:35.890668 pyobjc-framework-AVKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.844614 pyobjc-framework-AVKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-26 21:30:09.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avcaptureview.py
--rw-r--r--   0 ronald     (501) staff       (20)      194 2022-04-11 08:03:15.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avkit.py
--rw-r--r--   0 ronald     (501) staff       (20)     2500 2022-10-18 09:53:23.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avpictureInpicturecontroller_avsamplebufferdisplayLayersupport.py
--rw-r--r--   0 ronald     (501) staff       (20)     2004 2022-06-25 20:11:40.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avpictureinpicturecontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     4087 2022-06-25 08:58:33.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avplayerview.py
--rw-r--r--   0 ronald     (501) staff       (20)      908 2022-06-25 20:12:52.000000 pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avroutepickerview.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.849568 pyobjc-framework-AVKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2725 2021-08-03 12:49:20.000000 pyobjc-framework-AVKit-9.1b1/metadata/AVKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:35.889700 pyobjc-framework-AVKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    40384 2021-08-04 10:01:04.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40630 2022-02-24 08:47:16.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    47098 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12009 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28321 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29700 2021-03-21 10:08:22.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6095 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40385 2021-08-04 10:01:04.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40631 2022-02-24 08:47:16.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    47099 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AVKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:12:35.891276 pyobjc-framework-AVKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1196 2023-03-25 14:20:30.000000 pyobjc-framework-AVKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.324949 pyobjc-framework-AVKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.263032 pyobjc-framework-AVKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.272570 pyobjc-framework-AVKit-9.2/Lib/AVKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      732 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/Lib/AVKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12629 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.2/Lib/AVKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.276571 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-06-07 00:04:39.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1221 2023-06-07 00:04:39.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:04:39.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:06.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:04:39.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        6 2023-06-07 00:04:39.000000 pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AVKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.280885 pyobjc-framework-AVKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      759 2021-10-18 19:38:40.000000 pyobjc-framework-AVKit-9.2/Modules/_AVKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      865 2021-07-31 09:40:12.000000 pyobjc-framework-AVKit-9.2/Modules/_AVKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AVKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-AVKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-06-07 00:04:39.324584 pyobjc-framework-AVKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.298876 pyobjc-framework-AVKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-26 21:30:09.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avcaptureview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      194 2022-04-11 08:03:15.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2500 2022-10-18 09:53:23.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avpictureInpicturecontroller_avsamplebufferdisplayLayersupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2004 2022-06-25 20:11:40.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avpictureinpicturecontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4087 2022-06-25 08:58:33.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avplayerview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      908 2022-06-25 20:12:52.000000 pyobjc-framework-AVKit-9.2/PyObjCTest/test_avroutepickerview.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.301839 pyobjc-framework-AVKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2725 2021-08-03 12:49:20.000000 pyobjc-framework-AVKit-9.2/metadata/AVKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:39.323639 pyobjc-framework-AVKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    40384 2021-08-04 10:01:04.000000 pyobjc-framework-AVKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40630 2022-02-24 08:47:16.000000 pyobjc-framework-AVKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    47098 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12009 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28321 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29700 2021-03-21 10:08:22.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6095 2020-11-30 18:45:14.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40385 2021-08-04 10:01:04.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40631 2022-02-24 08:47:16.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    47099 2022-06-25 20:19:21.000000 pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AVKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AVKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:04:39.325057 pyobjc-framework-AVKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1268 2023-05-29 10:07:45.000000 pyobjc-framework-AVKit-9.2/setup.py
```

### Comparing `pyobjc-framework-AVKit-9.1b1/Lib/AVKit/__init__.py` & `pyobjc-framework-AVKit-9.2/Lib/AVKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Lib/AVKit/_metadata.py` & `pyobjc-framework-AVKit-9.2/Lib/AVKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/PKG-INFO` & `pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AVKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AVKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AVKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-AVKit-9.1b1/Lib/pyobjc_framework_AVKit.egg-info/SOURCES.txt` & `pyobjc-framework-AVKit-9.2/Lib/pyobjc_framework_AVKit.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AVKit/__init__.py
 Lib/AVKit/_metadata.py
 Lib/pyobjc_framework_AVKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_AVKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AVKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AVKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AVKit-9.1b1/License.txt` & `pyobjc-framework-AVKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Modules/_AVKit.m` & `pyobjc-framework-AVKit-9.2/Modules/_AVKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Modules/_AVKit_protocols.m` & `pyobjc-framework-AVKit-9.2/Modules/_AVKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-AVKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-AVKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-AVKit-9.1b1/PKG-INFO` & `pyobjc-framework-AVKit-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AVKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AVKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AVKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avcaptureview.py` & `pyobjc-framework-AVKit-9.2/PyObjCTest/test_avcaptureview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avpictureInpicturecontroller_avsamplebufferdisplayLayersupport.py` & `pyobjc-framework-AVKit-9.2/PyObjCTest/test_avpictureInpicturecontroller_avsamplebufferdisplayLayersupport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avpictureinpicturecontroller.py` & `pyobjc-framework-AVKit-9.2/PyObjCTest/test_avpictureinpicturecontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avplayerview.py` & `pyobjc-framework-AVKit-9.2/PyObjCTest/test_avplayerview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/PyObjCTest/test_avroutepickerview.py` & `pyobjc-framework-AVKit-9.2/PyObjCTest/test_avroutepickerview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/AVKit.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/AVKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-AVKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AVKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVKit-9.1b1/setup.py` & `pyobjc-framework-AVKit-9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 import os
 
-from pyobjc_setup import Extension, setup
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-AVKit",
     description="Wrappers for the framework AVKit on macOS",
     min_os_level="10.9",
     packages=["AVKit"],
     ext_modules=[
```

