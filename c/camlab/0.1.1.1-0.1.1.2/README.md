# Comparing `tmp/camlab-0.1.1.1.tar.gz` & `tmp/camlab-0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.1.1.1.tar", last modified: Tue May 28 15:27:06 2024, max compression
+gzip compressed data, was "camlab-0.1.1.2.tar", last modified: Tue May 28 15:35:15 2024, max compression
```

## Comparing `camlab-0.1.1.1.tar` & `camlab-0.1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.086759 camlab-0.1.1.1/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-05-28 15:23:20.000000 camlab-0.1.1.1/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:27:06.086579 camlab-0.1.1.1/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-05-28 15:23:20.000000 camlab-0.1.1.1/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-05-28 15:24:23.000000 camlab-0.1.1.1/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-05-28 15:27:06.086806 camlab-0.1.1.1/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.083464 camlab-0.1.1.1/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.084957 camlab-0.1.1.1/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)     2365 2024-05-28 15:25:05.000000 camlab-0.1.1.1/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-05-28 15:23:21.000000 camlab-0.1.1.1/src/camlab/camera.py
--rw-r--r--   0 muzhan     (501) staff       (20)     3435 2024-05-28 15:24:54.000000 camlab-0.1.1.1/src/camlab/camera_torch.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.086249 camlab-0.1.1.1/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      239 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:35:15.653647 camlab-0.1.1.2/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-05-28 15:23:20.000000 camlab-0.1.1.2/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:35:15.653489 camlab-0.1.1.2/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-05-28 15:23:20.000000 camlab-0.1.1.2/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-05-28 15:34:50.000000 camlab-0.1.1.2/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-05-28 15:35:15.653706 camlab-0.1.1.2/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:35:15.651094 camlab-0.1.1.2/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:35:15.652361 camlab-0.1.1.2/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2365 2024-05-28 15:32:15.000000 camlab-0.1.1.2/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6974 2024-05-28 15:33:19.000000 camlab-0.1.1.2/src/camlab/camera.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     3435 2024-05-28 15:32:15.000000 camlab-0.1.1.2/src/camlab/camera_torch.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:35:15.653259 camlab-0.1.1.2/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:35:15.000000 camlab-0.1.1.2/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      239 2024-05-28 15:35:15.000000 camlab-0.1.1.2/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-05-28 15:35:15.000000 camlab-0.1.1.2/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-05-28 15:35:15.000000 camlab-0.1.1.2/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.1.1.1/LICENSE` & `camlab-0.1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1.1/PKG-INFO` & `camlab-0.1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.1.1.1/README.md` & `camlab-0.1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1.1/pyproject.toml` & `camlab-0.1.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.1.1.1"
+version = "0.1.1.2"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.1.1.1/src/camlab/__init__.py` & `camlab-0.1.1.2/src/camlab/__init__.py`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1.1/src/camlab/camera.py` & `camlab-0.1.1.2/src/camlab/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 class CameraObj:
-    def __init__(self, intri_mat=None):
+    def __init__(self, intri_mat=None, image_name=None):
         # intrinsic
         self.focal_x = None
         self.focal_y = None
         self.o_x = None
         self.o_y = None
         self.K = None
 
@@ -14,14 +14,17 @@
         self.w = None
 
         # extrinsic
         self.R = None
         self.T = None
         self.is_intri_set = False
         
+        # image
+        self.image_name = image_name
+        
         self.touch = 0
 
         if intri_mat:
             self.K = intri_mat
             self.focal_x = intri_mat[0][0]
             self.focal_y = intri_mat[1][1]
             self.o_x = intri_mat[0][2]
```

### Comparing `camlab-0.1.1.1/src/camlab/camera_torch.py` & `camlab-0.1.1.2/src/camlab/camera_torch.py`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1.1/src/camlab.egg-info/PKG-INFO` & `camlab-0.1.1.2/src/camlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

