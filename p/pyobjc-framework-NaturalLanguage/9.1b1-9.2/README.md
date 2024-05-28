# Comparing `tmp/pyobjc-framework-NaturalLanguage-9.1b1.tar.gz` & `tmp/pyobjc-framework-NaturalLanguage-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-NaturalLanguage-9.1b1.tar", last modified: Sun Mar 26 11:31:30 2023, max compression
+gzip compressed data, was "pyobjc-framework-NaturalLanguage-9.2.tar", last modified: Wed Jun  7 00:21:47 2023, max compression
```

## Comparing `pyobjc-framework-NaturalLanguage-9.1b1.tar` & `pyobjc-framework-NaturalLanguage-9.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:30.002984 pyobjc-framework-NaturalLanguage-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:29.936644 pyobjc-framework-NaturalLanguage-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:29.940712 pyobjc-framework-NaturalLanguage-9.1b1/Lib/NaturalLanguage/
--rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/NaturalLanguage/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9123 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/NaturalLanguage/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:29.944100 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2132 2023-03-26 11:31:29.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1120 2023-03-26 11:31:29.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:31:29.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:38.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:31:29.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:31:29.000000 pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NaturalLanguage-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1921 2023-03-26 11:31:30.002059 pyobjc-framework-NaturalLanguage-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:29.958495 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_naturallanguage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1791 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlembedding.py
--rw-r--r--   0 ronald     (501) staff       (20)      853 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlgazetteer.py
--rw-r--r--   0 ronald     (501) staff       (20)     4289 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nllanguage.py
--rw-r--r--   0 ronald     (501) staff       (20)      185 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nllanguagerecognizer.py
--rw-r--r--   0 ronald     (501) staff       (20)      547 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlmodel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1791 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltagger.py
--rw-r--r--   0 ronald     (501) staff       (20)     3130 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltagscheme.py
--rw-r--r--   0 ronald     (501) staff       (20)     1147 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltokenizer.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:29.959955 pyobjc-framework-NaturalLanguage-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     9577 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/NaturalLanguage.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:30.000439 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    42488 2021-08-01 10:28:32.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42793 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43253 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21762 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36383 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42489 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42489 2021-08-01 10:28:32.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42794 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43254 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NaturalLanguage-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:31:30.003114 pyobjc-framework-NaturalLanguage-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      689 2023-03-25 14:20:32.000000 pyobjc-framework-NaturalLanguage-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.755321 pyobjc-framework-NaturalLanguage-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.712197 pyobjc-framework-NaturalLanguage-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.716752 pyobjc-framework-NaturalLanguage-9.2/Lib/NaturalLanguage/
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/NaturalLanguage/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9123 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/NaturalLanguage/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.720180 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2130 2023-06-07 00:21:47.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1135 2023-06-07 00:21:47.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:47.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:38.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:21:47.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:21:47.000000 pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NaturalLanguage-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1919 2023-06-07 00:21:47.754909 pyobjc-framework-NaturalLanguage-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.730772 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      214 2022-04-11 08:03:15.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_naturallanguage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1791 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlembedding.py
+-rw-r--r--   0 ronald     (501) staff       (20)      853 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlgazetteer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4289 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nllanguage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      185 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nllanguagerecognizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      547 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlmodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1791 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltagger.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3130 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltagscheme.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1147 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltokenizer.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.742572 pyobjc-framework-NaturalLanguage-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     9577 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/NaturalLanguage.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:47.753807 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    42488 2021-08-01 10:28:32.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42793 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43253 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21762 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36383 2020-11-30 18:45:15.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42489 2021-03-21 10:08:23.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42489 2021-08-01 10:28:32.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42794 2022-02-24 08:47:16.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43254 2022-06-25 20:19:21.000000 pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NaturalLanguage-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-NaturalLanguage-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:47.755419 pyobjc-framework-NaturalLanguage-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      770 2023-05-29 10:07:46.000000 pyobjc-framework-NaturalLanguage-9.2/setup.py
```

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/Lib/NaturalLanguage/__init__.py` & `pyobjc-framework-NaturalLanguage-9.2/Lib/NaturalLanguage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/Lib/NaturalLanguage/_metadata.py` & `pyobjc-framework-NaturalLanguage-9.2/Lib/NaturalLanguage/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/PKG-INFO` & `pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NaturalLanguage
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NaturalLanguage on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NaturalLanguage
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/Lib/pyobjc_framework_NaturalLanguage.egg-info/SOURCES.txt` & `pyobjc-framework-NaturalLanguage-9.2/Lib/pyobjc_framework_NaturalLanguage.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/NaturalLanguage/__init__.py
 Lib/NaturalLanguage/_metadata.py
 Lib/pyobjc_framework_NaturalLanguage.egg-info/PKG-INFO
 Lib/pyobjc_framework_NaturalLanguage.egg-info/SOURCES.txt
 Lib/pyobjc_framework_NaturalLanguage.egg-info/dependency_links.txt
 Lib/pyobjc_framework_NaturalLanguage.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/License.txt` & `pyobjc-framework-NaturalLanguage-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PKG-INFO` & `pyobjc-framework-NaturalLanguage-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NaturalLanguage
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NaturalLanguage on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NaturalLanguage
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlembedding.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlembedding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlgazetteer.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlgazetteer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nllanguage.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nllanguage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nlmodel.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nlmodel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltagger.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltagger.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltagscheme.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltagscheme.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/PyObjCTest/test_nltokenizer.py` & `pyobjc-framework-NaturalLanguage-9.2/PyObjCTest/test_nltokenizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/NaturalLanguage.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/NaturalLanguage.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-NaturalLanguage-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NaturalLanguage-9.1b1/pyobjc_setup.py` & `pyobjc-framework-NaturalLanguage-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

