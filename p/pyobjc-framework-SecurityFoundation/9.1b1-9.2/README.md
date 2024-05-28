# Comparing `tmp/pyobjc-framework-SecurityFoundation-9.1b1.tar.gz` & `tmp/pyobjc-framework-SecurityFoundation-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SecurityFoundation-9.1b1.tar", last modified: Sun Mar 26 11:39:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-SecurityFoundation-9.2.tar", last modified: Wed Jun  7 00:27:51 2023, max compression
```

## Comparing `pyobjc-framework-SecurityFoundation-9.1b1.tar` & `pyobjc-framework-SecurityFoundation-9.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:34.018910 pyobjc-framework-SecurityFoundation-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:33.981416 pyobjc-framework-SecurityFoundation-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:33.985795 pyobjc-framework-SecurityFoundation-9.1b1/Lib/SecurityFoundation/
--rw-r--r--   0 ronald     (501) staff       (20)      782 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/SecurityFoundation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2629 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/SecurityFoundation/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:33.988764 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2134 2023-03-26 11:39:33.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      840 2023-03-26 11:39:33.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:39:33.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:35.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       82 2023-03-26 11:39:33.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:39:33.000000 pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SecurityFoundation-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1923 2023-03-26 11:39:34.017856 pyobjc-framework-SecurityFoundation-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:33.997688 pyobjc-framework-SecurityFoundation-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/PyObjCTest/test_securityfoundation.py
--rw-r--r--   0 ronald     (501) staff       (20)      919 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityFoundation-9.1b1/PyObjCTest/test_sfauthorization.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:33.999599 pyobjc-framework-SecurityFoundation-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/SecurityFoundation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:34.014646 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)      656 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5311 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      624 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      657 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      657 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5312 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SecurityFoundation-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:39:34.019059 pyobjc-framework-SecurityFoundation-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      747 2023-03-25 14:20:32.000000 pyobjc-framework-SecurityFoundation-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.356129 pyobjc-framework-SecurityFoundation-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.336107 pyobjc-framework-SecurityFoundation-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.340784 pyobjc-framework-SecurityFoundation-9.2/Lib/SecurityFoundation/
+-rw-r--r--   0 ronald     (501) staff       (20)      782 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/SecurityFoundation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2629 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/SecurityFoundation/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.343968 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2132 2023-06-07 00:27:51.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      855 2023-06-07 00:27:51.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:51.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:35.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       76 2023-06-07 00:27:51.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-06-07 00:27:51.000000 pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SecurityFoundation-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1921 2023-06-07 00:27:51.355745 pyobjc-framework-SecurityFoundation-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.345915 pyobjc-framework-SecurityFoundation-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-SecurityFoundation-9.2/PyObjCTest/test_securityfoundation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      919 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityFoundation-9.2/PyObjCTest/test_sfauthorization.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.347566 pyobjc-framework-SecurityFoundation-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/SecurityFoundation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:51.351883 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)      656 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5311 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      624 2020-11-30 18:45:15.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      657 2021-03-21 10:08:23.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      657 2021-07-30 09:00:38.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5312 2022-02-24 08:47:17.000000 pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SecurityFoundation-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SecurityFoundation-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:51.356256 pyobjc-framework-SecurityFoundation-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2023-05-29 10:07:47.000000 pyobjc-framework-SecurityFoundation-9.2/setup.py
```

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/Lib/SecurityFoundation/__init__.py` & `pyobjc-framework-SecurityFoundation-9.2/Lib/SecurityFoundation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/Lib/SecurityFoundation/_metadata.py` & `pyobjc-framework-SecurityFoundation-9.2/Lib/SecurityFoundation/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/PKG-INFO` & `pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SecurityFoundation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SecurityFoundation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SecurityFoundation
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/Lib/pyobjc_framework_SecurityFoundation.egg-info/SOURCES.txt` & `pyobjc-framework-SecurityFoundation-9.2/Lib/pyobjc_framework_SecurityFoundation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SecurityFoundation/__init__.py
 Lib/SecurityFoundation/_metadata.py
 Lib/pyobjc_framework_SecurityFoundation.egg-info/PKG-INFO
 Lib/pyobjc_framework_SecurityFoundation.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SecurityFoundation.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SecurityFoundation.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/License.txt` & `pyobjc-framework-SecurityFoundation-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/PKG-INFO` & `pyobjc-framework-SecurityFoundation-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SecurityFoundation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SecurityFoundation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SecurityFoundation
 Platform: MacOS X
```

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/PyObjCTest/test_sfauthorization.py` & `pyobjc-framework-SecurityFoundation-9.2/PyObjCTest/test_sfauthorization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/SecurityFoundation.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/SecurityFoundation.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SecurityFoundation-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SecurityFoundation-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SecurityFoundation-9.1b1/setup.py` & `pyobjc-framework-SecurityFoundation-9.2/setup.py`

 * *Files 21% similar despite different names*

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
     name="pyobjc-framework-SecurityFoundation",
     description="Wrappers for the framework SecurityFoundation on macOS",
     packages=["SecurityFoundation"],
     version=VERSION,
     install_requires=[
```

