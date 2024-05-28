# Comparing `tmp/pyobjc-framework-UserNotificationsUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-UserNotificationsUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-UserNotificationsUI-9.1b1.tar", last modified: Sun Mar 26 11:43:18 2023, max compression
+gzip compressed data, was "pyobjc-framework-UserNotificationsUI-9.2.tar", last modified: Wed Jun  7 00:31:04 2023, max compression
```

## Comparing `pyobjc-framework-UserNotificationsUI-9.1b1.tar` & `pyobjc-framework-UserNotificationsUI-9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.956888 pyobjc-framework-UserNotificationsUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.928451 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.933294 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/UserNotificationsUI/
--rw-r--r--   0 ronald     (501) staff       (20)      798 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/UserNotificationsUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2567 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/UserNotificationsUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.936780 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2148 2023-03-26 11:43:18.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      895 2023-03-26 11:43:18.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:18.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:20.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      110 2023-03-26 11:43:18.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       20 2023-03-26 11:43:18.000000 pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-UserNotificationsUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1937 2023-03-26 11:43:18.956566 pyobjc-framework-UserNotificationsUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.948982 pyobjc-framework-UserNotificationsUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2247 2022-06-25 09:27:12.000000 pyobjc-framework-UserNotificationsUI-9.1b1/PyObjCTest/test_unnotificationcontentextension.py
--rw-r--r--   0 ronald     (501) staff       (20)      222 2022-04-11 08:03:15.000000 pyobjc-framework-UserNotificationsUI-9.1b1/PyObjCTest/test_usernotificationsui.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.950586 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      472 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/UserNotificationsUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       54 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:18.955909 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     5770 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5951 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6199 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5771 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5771 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5952 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6200 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-UserNotificationsUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:18.956997 pyobjc-framework-UserNotificationsUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      821 2023-03-25 14:20:32.000000 pyobjc-framework-UserNotificationsUI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.363735 pyobjc-framework-UserNotificationsUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.340074 pyobjc-framework-UserNotificationsUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.345461 pyobjc-framework-UserNotificationsUI-9.2/Lib/UserNotificationsUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/UserNotificationsUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2567 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/UserNotificationsUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.349277 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2146 2023-06-07 00:31:04.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      910 2023-06-07 00:31:04.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:31:04.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:20.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      102 2023-06-07 00:31:04.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       20 2023-06-07 00:31:04.000000 pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-UserNotificationsUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1935 2023-06-07 00:31:04.363376 pyobjc-framework-UserNotificationsUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.351754 pyobjc-framework-UserNotificationsUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2247 2022-06-25 09:27:12.000000 pyobjc-framework-UserNotificationsUI-9.2/PyObjCTest/test_unnotificationcontentextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)      222 2022-04-11 08:03:15.000000 pyobjc-framework-UserNotificationsUI-9.2/PyObjCTest/test_usernotificationsui.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.353131 pyobjc-framework-UserNotificationsUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      472 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/UserNotificationsUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       54 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:04.362734 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     5770 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5951 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6199 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5771 2021-03-21 10:08:23.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5771 2021-07-30 09:00:38.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5952 2022-02-24 08:47:17.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6200 2023-02-19 10:50:37.000000 pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-UserNotificationsUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-UserNotificationsUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:31:04.363839 pyobjc-framework-UserNotificationsUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      903 2023-05-29 10:07:47.000000 pyobjc-framework-UserNotificationsUI-9.2/setup.py
```

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/Lib/UserNotificationsUI/__init__.py` & `pyobjc-framework-UserNotificationsUI-9.2/Lib/UserNotificationsUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/Lib/UserNotificationsUI/_metadata.py` & `pyobjc-framework-UserNotificationsUI-9.2/Lib/UserNotificationsUI/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/PKG-INFO` & `pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-UserNotificationsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework UserNotificationsUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,UserNotificationsUI
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/Lib/pyobjc_framework_UserNotificationsUI.egg-info/SOURCES.txt` & `pyobjc-framework-UserNotificationsUI-9.2/Lib/pyobjc_framework_UserNotificationsUI.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/UserNotificationsUI/__init__.py
 Lib/UserNotificationsUI/_metadata.py
 Lib/pyobjc_framework_UserNotificationsUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_UserNotificationsUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_UserNotificationsUI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_UserNotificationsUI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/License.txt` & `pyobjc-framework-UserNotificationsUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/PKG-INFO` & `pyobjc-framework-UserNotificationsUI-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-UserNotificationsUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework UserNotificationsUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,UserNotificationsUI
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/PyObjCTest/test_unnotificationcontentextension.py` & `pyobjc-framework-UserNotificationsUI-9.2/PyObjCTest/test_unnotificationcontentextension.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-UserNotificationsUI-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-UserNotificationsUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-UserNotificationsUI-9.1b1/setup.py` & `pyobjc-framework-UserNotificationsUI-9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-UserNotificationsUI",
     description="Wrappers for the framework UserNotificationsUI on macOS",
     min_os_level="10.16",
     packages=["UserNotificationsUI"],
     version=VERSION,
```

