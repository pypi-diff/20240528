# Comparing `tmp/pv_surrogate_data-1.0.1.tar.gz` & `tmp/pv_surrogate_data-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pv_surrogate_data-1.0.1.tar", max compression
+gzip compressed data, was "pv_surrogate_data-1.0.2.tar", max compression
```

## Comparing `pv_surrogate_data-1.0.1.tar` & `pv_surrogate_data-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4057 2024-05-14 17:09:13.543572 pv_surrogate_data-1.0.1/README.md
--rw-r--r--   0        0        0       33 2024-05-13 14:34:18.405418 pv_surrogate_data-1.0.1/pv_surrogate_data/__init__.py
--rw-r--r--   0        0        0    10151 2024-05-14 16:36:40.860944 pv_surrogate_data-1.0.1/pv_surrogate_data/dataset.py
--rw-r--r--   0        0        0     4115 2024-05-14 11:52:24.713350 pv_surrogate_data-1.0.1/pv_surrogate_data/typedef.py
--rw-r--r--   0        0        0     2549 2024-05-14 17:09:50.488602 pv_surrogate_data-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 pv_surrogate_data-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4057 2024-05-14 17:09:13.543572 pv_surrogate_data-1.0.2/README.md
+-rw-r--r--   0        0        0       33 2024-05-13 14:34:18.405418 pv_surrogate_data-1.0.2/pv_surrogate_data/__init__.py
+-rw-r--r--   0        0        0    10692 2024-05-28 13:20:04.082456 pv_surrogate_data-1.0.2/pv_surrogate_data/dataset.py
+-rw-r--r--   0        0        0     4115 2024-05-14 11:52:24.713350 pv_surrogate_data-1.0.2/pv_surrogate_data/typedef.py
+-rw-r--r--   0        0        0     2549 2024-05-28 13:20:40.423501 pv_surrogate_data-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 pv_surrogate_data-1.0.2/PKG-INFO
```

### Comparing `pv_surrogate_data-1.0.1/README.md` & `pv_surrogate_data-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pv_surrogate_data-1.0.1/pv_surrogate_data/dataset.py` & `pv_surrogate_data-1.0.2/pv_surrogate_data/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,23 @@
 
     def __init__(
         self,
         data_package_structure: DataPackage = DataPackage(),
         module_column_name: str = NormalizedPVGISSchema.power,
         included_data: IncludedData = IncludedData.all,
     ):
+        """
+        Parameters:
+            data_package_structure (DataPackage, optional): The structure of the data package.
+                Defaults to an empty DataPackage.
+            module_column_name (str, optional): The name of the column to use as the target. Can be any column from the PVGIS data
+                Defaults to NormalizedPVGISSchema.power.
+            included_data (IncludedData, optional): The subset of the data to load.
+                Defaults to IncludedData.all.
+        """
         self.data_package = data_package_structure
         self.data_path = data_package_structure.pvgis_data_path
         self.target_column = module_column_name
 
         match included_data:
             case IncludedData.train:
                 self.metadata = pd.read_parquet(
@@ -140,15 +149,17 @@
     This dataset is used to evaluate the models on a fixed location.
     All the time series here are sampled from a single location only
     varying the parameters (kwP, tilt, orientation).
     This is only used for evaluation purposes
     """
 
     def __init__(
-        self, data_package_structure: DataPackage = DataPackage(), module_column_name: str = NormalizedPVGISSchema.power
+        self,
+        data_package_structure: DataPackage = DataPackage(),
+        module_column_name: str = NormalizedPVGISSchema.power,
     ):
         self.data_package = data_package_structure
         self.data_path = data_package_structure.fixed_location_pvgis_data_path
         self.target_column = module_column_name
 
         self.metadata = pd.read_parquet(data_package_structure.system_data_path / "german_fixed_location.parquet")
 
@@ -185,15 +196,17 @@
     and moving outward in increments of 5 kilometers.
 
     File names are expected to be constructed like:
     f'{meta["sample_id"]}_{meta["bearing"]}_{meta["distance"]}.parquet'
     """
 
     def __init__(
-        self, data_package_structure: DataPackage = DataPackage(), module_column_name: str = NormalizedPVGISSchema.power
+        self,
+        data_package_structure: DataPackage = DataPackage(),
+        module_column_name: str = NormalizedPVGISSchema.power,
     ):
         self.data_package = data_package_structure
         self.data_path = data_package_structure.outward_pvgis_data_path
         self.target_column = module_column_name
 
         self.metadata = pd.read_parquet(data_package_structure.system_data_path / "german_outward_points.parquet")
         self.metadata["id"] = self.metadata["sample_id"]
```

### Comparing `pv_surrogate_data-1.0.1/pv_surrogate_data/typedef.py` & `pv_surrogate_data-1.0.2/pv_surrogate_data/typedef.py`

 * *Files identical despite different names*

### Comparing `pv_surrogate_data-1.0.1/pyproject.toml` & `pv_surrogate_data-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "pv-surrogate-data"
-version = "1.0.1"
+version = "1.0.2"
 description = "This repository allows for easy data access for fair-weather photovoltaic module output."
 authors = [
   "Dominik Falkner <dominik.falkner@risc-software.at>"
 ]
 readme = "README.md"
 repository = "https://github.com/prescriptiveanalytics/pv_surrogate_data"
 packages = [
@@ -75,15 +75,15 @@
 # ignore any of these paths
 norecursedirs = [ ]
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]  
 fix = true
 ignore-init-module-imports = true
-line-length = 120
+line-length = 160
 src = ["pv_surrogate_data", "tests"]
 
 [tool.ruff.pycodestyle]
 max-doc-length = 120
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `pv_surrogate_data-1.0.1/PKG-INFO` & `pv_surrogate_data-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-surrogate-data
-Version: 1.0.1
+Version: 1.0.2
 Summary: This repository allows for easy data access for fair-weather photovoltaic module output.
 Home-page: https://github.com/prescriptiveanalytics/pv_surrogate_data
 Author: Dominik Falkner
 Author-email: dominik.falkner@risc-software.at
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

