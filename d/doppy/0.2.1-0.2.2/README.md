# Comparing `tmp/doppy-0.2.1.tar.gz` & `tmp/doppy-0.2.2.tar.gz`

## Comparing `doppy-0.2.1.tar` & `doppy-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0     1001      127      206 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/Cargo.toml
--rw-r--r--   0     1001      127       21 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/.gitignore
--rw-r--r--   0     1001      127       13 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/src/lib.rs
--rw-r--r--   0     1001      127     2047 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/src/raw/error.rs
--rw-r--r--   0     1001      127     9448 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127     7246 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/src/raw/wls70.rs
--rw-r--r--   0     1001      127       48 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doprs/src/raw.rs
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.2.1/crates/doppy_rs/Cargo.toml
--rw-r--r--   0     1001      127      279 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doppy_rs/src/lib.rs
--rw-r--r--   0     1001      127     4526 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doppy_rs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127     2340 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doppy_rs/src/raw/wls70.rs
--rw-r--r--   0     1001      127      269 2024-05-07 13:10:08.000000 doppy-0.2.1/crates/doppy_rs/src/raw.rs
--rw-r--r--   0     1001      127    18041 2024-05-07 13:10:13.000000 doppy-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.2.1/Cargo.toml
--rw-r--r--   0     1001      127     2393 2024-05-07 13:10:08.000000 doppy-0.2.1/pyproject.toml
--rw-r--r--   0     1001      127      205 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/options.py
--rw-r--r--   0     1001      127        0 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/py.typed
--rw-r--r--   0     1001      127     4809 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/halo_bg.py
--rw-r--r--   0     1001      127    18485 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/halo_hpl.py
--rw-r--r--   0     1001      127     9906 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/windcube.py
--rw-r--r--   0     1001      127     7008 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/wls70.py
--rw-r--r--   0     1001      127     3937 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/halo_sys_params.py
--rw-r--r--   0     1001      127      228 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/raw/__init__.py
--rw-r--r--   0     1001      127     1863 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/data/api.py
--rw-r--r--   0     1001      127      996 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/data/cache.py
--rw-r--r--   0     1001      127        0 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/data/__init__.py
--rw-r--r--   0     1001      127       89 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/data/exceptions.py
--rw-r--r--   0     1001      127      191 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/__init__.py
--rw-r--r--   0     1001      127      248 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/bench.py
--rw-r--r--   0     1001      127      214 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/utils.py
--rw-r--r--   0     1001      127    19907 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/product/stare.py
--rw-r--r--   0     1001      127      103 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/product/__init__.py
--rw-r--r--   0     1001      127    12151 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/product/wind.py
--rw-r--r--   0     1001      127      346 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/__main__.py
--rw-r--r--   0     1001      127       38 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/defaults.py
--rw-r--r--   0     1001      127      138 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/exceptions.py
--rw-r--r--   0     1001      127     3416 2024-05-07 13:10:08.000000 doppy-0.2.1/src/doppy/netcdf.py
--rw-r--r--   0     1001      127      279 2024-05-07 13:10:08.000000 doppy-0.2.1/README.md
--rw-r--r--   0     1001      127     1089 2024-05-07 13:10:08.000000 doppy-0.2.1/LICENSE
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 doppy-0.2.1/PKG-INFO
+-rw-r--r--   0     1001      127      206 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/Cargo.toml
+-rw-r--r--   0     1001      127       21 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/.gitignore
+-rw-r--r--   0     1001      127       13 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/src/lib.rs
+-rw-r--r--   0     1001      127     2047 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/src/raw/error.rs
+-rw-r--r--   0     1001      127     9448 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127     7246 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/src/raw/wls70.rs
+-rw-r--r--   0     1001      127       48 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doprs/src/raw.rs
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.2.2/crates/doppy_rs/Cargo.toml
+-rw-r--r--   0     1001      127      279 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doppy_rs/src/lib.rs
+-rw-r--r--   0     1001      127     4526 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doppy_rs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127     2340 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doppy_rs/src/raw/wls70.rs
+-rw-r--r--   0     1001      127      269 2024-05-28 12:35:15.000000 doppy-0.2.2/crates/doppy_rs/src/raw.rs
+-rw-r--r--   0     1001      127    18041 2024-05-28 12:35:21.000000 doppy-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      127     2393 2024-05-28 12:35:15.000000 doppy-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      127      996 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/data/cache.py
+-rw-r--r--   0     1001      127        0 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/data/__init__.py
+-rw-r--r--   0     1001      127     1863 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/data/api.py
+-rw-r--r--   0     1001      127       89 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/data/exceptions.py
+-rw-r--r--   0     1001      127      346 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/__main__.py
+-rw-r--r--   0     1001      127     3416 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/netcdf.py
+-rw-r--r--   0     1001      127      191 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/__init__.py
+-rw-r--r--   0     1001      127       38 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/defaults.py
+-rw-r--r--   0     1001      127     7008 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/wls70.py
+-rw-r--r--   0     1001      127      228 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/__init__.py
+-rw-r--r--   0     1001      127     9906 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/windcube.py
+-rw-r--r--   0     1001      127     3937 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/halo_sys_params.py
+-rw-r--r--   0     1001      127     4809 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/halo_bg.py
+-rw-r--r--   0     1001      127    18485 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/raw/halo_hpl.py
+-rw-r--r--   0     1001      127        0 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/py.typed
+-rw-r--r--   0     1001      127    19907 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/product/stare.py
+-rw-r--r--   0     1001      127    13042 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/product/wind.py
+-rw-r--r--   0     1001      127      172 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/product/__init__.py
+-rw-r--r--   0     1001      127      248 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/bench.py
+-rw-r--r--   0     1001      127      214 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/utils.py
+-rw-r--r--   0     1001      127      205 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/options.py
+-rw-r--r--   0     1001      127      138 2024-05-28 12:35:15.000000 doppy-0.2.2/src/doppy/exceptions.py
+-rw-r--r--   0     1001      127      279 2024-05-28 12:35:15.000000 doppy-0.2.2/README.md
+-rw-r--r--   0     1001      127     1089 2024-05-28 12:35:15.000000 doppy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 doppy-0.2.2/PKG-INFO
```

### Comparing `doppy-0.2.1/crates/doprs/src/raw/error.rs` & `doppy-0.2.2/crates/doprs/src/raw/error.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/crates/doprs/src/raw/halo_hpl.rs` & `doppy-0.2.2/crates/doprs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/crates/doprs/src/raw/wls70.rs` & `doppy-0.2.2/crates/doprs/src/raw/wls70.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/crates/doppy_rs/src/raw/halo_hpl.rs` & `doppy-0.2.2/crates/doppy_rs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/crates/doppy_rs/src/raw/wls70.rs` & `doppy-0.2.2/crates/doppy_rs/src/raw/wls70.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/Cargo.lock` & `doppy-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -102,24 +102,24 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "doppy_rs"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "doprs",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "doprs"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "chrono",
  "rayon",
  "regex",
 ]
 
 [[package]]
