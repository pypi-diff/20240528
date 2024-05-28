# Comparing `tmp/pyobjc-framework-PubSub-9.1b1.tar.gz` & `tmp/pyobjc-framework-PubSub-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PubSub-9.1b1.tar", last modified: Sun Mar 26 11:34:31 2023, max compression
+gzip compressed data, was "pyobjc-framework-PubSub-9.2.tar", last modified: Wed Jun  7 00:24:06 2023, max compression
```

## Comparing `pyobjc-framework-PubSub-9.1b1.tar` & `pyobjc-framework-PubSub-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.334381 pyobjc-framework-PubSub-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PubSub-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.303297 pyobjc-framework-PubSub-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.309042 pyobjc-framework-PubSub-9.1b1/Lib/PubSub/
--rw-r--r--   0 ronald     (501) staff       (20)      673 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/Lib/PubSub/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4793 2022-02-24 08:47:16.000000 pyobjc-framework-PubSub-9.1b1/Lib/PubSub/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.314149 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2088 2023-03-26 11:34:31.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      772 2023-03-26 11:34:31.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:34:31.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:05.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:34:31.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:34:31.000000 pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2088 2023-03-26 11:34:31.332861 pyobjc-framework-PubSub-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.322620 pyobjc-framework-PubSub-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      357 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psclient.py
--rw-r--r--   0 ronald     (501) staff       (20)      748 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psenclosure.py
--rw-r--r--   0 ronald     (501) staff       (20)      405 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psentry.py
--rw-r--r--   0 ronald     (501) staff       (20)     1126 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psfeed.py
--rw-r--r--   0 ronald     (501) staff       (20)      728 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psfeedsettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      521 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_pslink.py
--rw-r--r--   0 ronald     (501) staff       (20)      721 2022-04-11 08:03:15.000000 pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_pubsub.py
--rw-r--r--   0 ronald     (501) staff       (20)      283 2021-10-18 19:38:40.000000 pyobjc-framework-PubSub-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.327905 pyobjc-framework-PubSub-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3153 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/metadata/PubSub.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:31.331183 pyobjc-framework-PubSub-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    27837 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27837 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    27905 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PubSub-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:34:31.334571 pyobjc-framework-PubSub-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      846 2023-03-25 14:20:32.000000 pyobjc-framework-PubSub-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.424737 pyobjc-framework-PubSub-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PubSub-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.401835 pyobjc-framework-PubSub-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.407988 pyobjc-framework-PubSub-9.2/Lib/PubSub/
+-rw-r--r--   0 ronald     (501) staff       (20)      673 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/Lib/PubSub/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4793 2022-02-24 08:47:16.000000 pyobjc-framework-PubSub-9.2/Lib/PubSub/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.411094 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2086 2023-06-07 00:24:06.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      787 2023-06-07 00:24:06.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:24:06.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:05.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:24:06.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:24:06.000000 pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2086 2023-06-07 00:24:06.424358 pyobjc-framework-PubSub-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.416322 pyobjc-framework-PubSub-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      357 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_psclient.py
+-rw-r--r--   0 ronald     (501) staff       (20)      748 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_psenclosure.py
+-rw-r--r--   0 ronald     (501) staff       (20)      405 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_psentry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1126 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_psfeed.py
+-rw-r--r--   0 ronald     (501) staff       (20)      728 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_psfeedsettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      521 2021-03-21 10:08:23.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_pslink.py
+-rw-r--r--   0 ronald     (501) staff       (20)      721 2022-04-11 08:03:15.000000 pyobjc-framework-PubSub-9.2/PyObjCTest/test_pubsub.py
+-rw-r--r--   0 ronald     (501) staff       (20)      283 2021-10-18 19:38:40.000000 pyobjc-framework-PubSub-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.417631 pyobjc-framework-PubSub-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3153 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/metadata/PubSub.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:06.423441 pyobjc-framework-PubSub-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    27837 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27837 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    27905 2020-11-30 18:45:15.000000 pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PubSub-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PubSub-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:24:06.424853 pyobjc-framework-PubSub-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      928 2023-05-29 10:07:47.000000 pyobjc-framework-PubSub-9.2/setup.py
```

### Comparing `pyobjc-framework-PubSub-9.1b1/LICENSE.txt` & `pyobjc-framework-PubSub-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/Lib/PubSub/__init__.py` & `pyobjc-framework-PubSub-9.2/Lib/PubSub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/Lib/PubSub/_metadata.py` & `pyobjc-framework-PubSub-9.2/Lib/PubSub/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/PKG-INFO` & `pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PubSub
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PubSub on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PubSub
 Platform: MacOS X (>=10.5, <=10.14)
```

### Comparing `pyobjc-framework-PubSub-9.1b1/Lib/pyobjc_framework_PubSub.egg-info/SOURCES.txt` & `pyobjc-framework-PubSub-9.2/Lib/pyobjc_framework_PubSub.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/PubSub/__init__.py
 Lib/PubSub/_metadata.py
 Lib/pyobjc_framework_PubSub.egg-info/PKG-INFO
 Lib/pyobjc_framework_PubSub.egg-info/SOURCES.txt
 Lib/pyobjc_framework_PubSub.egg-info/dependency_links.txt
 Lib/pyobjc_framework_PubSub.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-PubSub-9.1b1/PKG-INFO` & `pyobjc-framework-PubSub-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PubSub
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PubSub on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PubSub
 Platform: MacOS X (>=10.5, <=10.14)
```

### Comparing `pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psenclosure.py` & `pyobjc-framework-PubSub-9.2/PyObjCTest/test_psenclosure.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psfeed.py` & `pyobjc-framework-PubSub-9.2/PyObjCTest/test_psfeed.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_psfeedsettings.py` & `pyobjc-framework-PubSub-9.2/PyObjCTest/test_psfeedsettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_pslink.py` & `pyobjc-framework-PubSub-9.2/PyObjCTest/test_pslink.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/PyObjCTest/test_pubsub.py` & `pyobjc-framework-PubSub-9.2/PyObjCTest/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/metadata/PubSub.fwinfo` & `pyobjc-framework-PubSub-9.2/metadata/PubSub.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-PubSub-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PubSub-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PubSub-9.1b1/setup.py` & `pyobjc-framework-PubSub-9.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 
 Note that this framework is deprecated in OSX 10.9
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
     name="pyobjc-framework-PubSub",
     description="Wrappers for the framework PubSub on macOS",
     min_os_level="10.5",
     max_os_level="10.14",
     packages=["PubSub"],
```

