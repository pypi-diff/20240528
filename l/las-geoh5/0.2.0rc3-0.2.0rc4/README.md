# Comparing `tmp/las_geoh5-0.2.0rc3.tar.gz` & `tmp/las_geoh5-0.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las_geoh5-0.2.0rc3.tar", max compression
+gzip compressed data, was "las_geoh5-0.2.0rc4.tar", max compression
```

## Comparing `las_geoh5-0.2.0rc3.tar` & `las_geoh5-0.2.0rc4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      702 2024-05-13 19:27:23.598067 las_geoh5-0.2.0rc3/las_geoh5/__init__.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc3/las_geoh5/export_files/__init__.py
--rw-r--r--   0        0        0     2262 2024-05-14 20:25:48.897070 las_geoh5-0.2.0rc3/las_geoh5/export_files/driver.py
--rw-r--r--   0        0        0     1264 2024-05-14 18:03:54.730380 las_geoh5-0.2.0rc3/las_geoh5/export_files/uijson.py
--rw-r--r--   0        0        0     6748 2024-05-14 18:18:52.463471 las_geoh5-0.2.0rc3/las_geoh5/export_las.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc3/las_geoh5/import_directories/__init__.py
--rw-r--r--   0        0        0     2300 2024-05-14 20:25:48.898069 las_geoh5-0.2.0rc3/las_geoh5/import_directories/driver.py
--rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc3/las_geoh5/import_directories/uijson.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc3/las_geoh5/import_files/__init__.py
--rw-r--r--   0        0        0     5797 2024-05-14 20:56:13.468616 las_geoh5-0.2.0rc3/las_geoh5/import_files/driver.py
--rw-r--r--   0        0        0     1468 2024-05-14 18:03:54.747566 las_geoh5-0.2.0rc3/las_geoh5/import_files/params.py
--rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc3/las_geoh5/import_files/uijson.py
--rw-r--r--   0        0        0    13319 2024-05-14 18:03:54.762581 las_geoh5-0.2.0rc3/las_geoh5/import_las.py
--rw-r--r--   0        0        0      237 2024-05-13 17:12:35.795341 las_geoh5-0.2.0rc3/las_geoh5/scripts/__init__.py
--rw-r--r--   0        0        0     1390 2024-05-14 16:07:37.620031 las_geoh5-0.2.0rc3/las_geoh5/scripts/geoh5_to_las.py
--rw-r--r--   0        0        0     1826 2024-05-14 16:07:37.539510 las_geoh5-0.2.0rc3/las_geoh5/scripts/las_to_geoh5.py
--rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc3/las_geoh5/uijson/__init__.py
--rw-r--r--   0        0        0     2119 2024-05-14 18:03:54.739474 las_geoh5-0.2.0rc3/las_geoh5/uijson/write_uijson.py
--rw-r--r--   0        0        0      122 2024-05-14 04:22:36.345473 las_geoh5-0.2.0rc3/las_geoh5-assets/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-02 03:50:51.043275 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/export_las_files.ui.json
--rw-r--r--   0        0        0      976 2024-05-02 03:50:51.044307 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_directories.ui.json
--rw-r--r--   0        0        0     2656 2024-05-02 03:50:51.045439 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_files.ui.json
--rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 las_geoh5-0.2.0rc3/LICENSE
--rw-r--r--   0        0        0     2875 2024-05-13 19:29:43.964478 las_geoh5-0.2.0rc3/pyproject.toml
--rw-r--r--   0        0        0     5588 2024-05-14 04:13:37.741819 las_geoh5-0.2.0rc3/README.rst
--rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      702 2024-05-28 15:21:03.327584 las_geoh5-0.2.0rc4/las_geoh5/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-21 20:57:00.583221 las_geoh5-0.2.0rc4/las_geoh5/export_files/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/export_files/driver.py
+-rw-r--r--   0        0        0     1264 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/export_files/uijson.py
+-rw-r--r--   0        0        0     6748 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/export_las.py
+-rw-r--r--   0        0        0      240 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/import_directories/__init__.py
+-rw-r--r--   0        0        0     2308 2024-05-28 14:50:59.422649 las_geoh5-0.2.0rc4/las_geoh5/import_directories/driver.py
+-rw-r--r--   0        0        0     1057 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/import_directories/uijson.py
+-rw-r--r--   0        0        0      240 2024-05-21 20:57:00.584005 las_geoh5-0.2.0rc4/las_geoh5/import_files/__init__.py
+-rw-r--r--   0        0        0     5814 2024-05-28 14:50:59.422649 las_geoh5-0.2.0rc4/las_geoh5/import_files/driver.py
+-rw-r--r--   0        0        0     1468 2024-05-21 20:57:00.585201 las_geoh5-0.2.0rc4/las_geoh5/import_files/params.py
+-rw-r--r--   0        0        0     3080 2024-05-21 20:57:00.585201 las_geoh5-0.2.0rc4/las_geoh5/import_files/uijson.py
+-rw-r--r--   0        0        0    13935 2024-05-28 14:50:59.422649 las_geoh5-0.2.0rc4/las_geoh5/import_las.py
+-rw-r--r--   0        0        0      237 2024-05-21 20:57:00.585201 las_geoh5-0.2.0rc4/las_geoh5/scripts/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-21 20:57:00.585201 las_geoh5-0.2.0rc4/las_geoh5/scripts/geoh5_to_las.py
+-rw-r--r--   0        0        0     1826 2024-05-21 20:57:00.585874 las_geoh5-0.2.0rc4/las_geoh5/scripts/las_to_geoh5.py
+-rw-r--r--   0        0        0      122 2024-05-21 20:57:00.585874 las_geoh5-0.2.0rc4/las_geoh5/uijson/__init__.py
+-rw-r--r--   0        0        0     2119 2024-05-21 20:57:00.585874 las_geoh5-0.2.0rc4/las_geoh5/uijson/write_uijson.py
+-rw-r--r--   0        0        0      122 2024-05-21 20:57:00.581010 las_geoh5-0.2.0rc4/las_geoh5-assets/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-21 20:57:00.583221 las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/export_las_files.ui.json
+-rw-r--r--   0        0        0      976 2024-05-21 20:57:00.583221 las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/import_las_directories.ui.json
+-rw-r--r--   0        0        0     2656 2024-05-21 20:57:00.583221 las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/import_las_files.ui.json
+-rw-r--r--   0        0        0     1093 2024-05-21 20:57:00.562273 las_geoh5-0.2.0rc4/LICENSE
+-rw-r--r--   0        0        0     2875 2024-05-28 15:21:03.338115 las_geoh5-0.2.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     5588 2024-05-21 20:57:00.563659 las_geoh5-0.2.0rc4/README.rst
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc4/PKG-INFO
```

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/__init__.py` & `las_geoh5-0.2.0rc4/las_geoh5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # flake8: noqa
 
 from __future__ import annotations
 
 from pathlib import Path
 
-__version__ = "0.2.0-rc.3"
+__version__ = "0.2.0-rc.4"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     parent = Path(__file__).parent
     folder_name = f"{parent.name}-assets"
```

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/export_files/driver.py` & `las_geoh5-0.2.0rc4/las_geoh5/export_files/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/export_files/uijson.py` & `las_geoh5-0.2.0rc4/las_geoh5/export_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/export_las.py` & `las_geoh5-0.2.0rc4/las_geoh5/export_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_directories/driver.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_directories/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         for file in [k for k in prop.iterdir() if k.suffix == ".las"]:
             lasfiles.append(lasio.read(file, mnemonic_case="preserve"))
         print(f"Importing property group data from to '{prop.name}'")
         las_to_drillhole(
             lasfiles,
             dh_group,
             prop.name,
-            surveys,
+            surveys=surveys,
             options=ImportOptions(),
         )
 
     return dh_group
 
 
 if __name__ == "__main__":
