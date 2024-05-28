# Comparing `tmp/pyobjc-framework-ExceptionHandling-9.1b1.tar.gz` & `tmp/pyobjc-framework-ExceptionHandling-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ExceptionHandling-9.1b1.tar", last modified: Sun Mar 26 11:23:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-ExceptionHandling-9.2.tar", last modified: Wed Jun  7 00:13:48 2023, max compression
```

## Comparing `pyobjc-framework-ExceptionHandling-9.1b1.tar` & `pyobjc-framework-ExceptionHandling-9.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.890915 pyobjc-framework-ExceptionHandling-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.872173 pyobjc-framework-ExceptionHandling-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)      851 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/Examples/debugging.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExceptionHandling-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.867603 pyobjc-framework-ExceptionHandling-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.873399 pyobjc-framework-ExceptionHandling-9.1b1/Lib/ExceptionHandling/
--rw-r--r--   0 ronald     (501) staff       (20)      750 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/ExceptionHandling/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2754 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/ExceptionHandling/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.873887 pyobjc-framework-ExceptionHandling-9.1b1/Lib/PyObjCTools/
--rw-r--r--   0 ronald     (501) staff       (20)     6164 2021-10-18 19:38:40.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/PyObjCTools/Debugging.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.876870 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2416 2023-03-26 11:23:41.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      987 2023-03-26 11:23:41.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:41.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:03.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:41.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       30 2023-03-26 11:23:41.000000 pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2205 2023-03-26 11:23:41.890214 pyobjc-framework-ExceptionHandling-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.883136 pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3858 2021-03-21 10:08:22.000000 pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_debugging.py
--rw-r--r--   0 ronald     (501) staff       (20)      525 2022-04-11 08:03:15.000000 pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_exceptionhandling.py
--rw-r--r--   0 ronald     (501) staff       (20)     3928 2021-03-21 10:08:22.000000 pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_nsexceptionhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      294 2021-10-18 19:38:40.000000 pyobjc-framework-ExceptionHandling-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.884398 pyobjc-framework-ExceptionHandling-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/ExceptionHandling.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:41.889479 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     6225 2021-07-30 09:00:37.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6244 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6226 2021-03-21 10:08:22.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6050 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6050 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6118 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6226 2021-07-30 09:00:37.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6245 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExceptionHandling-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:41.891033 pyobjc-framework-ExceptionHandling-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      945 2023-03-25 14:20:31.000000 pyobjc-framework-ExceptionHandling-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.891167 pyobjc-framework-ExceptionHandling-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.851461 pyobjc-framework-ExceptionHandling-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)      851 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/Examples/debugging.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ExceptionHandling-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.845777 pyobjc-framework-ExceptionHandling-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.852634 pyobjc-framework-ExceptionHandling-9.2/Lib/ExceptionHandling/
+-rw-r--r--   0 ronald     (501) staff       (20)      750 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/ExceptionHandling/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2754 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/ExceptionHandling/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.853220 pyobjc-framework-ExceptionHandling-9.2/Lib/PyObjCTools/
+-rw-r--r--   0 ronald     (501) staff       (20)     6164 2021-10-18 19:38:40.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/PyObjCTools/Debugging.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.856977 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2414 2023-06-07 00:13:48.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1002 2023-06-07 00:13:48.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:48.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:03.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:48.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2023-06-07 00:13:48.000000 pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2203 2023-06-07 00:13:48.890412 pyobjc-framework-ExceptionHandling-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.864847 pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4009 2023-05-04 11:00:07.000000 pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_debugging.py
+-rw-r--r--   0 ronald     (501) staff       (20)      525 2022-04-11 08:03:15.000000 pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_exceptionhandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3928 2021-03-21 10:08:22.000000 pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_nsexceptionhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2021-10-18 19:38:40.000000 pyobjc-framework-ExceptionHandling-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.866254 pyobjc-framework-ExceptionHandling-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/ExceptionHandling.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:48.889201 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     6225 2021-07-30 09:00:37.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6244 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6226 2021-03-21 10:08:22.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6050 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6050 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6118 2020-11-30 18:45:14.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6226 2021-07-30 09:00:37.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6245 2022-02-24 08:47:16.000000 pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ExceptionHandling-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ExceptionHandling-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:48.891277 pyobjc-framework-ExceptionHandling-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1027 2023-05-29 10:07:46.000000 pyobjc-framework-ExceptionHandling-9.2/setup.py
```

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Examples/debugging.py` & `pyobjc-framework-ExceptionHandling-9.2/Examples/debugging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/LICENSE.txt` & `pyobjc-framework-ExceptionHandling-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Lib/ExceptionHandling/__init__.py` & `pyobjc-framework-ExceptionHandling-9.2/Lib/ExceptionHandling/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Lib/ExceptionHandling/_metadata.py` & `pyobjc-framework-ExceptionHandling-9.2/Lib/ExceptionHandling/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Lib/PyObjCTools/Debugging.py` & `pyobjc-framework-ExceptionHandling-9.2/Lib/PyObjCTools/Debugging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/PKG-INFO` & `pyobjc-framework-ExceptionHandling-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExceptionHandling
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExceptionHandling on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExceptionHandling
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
 
 
 Wrappers for the "ExceptionHandling" framework on macOS. The ExceptionHandling
 framework provides facilities for monitoring and debugging exceptional
 conditions in Cocoa programs.
 
 PyObjC also provides low-level debugging utilities beyond the core
```

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/Lib/pyobjc_framework_ExceptionHandling.egg-info/SOURCES.txt` & `pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/debugging.py
 Lib/ExceptionHandling/__init__.py
 Lib/ExceptionHandling/_metadata.py
 Lib/PyObjCTools/Debugging.py
 Lib/pyobjc_framework_ExceptionHandling.egg-info/PKG-INFO
 Lib/pyobjc_framework_ExceptionHandling.egg-info/SOURCES.txt
