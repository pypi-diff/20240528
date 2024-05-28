# Comparing `tmp/kossou_hillshade_base-0.0.2.tar.gz` & `tmp/kossou_hillshade_base-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_base-0.0.2.tar", last modified: Tue May 28 01:58:34 2024, max compression
+gzip compressed data, was "kossou_hillshade_base-0.0.3.tar", last modified: Tue May 28 04:11:07 2024, max compression
```

## Comparing `kossou_hillshade_base-0.0.2.tar` & `kossou_hillshade_base-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.442705 kossou_hillshade_base-0.0.2/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.2/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:58:34.442235 kossou_hillshade_base-0.0.2/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.2/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      911 2024-05-28 01:57:49.000000 kossou_hillshade_base-0.0.2/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 01:58:34.442876 kossou_hillshade_base-0.0.2/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.2/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.422979 kossou_hillshade_base-0.0.2/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.428822 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      354 2024-05-28 01:57:18.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3497 2024-05-28 01:40:59.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/kossou_hillshade_base.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.433170 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 01:57:53.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 01:58:34.441573 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      521 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       91 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       41 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 01:58:34.000000 kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.976084 kossou_hillshade_base-0.0.3/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.3/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 04:11:07.974635 kossou_hillshade_base-0.0.3/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.3/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      817 2024-05-28 04:08:32.000000 kossou_hillshade_base-0.0.3/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:11:07.976829 kossou_hillshade_base-0.0.3/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.3/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.904227 kossou_hillshade_base-0.0.3/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.938322 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      382 2024-05-28 04:02:21.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1945 2024-05-28 04:10:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/kossou_hillshade_base.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.947314 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:08:08.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:11:07.973724 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3374 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      469 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       41 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 04:11:07.000000 kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_base-0.0.2/PKG-INFO` & `kossou_hillshade_base-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_base-0.0.2/README.md` & `kossou_hillshade_base-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.2/pyproject.toml` & `kossou_hillshade_base-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-base"
-version = "0.0.2" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.3" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -23,10 +23,7 @@
     "numpy",
     "rasterio"
 ]
 
 [project.urls]
 "Homepage" = "https://https://gitlab.com/aaylward/kossou-hillshade-base"
 "Documentation" = "https://aaylward.gitlab.io/kossou-hillshade-base"
-
-[project.scripts]
-kossou-hillshade-base = "kossou_hillshade_base.kossou_hillshade_base:main"
```

### Comparing `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif` & `kossou_hillshade_base-0.0.3/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.2/src/kossou_hillshade_base.egg-info/PKG-INFO` & `kossou_hillshade_base-0.0.3/src/kossou_hillshade_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

