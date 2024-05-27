# Comparing `tmp/trame-3.6.0.tar.gz` & `tmp/trame-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-3.6.0.tar", last modified: Wed Apr 10 23:38:32 2024, max compression
+gzip compressed data, was "trame-3.6.1.tar", last modified: Mon May 27 22:50:21 2024, max compression
```

## Comparing `trame-3.6.0.tar` & `trame-3.6.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 23:38:28.000000 trame-3.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-10 23:38:28.000000 trame-3.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7169 2024-04-10 23:38:32.242495 trame-3.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6431 2024-04-10 23:38:28.000000 trame-3.6.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      918 2024-04-10 23:38:32.246495 trame-3.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 23:38:29.000000 trame-3.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.238495 trame-3.6.0/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 23:38:28.000000 trame-3.6.0/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.238495 trame-3.6.0/trame/app/
--rw-r--r--   0 root         (0) root         (0)     3132 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     2089 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2320 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2024-04-10 23:38:29.000000 trame-3.6.0/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.238495 trame-3.6.0/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2024-04-10 23:38:29.000000 trame-3.6.0/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2024-04-10 23:38:29.000000 trame-3.6.0/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/decorators/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-10 23:38:29.000000 trame-3.6.0/trame/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-10 23:38:29.000000 trame-3.6.0/trame/decorators/dev.py
--rw-r--r--   0 root         (0) root         (0)     5665 2024-04-10 23:38:29.000000 trame-3.6.0/trame/decorators/klass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:38:29.000000 trame-3.6.0/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-10 23:38:29.000000 trame-3.6.0/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2024-04-10 23:38:29.000000 trame-3.6.0/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-04-10 23:38:29.000000 trame-3.6.0/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     4461 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/serve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/tools/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/widgets/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13960 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/widgets/utils.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-10 23:38:29.000000 trame-3.6.0/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.242495 trame-3.6.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:38:29.000000 trame-3.6.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-10 23:38:29.000000 trame-3.6.0/trame/widgets/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:38:32.238495 trame-3.6.0/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7169 2024-04-10 23:38:32.000000 trame-3.6.0/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-10 23:38:32.000000 trame-3.6.0/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 23:38:32.000000 trame-3.6.0/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 23:38:32.000000 trame-3.6.0/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 23:38:32.000000 trame-3.6.0/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-27 22:50:18.000000 trame-3.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-27 22:50:18.000000 trame-3.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-05-27 22:50:21.933843 trame-3.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-27 22:50:18.000000 trame-3.6.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      918 2024-05-27 22:50:21.933843 trame-3.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 22:50:19.000000 trame-3.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.925844 trame-3.6.1/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-27 22:50:18.000000 trame-3.6.1/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/decorators/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/dev.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/klass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/serve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/tools/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13964 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-27 22:50:19.000000 trame-3.6.1/trame/widgets/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.925844 trame-3.6.1/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/top_level.txt
```

### Comparing `trame-3.6.0/LICENSE` & `trame-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/PKG-INFO` & `trame-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.6.0
+Version: 3.6.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.6.0/README.rst` & `trame-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/setup.cfg` & `trame-3.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 3.6.0
+version = 3.6.1
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-3.6.0/trame/LICENSE` & `trame-3.6.1/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/__init__.py` & `trame-3.6.1/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/demo.py` & `trame-3.6.1/trame/app/demo.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/dev.py` & `trame-3.6.1/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/file_upload.py` & `trame-3.6.1/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/jupyter.py` & `trame-3.6.1/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/mimetypes.py` & `trame-3.6.1/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/singleton.py` & `trame-3.6.1/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/app/testing.py` & `trame-3.6.1/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/assets/local.py` & `trame-3.6.1/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/assets/remote.py` & `trame-3.6.1/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/decorators/klass.py` & `trame-3.6.1/trame/decorators/klass.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/env/paraview.py` & `trame-3.6.1/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/env/utils.py` & `trame-3.6.1/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/env/venv.py` & `trame-3.6.1/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/tools/app.py` & `trame-3.6.1/trame/tools/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 r"""
 From the directory containing the static content for a trame application to work,
 generate another application specific HTML file.
 """
+
 import argparse
 import re
 from pathlib import Path
 import sys
 
 APP_PATTERN = re.compile(r'data-app-name="\w+"')
```

### Comparing `trame-3.6.0/trame/tools/serve.py` & `trame-3.6.1/trame/tools/serve.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/tools/widgets/__main__.py` & `trame-3.6.1/trame/tools/widgets/__main__.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/tools/widgets/generator.py` & `trame-3.6.1/trame/tools/widgets/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
                     for web_dir in config[name][sub_name][module]:
                         module_conf_init[web_dir] = await create_web_content(
                             ref_path,
                             (module_root / web_dir),
                             config[name][sub_name][module][web_dir],
                         )
                     # Register trame/modules/{webdir}
-                    trame_plugins[
-                        f"trame/modules/{module}.py"
-                    ] = f"from {name}.module.{module} import *\n"
+                    trame_plugins[f"trame/modules/{module}.py"] = (
+                        f"from {name}.module.{module} import *\n"
+                    )
                     create_module_init(module_root_init, module_conf_init)
 
                 elif sub_name == "widgets":
                     file_path = sub_package / f"{module}.py"
                     with file_path.open("w") as file:
                         file.write(
                             "from trame_client.widgets.core import AbstractElement, Template  # noqa\n"
@@ -161,17 +161,17 @@
                         file.write("\n__all__ = [")
                         for class_name in all_class_names:
                             file.write(f'\n{" " * 4}"{class_name}",')
                         file.write("\n]")
                         file.write("\n")
 
                     # Register trame/modules/{webdir}
-                    trame_plugins[
-                        f"trame/widgets/{module}.py"
-                    ] = f"from {name}.widgets.{module} import *\n\ndef initialize(server):\n    from {name}.module import {module}\n\n    server.enable_module({module})\n"
+                    trame_plugins[f"trame/widgets/{module}.py"] = (
+                        f"from {name}.widgets.{module} import *\n\ndef initialize(server):\n    from {name}.module import {module}\n\n    server.enable_module({module})\n"
+                    )
 
     # Create trame package connectors
     for file, content in trame_plugins.items():
         (output / file).write_text(content)
 
 
 def create_module_init(init_path, init_conf):
```

### Comparing `trame-3.6.0/trame/tools/widgets/utils.py` & `trame-3.6.1/trame/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame/tools/www.py` & `trame-3.6.1/trame/tools/www.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 r"""
 From a list of trame modules name, gather and generate the required static
 content that needs to be served for a trame application to work.
 """
+
 import argparse
 import importlib
 import shutil
 from pathlib import Path
 
 
 class StaticContentGenerator:
     def __init__(self):
+        self.name = "www_generator"  # required to look like a server
         self.www = None
         self.serve = {}
         self.client_type = "vue3"
 
     def enable_all(self):
         import pkgutil
```

### Comparing `trame-3.6.0/trame/widgets/helper.py` & `trame-3.6.1/trame/widgets/helper.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.0/trame.egg-info/PKG-INFO` & `trame-3.6.1/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.6.0
+Version: 3.6.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.6.0/trame.egg-info/SOURCES.txt` & `trame-3.6.1/trame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

