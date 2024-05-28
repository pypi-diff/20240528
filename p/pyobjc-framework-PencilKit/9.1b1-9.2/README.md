# Comparing `tmp/pyobjc-framework-PencilKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-PencilKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PencilKit-9.1b1.tar", last modified: Sun Mar 26 11:33:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-PencilKit-9.2.tar", last modified: Wed Jun  7 00:23:23 2023, max compression
```

## Comparing `pyobjc-framework-PencilKit-9.1b1.tar` & `pyobjc-framework-PencilKit-9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.306421 pyobjc-framework-PencilKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.267042 pyobjc-framework-PencilKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.271555 pyobjc-framework-PencilKit-9.1b1/Lib/PencilKit/
--rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.1b1/Lib/PencilKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2548 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.1b1/Lib/PencilKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.275141 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2124 2023-03-26 11:33:34.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      964 2023-03-26 11:33:34.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:33:34.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:46.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:33:34.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:33:34.000000 pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PencilKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-03-26 11:33:34.305956 pyobjc-framework-PencilKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.294368 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pencilkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      370 2021-03-21 10:08:23.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pkdrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)      399 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pkerasertool.py
--rw-r--r--   0 ronald     (501) staff       (20)      443 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pkinkttype.py
--rw-r--r--   0 ronald     (501) staff       (20)      703 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pkstrokepath.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.296282 pyobjc-framework-PencilKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      491 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.1b1/metadata/PencilKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:34.304866 pyobjc-framework-PencilKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    24908 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24972 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26087 2022-10-18 09:53:23.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27769 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3182 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24909 2021-03-21 10:08:23.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24909 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24973 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26088 2022-10-18 09:53:23.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27770 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PencilKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:33:34.306540 pyobjc-framework-PencilKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      681 2023-03-25 14:20:32.000000 pyobjc-framework-PencilKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.078903 pyobjc-framework-PencilKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.051565 pyobjc-framework-PencilKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.056541 pyobjc-framework-PencilKit-9.2/Lib/PencilKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.2/Lib/PencilKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2548 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.2/Lib/PencilKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.059729 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-06-07 00:23:23.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      979 2023-06-07 00:23:23.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:23:23.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:46.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:23:23.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:23:23.000000 pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PencilKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-06-07 00:23:23.078529 pyobjc-framework-PencilKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.063367 pyobjc-framework-PencilKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pencilkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      370 2021-03-21 10:08:23.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pkdrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)      399 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pkerasertool.py
+-rw-r--r--   0 ronald     (501) staff       (20)      443 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pkinkttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      703 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pkstrokepath.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.064882 pyobjc-framework-PencilKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      491 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.2/metadata/PencilKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:23.077652 pyobjc-framework-PencilKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    24908 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24972 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26087 2022-10-18 09:53:23.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27769 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3182 2020-11-30 18:45:15.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24909 2021-03-21 10:08:23.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24909 2021-07-30 09:00:38.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24973 2022-02-24 08:47:16.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26088 2022-10-18 09:53:23.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27770 2023-02-19 10:50:35.000000 pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PencilKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PencilKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:23:23.079012 pyobjc-framework-PencilKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      762 2023-05-29 10:07:46.000000 pyobjc-framework-PencilKit-9.2/setup.py
```

### Comparing `pyobjc-framework-PencilKit-9.1b1/Lib/PencilKit/__init__.py` & `pyobjc-framework-PencilKit-9.2/Lib/PencilKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/Lib/PencilKit/_metadata.py` & `pyobjc-framework-PencilKit-9.2/Lib/PencilKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/PKG-INFO` & `pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PencilKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PencilKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PencilKit
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-PencilKit-9.1b1/Lib/pyobjc_framework_PencilKit.egg-info/SOURCES.txt` & `pyobjc-framework-PencilKit-9.2/Lib/pyobjc_framework_PencilKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PencilKit/__init__.py
 Lib/PencilKit/_metadata.py
 Lib/pyobjc_framework_PencilKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_PencilKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PencilKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PencilKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PencilKit-9.1b1/License.txt` & `pyobjc-framework-PencilKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/PKG-INFO` & `pyobjc-framework-PencilKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PencilKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PencilKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PencilKit
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-PencilKit-9.1b1/PyObjCTest/test_pkstrokepath.py` & `pyobjc-framework-PencilKit-9.2/PyObjCTest/test_pkstrokepath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-PencilKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PencilKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PencilKit-9.1b1/setup.py` & `pyobjc-framework-PencilKit-9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "PencilKit" framework on macOS 10.15 and later.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-PencilKit",
     description="Wrappers for the framework PencilKit on macOS",
     min_os_level="10.15",
     packages=["PencilKit"],
     version=VERSION,
```