```

### Comparing `doppy-0.2.1/pyproject.toml` & `doppy-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/raw/halo_bg.py` & `doppy-0.2.2/src/doppy/raw/halo_bg.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/raw/halo_hpl.py` & `doppy-0.2.2/src/doppy/raw/halo_hpl.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/raw/windcube.py` & `doppy-0.2.2/src/doppy/raw/windcube.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/raw/wls70.py` & `doppy-0.2.2/src/doppy/raw/wls70.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/raw/halo_sys_params.py` & `doppy-0.2.2/src/doppy/raw/halo_sys_params.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/data/api.py` & `doppy-0.2.2/src/doppy/data/api.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/data/cache.py` & `doppy-0.2.2/src/doppy/data/cache.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/product/stare.py` & `doppy-0.2.2/src/doppy/product/stare.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/src/doppy/product/wind.py` & `doppy-0.2.2/src/doppy/product/wind.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 import doppy
 
 # ngates, gate points, elevation angle, tuple of sorted azimuth angles
 SelectionGroupKeyType: TypeAlias = tuple[int, int, tuple[int, ...]]
 
 
 @dataclass
+class Options:
+    azimuth_offset_deg: float | None
+
+
+@dataclass
 class Wind:
     time: npt.NDArray[np.datetime64]
     height: npt.NDArray[np.float64]
     zonal_wind: npt.NDArray[np.float64]
     meridional_wind: npt.NDArray[np.float64]
     vertical_wind: npt.NDArray[np.float64]
     mask: npt.NDArray[np.bool_]
