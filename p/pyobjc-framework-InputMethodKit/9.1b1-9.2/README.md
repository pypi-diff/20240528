# Comparing `tmp/pyobjc-framework-InputMethodKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-InputMethodKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-InputMethodKit-9.1b1.tar", last modified: Sun Mar 26 11:27:03 2023, max compression
+gzip compressed data, was "pyobjc-framework-InputMethodKit-9.2.tar", last modified: Wed Jun  7 00:17:25 2023, max compression
```

## Comparing `pyobjc-framework-InputMethodKit-9.1b1.tar` & `pyobjc-framework-InputMethodKit-9.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.938383 pyobjc-framework-InputMethodKit-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InputMethodKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.878804 pyobjc-framework-InputMethodKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.889017 pyobjc-framework-InputMethodKit-9.1b1/Lib/InputMethodKit/
--rw-r--r--   0 ronald     (501) staff       (20)      788 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/InputMethodKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     6789 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/InputMethodKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.892410 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2236 2023-03-26 11:27:03.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1046 2023-03-26 11:27:03.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:03.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:19.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:27:03.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:27:03.000000 pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.899242 pyobjc-framework-InputMethodKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1489 2021-10-18 19:38:40.000000 pyobjc-framework-InputMethodKit-9.1b1/Modules/_InputMethodKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/Modules/_InputMethodKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-InputMethodKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-InputMethodKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2025 2023-03-26 11:27:03.938048 pyobjc-framework-InputMethodKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.903698 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1533 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkcandidates.py
--rw-r--r--   0 ronald     (501) staff       (20)     4525 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkinputcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      764 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkserver.py
--rw-r--r--   0 ronald     (501) staff       (20)     1260 2023-03-03 17:21:59.000000 pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_inputmethodkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-InputMethodKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.905155 pyobjc-framework-InputMethodKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     4426 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/InputMethodKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:03.934128 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    28192 2021-07-30 09:00:38.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28211 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28193 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22195 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28879 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28921 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28193 2021-07-30 09:00:38.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    28212 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InputMethodKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:03.938627 pyobjc-framework-InputMethodKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1264 2023-03-25 14:20:31.000000 pyobjc-framework-InputMethodKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.308304 pyobjc-framework-InputMethodKit-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InputMethodKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.265562 pyobjc-framework-InputMethodKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.271961 pyobjc-framework-InputMethodKit-9.2/Lib/InputMethodKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      788 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/Lib/InputMethodKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6789 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.2/Lib/InputMethodKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.275317 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2234 2023-06-07 00:17:25.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1061 2023-06-07 00:17:25.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:25.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:19.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:17:25.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:17:25.000000 pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.277755 pyobjc-framework-InputMethodKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1489 2021-10-18 19:38:40.000000 pyobjc-framework-InputMethodKit-9.2/Modules/_InputMethodKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/Modules/_InputMethodKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-InputMethodKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-InputMethodKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2023 2023-06-07 00:17:25.307891 pyobjc-framework-InputMethodKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.286091 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1533 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkcandidates.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4525 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkinputcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      764 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1260 2023-03-03 17:21:59.000000 pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_inputmethodkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-InputMethodKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.287475 pyobjc-framework-InputMethodKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     4426 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/metadata/InputMethodKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:25.306582 pyobjc-framework-InputMethodKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    28192 2021-07-30 09:00:38.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28211 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28193 2021-03-21 10:08:22.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22195 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28879 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28921 2020-11-30 18:45:15.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28193 2021-07-30 09:00:38.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    28212 2022-02-24 08:47:16.000000 pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InputMethodKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-InputMethodKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:25.308405 pyobjc-framework-InputMethodKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1335 2023-05-29 10:07:46.000000 pyobjc-framework-InputMethodKit-9.2/setup.py
```

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/LICENSE.txt` & `pyobjc-framework-InputMethodKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Lib/InputMethodKit/__init__.py` & `pyobjc-framework-InputMethodKit-9.2/Lib/InputMethodKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Lib/InputMethodKit/_metadata.py` & `pyobjc-framework-InputMethodKit-9.2/Lib/InputMethodKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/PKG-INFO` & `pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InputMethodKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InputMethodKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InputMethodKit
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Lib/pyobjc_framework_InputMethodKit.egg-info/SOURCES.txt` & `pyobjc-framework-InputMethodKit-9.2/Lib/pyobjc_framework_InputMethodKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/InputMethodKit/__init__.py
 Lib/InputMethodKit/_metadata.py
 Lib/pyobjc_framework_InputMethodKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_InputMethodKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_InputMethodKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_InputMethodKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Modules/_InputMethodKit.m` & `pyobjc-framework-InputMethodKit-9.2/Modules/_InputMethodKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-InputMethodKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-InputMethodKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/PKG-INFO` & `pyobjc-framework-InputMethodKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InputMethodKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InputMethodKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InputMethodKit
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkcandidates.py` & `pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkcandidates.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkinputcontroller.py` & `pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkinputcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_imkserver.py` & `pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_imkserver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/PyObjCTest/test_inputmethodkit.py` & `pyobjc-framework-InputMethodKit-9.2/PyObjCTest/test_inputmethodkit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/InputMethodKit.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/InputMethodKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-InputMethodKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-InputMethodKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InputMethodKit-9.1b1/setup.py` & `pyobjc-framework-InputMethodKit-9.2/setup.py`

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
     name="pyobjc-framework-InputMethodKit",
     description="Wrappers for the framework InputMethodKit on macOS",
     min_os_level="10.5",
     packages=["InputMethodKit"],
     ext_modules=[
```

