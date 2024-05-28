# Comparing `tmp/lightquakevisualizer-0.0.3.tar.gz` & `tmp/lightquakevisualizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightquakevisualizer-0.0.3.tar", last modified: Tue May 21 12:05:29 2024, max compression
+gzip compressed data, was "lightquakevisualizer-0.0.4.tar", last modified: Tue May 28 13:23:47 2024, max compression
```

## Comparing `lightquakevisualizer-0.0.3.tar` & `lightquakevisualizer-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.3/LICENSE
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.3/README.md
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/lightquakevisualizer/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/__init__.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/generateColorBar.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombiner.py
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombinernew.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23211 2024-05-21 12:02:59.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/lightQuakeVisualizer.py
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/SOURCES.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/entry_points.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/requires.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/top_level.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-05-21 12:05:06.000000 lightquakevisualizer-0.0.3/pyproject.toml
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/setup.cfg
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.4/LICENSE
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.4/README.md
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/lightquakevisualizer/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/__init__.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/generateColorBar.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombiner.py
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombinernew.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23507 2024-05-28 13:22:12.000000 lightquakevisualizer-0.0.4/lightquakevisualizer/lightQuakeVisualizer.py
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/entry_points.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/requires.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-05-28 13:23:47.000000 lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/top_level.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-05-28 13:23:18.000000 lightquakevisualizer-0.0.4/pyproject.toml
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-05-28 13:23:47.670257 lightquakevisualizer-0.0.4/setup.cfg
```

### Comparing `lightquakevisualizer-0.0.3/LICENSE` & `lightquakevisualizer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.3/PKG-INFO` & `lightquakevisualizer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.3/README.md` & `lightquakevisualizer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.3/lightquakevisualizer/generateColorBar.py` & `lightquakevisualizer-0.0.4/lightquakevisualizer/generateColorBar.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombiner.py` & `lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombiner.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombinernew.py` & `lightquakevisualizer-0.0.4/lightquakevisualizer/imageCombinernew.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.3/lightquakevisualizer/lightQuakeVisualizer.py` & `lightquakevisualizer-0.0.4/lightquakevisualizer/lightQuakeVisualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,19 +307,23 @@
             plotter.view_xy()
         case "xz":
             plotter.view_xz()
         case "yz":
             plotter.view_yz()
         case "normal":
             center = mesh.center
-            plane_normal = mesh.compute_normals()["Normals"].mean(axis=0)
-            if plane_normal[2] < 0:
-                plane_normal = -plane_normal
-            plotter.camera.focal_point = center
-            plotter.camera.position = center + plane_normal
+            try:
+                plane_normal = mesh.compute_normals()["Normals"].mean(axis=0)
+                if plane_normal[2] < 0:
+                    plane_normal = -plane_normal
+                plotter.camera.focal_point = center
+                plotter.camera.position = center + plane_normal
+            except AttributeError:
+                print("cannot compute normal, using xy view instead")
+                plotter.view_xy()
         case _:
             if is_pvcc:
                 plotter.camera = pv.Camera.from_paraview_pvcc(view_arg)
             else:
                 raise ValueError(f"unknown view name {view_name}")
 
     plotter.parallel_scale = 1
@@ -343,21 +347,14 @@
         "--annotate_time",
         nargs=1,
         metavar="color xr yr",
         help="Display the time on the plot (xr and yr are relative location of the text)",
     )
 
     parser.add_argument(
-        "--vtk_meshes",
-        nargs=1,
-        metavar="fname color linewidth",
-        help="Plot VTK meshes (e.g. coastline), group of 3 arguments separated by ';'",
-    )
-
-    parser.add_argument(
         "--color_ranges",
         nargs=1,
         help="Color range for each file, separated by ';'",
     )
 
     parser.add_argument(
         "--contours",
@@ -414,22 +411,14 @@
     )
 
     parser.add_argument(
         "--output_prefix", nargs=1, help="Specify output prefix of the snapshot"
     )
 
     parser.add_argument(
-        "--view",
-        nargs=1,
-        default=["normal"],
-        metavar="pvcc_file_or_specific_view",
-        help="Setup the camera view: e.g. normal, xy, xz, yz or path to a pvcc_file",
-    )
-
-    parser.add_argument(
         "--scalar_bar",
         nargs=1,
         metavar="xr yr (height_pxl)",
         help="Show scalar bar",
     )
 
     parser.add_argument(
@@ -461,14 +450,29 @@
         "--variables",
         nargs=1,
         help="Variable(s) to visualize, separated by ';'",
         required=True,
     )
 
     parser.add_argument(
+        "--view",
+        nargs=1,
+        default=["normal"],
+        metavar="pvcc_file_or_specific_view",
+        help="Setup the camera view: e.g. normal, xy, xz, yz or path to a pvcc_file",
+    )
+
+    parser.add_argument(
+        "--vtk_meshes",
+        nargs=1,
+        metavar="fname color linewidth",
+        help="Plot VTK meshes (e.g. coastline), group of 3 arguments separated by ';'",
+    )
+
+    parser.add_argument(
         "--window_size",
         nargs=2,
         metavar=("width", "height"),
         default=([1200, 900]),
         help="Size of the window, in pixels",
         type=int,
     )
@@ -577,15 +581,19 @@
 
             if args.slice:
                 args_slice = [float(v) for v in args.slice[0].split()]
                 enabled_slice = [int(v) for v in args.slice[1].split(";")]
                 if enabled_slice[i]:
                     assert len(args_slice) == 6
                     px, py, pz, nx, ny, nz = args_slice
-                    mesh = mesh.slice(normal=(nx, ny, nz), origin=(px, py, pz))
+                    mesh = mesh.slice(
+                        normal=(nx, ny, nz),
+                        origin=(px, py, pz),
+                        generate_triangles=True,
+                    )
                     assert mesh.n_points > 0
 
             clim_dic = color_ranges[i] if args.color_ranges else {"clim": None}
 
             if args.scalar_bar:
                 sb_args = args.scalar_bar[0].split()
                 height_pxl = int(sb_args[2]) if len(sb_args) == 3 else 150
```

### Comparing `lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/PKG-INFO` & `lightquakevisualizer-0.0.4/lightquakevisualizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.3/pyproject.toml` & `lightquakevisualizer-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightquakevisualizer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Thomas Ulrich"},
 ]
 description = "A collection of scripts to visualize SeisSol output using pyvista"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["pyvista", "SeisSol"]
```

