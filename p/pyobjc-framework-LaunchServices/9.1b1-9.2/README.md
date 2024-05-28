# Comparing `tmp/pyobjc-framework-LaunchServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-LaunchServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LaunchServices-9.1b1.tar", last modified: Sun Mar 26 11:28:04 2023, max compression
+gzip compressed data, was "pyobjc-framework-LaunchServices-9.2.tar", last modified: Wed Jun  7 00:18:31 2023, max compression
```

## Comparing `pyobjc-framework-LaunchServices-9.1b1.tar` & `pyobjc-framework-LaunchServices-9.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:04.439201 pyobjc-framework-LaunchServices-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LaunchServices-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:04.419574 pyobjc-framework-LaunchServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:04.423891 pyobjc-framework-LaunchServices-9.1b1/Lib/LaunchServices/
--rw-r--r--   0 ronald     (501) staff       (20)      803 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/LaunchServices/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:04.426734 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     1947 2023-03-26 11:28:04.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      705 2023-03-26 11:28:04.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:04.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:24.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:28:04.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:28:04.000000 pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1736 2023-03-26 11:28:04.438863 pyobjc-framework-LaunchServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:04.434170 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    24107 2021-04-09 10:15:21.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_iconscore.py
--rw-r--r--   0 ronald     (501) staff       (20)     2976 2022-04-11 08:03:15.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_launchservices.py
--rw-r--r--   0 ronald     (501) staff       (20)    17085 2021-04-09 10:15:21.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     6262 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsopen.py
--rw-r--r--   0 ronald     (501) staff       (20)     1250 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsquarantine.py
--rw-r--r--   0 ronald     (501) staff       (20)     7270 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lssharedfilelist.py
--rw-r--r--   0 ronald     (501) staff       (20)     9058 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_utcoretypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     4312 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_uttype.py
--rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-LaunchServices-9.1b1/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LaunchServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:04.439301 pyobjc-framework-LaunchServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      491 2023-03-25 14:20:31.000000 pyobjc-framework-LaunchServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:31.999402 pyobjc-framework-LaunchServices-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LaunchServices-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:31.980415 pyobjc-framework-LaunchServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:31.984807 pyobjc-framework-LaunchServices-9.2/Lib/LaunchServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.2/Lib/LaunchServices/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:31.992324 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     1945 2023-06-07 00:18:31.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      720 2023-06-07 00:18:31.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:31.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:24.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:18:31.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:18:31.000000 pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1734 2023-06-07 00:18:31.999048 pyobjc-framework-LaunchServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:31.998463 pyobjc-framework-LaunchServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24123 2023-05-27 09:46:33.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_iconscore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2976 2022-04-11 08:03:15.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_launchservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17085 2021-04-09 10:15:21.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6262 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsopen.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1250 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsquarantine.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7270 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lssharedfilelist.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9058 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_utcoretypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4312 2021-03-21 10:08:22.000000 pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_uttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-LaunchServices-9.2/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LaunchServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-LaunchServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:31.999508 pyobjc-framework-LaunchServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      573 2023-05-29 10:07:46.000000 pyobjc-framework-LaunchServices-9.2/setup.py
```

### Comparing `pyobjc-framework-LaunchServices-9.1b1/LICENSE.txt` & `pyobjc-framework-LaunchServices-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/Lib/LaunchServices/__init__.py` & `pyobjc-framework-LaunchServices-9.2/Lib/LaunchServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/PKG-INFO` & `pyobjc-framework-LaunchServices-9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LaunchServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LaunchServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LaunchServices
 Platform: MacOS X
@@ -26,17 +26,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Deprecated wrappers for the "LaunchServices" framework on macOS.
 
 Use the "CoreServices" bindings instead.
```

### Comparing `pyobjc-framework-LaunchServices-9.1b1/Lib/pyobjc_framework_LaunchServices.egg-info/SOURCES.txt` & `pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/LaunchServices/__init__.py
 Lib/pyobjc_framework_LaunchServices.egg-info/PKG-INFO
 Lib/pyobjc_framework_LaunchServices.egg-info/SOURCES.txt
 Lib/pyobjc_framework_LaunchServices.egg-info/dependency_links.txt
 Lib/pyobjc_framework_LaunchServices.egg-info/not-zip-safe
 Lib/pyobjc_framework_LaunchServices.egg-info/requires.txt
```

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PKG-INFO` & `pyobjc-framework-LaunchServices-9.2/Lib/pyobjc_framework_LaunchServices.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LaunchServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LaunchServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LaunchServices
 Platform: MacOS X
@@ -26,14 +26,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Deprecated wrappers for the "LaunchServices" framework on macOS.
 
 Use the "CoreServices" bindings instead.
```

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_iconscore.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_iconscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,23 +400,23 @@
             self.assertArgIsOut(LaunchServices.GetIconRefFromFileInfo, 7)
 
             self.assertArgIsOut(LaunchServices.GetIconRefFromTypeInfo, 5)
 
             self.assertArgIsIn(LaunchServices.GetIconRefFromIconFamilyPtr, 0)
             self.assertArgIsOut(LaunchServices.GetIconRefFromIconFamilyPtr, 2)
 
-            self.assertArgIsOut(LaunchServices.GetIconRefFromComponent, 1)
+            # self.assertArgIsOut(LaunchServices.GetIconRefFromComponent, 1)
 
             # XXX: Untested for now...
-            LaunchServices.RegisterIconRefFromIconFamily
-            LaunchServices.RegisterIconRefFromFSRef
-            LaunchServices.UnregisterIconRef
-            LaunchServices.UpdateIconRef
-            LaunchServices.OverrideIconRef
-            LaunchServices.RemoveIconRefOverride
+            # LaunchServices.RegisterIconRefFromIconFamily
+            # LaunchServices.RegisterIconRefFromFSRef
+            # LaunchServices.UnregisterIconRef
+            # LaunchServices.UpdateIconRef
+            # LaunchServices.OverrideIconRef
+            # LaunchServices.RemoveIconRefOverride
 
             self.assertArgIsOut(LaunchServices.CompositeIconRef, 2)
 
             self.assertArgIsOut(LaunchServices.IsIconRefComposite, 1)
             self.assertArgIsOut(LaunchServices.IsIconRefComposite, 2)
 
             self.assertResultIsBOOL(LaunchServices.IsValidIconRef)
@@ -427,15 +427,15 @@
             self.assertArgHasType(
                 LaunchServices.GetCustomIconsEnabled,
                 1,
                 objc._C_OUT + objc._C_PTR + objc._C_NSBOOL,
             )
 
             # Untested...
-            LaunchServices.ReadIconFromFSRef
+            # LaunchServices.ReadIconFromFSRef
 
         finally:
             err = LaunchServices.ReleaseIconRef(icon)
             self.assertEqual(err, 0)
 
     def testOpaque(self):
         self.assertIsOpaquePointer(LaunchServices.IconRef)
```

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_launchservices.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_launchservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsinfo.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsopen.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsopen.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lsquarantine.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lsquarantine.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_lssharedfilelist.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_lssharedfilelist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_utcoretypes.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_utcoretypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/PyObjCTest/test_uttype.py` & `pyobjc-framework-LaunchServices-9.2/PyObjCTest/test_uttype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LaunchServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-LaunchServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

