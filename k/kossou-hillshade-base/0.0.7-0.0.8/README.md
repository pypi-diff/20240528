# Comparing `tmp/kossou_hillshade_base-0.0.7.tar.gz` & `tmp/kossou_hillshade_base-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_base-0.0.7.tar", last modified: Tue May 28 05:16:45 2024, max compression
+gzip compressed data, was "kossou_hillshade_base-0.0.8.tar", last modified: Tue May 28 05:21:18 2024, max compression
```

## Comparing `kossou_hillshade_base-0.0.7.tar` & `kossou_hillshade_base-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:16:45.327182 kossou_hillshade_base-0.0.7/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.7/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 05:16:45.326457 kossou_hillshade_base-0.0.7/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.7/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      803 2024-05-28 05:09:30.000000 kossou_hillshade_base-0.0.7/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 05:16:45.327304 kossou_hillshade_base-0.0.7/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.7/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:16:45.305791 kossou_hillshade_base-0.0.7/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:16:45.309828 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      448 2024-05-28 05:13:51.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1938 2024-05-28 05:14:18.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/kossou_hillshade_base.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:16:45.313925 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/static/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 05:09:44.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:16:45.325601 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 05:16:45.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      469 2024-05-28 05:16:45.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 05:16:45.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       34 2024-05-28 05:16:45.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 05:16:45.000000 kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:21:18.463285 kossou_hillshade_base-0.0.8/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       60 2024-05-28 00:35:05.000000 kossou_hillshade_base-0.0.8/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 05:21:18.462632 kossou_hillshade_base-0.0.8/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 00:41:04.000000 kossou_hillshade_base-0.0.8/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      803 2024-05-28 05:21:01.000000 kossou_hillshade_base-0.0.8/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 05:21:18.463480 kossou_hillshade_base-0.0.8/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 00:36:43.000000 kossou_hillshade_base-0.0.8/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:21:18.446089 kossou_hillshade_base-0.0.8/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:21:18.451622 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      448 2024-05-28 05:13:51.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1946 2024-05-28 05:20:47.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/kossou_hillshade_base.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:21:18.456239 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/static/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  2889600 2024-05-28 00:46:53.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 05:21:03.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:21:18.461884 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3352 2024-05-28 05:21:18.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      469 2024-05-28 05:21:18.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 05:21:18.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       34 2024-05-28 05:21:18.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       22 2024-05-28 05:21:18.000000 kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_base-0.0.7/PKG-INFO` & `kossou_hillshade_base-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.7
+Version: 0.0.8
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_base-0.0.7/README.md` & `kossou_hillshade_base-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.7/pyproject.toml` & `kossou_hillshade_base-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-base"
-version = "0.0.7" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.8" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/kossou_hillshade_base.py` & `kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/kossou_hillshade_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,22 @@
     input_dtm: str,
     output_file: str,
     azimuth: int = AZIMUTH,
     altitude: int = ALTITUDE,
     width: float = WIDTH,
     height: float = HEIGHT,
     title=None,
-    cmap: str = DEFAULT_COLORMAP
+    colormap: str = DEFAULT_COLORMAP
 ):
     np.seterr(divide='ignore', invalid='ignore')
     with rio.open(input_dtm) as src:
         elevation = src.read(1)
     hillshade = es.hillshade(elevation, azimuth=azimuth, altitude=altitude)
     _, ax = plt.subplots(figsize=(width, height))
-    ep.plot_bands(hillshade, ax=ax, cbar=True, cmap=cmap, title=title)
+    ep.plot_bands(hillshade, ax=ax, cbar=True, cmap=colormap, title=title)
     plt.savefig(output_file, dpi=300)
     # fig = ax.get_figure()
     # fig.tight_layout()
     # fig.savefig(output_file, format='jpg', dpi=300)
     # fig.clf()
 
 def generate_report(
```

### Comparing `kossou_hillshade_base-0.0.7/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif` & `kossou_hillshade_base-0.0.8/src/kossou_hillshade_base/static/n07_w006_3arc_v2.tif`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_base-0.0.7/src/kossou_hillshade_base.egg-info/PKG-INFO` & `kossou_hillshade_base-0.0.8/src/kossou_hillshade_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-base
-Version: 0.0.7
+Version: 0.0.8
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-base
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-base
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

