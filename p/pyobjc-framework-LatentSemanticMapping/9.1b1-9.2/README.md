# Comparing `tmp/pyobjc-framework-LatentSemanticMapping-9.1b1.tar.gz` & `tmp/pyobjc-framework-LatentSemanticMapping-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LatentSemanticMapping-9.1b1.tar", last modified: Sun Mar 26 11:28:00 2023, max compression
+gzip compressed data, was "pyobjc-framework-LatentSemanticMapping-9.2.tar", last modified: Wed Jun  7 00:18:26 2023, max compression
```

## Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1.tar` & `pyobjc-framework-LatentSemanticMapping-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:00.019619 pyobjc-framework-LatentSemanticMapping-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:59.987173 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:59.992379 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/LatentSemanticMapping/
--rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/LatentSemanticMapping/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4139 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/LatentSemanticMapping/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:00.000654 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2466 2023-03-26 11:27:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      942 2023-03-26 11:27:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:24.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:27:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       22 2023-03-26 11:27:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2255 2023-03-26 11:28:00.019272 pyobjc-framework-LatentSemanticMapping-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:00.005480 pyobjc-framework-LatentSemanticMapping-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    10273 2022-04-11 08:03:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/PyObjCTest/test_latentsemanticmapping.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-10-18 19:38:40.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:00.011216 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2973 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/LatentSemanticMapping.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:00.018549 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10128 2021-07-30 09:00:38.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10147 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10004 2021-03-21 10:08:22.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10129 2021-03-21 10:08:22.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9931 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9960 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10028 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10129 2021-07-30 09:00:38.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10148 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:00.019717 pyobjc-framework-LatentSemanticMapping-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      996 2023-03-25 14:20:31.000000 pyobjc-framework-LatentSemanticMapping-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.970612 pyobjc-framework-LatentSemanticMapping-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LatentSemanticMapping-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.947742 pyobjc-framework-LatentSemanticMapping-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.953724 pyobjc-framework-LatentSemanticMapping-9.2/Lib/LatentSemanticMapping/
+-rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/LatentSemanticMapping/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4139 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/LatentSemanticMapping/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.956932 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2464 2023-06-07 00:18:26.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      957 2023-06-07 00:18:26.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:26.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:24.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:18:26.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       22 2023-06-07 00:18:26.000000 pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2253 2023-06-07 00:18:26.970254 pyobjc-framework-LatentSemanticMapping-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.958094 pyobjc-framework-LatentSemanticMapping-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10273 2022-04-11 08:03:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/PyObjCTest/test_latentsemanticmapping.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-10-18 19:38:40.000000 pyobjc-framework-LatentSemanticMapping-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.963104 pyobjc-framework-LatentSemanticMapping-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2973 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/LatentSemanticMapping.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       58 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:26.969594 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10128 2021-07-30 09:00:38.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10147 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10004 2021-03-21 10:08:22.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10129 2021-03-21 10:08:22.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9931 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9960 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10028 2020-11-30 18:45:15.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10129 2021-07-30 09:00:38.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10148 2022-02-24 08:47:16.000000 pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LatentSemanticMapping-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-LatentSemanticMapping-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:26.970914 pyobjc-framework-LatentSemanticMapping-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1078 2023-05-29 10:07:46.000000 pyobjc-framework-LatentSemanticMapping-9.2/setup.py
```

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/LICENSE.txt` & `pyobjc-framework-LatentSemanticMapping-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/LatentSemanticMapping/__init__.py` & `pyobjc-framework-LatentSemanticMapping-9.2/Lib/LatentSemanticMapping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/LatentSemanticMapping/_metadata.py` & `pyobjc-framework-LatentSemanticMapping-9.2/Lib/LatentSemanticMapping/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/PKG-INFO` & `pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LatentSemanticMapping
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LatentSemanticMapping on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LatentSemanticMapping
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/SOURCES.txt` & `pyobjc-framework-LatentSemanticMapping-9.2/Lib/pyobjc_framework_LatentSemanticMapping.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/LatentSemanticMapping/__init__.py
 Lib/LatentSemanticMapping/_metadata.py
 Lib/pyobjc_framework_LatentSemanticMapping.egg-info/PKG-INFO
 Lib/pyobjc_framework_LatentSemanticMapping.egg-info/SOURCES.txt
 Lib/pyobjc_framework_LatentSemanticMapping.egg-info/dependency_links.txt
 Lib/pyobjc_framework_LatentSemanticMapping.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/PKG-INFO` & `pyobjc-framework-LatentSemanticMapping-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LatentSemanticMapping
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LatentSemanticMapping on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LatentSemanticMapping
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/PyObjCTest/test_latentsemanticmapping.py` & `pyobjc-framework-LatentSemanticMapping-9.2/PyObjCTest/test_latentsemanticmapping.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/LatentSemanticMapping.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/LatentSemanticMapping.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-LatentSemanticMapping-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/pyobjc_setup.py` & `pyobjc-framework-LatentSemanticMapping-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LatentSemanticMapping-9.1b1/setup.py` & `pyobjc-framework-LatentSemanticMapping-9.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks.
 
 NOTE: Apple's documentation for this framework is very minimal at the moment,
 making it very hard to actually use the framework.
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
     name="pyobjc-framework-LatentSemanticMapping",
     description="Wrappers for the framework LatentSemanticMapping on macOS",
     min_os_level="10.5",
     packages=["LatentSemanticMapping"],
     version=VERSION,
```

