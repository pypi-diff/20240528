# Comparing `tmp/pyobjc-framework-Accounts-9.1b1.tar.gz` & `tmp/pyobjc-framework-Accounts-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Accounts-9.1b1.tar", last modified: Sun Mar 26 11:13:32 2023, max compression
+gzip compressed data, was "pyobjc-framework-Accounts-9.2.tar", last modified: Wed Jun  7 00:05:23 2023, max compression
```

## Comparing `pyobjc-framework-Accounts-9.1b1.tar` & `pyobjc-framework-Accounts-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.988942 pyobjc-framework-Accounts-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.960472 pyobjc-framework-Accounts-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)      666 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/Examples/demo.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Accounts-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.955239 pyobjc-framework-Accounts-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.961589 pyobjc-framework-Accounts-9.1b1/Lib/Accounts/
--rw-r--r--   0 ronald     (501) staff       (20)      688 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/Lib/Accounts/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4840 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.1b1/Lib/Accounts/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.964901 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2129 2023-03-26 11:13:32.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      859 2023-03-26 11:13:32.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:13:32.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:14.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:13:32.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:13:32.000000 pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1918 2023-03-26 11:13:32.988321 pyobjc-framework-Accounts-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.968636 pyobjc-framework-Accounts-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1662 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acaccountstore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1279 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acaccounttype.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_accounts.py
--rw-r--r--   0 ronald     (501) staff       (20)     1829 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-Accounts-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.970323 pyobjc-framework-Accounts-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2369 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/metadata/Accounts.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:32.986694 pyobjc-framework-Accounts-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    14012 2021-07-30 09:00:37.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14136 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    12847 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14013 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7793 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14013 2021-07-30 09:00:37.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14137 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Accounts-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:13:32.989081 pyobjc-framework-Accounts-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      660 2023-03-25 14:20:30.000000 pyobjc-framework-Accounts-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.557315 pyobjc-framework-Accounts-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.524097 pyobjc-framework-Accounts-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)      666 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/Examples/demo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Accounts-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.517659 pyobjc-framework-Accounts-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.525349 pyobjc-framework-Accounts-9.2/Lib/Accounts/
+-rw-r--r--   0 ronald     (501) staff       (20)      688 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/Lib/Accounts/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4840 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.2/Lib/Accounts/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.528967 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2127 2023-06-07 00:05:23.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      874 2023-06-07 00:05:23.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:23.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:14.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:23.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:05:23.000000 pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1916 2023-06-07 00:05:23.556789 pyobjc-framework-Accounts-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.546329 pyobjc-framework-Accounts-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1662 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.2/PyObjCTest/test_acaccountstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1279 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.2/PyObjCTest/test_acaccounttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-Accounts-9.2/PyObjCTest/test_accounts.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1829 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.2/PyObjCTest/test_acerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-Accounts-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.548582 pyobjc-framework-Accounts-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2369 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/metadata/Accounts.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:23.555739 pyobjc-framework-Accounts-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    14012 2021-07-30 09:00:37.000000 pyobjc-framework-Accounts-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14136 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    12847 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14013 2021-03-21 10:08:22.000000 pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7793 2020-11-30 18:45:14.000000 pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14013 2021-07-30 09:00:37.000000 pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14137 2022-02-24 08:47:16.000000 pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Accounts-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Accounts-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:23.557419 pyobjc-framework-Accounts-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2023-05-29 10:07:45.000000 pyobjc-framework-Accounts-9.2/setup.py
```

### Comparing `pyobjc-framework-Accounts-9.1b1/Examples/demo.py` & `pyobjc-framework-Accounts-9.2/Examples/demo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/LICENSE.txt` & `pyobjc-framework-Accounts-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/Lib/Accounts/__init__.py` & `pyobjc-framework-Accounts-9.2/Lib/Accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/Lib/Accounts/_metadata.py` & `pyobjc-framework-Accounts-9.2/Lib/Accounts/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/PKG-INFO` & `pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Accounts
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Accounts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Accounts
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-Accounts-9.1b1/Lib/pyobjc_framework_Accounts.egg-info/SOURCES.txt` & `pyobjc-framework-Accounts-9.2/Lib/pyobjc_framework_Accounts.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/demo.py
 Lib/Accounts/__init__.py
 Lib/Accounts/_metadata.py
 Lib/pyobjc_framework_Accounts.egg-info/PKG-INFO
 Lib/pyobjc_framework_Accounts.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Accounts.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-Accounts-9.1b1/PKG-INFO` & `pyobjc-framework-Accounts-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Accounts
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Accounts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Accounts
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acaccountstore.py` & `pyobjc-framework-Accounts-9.2/PyObjCTest/test_acaccountstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acaccounttype.py` & `pyobjc-framework-Accounts-9.2/PyObjCTest/test_acaccounttype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/PyObjCTest/test_acerror.py` & `pyobjc-framework-Accounts-9.2/PyObjCTest/test_acerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/Accounts.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/Accounts.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Accounts-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Accounts-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Accounts-9.1b1/setup.py` & `pyobjc-framework-Accounts-9.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "Accounts" framework on macOS.
 
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
     name="pyobjc-framework-Accounts",
     description="Wrappers for the framework Accounts on macOS",
     min_os_level="10.8",
     packages=["Accounts"],
     version=VERSION,
```