```

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_directories/uijson.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_directories/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_files/driver.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_files/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,8 +161,9 @@
         geoh5.h5file.unlink()
         workspace.save_as(geoh5_path)
 
     workspace.close()
 
 
 if __name__ == "__main__":
-    run(Path(sys.argv[1]))
+    FILE = sys.argv[1]
+    run(Path(FILE))
```

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_files/params.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_files/params.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_files/uijson.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/import_las.py` & `las_geoh5-0.2.0rc4/las_geoh5/import_las.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,52 +344,71 @@
     return drillhole
 
 
 def las_to_drillhole(
     data: lasio.LASFile | list[lasio.LASFile],
     drillhole_group: DrillholeGroup,
     property_group: str,
-    survey: Path | list[Path] | None = None,
+    surveys: Path | list[Path] | None = None,
     logger: logging.Logger | None = None,
     options: ImportOptions | None = None,
 ):
     """
     Import a LAS file containing collocated datasets for a single drillhole.
 
     :param data: Las file(s) containing drillhole data.
     :param drillhole_group: Drillhole group container.
     :param property_group: Property group name.
-    :param survey: Path to a survey file stored as .csv or .las format.
+    :param surveys: Path to a survey file stored as .csv or .las format.
     :param logger: Logger object if warnings are enabled.
     :param options: Import options covering name translations, collocation
         tolerance, and warnings control.
 
     :return: A :obj:`geoh5py.objects.Drillhole` object
     """
 
     if options is None:
         options = ImportOptions()
 
     translator = LASTranslator(names=options.names)
 
     if not isinstance(data, list):
         data = [data]
