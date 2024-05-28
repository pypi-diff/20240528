# Comparing `tmp/pyobjc-framework-SoundAnalysis-9.1b1.tar.gz` & `tmp/pyobjc-framework-SoundAnalysis-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SoundAnalysis-9.1b1.tar", last modified: Sun Mar 26 11:41:07 2023, max compression
+gzip compressed data, was "pyobjc-framework-SoundAnalysis-9.2.tar", last modified: Wed Jun  7 00:29:06 2023, max compression
```

## Comparing `pyobjc-framework-SoundAnalysis-9.1b1.tar` & `pyobjc-framework-SoundAnalysis-9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.649746 pyobjc-framework-SoundAnalysis-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.564932 pyobjc-framework-SoundAnalysis-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.588429 pyobjc-framework-SoundAnalysis-9.1b1/Lib/SoundAnalysis/
--rw-r--r--   0 ronald     (501) staff       (20)      723 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/SoundAnalysis/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/SoundAnalysis/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.593820 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2124 2023-03-26 11:41:07.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      982 2023-03-26 11:41:07.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:41:07.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:40.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:41:07.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:41:07.000000 pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SoundAnalysis-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-03-26 11:41:07.649397 pyobjc-framework-SoundAnalysis-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.600636 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      875 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snanalyzer.py
--rw-r--r--   0 ronald     (501) staff       (20)      486 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snclassifysoundrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      465 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      233 2022-06-25 20:08:27.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      287 2022-06-25 20:07:38.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      409 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_sntimedurationconstraint.py
--rw-r--r--   0 ronald     (501) staff       (20)      358 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_sntypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_soundanalysis.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.602130 pyobjc-framework-SoundAnalysis-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1360 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/SoundAnalysis.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:07.648575 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    16699 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16821 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11445 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11792 2021-03-21 10:08:23.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16700 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16822 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SoundAnalysis-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:41:07.649853 pyobjc-framework-SoundAnalysis-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      681 2023-03-25 14:20:32.000000 pyobjc-framework-SoundAnalysis-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.785880 pyobjc-framework-SoundAnalysis-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.747715 pyobjc-framework-SoundAnalysis-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.752773 pyobjc-framework-SoundAnalysis-9.2/Lib/SoundAnalysis/
+-rw-r--r--   0 ronald     (501) staff       (20)      723 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/SoundAnalysis/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/SoundAnalysis/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.756466 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-06-07 00:29:06.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      997 2023-06-07 00:29:06.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:29:06.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:40.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:29:06.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:29:06.000000 pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SoundAnalysis-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-06-07 00:29:06.785445 pyobjc-framework-SoundAnalysis-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.766010 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      875 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snanalyzer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      486 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snclassifysoundrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      465 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      233 2022-06-25 20:08:27.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      287 2022-06-25 20:07:38.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      409 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_sntimedurationconstraint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      358 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_sntypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-04-11 08:03:15.000000 pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_soundanalysis.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.767167 pyobjc-framework-SoundAnalysis-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1360 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/SoundAnalysis.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:06.784231 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    16699 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16821 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11445 2020-11-30 18:45:15.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11792 2021-03-21 10:08:23.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16700 2021-07-30 09:00:38.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16822 2022-02-24 08:47:17.000000 pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SoundAnalysis-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SoundAnalysis-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:29:06.785971 pyobjc-framework-SoundAnalysis-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      763 2023-05-29 10:07:47.000000 pyobjc-framework-SoundAnalysis-9.2/setup.py
```

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/Lib/SoundAnalysis/__init__.py` & `pyobjc-framework-SoundAnalysis-9.2/Lib/SoundAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/Lib/SoundAnalysis/_metadata.py` & `pyobjc-framework-SoundAnalysis-9.2/Lib/SoundAnalysis/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/PKG-INFO` & `pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SoundAnalysis
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SoundAnalysis on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SoundAnalysis
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/Lib/pyobjc_framework_SoundAnalysis.egg-info/SOURCES.txt` & `pyobjc-framework-SoundAnalysis-9.2/Lib/pyobjc_framework_SoundAnalysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SoundAnalysis/__init__.py
 Lib/SoundAnalysis/_metadata.py
 Lib/pyobjc_framework_SoundAnalysis.egg-info/PKG-INFO
 Lib/pyobjc_framework_SoundAnalysis.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SoundAnalysis.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SoundAnalysis.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/License.txt` & `pyobjc-framework-SoundAnalysis-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/PKG-INFO` & `pyobjc-framework-SoundAnalysis-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SoundAnalysis
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SoundAnalysis on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SoundAnalysis
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/PyObjCTest/test_snanalyzer.py` & `pyobjc-framework-SoundAnalysis-9.2/PyObjCTest/test_snanalyzer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/SoundAnalysis.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/SoundAnalysis.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SoundAnalysis-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SoundAnalysis-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SoundAnalysis-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

