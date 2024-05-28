# Comparing `tmp/kossou_hillshade_cli-0.0.1.tar.gz` & `tmp/kossou_hillshade_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_cli-0.0.1.tar", last modified: Tue May 28 04:28:02 2024, max compression
+gzip compressed data, was "kossou_hillshade_cli-0.0.2.tar", last modified: Tue May 28 04:33:46 2024, max compression
```

## Comparing `kossou_hillshade_cli-0.0.1.tar` & `kossou_hillshade_cli-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:28:02.938291 kossou_hillshade_cli-0.0.1/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 04:03:41.000000 kossou_hillshade_cli-0.0.1/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:28:02.937708 kossou_hillshade_cli-0.0.1/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 04:04:58.000000 kossou_hillshade_cli-0.0.1/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 04:16:03.000000 kossou_hillshade_cli-0.0.1/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:28:02.938454 kossou_hillshade_cli-0.0.1/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 04:05:46.000000 kossou_hillshade_cli-0.0.1/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:28:02.929185 kossou_hillshade_cli-0.0.1/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:28:02.933401 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 04:16:31.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2401 2024-05-28 04:19:11.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli/kossou_hillshade_cli.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:16:12.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:28:02.937059 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 04:28:02.000000 kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.008200 kossou_hillshade_cli-0.0.2/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 04:03:41.000000 kossou_hillshade_cli-0.0.2/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:33:46.007728 kossou_hillshade_cli-0.0.2/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 04:04:58.000000 kossou_hillshade_cli-0.0.2/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 04:31:06.000000 kossou_hillshade_cli-0.0.2/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:33:46.008307 kossou_hillshade_cli-0.0.2/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 04:05:46.000000 kossou_hillshade_cli-0.0.2/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:45.998472 kossou_hillshade_cli-0.0.2/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.001568 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 04:16:31.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2230 2024-05-28 04:30:47.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/kossou_hillshade_cli.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:31:09.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.006679 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_cli-0.0.1/PKG-INFO` & `kossou_hillshade_cli-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_cli-0.0.1/README.md` & `kossou_hillshade_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_cli-0.0.1/pyproject.toml` & `kossou_hillshade_cli-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-cli"
-version = "0.0.1" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.2" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli/kossou_hillshade_cli.py` & `kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/kossou_hillshade_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 #===============================================================================
-# kossou_hillshade_base.py
+# kossou_hillshade_cli.py
 #===============================================================================
 
 # Imports ======================================================================
 
-import earthpy.plot as ep
-import earthpy.spatial as es
-import matplotlib; matplotlib.use('agg')
-import matplotlib.pyplot as plt
 import misaka as m
-import numpy as np
 import os
 import os.path
-import rasterio as rio
 
 from argparse import ArgumentParser
 
 from kossou_hillshade_base import (AZIMUTH, ALTITUDE, WIDTH, HEIGHT,
                                    DEFAULT_ELEVATION_TIFF, REPORT,
                                    plot_hillshade, generate_report)
```

### Comparing `kossou_hillshade_cli-0.0.1/src/kossou_hillshade_cli.egg-info/PKG-INFO` & `kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

