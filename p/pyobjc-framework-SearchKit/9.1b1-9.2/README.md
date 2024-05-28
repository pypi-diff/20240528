# Comparing `tmp/pyobjc-framework-SearchKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-SearchKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SearchKit-9.1b1.tar", last modified: Sun Mar 26 11:39:07 2023, max compression
+gzip compressed data, was "pyobjc-framework-SearchKit-9.2.tar", last modified: Wed Jun  7 00:27:31 2023, max compression
```

## Comparing `pyobjc-framework-SearchKit-9.1b1.tar` & `pyobjc-framework-SearchKit-9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.455477 pyobjc-framework-SearchKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.367565 pyobjc-framework-SearchKit-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.398512 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/
--rw-r--r--   0 ronald     (501) staff       (20)    11911 2023-03-03 17:21:59.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/AppController.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.367805 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.407043 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      751 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    17116 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     8387 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      191 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SearchKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.368140 pyobjc-framework-SearchKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.407594 pyobjc-framework-SearchKit-9.1b1/Lib/SearchKit/
--rw-r--r--   0 ronald     (501) staff       (20)      793 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/Lib/SearchKit/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.411636 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     1933 2023-03-26 11:39:07.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      879 2023-03-26 11:39:07.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:39:07.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:33.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:39:07.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:39:07.000000 pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1722 2023-03-26 11:39:07.416722 pyobjc-framework-SearchKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:07.415222 pyobjc-framework-SearchKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1653 2022-04-11 08:03:15.000000 pyobjc-framework-SearchKit-9.1b1/PyObjCTest/test_searchkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-SearchKit-9.1b1/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SearchKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:39:07.505776 pyobjc-framework-SearchKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      493 2023-03-25 14:20:32.000000 pyobjc-framework-SearchKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.906525 pyobjc-framework-SearchKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.883655 pyobjc-framework-SearchKit-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.894769 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/
+-rw-r--r--   0 ronald     (501) staff       (20)    11911 2023-03-03 17:21:59.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/AppController.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.884947 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.899534 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      751 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    17116 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     8387 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      191 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SearchKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.886412 pyobjc-framework-SearchKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.900307 pyobjc-framework-SearchKit-9.2/Lib/SearchKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      793 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/Lib/SearchKit/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.903816 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     1931 2023-06-07 00:27:31.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      894 2023-06-07 00:27:31.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:31.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:33.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:27:31.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:27:31.000000 pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1720 2023-06-07 00:27:31.906030 pyobjc-framework-SearchKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:31.905118 pyobjc-framework-SearchKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SearchKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1653 2022-04-11 08:03:15.000000 pyobjc-framework-SearchKit-9.2/PyObjCTest/test_searchkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-SearchKit-9.2/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SearchKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SearchKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:31.906640 pyobjc-framework-SearchKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      575 2023-05-29 10:07:47.000000 pyobjc-framework-SearchKit-9.2/setup.py
```

### Comparing `pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/AppController.py` & `pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/AppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Examples/SearchKitExample1/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-SearchKit-9.2/Examples/SearchKitExample1/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/LICENSE.txt` & `pyobjc-framework-SearchKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Lib/SearchKit/__init__.py` & `pyobjc-framework-SearchKit-9.2/Lib/SearchKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/PKG-INFO` & `pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SearchKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SearchKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SearchKit
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-SearchKit-9.1b1/Lib/pyobjc_framework_SearchKit.egg-info/SOURCES.txt` & `pyobjc-framework-SearchKit-9.2/Lib/pyobjc_framework_SearchKit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/SearchKitExample1/AppController.py
 Examples/SearchKitExample1/main.py
 Examples/SearchKitExample1/setup.py
 Examples/SearchKitExample1/summary.txt
 Examples/SearchKitExample1/English.lproj/MainMenu.nib/classes.nib
 Examples/SearchKitExample1/English.lproj/MainMenu.nib/info.nib
```

### Comparing `pyobjc-framework-SearchKit-9.1b1/PKG-INFO` & `pyobjc-framework-SearchKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SearchKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SearchKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SearchKit
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-SearchKit-9.1b1/PyObjCTest/test_searchkit.py` & `pyobjc-framework-SearchKit-9.2/PyObjCTest/test_searchkit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SearchKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SearchKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