-    if not isinstance(survey, list):
-        survey = [survey] if survey else []
+    if not isinstance(surveys, list):
+        surveys = [surveys] if surveys else []
 
     for datum in tqdm(data, desc="Adding drillholes and data to workspace"):
         collar = get_collar(datum, translator, logger)
         if all(k == 0 for k in collar) and options.skip_empty_header:
             continue
 
-        drillhole = create_or_append_drillhole(
+        create_or_append_drillhole(
             datum,
             drillhole_group,
             property_group,
             translator=translator,
             logger=logger,
             collocation_tolerance=options.collocation_tolerance,
         )
-        ind = [drillhole.name == s.name.rstrip(".las") for s in survey]
-        if any(ind):
-            survey_path = survey[np.where(ind)[0][0]]
-            _ = add_survey(survey_path, drillhole, logger)
+
+    for drillhole in tqdm(drillhole_group.children, desc="Attaching survey data."):
+
+        survey = [
+            survey for survey in surveys if drillhole.name == survey.name.rstrip(".las")
+        ]
+
+        if any(survey):
+            _ = add_survey(survey[0], drillhole, logger)
+
+        elif len(drillhole.surveys) == 1:
+            depths = []
+            if drillhole.depth_ is not None:
+                depths = [depth.values.max() for depth in drillhole.depth_]
+            elif drillhole.to_ is not None:
+                depths = [depth.values.max() for depth in drillhole.to_]
+
+            if len(depths) == 0:
+                continue
+
+            new_row = drillhole.surveys[0, :]
+            new_row[0] = np.max(depths)
+            drillhole.surveys = np.vstack([drillhole.surveys, new_row])
```

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/scripts/geoh5_to_las.py` & `las_geoh5-0.2.0rc4/las_geoh5/scripts/geoh5_to_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/scripts/las_to_geoh5.py` & `las_geoh5-0.2.0rc4/las_geoh5/scripts/las_to_geoh5.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5/uijson/write_uijson.py` & `las_geoh5-0.2.0rc4/las_geoh5/uijson/write_uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/export_las_files.ui.json` & `las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/export_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_directories.ui.json` & `las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/import_las_directories.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_files.ui.json` & `las_geoh5-0.2.0rc4/las_geoh5-assets/uijson/import_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/LICENSE` & `las_geoh5-0.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/pyproject.toml` & `las_geoh5-0.2.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "las-geoh5"
-version = "0.2.0-rc.3"
+version = "0.2.0-rc.4"
 description = "Las/Geoh5 conversion"
 license = "MIT"
 readme = "README.rst"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Benjamin Kary <benjamink@mirageoscience.com>"]
 keywords = ["geology", "geophysics", "earth sciences", "io", "data", "interoperability"]
 repository = "https://github.com/MiraGeoscience/las-geoh5"
```

### Comparing `las_geoh5-0.2.0rc3/README.rst` & `las_geoh5-0.2.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc3/PKG-INFO` & `las_geoh5-0.2.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: las-geoh5
-Version: 0.2.0rc3
+Version: 0.2.0rc4
 Summary: Las/Geoh5 conversion
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Keywords: geology,geophysics,earth sciences,io,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
```

