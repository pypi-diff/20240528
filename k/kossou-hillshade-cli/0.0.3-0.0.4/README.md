# Comparing `tmp/kossou_hillshade_cli-0.0.3.tar.gz` & `tmp/kossou_hillshade_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_cli-0.0.3.tar", last modified: Tue May 28 05:26:22 2024, max compression
+gzip compressed data, was "kossou_hillshade_cli-0.0.4.tar", last modified: Tue May 28 14:46:45 2024, max compression
```

## Comparing `kossou_hillshade_cli-0.0.3.tar` & `kossou_hillshade_cli-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.063624 kossou_hillshade_cli-0.0.3/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 04:03:41.000000 kossou_hillshade_cli-0.0.3/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 05:26:22.063102 kossou_hillshade_cli-0.0.3/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 04:04:58.000000 kossou_hillshade_cli-0.0.3/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 05:07:38.000000 kossou_hillshade_cli-0.0.3/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 05:26:22.063722 kossou_hillshade_cli-0.0.3/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 04:05:46.000000 kossou_hillshade_cli-0.0.3/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.053648 kossou_hillshade_cli-0.0.3/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.058157 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 04:16:31.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3112 2024-05-28 05:24:57.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/kossou_hillshade_cli.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 05:07:43.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.062375 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 14:46:45.972276 kossou_hillshade_cli-0.0.4/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 14:06:17.000000 kossou_hillshade_cli-0.0.4/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4014 2024-05-28 14:46:45.971452 kossou_hillshade_cli-0.0.4/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3388 2024-05-28 14:33:54.000000 kossou_hillshade_cli-0.0.4/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 14:14:17.000000 kossou_hillshade_cli-0.0.4/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 14:46:45.972493 kossou_hillshade_cli-0.0.4/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 14:06:17.000000 kossou_hillshade_cli-0.0.4/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 14:46:45.943198 kossou_hillshade_cli-0.0.4/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 14:46:45.956570 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 14:06:17.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2976 2024-05-28 14:32:28.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli/kossou_hillshade_cli.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 14:14:20.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 14:46:45.970470 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4014 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 14:46:45.000000 kossou_hillshade_cli-0.0.4/src/kossou_hillshade_cli.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_cli-0.0.3/PKG-INFO` & `kossou_hillshade_cli-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-Metadata-Version: 2.1
-Name: kossou-hillshade-cli
-Version: 0.0.3
-Summary: Plot hillshade over Lake Kossou using satellite elevation data
-Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
-Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
-Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: kossou-hillshade-base
-Requires-Dist: misaka
-
 # Python-based analysis of geospatial data
 
 Replication of results described in [^1].
 
