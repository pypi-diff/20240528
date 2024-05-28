# Comparing `tmp/pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1.tar.gz` & `tmp/pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1.tar", last modified: Sun Mar 26 11:28:17 2023, max compression
+gzip compressed data, was "pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2.tar", last modified: Wed Jun  7 00:18:47 2023, max compression
```

## Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1.tar` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.957895 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.921947 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.927367 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/LocalAuthenticationEmbeddedUI/
--rw-r--r--   0 ronald     (501) staff       (20)      880 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/LocalAuthenticationEmbeddedUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/LocalAuthenticationEmbeddedUI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.930287 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2187 2023-03-26 11:28:17.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1792 2023-03-26 11:28:17.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:17.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:32.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       93 2023-03-26 11:28:17.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       30 2023-03-26 11:28:17.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.934136 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2039 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)        0 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       93 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.943069 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2007 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)        0 2021-07-30 09:25:24.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:24.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       93 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       26 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1976 2023-03-26 11:28:17.957414 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.949807 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PyObjCTest/test_laauthenticationview.py
--rw-r--r--   0 ronald     (501) staff       (20)      242 2022-04-11 08:03:15.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PyObjCTest/test_localauthenticationembeddedui.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.951953 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/LocalAuthenticationEmbeddedUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       74 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:17.956296 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     2135 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2907 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2908 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:17.958002 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      827 2023-03-25 14:20:31.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      568 2022-06-27 19:02:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/test_laright_ui.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.406939 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.377226 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.383333 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/LocalAuthenticationEmbeddedUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      880 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/LocalAuthenticationEmbeddedUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      499 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/LocalAuthenticationEmbeddedUI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.386918 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2185 2023-06-07 00:18:47.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1807 2023-06-07 00:18:47.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:47.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:32.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       87 2023-06-07 00:18:47.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2023-06-07 00:18:47.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.394983 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2039 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)        0 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       93 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2021-07-30 12:02:07.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.400217 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2007 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)        0 2021-07-30 09:25:24.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:25:24.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       93 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2021-07-30 12:01:36.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1974 2023-06-07 00:18:47.406564 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.402272 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PyObjCTest/test_laauthenticationview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      242 2022-04-11 08:03:15.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PyObjCTest/test_localauthenticationembeddedui.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.403457 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      217 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/LocalAuthenticationEmbeddedUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:47.405946 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     2135 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2907 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2136 2021-07-30 09:00:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2908 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:47.407050 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      908 2023-05-29 10:07:46.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      568 2022-06-27 19:02:38.000000 pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/test_laright_ui.py
```

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/LocalAuthenticationEmbeddedUI/__init__.py` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/LocalAuthenticationEmbeddedUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/PKG-INFO` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LocalAuthenticationEmbeddedUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LocalAuthenticationEmbeddedUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LocalAuthenticationEmbeddedUI
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/SOURCES.txt` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 test_laright_ui.py
 Lib/LocalAuthenticationEmbeddedUI/__init__.py
 Lib/LocalAuthenticationEmbeddedUI/_metadata.py
 Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/PKG-INFO
 Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_LocalAuthenticationEmbeddedUI.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/PKG-INFO` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationEmbeddedUIView.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/PKG-INFO` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/Lib/pyobjc_framework_LocalAuthenticationUIView.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/License.txt` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/PKG-INFO` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LocalAuthenticationEmbeddedUI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework LocalAuthenticationEmbeddedUI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LocalAuthenticationEmbeddedUI
 Platform: MacOS X (>=12.0)
```

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/setup.py` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "LocalAuthenticationEmbeddedUI" framework on macOS.
 
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
     name="pyobjc-framework-LocalAuthenticationEmbeddedUI",
     description="Wrappers for the framework LocalAuthenticationEmbeddedUI on macOS",
     min_os_level="12.0",
     packages=["LocalAuthenticationEmbeddedUI"],
     version=VERSION,
```

### Comparing `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.1b1/test_laright_ui.py` & `pyobjc-framework-LocalAuthenticationEmbeddedUI-9.2/test_laright_ui.py`

 * *Files identical despite different names*

