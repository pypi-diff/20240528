# Comparing `tmp/kossou_hillshade_base-0.0.1.tar.gz` & `tmp/kossou_hillshade_base-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_base-0.0.1.tar", last modified: Tue May 28 01:46:26 2024, max compression
+gzip compressed data, was "kossou_hillshade_base-0.0.2.tar", last modified: Tue May 28 01:58:34 2024, max compression
```

## Comparing `kossou_hillshade_base-0.0.1.tar` & `kossou_hillshade_base-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:46:26.092197 kossou_hillshade_base-0.0.1/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.1/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:46:26.091401 kossou_hillshade_base-0.0.1/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.1/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      911 2024-05-28 01:22:18.000000 kossou_hillshade_base-0.0.1/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 01:46:26.092349 kossou_hillshade_base-0.0.1/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.1/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:46:26.079145 kossou_hillshade_base-0.0.1/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:46:26.082614 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      332 2024-05-28 01:29:48.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3497 2024-05-28 01:40:59.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/kossou_hillshade_base.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:46:26.086199 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/static/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 00:38:44.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:46:26.090629 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      521 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       91 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       41 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 01:46:26.000000 kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.442705 kossou_hillshade_base-0.0.2/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.2/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:58:34.442235 kossou_hillshade_base-0.0.2/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.2/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      911 2024-05-28 01:57:49.000000 kossou_hillshade_base-0.0.2/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 01:58:34.442876 kossou_hillshade_base-0.0.2/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.2/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.422979 kossou_hillshade_base-0.0.2/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.428822 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      354 2024-05-28 01:57:18.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3497 2024-05-28 01:40:59.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/kossou_hillshade_base.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.433170 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 01:57:53.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.441573 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      521 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       91 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       41 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_base-0.0.1/PKG-INFO` & `kossou_hillshade_base-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_base-0.0.1/README.md` & `kossou_hillshade_base-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.1/pyproject.toml` & `kossou_hillshade_base-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-base"
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

### Comparing `kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/kossou_hillshade_base.py` & `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/kossou_hillshade_base.py`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.1/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif` & `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/PKG-INFO` & `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_base-0.0.1/src/kossou_hillshade_base.egg-info/SOURCES.txt` & `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

