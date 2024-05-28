# Comparing `tmp/pyobjc-framework-Speech-9.1b1.tar.gz` & `tmp/pyobjc-framework-Speech-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Speech-9.1b1.tar", last modified: Sun Mar 26 11:41:14 2023, max compression
+gzip compressed data, was "pyobjc-framework-Speech-9.2.tar", last modified: Wed Jun  7 00:29:11 2023, max compression
```

## Comparing `pyobjc-framework-Speech-9.1b1.tar` & `pyobjc-framework-Speech-9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:14.006290 pyobjc-framework-Speech-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.963920 pyobjc-framework-Speech-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.973946 pyobjc-framework-Speech-9.1b1/Lib/Speech/
--rw-r--r--   0 ronald     (501) staff       (20)      691 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/Lib/Speech/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5139 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.1b1/Lib/Speech/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.980006 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2096 2023-03-26 11:41:13.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1058 2023-03-26 11:41:13.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:41:13.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:41.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:41:13.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:41:13.000000 pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Speech-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.983079 pyobjc-framework-Speech-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      799 2021-10-18 19:38:40.000000 pyobjc-framework-Speech-9.1b1/Modules/_Speech.m
--rw-r--r--   0 ronald     (501) staff       (20)      382 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/Modules/_Speech_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Speech-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Speech-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2023-03-26 11:41:14.005702 pyobjc-framework-Speech-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.993111 pyobjc-framework-Speech-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      886 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitionrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitionresult.py
--rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-06-25 20:10:18.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitiontask.py
--rw-r--r--   0 ronald     (501) staff       (20)      532 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitiontaskhint.py
--rw-r--r--   0 ronald     (501) staff       (20)     1441 2022-06-25 09:25:24.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognizer.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Speech-9.1b1/PyObjCTest/test_speech.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:13.994343 pyobjc-framework-Speech-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1040 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/metadata/Speech.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:14.002584 pyobjc-framework-Speech-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    30360 2021-07-30 09:00:38.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30566 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31472 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27261 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27770 2021-03-21 10:08:23.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30361 2021-07-30 09:00:38.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30567 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31473 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Speech-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:41:14.006432 pyobjc-framework-Speech-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1111 2023-03-25 14:20:32.000000 pyobjc-framework-Speech-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.904571 pyobjc-framework-Speech-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.861524 pyobjc-framework-Speech-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.866639 pyobjc-framework-Speech-9.2/Lib/Speech/
+-rw-r--r--   0 ronald     (501) staff       (20)      691 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/Lib/Speech/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5139 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.2/Lib/Speech/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.869999 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-06-07 00:29:11.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1073 2023-06-07 00:29:11.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:29:11.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:41.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:29:11.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:29:11.000000 pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Speech-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.872817 pyobjc-framework-Speech-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2021-10-18 19:38:40.000000 pyobjc-framework-Speech-9.2/Modules/_Speech.m
+-rw-r--r--   0 ronald     (501) staff       (20)      382 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/Modules/_Speech_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Speech-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Speech-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-06-07 00:29:11.904163 pyobjc-framework-Speech-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.882262 pyobjc-framework-Speech-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      886 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitionrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitionresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-06-25 20:10:18.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitiontask.py
+-rw-r--r--   0 ronald     (501) staff       (20)      532 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitiontaskhint.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1441 2022-06-25 09:25:24.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Speech-9.2/PyObjCTest/test_speech.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.883526 pyobjc-framework-Speech-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1040 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/metadata/Speech.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:11.903058 pyobjc-framework-Speech-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    30360 2021-07-30 09:00:38.000000 pyobjc-framework-Speech-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30566 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31472 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27261 2020-11-30 18:45:15.000000 pyobjc-framework-Speech-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27770 2021-03-21 10:08:23.000000 pyobjc-framework-Speech-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30361 2021-07-30 09:00:38.000000 pyobjc-framework-Speech-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30567 2022-02-24 08:47:17.000000 pyobjc-framework-Speech-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31473 2022-06-15 11:57:00.000000 pyobjc-framework-Speech-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Speech-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Speech-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:29:11.904667 pyobjc-framework-Speech-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1182 2023-05-29 10:07:47.000000 pyobjc-framework-Speech-9.2/setup.py
```

### Comparing `pyobjc-framework-Speech-9.1b1/Lib/Speech/__init__.py` & `pyobjc-framework-Speech-9.2/Lib/Speech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/Lib/Speech/_metadata.py` & `pyobjc-framework-Speech-9.2/Lib/Speech/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/PKG-INFO` & `pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Speech
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Speech on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Speech
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-Speech-9.1b1/Lib/pyobjc_framework_Speech.egg-info/SOURCES.txt` & `pyobjc-framework-Speech-9.2/Lib/pyobjc_framework_Speech.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Speech/__init__.py
 Lib/Speech/_metadata.py
 Lib/pyobjc_framework_Speech.egg-info/PKG-INFO
 Lib/pyobjc_framework_Speech.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Speech.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Speech.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Speech-9.1b1/License.txt` & `pyobjc-framework-Speech-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/Modules/_Speech.m` & `pyobjc-framework-Speech-9.2/Modules/_Speech.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Speech-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Speech-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Speech-9.1b1/PKG-INFO` & `pyobjc-framework-Speech-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Speech
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Speech on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Speech
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitionrequest.py` & `pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitionrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitiontask.py` & `pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitiontask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognitiontaskhint.py` & `pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognitiontaskhint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/PyObjCTest/test_sfspeechrecognizer.py` & `pyobjc-framework-Speech-9.2/PyObjCTest/test_sfspeechrecognizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/Speech.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/Speech.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Speech-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Speech-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Speech-9.1b1/setup.py` & `pyobjc-framework-Speech-9.2/setup.py`

 * *Files 9% similar despite different names*

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
     name="pyobjc-framework-Speech",
     description="Wrappers for the framework Speech on macOS",
     min_os_level="10.15",
     packages=["Speech"],
     ext_modules=[
```

