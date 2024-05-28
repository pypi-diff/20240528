# Comparing `tmp/brainglobe-heatmap-0.5.2.tar.gz` & `tmp/brainglobe_heatmap-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-heatmap-0.5.2.tar", last modified: Thu Dec 21 14:47:10 2023, max compression
+gzip compressed data, was "brainglobe_heatmap-0.5.3.tar", last modified: Tue May 28 10:46:55 2024, max compression
```

## Comparing `brainglobe-heatmap-0.5.2.tar` & `brainglobe_heatmap-0.5.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:47:10.567639 brainglobe-heatmap-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:47:10.563639 brainglobe-heatmap-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:47:10.563639 brainglobe-heatmap-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2023-12-21 14:47:10.567639 brainglobe-heatmap-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:47:10.563639 brainglobe-heatmap-0.5.2/brainglobe_heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:47:10.563639 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2023-12-21 14:47:10.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-21 14:47:10.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 14:47:10.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-21 14:47:10.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-21 14:47:10.000000 brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-21 14:47:03.000000 brainglobe-heatmap-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 14:47:10.567639 brainglobe-heatmap-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:46:55.825127 brainglobe_heatmap-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:46:55.821127 brainglobe_heatmap-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:46:55.821127 brainglobe_heatmap-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-28 10:46:55.825127 brainglobe_heatmap-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:46:55.821127 brainglobe_heatmap-0.5.3/brainglobe_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap/planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:46:55.821127 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-28 10:46:55.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-28 10:46:55.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:46:55.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 10:46:55.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 10:46:55.000000 brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-28 10:46:51.000000 brainglobe_heatmap-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 10:46:55.825127 brainglobe_heatmap-0.5.3/setup.cfg
```

### Comparing `brainglobe-heatmap-0.5.2/.github/workflows/test_and_deploy.yml` & `brainglobe_heatmap-0.5.3/.github/workflows/test_and_deploy.yml`

 * *Files 21% similar despite different names*

```diff
@@ -27,24 +27,37 @@
     strategy:
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
         # Include one windows and macos run
         include:
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.10"
+        - os: macos-latest # ARM Mac
           python-version: "3.10"
         - os: windows-latest
           python-version: "3.10"
 
     steps:
+      - name: Cache brainglobe directory
+        uses: actions/cache@v3
+        with:
+          path: | # ensure we don't cache any interrupted atlas download and extraction, if e.g. we cancel the workflow manually
+            ~/.brainglobe
+            !~/.brainglobe/atlas.tar.gz
+          key: brainglobe
+      - name: install HDF libs on ARM Mac
+        if: matrix.os == 'macos-latest'
+        run: brew install hdf5
       # Run tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
@@ -52,15 +65,10 @@
 
 
   upload_all:
     name: Publish build distributions
     needs: [build_sdist_wheels]
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/download-artifact@v3
-      with:
-        name: artifact
-        path: dist
-    - uses: pypa/gh-action-pypi-publish@v1.5.0
+    - uses: neuroinformatics-unit/actions/upload_pypi@v2
       with:
-        user: __token__
-        password: ${{ secrets.TWINE_API_KEY }}
+        secret-pypi-key: ${{ secrets.TWINE_API_KEY }}
```

### Comparing `brainglobe-heatmap-0.5.2/.gitignore` & `brainglobe_heatmap-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-heatmap-0.5.2/LICENSE` & `brainglobe_heatmap-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-heatmap-0.5.2/PKG-INFO` & `brainglobe_heatmap-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-heatmap
-Version: 0.5.2
+Version: 0.5.3
 Summary: Rendering anatomical heatmaps with brainrender and matplotlib
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/brainglobe-heatmap
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainglobe-heatmap/issues
 Project-URL: Documentation, https://github.com/brainglobe/brainglobe-heatmap
 Project-URL: Source Code, https://github.com/brainglobe/brainglobe-heatmap
@@ -105,51 +105,55 @@
 ```
 
 The position of the center of the plane is given by a set of `(x, y, z)` coordinates. The orientation can be specified by a string (`frontal`, `sagittal`, `horizontal`) which will result in a standard orthogonal slice, or by a vector `(x, y, z)` with the orientation along the 3 axes.
 
 Whe using one of the named orientation, you don't need to pass a whole set of `(x, y, z)` coordinates for the plane center. A single value is sufficient as the other two won't affect the plane position:
 
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=1000,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="allen_cord_20um",
     format='2D',
 ).show()
 
 ```
 
 Also, you can create a slice with a plane centered in the brain by passing `position=None`:
+
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=None,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="mpin_zfish_1um",
     format='2D',
     title='zebra fish heatmap'
 ).show(xlabel='AP (μm)', ylabel='DV (μm)')
 ```
 
 ### Visualization
 Once happy with the position of the slicing planes, creating a visualization is as simple as:
 
 ```python
 
-bgh.heatmap(
+bgh.Heatmap(
     values,
     position=(
         8000,
         5000,
         5000,
     ),
-    orientation="horizontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="horizontal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     title="horizontal view",
     vmin=-5,
     vmax=3,
     cmap='Red',
     format="2D",
 ).show()
 ```
@@ -175,20 +179,41 @@
     orientation="frontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
 )
 ```
 
 ## Using `brainglobe-heatmap` with other atlases.
 
 `brainglobe-heatmap` uses `brainrender` which, in turn, uses brainglobe's `Atlas API` under the hood. That means that all of `brainglobe-heatmap`'s functionality is compatible with any of the atlases supported by the atlas API. `bgh.heatmap`, `bgh.planner` and `bgh.get_plane_coordinates` all accept a `atlas_name` argument, pass the name of the atlas name you'd like to use!
-For more information see the API's [documentation](https://brainglobe.info/documentation/bg-atlasapi/index.html).
-
-## Contributing
-Contributions to `brainglobe-heatmap` are more than welcome. Please see the [Developer's guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+For more information see the API's [documentation](https://brainglobe.info/documentation/brainglobe-atlasapi/index.html).
 
 ## Citing `brainglobe-heatmap`
 If you use `brainglobe-heatmap` in your work, please cite it as:
 
 ```
 Federico Claudi, & Luigi Petrucco. (2022). brainglobe/bg-heatmaps: (V0.2). Zenodo. https://doi.org/10.5281/zenodo.5891814
 ```
 
-`brainglobe-heatmap` was originally developed by Federico Claudi and Luigi Petrucco, with the help of Marco Musy (the developer of [`vedo`](https://github.com/marcomusy/vedo))
+If you use `brainrender` via `brainglobe-heatmap` (i.e. for 3D visualisation), please also cite it:
+```
+Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
+```
+
+BibTeX:
+
+``` bibtex
+@article{Claudi2021,
+author = {Claudi, Federico and Tyson, Adam L. and Petrucco, Luigi and Margrie, Troy W. and Portugues, Ruben and Branco, Tiago},
+doi = {10.7554/eLife.65751},
+issn = {2050084X},
+journal = {eLife},
+pages = {1--16},
+pmid = {33739286},
+title = {{Visualizing anatomically registered data with brainrender}},
+volume = {10},
+year = {2021}
+}
+
+```
+
+## Contributing
+
+Contributions to brainrender are more than welcome. Please see the [developers guide](https://brainglobe.info/community/developers/index.html).
```

### Comparing `brainglobe-heatmap-0.5.2/README.md` & `brainglobe_heatmap-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,51 +67,55 @@
 ```
 
 The position of the center of the plane is given by a set of `(x, y, z)` coordinates. The orientation can be specified by a string (`frontal`, `sagittal`, `horizontal`) which will result in a standard orthogonal slice, or by a vector `(x, y, z)` with the orientation along the 3 axes.
 
 Whe using one of the named orientation, you don't need to pass a whole set of `(x, y, z)` coordinates for the plane center. A single value is sufficient as the other two won't affect the plane position:
 
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=1000,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="allen_cord_20um",
     format='2D',
 ).show()
 
 ```
 
 Also, you can create a slice with a plane centered in the brain by passing `position=None`:
+
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=None,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="mpin_zfish_1um",
     format='2D',
     title='zebra fish heatmap'
 ).show(xlabel='AP (μm)', ylabel='DV (μm)')
 ```
 
 ### Visualization
 Once happy with the position of the slicing planes, creating a visualization is as simple as:
 
 ```python
 
-bgh.heatmap(
+bgh.Heatmap(
     values,
     position=(
         8000,
         5000,
         5000,
     ),
-    orientation="horizontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="horizontal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     title="horizontal view",
     vmin=-5,
     vmax=3,
     cmap='Red',
     format="2D",
 ).show()
 ```
@@ -137,20 +141,41 @@
     orientation="frontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
 )
 ```
 
 ## Using `brainglobe-heatmap` with other atlases.
 
 `brainglobe-heatmap` uses `brainrender` which, in turn, uses brainglobe's `Atlas API` under the hood. That means that all of `brainglobe-heatmap`'s functionality is compatible with any of the atlases supported by the atlas API. `bgh.heatmap`, `bgh.planner` and `bgh.get_plane_coordinates` all accept a `atlas_name` argument, pass the name of the atlas name you'd like to use!
-For more information see the API's [documentation](https://brainglobe.info/documentation/bg-atlasapi/index.html).
-
-## Contributing
-Contributions to `brainglobe-heatmap` are more than welcome. Please see the [Developer's guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+For more information see the API's [documentation](https://brainglobe.info/documentation/brainglobe-atlasapi/index.html).
 
 ## Citing `brainglobe-heatmap`
 If you use `brainglobe-heatmap` in your work, please cite it as:
 
 ```
 Federico Claudi, & Luigi Petrucco. (2022). brainglobe/bg-heatmaps: (V0.2). Zenodo. https://doi.org/10.5281/zenodo.5891814
 ```
 
-`brainglobe-heatmap` was originally developed by Federico Claudi and Luigi Petrucco, with the help of Marco Musy (the developer of [`vedo`](https://github.com/marcomusy/vedo))
+If you use `brainrender` via `brainglobe-heatmap` (i.e. for 3D visualisation), please also cite it:
+```
+Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
+```
+
+BibTeX:
+
+``` bibtex
+@article{Claudi2021,
+author = {Claudi, Federico and Tyson, Adam L. and Petrucco, Luigi and Margrie, Troy W. and Portugues, Ruben and Branco, Tiago},
+doi = {10.7554/eLife.65751},
+issn = {2050084X},
+journal = {eLife},
+pages = {1--16},
+pmid = {33739286},
+title = {{Visualizing anatomically registered data with brainrender}},
+volume = {10},
+year = {2021}
+}
+
+```
+
+## Contributing
+
+Contributions to brainrender are more than welcome. Please see the [developers guide](https://brainglobe.info/community/developers/index.html).
```

### Comparing `brainglobe-heatmap-0.5.2/brainglobe_heatmap/heatmaps.py` & `brainglobe_heatmap-0.5.3/brainglobe_heatmap/heatmaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,18 +44,18 @@
     not_nan = [v for v in values.values() if not np.isnan(v)]
     if len(not_nan) == 0:
         return np.nan, np.nan
     vmax, vmin = max(not_nan), min(not_nan)
     return vmax, vmin
 
 
-class heatmap:
+class Heatmap:
     def __init__(
         self,
-        values: Dict[str, float],
+        values: Dict,
         position: Union[list, tuple, np.ndarray],
         orientation: Union[str, tuple] = "frontal",
         hemisphere: str = "both",
         title: Optional[str] = None,
         cmap: str = "Reds",
         vmin: Optional[float] = None,
         vmax: Optional[float] = None,
@@ -117,15 +117,15 @@
         vmax = vmax if vmax == 0 or vmax else _vmax
         self.vmin, self.vmax = vmin, vmax
 
         self.colors = {
             r: list(map_color(v, name=cmap, vmin=vmin, vmax=vmax))
             for r, v in values.items()
         }
-        self.colors["root"] = grey_darker
+        self.colors["root"] = settings.ROOT_COLOR
 
     def show(self, **kwargs) -> Union[Scene, plt.Figure]:
         """
         Creates a 2D plot or 3D rendering of the heatmap
         """
         if self.format == "3D":
             self.slicer.slice_scene(self.scene, self.regions_meshes)
@@ -249,44 +249,7 @@
             plt.savefig(filename, dpi=300)
 
         if show_legend:
             ax.legend()
         plt.show()
 
         return f
-
-
-if __name__ == "__main__":
-    values = dict(  # scalar values for each region
-        TH=1,
-        RSP=0.2,
-        AI=0.4,
-        SS=-3,
-        MO=2.6,
-        PVZ=-4,
-        LZ=-3,
-        VIS=2,
-        AUD=0.3,
-        RHP=-0.2,
-        STR=0.5,
-        CB=0.5,
-        FRP=-1.7,
-        HIP=3,
-        PA=-4,
-    )
-
-    heatmap(
-        values,
-        position=None,
-        # or 'sagittal', or 'horizontal' or a tuple (x,y,z)
-        orientation=(
-            1,
-            1,
-            0,
-        ),
-        # thickness of the slices used for rendering (in microns)
-        thickness=250,
-        title="frontal",
-        vmin=-5,
-        vmax=3,
-        format="3D",
-    ).show()
```

### Comparing `brainglobe-heatmap-0.5.2/brainglobe_heatmap/plane.py` & `brainglobe_heatmap-0.5.3/brainglobe_heatmap/plane.py`

 * *Files identical despite different names*

### Comparing `brainglobe-heatmap-0.5.2/brainglobe_heatmap/slicer.py` & `brainglobe_heatmap-0.5.3/brainglobe_heatmap/slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Computes the position of two planes given a point (position) and an
         orientation (named orientation or
         3D vector) + thickness (spacing between the two planes)
         """
         if position is None:
             position = root.center_of_mass()
 
-        if isinstance(position, (float, int)):
+        if isinstance(position, (float, int, np.number)):
             if isinstance(orientation, str):
                 pval = position
                 position = root.center_of_mass()
                 position[get_ax_idx(orientation)] = pval
             else:
                 raise ValueError(
                     "When a single float value is passed for "
@@ -64,15 +64,15 @@
             # get the two planes
             # assures that u0×v0 is all-positive -> it's for plane0
             if orientation == "frontal":
                 u0, v0 = np.array([[0, 0, -1], [0, 1, 0]])
             elif orientation == "sagittal":
                 u0, v0 = np.array([[1, 0, 0], [0, 1, 0]])
             else:  # orientation == "horizontal"
-                u0, v0 = np.array([[0, 0, -1], [-1, 0, 0]])
+                u0, v0 = np.array([[0, 0, 1], [1, 0, 0]])
             plane0 = Plane(position, u0, v0)
             u1, v1 = u0.copy(), -v0.copy()  # set u1:=u0 and v1:=-v0
             plane1 = Plane(p1, u1, v1)
         else:
             orientation = np.array(orientation)
 
             p1 = position + orientation * thickness  # type: ignore
@@ -132,15 +132,15 @@
                 scene.remove(region)
 
     def slice_scene(self, scene: Scene, regions: List[Actor]):
         """
         Slices the meshes in a 3D brainrender scene using the gien planes
         """
         # slice the scene
-        for n, plane in enumerate((self.plane0, self.plane1)):
+        for _, plane in enumerate((self.plane0, self.plane1)):
             scene.slice(plane, actors=regions, close_actors=True)
 
         scene.slice(self.plane0, actors=scene.root, close_actors=False)
 
 
 def get_structures_slice_coords(
     regions: List[str],
```

### Comparing `brainglobe-heatmap-0.5.2/brainglobe_heatmap.egg-info/PKG-INFO` & `brainglobe_heatmap-0.5.3/brainglobe_heatmap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-heatmap
-Version: 0.5.2
+Version: 0.5.3
 Summary: Rendering anatomical heatmaps with brainrender and matplotlib
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/brainglobe-heatmap
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainglobe-heatmap/issues
 Project-URL: Documentation, https://github.com/brainglobe/brainglobe-heatmap
 Project-URL: Source Code, https://github.com/brainglobe/brainglobe-heatmap
@@ -105,51 +105,55 @@
 ```
 
 The position of the center of the plane is given by a set of `(x, y, z)` coordinates. The orientation can be specified by a string (`frontal`, `sagittal`, `horizontal`) which will result in a standard orthogonal slice, or by a vector `(x, y, z)` with the orientation along the 3 axes.
 
 Whe using one of the named orientation, you don't need to pass a whole set of `(x, y, z)` coordinates for the plane center. A single value is sufficient as the other two won't affect the plane position:
 
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=1000,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="allen_cord_20um",
     format='2D',
 ).show()
 
 ```
 
 Also, you can create a slice with a plane centered in the brain by passing `position=None`:
+
 ```python
-f = bgh.heatmap(
+f = bgh.Heatmap(
     values,
     position=None,
-    orientation="sagittal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="sagittal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     thickness=1000,
     atlas_name="mpin_zfish_1um",
     format='2D',
     title='zebra fish heatmap'
 ).show(xlabel='AP (μm)', ylabel='DV (μm)')
 ```
 
 ### Visualization
 Once happy with the position of the slicing planes, creating a visualization is as simple as:
 
 ```python
 
-bgh.heatmap(
+bgh.Heatmap(
     values,
     position=(
         8000,
         5000,
         5000,
     ),
-    orientation="horizontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
+    orientation="horizontal",
+    # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
     title="horizontal view",
     vmin=-5,
     vmax=3,
     cmap='Red',
     format="2D",
 ).show()
 ```
@@ -175,20 +179,41 @@
     orientation="frontal",  # 'frontal' or 'sagittal', or 'horizontal' or a tuple (x,y,z)
 )
 ```
 
 ## Using `brainglobe-heatmap` with other atlases.
 
 `brainglobe-heatmap` uses `brainrender` which, in turn, uses brainglobe's `Atlas API` under the hood. That means that all of `brainglobe-heatmap`'s functionality is compatible with any of the atlases supported by the atlas API. `bgh.heatmap`, `bgh.planner` and `bgh.get_plane_coordinates` all accept a `atlas_name` argument, pass the name of the atlas name you'd like to use!
-For more information see the API's [documentation](https://brainglobe.info/documentation/bg-atlasapi/index.html).
-
-## Contributing
-Contributions to `brainglobe-heatmap` are more than welcome. Please see the [Developer's guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+For more information see the API's [documentation](https://brainglobe.info/documentation/brainglobe-atlasapi/index.html).
 
 ## Citing `brainglobe-heatmap`
 If you use `brainglobe-heatmap` in your work, please cite it as:
 
 ```
 Federico Claudi, & Luigi Petrucco. (2022). brainglobe/bg-heatmaps: (V0.2). Zenodo. https://doi.org/10.5281/zenodo.5891814
 ```
 
-`brainglobe-heatmap` was originally developed by Federico Claudi and Luigi Petrucco, with the help of Marco Musy (the developer of [`vedo`](https://github.com/marcomusy/vedo))
+If you use `brainrender` via `brainglobe-heatmap` (i.e. for 3D visualisation), please also cite it:
+```
+Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
+```
+
+BibTeX:
+
+``` bibtex
+@article{Claudi2021,
+author = {Claudi, Federico and Tyson, Adam L. and Petrucco, Luigi and Margrie, Troy W. and Portugues, Ruben and Branco, Tiago},
+doi = {10.7554/eLife.65751},
+issn = {2050084X},
+journal = {eLife},
+pages = {1--16},
+pmid = {33739286},
+title = {{Visualizing anatomically registered data with brainrender}},
+volume = {10},
+year = {2021}
+}
+
+```
+
+## Contributing
+
+Contributions to brainrender are more than welcome. Please see the [developers guide](https://brainglobe.info/community/developers/index.html).
```

### Comparing `brainglobe-heatmap-0.5.2/pyproject.toml` & `brainglobe_heatmap-0.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "brainglobe-heatmap"
-authors = [{name = "Federico Claudi", email= "hello@brainglobe.info"}]
+authors = [{ name = "Federico Claudi", email = "hello@brainglobe.info" }]
 description = "Rendering anatomical heatmaps with brainrender and matplotlib"
 readme = "README.md"
 requires-python = ">=3.9.0"
 dynamic = ["version"]
 
 dependencies = ["brainrender", "matplotlib", "numpy", "myterial", "rich"]
 
-license = {text = "MIT"}
+license = { text = "MIT" }
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -26,32 +26,28 @@
 "Bug Tracker" = "https://github.com/brainglobe/brainglobe-heatmap/issues"
 "Documentation" = "https://github.com/brainglobe/brainglobe-heatmap"
 "Source Code" = "https://github.com/brainglobe/brainglobe-heatmap"
 "User Support" = "https://github.com/brainglobe/brainglobe-heatmap/issues"
 
 [project.optional-dependencies]
 dev = [
-  "pytest",
-  "pytest-cov",
-  "coverage",
-  "tox",
-  "black",
-  "mypy",
-  "pre-commit",
-  "ruff",
-  "setuptools_scm",
+    "pytest",
+    "pytest-cov",
+    "coverage",
+    "tox",
+    "black",
+    "mypy",
+    "pre-commit",
+    "ruff",
+    "setuptools_scm",
 ]
 
 
 [build-system]
-requires = [
-    "setuptools>=45",
-    "wheel",
-    "setuptools_scm[toml]>=6.2",
-]
+requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["brainglobe_heatmap*"]
@@ -65,27 +61,29 @@
 skip-string-normalization = false
 line-length = 79
 
 [tool.setuptools_scm]
 
 [tool.check-manifest]
 ignore = [
-  ".yaml",
-  "tox.ini",
-  "tests/",
-  "tests/test_unit/",
-  "tests/test_integration/",
+    ".yaml",
+    "tox.ini",
+    "tests/",
+    "tests/test_unit/",
+    "tests/test_integration/",
 ]
 
 [tool.ruff]
 line-length = 79
-exclude = ["__init__.py","build",".eggs"]
-select = ["I", "E", "F"]
+exclude = ["__init__.py", "build", ".eggs"]
 fix = true
 
+[tool.ruff.lint]
+select = ["I", "E", "F", "B"]
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py{39,310,311}
 isolated_build = True
 
 [gh-actions]
```