@@ -41,14 +46,15 @@
     @classmethod
     def from_halo_data(
         cls,
         data: Sequence[str]
         | Sequence[Path]
         | Sequence[bytes]
         | Sequence[BufferedIOBase],
+        options: Options | None = None,
     ) -> Wind:
         raws = doppy.raw.HaloHpl.from_srcs(data)
 
         if len(raws) == 0:
             raise doppy.exceptions.NoDataError("HaloHpl data missing")
 
         raw = (
@@ -56,14 +62,17 @@
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
             .nans_removed()
         )
         if len(raw.time) == 0:
             raise doppy.exceptions.NoDataError("No suitable data for the wind product")
 
+        if options and options.azimuth_offset_deg:
+            raw.azimuth += options.azimuth_offset_deg
+
         groups = _group_scans_by_azimuth_rotation(raw)
         time_list = []
         elevation_list = []
         wind_list = []
         rmse_list = []
 
         for group_index in set(groups):
@@ -100,14 +109,15 @@
     @classmethod
     def from_windcube_data(
         cls,
         data: Sequence[str]
         | Sequence[Path]
         | Sequence[bytes]
         | Sequence[BufferedIOBase],
+        options: Options | None = None,
     ) -> Wind:
         raws = doppy.raw.WindCube.from_vad_srcs(data)
 
         if len(raws) == 0:
             raise doppy.exceptions.NoDataError("WindCube data missing")
 
         raw = (
@@ -115,14 +125,17 @@
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
             .reindex_scan_indices()
         )
         if len(raw.time) == 0:
             raise doppy.exceptions.NoDataError("No suitable data for the wind product")
 
+        if options and options.azimuth_offset_deg:
+            raw.azimuth += options.azimuth_offset_deg
+
         time_list = []
         elevation_list = []
         wind_list = []
         rmse_list = []
 
         for scan_index in set(raw.scan_index):
             pick = raw.scan_index == scan_index
@@ -155,35 +168,50 @@
     @classmethod
     def from_wls70_data(
         cls,
         data: Sequence[str]
         | Sequence[Path]
         | Sequence[bytes]
         | Sequence[BufferedIOBase],
+        options: Options | None = None,
     ) -> Wind:
         raws = doppy.raw.Wls70.from_srcs(data)
 
         if len(raws) == 0:
             raise doppy.exceptions.NoDataError("Wls70 data missing")
 
         raw = (
             doppy.raw.Wls70.merge(raws)
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
         )
+
+        if options and options.azimuth_offset_deg:
+            theta = np.deg2rad(options.azimuth_offset_deg)
+            cos_theta = np.cos(theta)
+            sin_theta = np.sin(theta)
+
+            meridional_wind = (
+                sin_theta * raw.zonal_wind + cos_theta * raw.meridional_wind
+            )
+            zonal_wind = cos_theta * raw.zonal_wind - sin_theta * raw.meridional_wind
+        else:
+            meridional_wind = raw.meridional_wind
+            zonal_wind = raw.zonal_wind
+
         mask = (
             np.isnan(raw.meridional_wind)
             | np.isnan(raw.zonal_wind)
             | np.isnan(raw.vertical_wind)
         )
         return Wind(
             time=raw.time,
             height=raw.altitude,
-            zonal_wind=raw.zonal_wind,
-            meridional_wind=raw.meridional_wind,
+            zonal_wind=zonal_wind,
+            meridional_wind=meridional_wind,
             vertical_wind=raw.vertical_wind,
             mask=mask,
             system_id=raw.system_id,
         )
 
 
 def _compute_wind(
```

### Comparing `doppy-0.2.1/src/doppy/netcdf.py` & `doppy-0.2.2/src/doppy/netcdf.py`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/LICENSE` & `doppy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doppy-0.2.1/PKG-INFO` & `doppy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: doppy
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

