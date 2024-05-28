# Comparing `tmp/pyobjc-framework-ContactsUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-ContactsUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ContactsUI-9.1b1.tar", last modified: Sun Mar 26 11:18:57 2023, max compression
+gzip compressed data, was "pyobjc-framework-ContactsUI-9.2.tar", last modified: Wed Jun  7 00:09:19 2023, max compression
```

## Comparing `pyobjc-framework-ContactsUI-9.1b1.tar` & `pyobjc-framework-ContactsUI-9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.716756 pyobjc-framework-ContactsUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.642492 pyobjc-framework-ContactsUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.647431 pyobjc-framework-ContactsUI-9.1b1/Lib/ContactsUI/
--rw-r--r--   0 ronald     (501) staff       (20)      777 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/ContactsUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1404 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/ContactsUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.650543 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2118 2023-03-26 11:18:57.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      834 2023-03-26 11:18:57.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:18:57.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:37.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       82 2023-03-26 11:18:57.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:18:57.000000 pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ContactsUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.653187 pyobjc-framework-ContactsUI-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      789 2021-10-18 19:38:40.000000 pyobjc-framework-ContactsUI-9.1b1/Modules/_ContactsUI.m
--rw-r--r--   0 ronald     (501) staff       (20)      289 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/Modules/_ContactsUI_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ContactsUI-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ContactsUI-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1907 2023-03-26 11:18:57.715139 pyobjc-framework-ContactsUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.666037 pyobjc-framework-ContactsUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      255 2022-06-25 20:12:16.000000 pyobjc-framework-ContactsUI-9.1b1/PyObjCTest/test_cncontactpickerdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      425 2022-04-12 20:05:08.000000 pyobjc-framework-ContactsUI-9.1b1/PyObjCTest/test_contactsui.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.697039 pyobjc-framework-ContactsUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)       25 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/ContactsUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:57.702768 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     5542 2021-07-30 09:00:37.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5561 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5543 2021-03-21 10:08:22.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5543 2021-07-30 09:00:37.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5562 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ContactsUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:18:57.716889 pyobjc-framework-ContactsUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1225 2023-03-25 14:20:30.000000 pyobjc-framework-ContactsUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:19.004073 pyobjc-framework-ContactsUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.959432 pyobjc-framework-ContactsUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.983937 pyobjc-framework-ContactsUI-9.2/Lib/ContactsUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/Lib/ContactsUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1404 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.2/Lib/ContactsUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.988500 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-06-07 00:09:18.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      849 2023-06-07 00:09:18.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:09:18.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:37.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       76 2023-06-07 00:09:18.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:09:18.000000 pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ContactsUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.992015 pyobjc-framework-ContactsUI-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2021-10-18 19:38:40.000000 pyobjc-framework-ContactsUI-9.2/Modules/_ContactsUI.m
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/Modules/_ContactsUI_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ContactsUI-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ContactsUI-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-06-07 00:09:19.003677 pyobjc-framework-ContactsUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.995181 pyobjc-framework-ContactsUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      255 2022-06-25 20:12:16.000000 pyobjc-framework-ContactsUI-9.2/PyObjCTest/test_cncontactpickerdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      425 2022-04-12 20:05:08.000000 pyobjc-framework-ContactsUI-9.2/PyObjCTest/test_contactsui.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:18.997589 pyobjc-framework-ContactsUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)       25 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/metadata/ContactsUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:14.000000 pyobjc-framework-ContactsUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:19.002742 pyobjc-framework-ContactsUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     5542 2021-07-30 09:00:37.000000 pyobjc-framework-ContactsUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5561 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5543 2021-03-21 10:08:22.000000 pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5543 2021-07-30 09:00:37.000000 pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5562 2022-02-24 08:47:16.000000 pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ContactsUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ContactsUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:09:19.004177 pyobjc-framework-ContactsUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1296 2023-05-29 10:07:45.000000 pyobjc-framework-ContactsUI-9.2/setup.py
```

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Lib/ContactsUI/__init__.py` & `pyobjc-framework-ContactsUI-9.2/Lib/ContactsUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Lib/ContactsUI/_metadata.py` & `pyobjc-framework-ContactsUI-9.2/Lib/ContactsUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/PKG-INFO` & `pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ContactsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ContactsUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ContactsUI
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Lib/pyobjc_framework_ContactsUI.egg-info/SOURCES.txt` & `pyobjc-framework-ContactsUI-9.2/Lib/pyobjc_framework_ContactsUI.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ContactsUI/__init__.py
 Lib/ContactsUI/_metadata.py
 Lib/pyobjc_framework_ContactsUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_ContactsUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ContactsUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ContactsUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ContactsUI-9.1b1/License.txt` & `pyobjc-framework-ContactsUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Modules/_ContactsUI.m` & `pyobjc-framework-ContactsUI-9.2/Modules/_ContactsUI.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ContactsUI-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ContactsUI-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ContactsUI-9.1b1/PKG-INFO` & `pyobjc-framework-ContactsUI-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ContactsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ContactsUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ContactsUI
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-ContactsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ContactsUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ContactsUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ContactsUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ContactsUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ContactsUI-9.1b1/setup.py` & `pyobjc-framework-ContactsUI-9.2/setup.py`

 * *Files 10% similar despite different names*

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
     name="pyobjc-framework-ContactsUI",
     description="Wrappers for the framework ContactsUI on macOS",
     min_os_level="10.11",
     packages=["ContactsUI"],
     ext_modules=[
```