+```sh
+conda create -c conda-forge -n kossou-hillshade earthpy matplotlib misaka numpy rasterio
+pip install kossou-hillshade-cli
+```
+
+```sh
+kossou-hillshade --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --azimuth 230 Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
+```
+
 ## Download elevation file
 
 To download the elevation file, first register an account on the [USGS EROS registration system](https://ers.cr.usgs.gov/login) to get download access via [EarthExplorer](https://earthexplorer.usgs.gov) and/or [GloVis](https://glovis.usgs.gov/).
 
 ### EarthExplorer
 
 Under the Datasets tab, under the Digital Elevation category, under the SRTM subcategory, select SRTM Void Filled.
@@ -61,15 +57,21 @@
 
 Similar to above, use EarthExplorer or GloVis to search the Landsat 8-9 OLI/TIRS C2 L1 dataset for a result with Landsat Product Identifier L1 of LC09_L1TP_197055_20220111_20230502_02_T1.
 
 ## Generate plots
 
 The results of [^1] may be replicated by running:
 
+```sh
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --azimuth 230 --colormap plasma Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
 ```
-python plot_geotiff.py n07_w006_3arc_v2.tif Figure_2_DEM_Kossou_1609.jpg
-python plot_hillshade.py n07_w006_3arc_v2.tif Figure_3_Hillshade_Kossou_1609.jpg
-python plot_hillshade.py --azimuth 230 --colormap plasma n07_w006_3arc_v2.tif Figure_4_Azimuth_hillshade_Kossou.jpg
-python plot_hillshade.py --altitude 10 --colormap magma n07_w006_3arc_v2.tif Figure_5_Angle_hillshade_Kossou.jpg
+
+In fact, the geotiff file `n07_w006_3arc_v2.tif` is included in the `kossou-hillshade-base` package, so this will also work:
+```sh
+kossou-hillshade --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --azimuth 230 --colormap plasma Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
 ```
 
-[^1]: Polina Lemenkova and Olivier Debeir, [Satellite Image Processing by Python and R Using Landsat 9 OLI/TIRS and SRTM DEM Data on Côte d’Ivoire, West Africa](https://www.mdpi.com/2313-433X/8/12/317). J. Imaging 2022
+[^1]: Polina Lemenkova and Olivier Debeir, [Satellite Image Processing by Python and R Using Landsat 9 OLI/TIRS and SRTM DEM Data on Côte d’Ivoire, West Africa](https://www.mdpi.com/2313-433X/8/12/317). J. Imaging 2022
```

### Comparing `kossou_hillshade_cli-0.0.3/pyproject.toml` & `kossou_hillshade_cli-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-cli"
-version = "0.0.3" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.4" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/PKG-INFO` & `kossou_hillshade_cli-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
@@ -13,14 +13,25 @@
 Requires-Dist: kossou-hillshade-base
 Requires-Dist: misaka
 
 # Python-based analysis of geospatial data
 
 Replication of results described in [^1].
 
+```sh
+conda create -c conda-forge -n kossou-hillshade earthpy matplotlib misaka numpy rasterio
+pip install kossou-hillshade-cli
+```
+
+```sh
+kossou-hillshade --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --azimuth 230 Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
+```
+
 ## Download elevation file
 
 To download the elevation file, first register an account on the [USGS EROS registration system](https://ers.cr.usgs.gov/login) to get download access via [EarthExplorer](https://earthexplorer.usgs.gov) and/or [GloVis](https://glovis.usgs.gov/).
 
 ### EarthExplorer
 
 Under the Datasets tab, under the Digital Elevation category, under the SRTM subcategory, select SRTM Void Filled.
@@ -61,15 +72,21 @@
 
 Similar to above, use EarthExplorer or GloVis to search the Landsat 8-9 OLI/TIRS C2 L1 dataset for a result with Landsat Product Identifier L1 of LC09_L1TP_197055_20220111_20230502_02_T1.
 
 ## Generate plots
 
 The results of [^1] may be replicated by running:
 
+```sh
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --azimuth 230 --colormap plasma Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --geotiff n07_w006_3arc_v2.tif --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
 ```
-python plot_geotiff.py n07_w006_3arc_v2.tif Figure_2_DEM_Kossou_1609.jpg
-python plot_hillshade.py n07_w006_3arc_v2.tif Figure_3_Hillshade_Kossou_1609.jpg
-python plot_hillshade.py --azimuth 230 --colormap plasma n07_w006_3arc_v2.tif Figure_4_Azimuth_hillshade_Kossou.jpg
-python plot_hillshade.py --altitude 10 --colormap magma n07_w006_3arc_v2.tif Figure_5_Angle_hillshade_Kossou.jpg
+
+In fact, the geotiff file `n07_w006_3arc_v2.tif` is included in the `kossou-hillshade-base` package, so this will also work:
+```sh
+kossou-hillshade --colormap cividis Figure_3_Hillshade_Kossou_1609.jpg
+kossou-hillshade --azimuth 230 --colormap plasma Figure_4_Azimuth_hillshade_Kossou.jpg
+kossou-hillshade --altitude 10 --colormap magma Figure_5_Angle_hillshade_Kossou.jpg
 ```
 
 [^1]: Polina Lemenkova and Olivier Debeir, [Satellite Image Processing by Python and R Using Landsat 9 OLI/TIRS and SRTM DEM Data on Côte d’Ivoire, West Africa](https://www.mdpi.com/2313-433X/8/12/317). J. Imaging 2022
```