```

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/PKG-INFO` & `pyobjc-framework-ExceptionHandling-9.2/Lib/pyobjc_framework_ExceptionHandling.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ExceptionHandling
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ExceptionHandling on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ExceptionHandling
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
 
 
 Wrappers for the "ExceptionHandling" framework on macOS. The ExceptionHandling
 framework provides facilities for monitoring and debugging exceptional
 conditions in Cocoa programs.
 
 PyObjC also provides low-level debugging utilities beyond the core
```

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_debugging.py` & `pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_debugging.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,20 @@
 
         except Exception as exc:
             self.assertTrue(Debugging.isPythonException(exc))
 
     @expectedFailureIf(sys.byteorder == "big")
     def testAtos(self):
         NSThread = objc.lookUpClass("NSThread")
-        v = " ".join(hex(x) for x in NSThread.callStackReturnAddresses())
+        NSArray = objc.lookUpClass("NSArray")
+
+        # The intermediate NSArray is necessary on 10.11
+        v = " ".join(
+            hex(x) for x in NSArray.arrayWithArray_(NSThread.callStackReturnAddresses())
+        )
         fp = Debugging._run_atos(v)
         value = fp.read()
         fp.close()
 
         self.assertTrue(any(x in value for x in {"_objc.", "ffi_call_unix64"}))
 
     def testInstallExceptionHandler(self):
```

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_exceptionhandling.py` & `pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_exceptionhandling.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/PyObjCTest/test_nsexceptionhandler.py` & `pyobjc-framework-ExceptionHandling-9.2/PyObjCTest/test_nsexceptionhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/ExceptionHandling.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/ExceptionHandling.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ExceptionHandling-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ExceptionHandling-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ExceptionHandling-9.1b1/setup.py` & `pyobjc-framework-ExceptionHandling-9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 ExceptionHandling framework in the module ``PyObjCTools.Debugging``.
 
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
     name="pyobjc-framework-ExceptionHandling",
     description="Wrappers for the framework ExceptionHandling on macOS",
     packages=["PyObjCTools", "ExceptionHandling"],
     version=VERSION,
     install_requires=["pyobjc-core>=" + VERSION, "pyobjc-framework-Cocoa>=" + VERSION],
```

