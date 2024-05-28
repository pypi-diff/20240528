# Comparing `tmp/kossou_hillshade_cli-0.0.2.tar.gz` & `tmp/kossou_hillshade_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kossou_hillshade_cli-0.0.2.tar", last modified: Tue May 28 04:33:46 2024, max compression
+gzip compressed data, was "kossou_hillshade_cli-0.0.3.tar", last modified: Tue May 28 05:26:22 2024, max compression
```

## Comparing `kossou_hillshade_cli-0.0.2.tar` & `kossou_hillshade_cli-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.008200 kossou_hillshade_cli-0.0.2/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 04:03:41.000000 kossou_hillshade_cli-0.0.2/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:33:46.007728 kossou_hillshade_cli-0.0.2/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 04:04:58.000000 kossou_hillshade_cli-0.0.2/README.md
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 04:31:06.000000 kossou_hillshade_cli-0.0.2/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 04:33:46.008307 kossou_hillshade_cli-0.0.2/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 04:05:46.000000 kossou_hillshade_cli-0.0.2/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:45.998472 kossou_hillshade_cli-0.0.2/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.001568 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 04:16:31.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2230 2024-05-28 04:30:47.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/kossou_hillshade_cli.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 04:31:09.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 04:33:46.006679 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 04:33:45.000000 kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.063624 kossou_hillshade_cli-0.0.3/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       20 2024-05-28 04:03:41.000000 kossou_hillshade_cli-0.0.3/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 05:26:22.063102 kossou_hillshade_cli-0.0.3/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2688 2024-05-28 04:04:58.000000 kossou_hillshade_cli-0.0.3/README.md
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      868 2024-05-28 05:07:38.000000 kossou_hillshade_cli-0.0.3/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2024-05-28 05:26:22.063722 kossou_hillshade_cli-0.0.3/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2024-05-28 04:05:46.000000 kossou_hillshade_cli-0.0.3/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.053648 kossou_hillshade_cli-0.0.3/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.058157 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      235 2024-05-28 04:16:31.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3112 2024-05-28 05:24:57.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/kossou_hillshade_cli.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2024-05-28 05:07:43.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2024-05-28 05:26:22.062375 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3314 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      457 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       84 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       29 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       21 2024-05-28 05:26:22.000000 kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/top_level.txt
```

### Comparing `kossou_hillshade_cli-0.0.2/PKG-INFO` & `kossou_hillshade_cli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `kossou_hillshade_cli-0.0.2/README.md` & `kossou_hillshade_cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kossou_hillshade_cli-0.0.2/pyproject.toml` & `kossou_hillshade_cli-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kossou-hillshade-cli"
-version = "0.0.2" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.0.3" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="anthony.aylward@protonmail.com" },
 ]
 description = "Plot hillshade over Lake Kossou using satellite elevation data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli/kossou_hillshade_cli.py` & `kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli/kossou_hillshade_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,40 +7,69 @@
 import misaka as m
 import os
 import os.path
 
 from argparse import ArgumentParser
 
 from kossou_hillshade_base import (AZIMUTH, ALTITUDE, WIDTH, HEIGHT,
-                                   DEFAULT_ELEVATION_TIFF, REPORT,
+                                   DEFAULT_ELEVATION_TIFF, DEFAULT_COLORMAP,
                                    plot_hillshade, generate_report)
 
 
 # Functions ====================================================================
 
 def parse_arguments():
     parser = ArgumentParser(description='Elevation data')
     parser.add_argument(
         'report_dir',
         metavar='<path/to/report/dir/>',
         nargs='?',
         help='write a HTML report'
     )
     parser.add_argument(
+        '--geotiff',
+        metavar='<path/to/geotiff.tif>',
+        default=DEFAULT_ELEVATION_TIFF,
+        help='input geotiff file'
+    )
+    parser.add_argument(
         '--azimuth',
-        metavar='int',
+        metavar='<int>',
         default=AZIMUTH,
         help='azimuth of sun'
     )
     parser.add_argument(
         '--altitude',
-        metavar='int',
+        metavar='<int>',
         default=ALTITUDE,
         help="angle altitude of sun"
     )
+    parser.add_argument(
+        '--width',
+        metavar='<int>',
+        default=WIDTH,
+        help='width of plot in inches [10]'
+    )
+    parser.add_argument(
+        '--height',
+        metavar='<int>',
+        default=HEIGHT,
+        help='height of plot in inches [10]'
+    )
+    parser.add_argument(
+        '--title',
+        metavar='<"title of plot">',
+        help='title of plot'
+    )
+    parser.add_argument(
+        '--colormap',
+        metavar='<"colormap">',
+        default=DEFAULT_COLORMAP,
+        help='colormap to use, e.g. "cividis", "plasma", or "magma" [plasma]'
+    )
     return parser.parse_args()
 
 
 def main():
     args = parse_arguments()
     if not args.report_dir:
         report_text = generate_report(
@@ -52,19 +81,22 @@
         report_text = generate_report(
             azimuth=args.azimuth,
             altitude=args.altitude
         )
         if not os.path.isdir(args.report_dir):
             os.mkdir(args.report_dir)
         plot_hillshade(
-            DEFAULT_ELEVATION_TIFF,
+            args.geotiff,
             os.path.join(args.report_dir, 'hillshade.jpg'),
             azimuth=args.azimuth,
             altitude=args.altitude,
-            title=f"Hillshade from DTM of Lake Kossou. Azimuth of sun is {args.azimuth} \N{DEGREE SIGN}, altitude is {args.altitude} \N{DEGREE SIGN}.",
+            width=args.width,
+            height=args.height,
+            title=args.title or f"Hillshade from DTM of Lake Kossou. Azimuth of sun is {args.azimuth} \N{DEGREE SIGN}, altitude is {args.altitude} \N{DEGREE SIGN}.",
+            colormap=args.colormap
         )
         with open(os.path.join(args.report_dir, 'kossou-hillshade.html'), 'w') as f:
             f.write(m.html(report_text, extensions=['tables']))
 
 
 # Execute ======================================================================
```

### Comparing `kossou_hillshade_cli-0.0.2/src/kossou_hillshade_cli.egg-info/PKG-INFO` & `kossou_hillshade_cli-0.0.3/src/kossou_hillshade_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kossou-hillshade-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plot hillshade over Lake Kossou using satellite elevation data
 Author-email: Anthony Aylward <anthony.aylward@protonmail.com>
 Project-URL: Homepage, https://https://gitlab.com/aaylward/kossou-hillshade-cli
 Project-URL: Documentation, https://aaylward.gitlab.io/kossou-hillshade-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

