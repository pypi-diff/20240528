# Comparing `tmp/pyobjc-framework-AdSupport-9.1b1.tar.gz` & `tmp/pyobjc-framework-AdSupport-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AdSupport-9.1b1.tar", last modified: Sun Mar 26 11:13:45 2023, max compression
+gzip compressed data, was "pyobjc-framework-AdSupport-9.2.tar", last modified: Wed Jun  7 00:05:34 2023, max compression
```

## Comparing `pyobjc-framework-AdSupport-9.1b1.tar` & `pyobjc-framework-AdSupport-9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.479177 pyobjc-framework-AdSupport-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.448616 pyobjc-framework-AdSupport-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.453824 pyobjc-framework-AdSupport-9.1b1/Lib/AdSupport/
--rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.1b1/Lib/AdSupport/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      750 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.1b1/Lib/AdSupport/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.457020 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2123 2023-03-26 11:13:45.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      784 2023-03-26 11:13:45.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:13:45.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:15.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:13:45.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:13:45.000000 pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AdSupport-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1912 2023-03-26 11:13:45.478660 pyobjc-framework-AdSupport-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.458839 pyobjc-framework-AdSupport-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-AdSupport-9.1b1/PyObjCTest/test_adsupport.py
--rw-r--r--   0 ronald     (501) staff       (20)      378 2021-03-21 10:08:22.000000 pyobjc-framework-AdSupport-9.1b1/PyObjCTest/test_asidentifiermanager.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.460266 pyobjc-framework-AdSupport-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      234 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.1b1/metadata/AdSupport.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:45.477228 pyobjc-framework-AdSupport-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     2142 2021-07-30 09:00:37.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2161 2022-02-24 08:47:16.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2179 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2143 2021-03-21 10:08:22.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2143 2021-07-30 09:00:37.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2162 2022-02-24 08:47:16.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2180 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AdSupport-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:13:45.479315 pyobjc-framework-AdSupport-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      680 2023-03-25 14:20:30.000000 pyobjc-framework-AdSupport-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.087733 pyobjc-framework-AdSupport-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.064663 pyobjc-framework-AdSupport-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.069784 pyobjc-framework-AdSupport-9.2/Lib/AdSupport/
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.2/Lib/AdSupport/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      750 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.2/Lib/AdSupport/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.073178 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2121 2023-06-07 00:05:34.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2023-06-07 00:05:34.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:34.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:15.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:34.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:05:34.000000 pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AdSupport-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1910 2023-06-07 00:05:34.087321 pyobjc-framework-AdSupport-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.075227 pyobjc-framework-AdSupport-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-AdSupport-9.2/PyObjCTest/test_adsupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      378 2021-03-21 10:08:22.000000 pyobjc-framework-AdSupport-9.2/PyObjCTest/test_asidentifiermanager.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.076953 pyobjc-framework-AdSupport-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      234 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.2/metadata/AdSupport.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-AdSupport-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:34.086083 pyobjc-framework-AdSupport-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     2142 2021-07-30 09:00:37.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2161 2022-02-24 08:47:16.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2179 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2143 2021-03-21 10:08:22.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2143 2021-07-30 09:00:37.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2162 2022-02-24 08:47:16.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2180 2023-02-19 10:50:34.000000 pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AdSupport-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AdSupport-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:34.087829 pyobjc-framework-AdSupport-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      762 2023-05-29 10:07:45.000000 pyobjc-framework-AdSupport-9.2/setup.py
```

### Comparing `pyobjc-framework-AdSupport-9.1b1/Lib/AdSupport/__init__.py` & `pyobjc-framework-AdSupport-9.2/Lib/AdSupport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/Lib/AdSupport/_metadata.py` & `pyobjc-framework-AdSupport-9.2/Lib/AdSupport/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/PKG-INFO` & `pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AdSupport
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AdSupport on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AdSupport
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-AdSupport-9.1b1/Lib/pyobjc_framework_AdSupport.egg-info/SOURCES.txt` & `pyobjc-framework-AdSupport-9.2/Lib/pyobjc_framework_AdSupport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AdSupport/__init__.py
 Lib/AdSupport/_metadata.py
 Lib/pyobjc_framework_AdSupport.egg-info/PKG-INFO
 Lib/pyobjc_framework_AdSupport.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AdSupport.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AdSupport.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AdSupport-9.1b1/License.txt` & `pyobjc-framework-AdSupport-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/PKG-INFO` & `pyobjc-framework-AdSupport-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AdSupport
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AdSupport on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AdSupport
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-AdSupport-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AdSupport-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AdSupport-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

