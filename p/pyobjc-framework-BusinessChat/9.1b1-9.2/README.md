# Comparing `tmp/pyobjc-framework-BusinessChat-9.1b1.tar.gz` & `tmp/pyobjc-framework-BusinessChat-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-BusinessChat-9.1b1.tar", last modified: Sun Mar 26 11:15:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-BusinessChat-9.2.tar", last modified: Wed Jun  7 00:07:11 2023, max compression
```

## Comparing `pyobjc-framework-BusinessChat-9.1b1.tar` & `pyobjc-framework-BusinessChat-9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.654092 pyobjc-framework-BusinessChat-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.582155 pyobjc-framework-BusinessChat-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.606607 pyobjc-framework-BusinessChat-9.1b1/Lib/BusinessChat/
--rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/BusinessChat/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      729 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/BusinessChat/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.610280 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2120 2023-03-26 11:15:56.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      809 2023-03-26 11:15:56.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:15:56.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:24.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:15:56.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:15:56.000000 pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-BusinessChat-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1909 2023-03-26 11:15:56.652956 pyobjc-framework-BusinessChat-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.612934 pyobjc-framework-BusinessChat-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      502 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/PyObjCTest/test_bcchataction.py
--rw-r--r--   0 ronald     (501) staff       (20)      417 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/PyObjCTest/test_bcchatbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-BusinessChat-9.1b1/PyObjCTest/test_businesschat.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.614240 pyobjc-framework-BusinessChat-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      302 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/BusinessChat.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:56.651731 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     2205 2021-07-30 09:00:37.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2274 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1900 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2206 2021-03-21 10:08:22.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2206 2021-07-30 09:00:37.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2275 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-BusinessChat-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:15:56.654288 pyobjc-framework-BusinessChat-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      677 2023-03-25 14:20:30.000000 pyobjc-framework-BusinessChat-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.224171 pyobjc-framework-BusinessChat-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.200727 pyobjc-framework-BusinessChat-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.205992 pyobjc-framework-BusinessChat-9.2/Lib/BusinessChat/
+-rw-r--r--   0 ronald     (501) staff       (20)      734 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.2/Lib/BusinessChat/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      729 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/Lib/BusinessChat/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.209972 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2118 2023-06-07 00:07:11.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      824 2023-06-07 00:07:11.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:11.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:24.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:07:11.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:07:11.000000 pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-BusinessChat-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1907 2023-06-07 00:07:11.223749 pyobjc-framework-BusinessChat-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.212386 pyobjc-framework-BusinessChat-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      502 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/PyObjCTest/test_bcchataction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      417 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/PyObjCTest/test_bcchatbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-BusinessChat-9.2/PyObjCTest/test_businesschat.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.213523 pyobjc-framework-BusinessChat-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      302 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/metadata/BusinessChat.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:11.222577 pyobjc-framework-BusinessChat-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     2205 2021-07-30 09:00:37.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2274 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1900 2020-11-30 18:45:14.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2206 2021-03-21 10:08:22.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2206 2021-07-30 09:00:37.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2275 2022-02-24 08:47:16.000000 pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-BusinessChat-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-BusinessChat-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:11.224264 pyobjc-framework-BusinessChat-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      758 2023-05-29 10:07:45.000000 pyobjc-framework-BusinessChat-9.2/setup.py
```

### Comparing `pyobjc-framework-BusinessChat-9.1b1/Lib/BusinessChat/__init__.py` & `pyobjc-framework-BusinessChat-9.2/Lib/BusinessChat/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/Lib/BusinessChat/_metadata.py` & `pyobjc-framework-BusinessChat-9.2/Lib/BusinessChat/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/PKG-INFO` & `pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-BusinessChat
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework BusinessChat on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,BusinessChat
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-BusinessChat-9.1b1/Lib/pyobjc_framework_BusinessChat.egg-info/SOURCES.txt` & `pyobjc-framework-BusinessChat-9.2/Lib/pyobjc_framework_BusinessChat.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/BusinessChat/__init__.py
 Lib/BusinessChat/_metadata.py
 Lib/pyobjc_framework_BusinessChat.egg-info/PKG-INFO
 Lib/pyobjc_framework_BusinessChat.egg-info/SOURCES.txt
 Lib/pyobjc_framework_BusinessChat.egg-info/dependency_links.txt
 Lib/pyobjc_framework_BusinessChat.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-BusinessChat-9.1b1/License.txt` & `pyobjc-framework-BusinessChat-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/PKG-INFO` & `pyobjc-framework-BusinessChat-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-BusinessChat
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework BusinessChat on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,BusinessChat
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-BusinessChat-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-BusinessChat-9.1b1/pyobjc_setup.py` & `pyobjc-framework-BusinessChat-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

