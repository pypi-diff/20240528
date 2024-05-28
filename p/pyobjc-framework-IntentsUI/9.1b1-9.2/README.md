# Comparing `tmp/pyobjc-framework-IntentsUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-IntentsUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-IntentsUI-9.1b1.tar", last modified: Sun Mar 26 11:27:42 2023, max compression
+gzip compressed data, was "pyobjc-framework-IntentsUI-9.2.tar", last modified: Wed Jun  7 00:18:06 2023, max compression
```

## Comparing `pyobjc-framework-IntentsUI-9.1b1.tar` & `pyobjc-framework-IntentsUI-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.806876 pyobjc-framework-IntentsUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.773420 pyobjc-framework-IntentsUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.783641 pyobjc-framework-IntentsUI-9.1b1/Lib/IntentsUI/
--rw-r--r--   0 ronald     (501) staff       (20)      712 2021-09-09 08:49:25.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/IntentsUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4611 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/IntentsUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.793944 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-03-26 11:27:42.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      901 2023-03-26 11:27:42.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:42.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:21.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       51 2023-03-26 11:27:42.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:27:42.000000 pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-IntentsUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.797042 pyobjc-framework-IntentsUI-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      818 2021-10-18 19:38:40.000000 pyobjc-framework-IntentsUI-9.1b1/Modules/_IntentsUI.m
--rw-r--r--   0 ronald     (501) staff       (20)      515 2021-09-06 11:04:10.000000 pyobjc-framework-IntentsUI-9.1b1/Modules/_IntentsUI_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-IntentsUI-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-IntentsUI-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-03-26 11:27:42.806517 pyobjc-framework-IntentsUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.800870 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      402 2022-04-11 08:03:15.000000 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/test_intentsui.py
--rw-r--r--   0 ronald     (501) staff       (20)      835 2022-06-25 20:17:22.000000 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/test_inuiaddvoiceshortcutbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)      244 2022-06-25 20:14:13.000000 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/test_inuiaddvoiceshortcutviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      246 2022-06-25 20:08:37.000000 pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/test_inuieditvoiceshortcutviewcontroller.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.802366 pyobjc-framework-IntentsUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-09-09 08:49:25.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/IntentsUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:42.805855 pyobjc-framework-IntentsUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16606 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11826 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16607 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11827 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IntentsUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:42.806981 pyobjc-framework-IntentsUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1101 2023-03-25 14:20:31.000000 pyobjc-framework-IntentsUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.798142 pyobjc-framework-IntentsUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.758765 pyobjc-framework-IntentsUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.764035 pyobjc-framework-IntentsUI-9.2/Lib/IntentsUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      712 2021-09-09 08:49:25.000000 pyobjc-framework-IntentsUI-9.2/Lib/IntentsUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4611 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.2/Lib/IntentsUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.767216 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2103 2023-06-07 00:18:06.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      916 2023-06-07 00:18:06.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:06.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:21.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       47 2023-06-07 00:18:06.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:18:06.000000 pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-IntentsUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.773565 pyobjc-framework-IntentsUI-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      818 2021-10-18 19:38:40.000000 pyobjc-framework-IntentsUI-9.2/Modules/_IntentsUI.m
+-rw-r--r--   0 ronald     (501) staff       (20)      515 2021-09-06 11:04:10.000000 pyobjc-framework-IntentsUI-9.2/Modules/_IntentsUI_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-IntentsUI-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-IntentsUI-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1892 2023-06-07 00:18:06.797718 pyobjc-framework-IntentsUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.789583 pyobjc-framework-IntentsUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      402 2022-04-11 08:03:15.000000 pyobjc-framework-IntentsUI-9.2/PyObjCTest/test_intentsui.py
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2022-06-25 20:17:22.000000 pyobjc-framework-IntentsUI-9.2/PyObjCTest/test_inuiaddvoiceshortcutbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)      244 2022-06-25 20:14:13.000000 pyobjc-framework-IntentsUI-9.2/PyObjCTest/test_inuiaddvoiceshortcutviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      246 2022-06-25 20:08:37.000000 pyobjc-framework-IntentsUI-9.2/PyObjCTest/test_inuieditvoiceshortcutviewcontroller.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.791897 pyobjc-framework-IntentsUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-09-09 08:49:25.000000 pyobjc-framework-IntentsUI-9.2/metadata/IntentsUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:06.796684 pyobjc-framework-IntentsUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16606 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11826 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16607 2021-07-30 09:00:38.000000 pyobjc-framework-IntentsUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11827 2022-02-24 08:47:16.000000 pyobjc-framework-IntentsUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IntentsUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-IntentsUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:06.798236 pyobjc-framework-IntentsUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1187 2023-05-29 10:07:46.000000 pyobjc-framework-IntentsUI-9.2/setup.py
```

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Lib/IntentsUI/__init__.py` & `pyobjc-framework-IntentsUI-9.2/Lib/IntentsUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Lib/IntentsUI/_metadata.py` & `pyobjc-framework-IntentsUI-9.2/Lib/IntentsUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/PKG-INFO` & `pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IntentsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Intents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IntentsUI
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Lib/pyobjc_framework_IntentsUI.egg-info/SOURCES.txt` & `pyobjc-framework-IntentsUI-9.2/Lib/pyobjc_framework_IntentsUI.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/IntentsUI/__init__.py
 Lib/IntentsUI/_metadata.py
 Lib/pyobjc_framework_IntentsUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_IntentsUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_IntentsUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_IntentsUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-IntentsUI-9.1b1/License.txt` & `pyobjc-framework-IntentsUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Modules/_IntentsUI.m` & `pyobjc-framework-IntentsUI-9.2/Modules/_IntentsUI.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Modules/_IntentsUI_protocols.m` & `pyobjc-framework-IntentsUI-9.2/Modules/_IntentsUI_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-IntentsUI-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-IntentsUI-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-IntentsUI-9.1b1/PKG-INFO` & `pyobjc-framework-IntentsUI-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IntentsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Intents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IntentsUI
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-IntentsUI-9.1b1/PyObjCTest/test_inuiaddvoiceshortcutbutton.py` & `pyobjc-framework-IntentsUI-9.2/PyObjCTest/test_inuiaddvoiceshortcutbutton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-IntentsUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-IntentsUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-IntentsUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-IntentsUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-IntentsUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IntentsUI-9.1b1/setup.py` & `pyobjc-framework-IntentsUI-9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
-from pyobjc_setup import setup, Extension
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup, Extension  # noqa: E402  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-IntentsUI",
     description="Wrappers for the framework Intents on macOS",
     min_os_level="12.0",
     packages=["IntentsUI"],
     ext_modules=[
```

