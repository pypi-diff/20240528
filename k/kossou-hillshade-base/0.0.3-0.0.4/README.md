# Comparing `tmp/kossou_hillshade_base-0.0.3.tar.gz` & `tmp/kossou_hillshade_base-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_base-0.0.3.tar", last modified: Tue May 28 04:11:07 2024, max compression
+gzip compressed data, was "kossou_hillshade_base-0.0.4.tar", last modified: Tue May 28 04:14:17 2024, max compression
```

## Comparing `kossou_hillshade_base-0.0.3.tar` & `kossou_hillshade_base-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.976084 kossou_hillshade_base-0.0.3/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.3/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 04:11:07.974635 kossou_hillshade_base-0.0.3/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.3/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      817 2024-05-28 04:08:32.000000 kossou_hillshade_base-0.0.3/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:11:07.976829 kossou_hillshade_base-0.0.3/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.3/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.904227 kossou_hillshade_base-0.0.3/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.938322 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      382 2024-05-28 04:02:21.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1945 2024-05-28 04:10:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/kossou_hillshade_base.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.947314 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:08:08.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.973724 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      469 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       41 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:14:17.668000 kossou_hillshade_base-0.0.4/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.4/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 04:14:17.667299 kossou_hillshade_base-0.0.4/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.4/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      803 2024-05-28 04:13:27.000000 kossou_hillshade_base-0.0.4/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:14:17.668168 kossou_hillshade_base-0.0.4/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.4/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:14:17.651564 kossou_hillshade_base-0.0.4/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:14:17.656517 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      382 2024-05-28 04:02:21.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1926 2024-05-28 04:13:08.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/kossou_hillshade_base.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:14:17.660328 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/static/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:12:51.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:14:17.666381 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 04:14:17.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      469 2024-05-28 04:14:17.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:14:17.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       34 2024-05-28 04:14:17.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 04:14:17.000000 kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_base-0.0.3/PKG-INFO` & `kossou_hillshade_base-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: earthpy
 Requires-Dist: matplotlib
-Requires-Dist: misaka
 Requires-Dist: numpy
 Requires-Dist: rasterio
 
 # Python-based analysis of geospatial data
 
 Replication of results described in [^1].
```

### Comparing `kossou_hillshade_base-0.0.3/README.md` & `kossou_hillshade_base-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.3/pyproject.toml` & `kossou_hillshade_base-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-base"
-version = "0.0.3" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.4" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
     "earthpy",
     "matplotlib",
-    "misaka",
     "numpy",
     "rasterio"
 ]
 
 [project.urls]
 "Homepage" = "https://https://gitlab.com/aaylward/kossou-hillshade-base"
 "Documentation" = "https://aaylward.gitlab.io/kossou-hillshade-base"
```

### Comparing `kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/kossou_hillshade_base.py` & `kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/kossou_hillshade_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 # Imports ======================================================================
 
 import earthpy.plot as ep
 import earthpy.spatial as es
 import matplotlib; matplotlib.use('agg')
 import matplotlib.pyplot as plt
-import misaka as m
 import numpy as np
 import os
 import os.path
 import rasterio as rio
 
 
 # Constants ====================================================================
```

### Comparing `kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif` & `kossou_hillshade_base-0.0.4/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/PKG-INFO` & `kossou_hillshade_base-0.0.4/src/kossou_hillshade_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: earthpy
 Requires-Dist: matplotlib
-Requires-Dist: misaka
 Requires-Dist: numpy
 Requires-Dist: rasterio
 
 # Python-based analysis of geospatial data
 
 Replication of results described in [^1].
```

