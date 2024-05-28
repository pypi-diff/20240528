# Comparing `tmp/calitp_data_analysis-2024.5.24.tar.gz` & `tmp/calitp_data_analysis-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_analysis-2024.5.24.tar", max compression
+gzip compressed data, was "calitp_data_analysis-2024.5.28.tar", max compression
```

## Comparing `calitp_data_analysis-2024.5.24.tar` & `calitp_data_analysis-2024.5.28.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      340 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/calitp_color_palette.py
--rw-r--r--   0        0        0     6404 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/geography_utils.py
--rw-r--r--   0        0        0     1427 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/magics.py
--rw-r--r--   0        0        0     3995 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/sql.py
--rw-r--r--   0        0        0     6944 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/styleguide.py
--rw-r--r--   0        0        0     3292 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/tables.py
--rw-r--r--   0        0        0     8990 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/calitp_data_analysis/utils.py
--rw-r--r--   0        0        0     1090 2024-05-24 17:54:29.655459 calitp_data_analysis-2024.5.24/pyproject.toml
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 calitp_data_analysis-2024.5.24/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/calitp_color_palette.py
+-rw-r--r--   0        0        0     6404 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/geography_utils.py
+-rw-r--r--   0        0        0     1427 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/magics.py
+-rw-r--r--   0        0        0     3995 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/sql.py
+-rw-r--r--   0        0        0     6944 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/styleguide.py
+-rw-r--r--   0        0        0     3292 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/tables.py
+-rw-r--r--   0        0        0     8990 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/calitp_data_analysis/utils.py
+-rw-r--r--   0        0        0     1194 2024-05-28 21:09:00.560351 calitp_data_analysis-2024.5.28/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 calitp_data_analysis-2024.5.28/PKG-INFO
```

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/calitp_color_palette.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/calitp_color_palette.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/geography_utils.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/geography_utils.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/magics.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/magics.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/sql.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/sql.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/styleguide.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/styleguide.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/tables.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/tables.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/calitp_data_analysis/utils.py` & `calitp_data_analysis-2024.5.28/calitp_data_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2024.5.24/pyproject.toml` & `calitp_data_analysis-2024.5.28/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "calitp-data-analysis"
-version = "2024.5.24"
+version = "2024.5.28"
 description = "Shared code for querying Cal-ITP data in notebooks, primarily."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = "~3.11"
 ipython = "^8.9.0"
-siuba = "0.4.2"
+siuba = "0.4.2" # pinned because new versions might need better sqlalchemy
 jinja2 = "^3.1.3"
 sqlalchemy-bigquery = "^1.6.1"
-sqlalchemy = "1.4.46"
+sqlalchemy = "1.4.46" # pinned because 2.0 breaks the sql.py file
 pandas-gbq = "^0.19.1"
 pandas = "<2" # keep us below pandas 2.0 since pandas-gbq does not specify, and siuba errors currently
 gcsfs = "!=2022.7.1"
 altair = "^5.1.1"
-dask-geopandas = "0.2.0"
+dask-geopandas = "^0.2.0"
 geopandas = "^0.14.0"
 requests = "^2.31.0"
-dask = "~2022.8"
+dask = "~2024.5"
 shapely = "^2.0.1"
 gtfs-segments = "0.1.0"
 pyairtable = "2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.0"
```

### Comparing `calitp_data_analysis-2024.5.24/PKG-INFO` & `calitp_data_analysis-2024.5.28/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: calitp-data-analysis
-Version: 2024.5.24
+Version: 2024.5.28
 Summary: Shared code for querying Cal-ITP data in notebooks, primarily.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=5.1.1,<6.0.0)
-Requires-Dist: dask (>=2022.8,<2022.9)
-Requires-Dist: dask-geopandas (==0.2.0)
+Requires-Dist: dask (>=2024.5,<2024.6)
+Requires-Dist: dask-geopandas (>=0.2.0,<0.3.0)
 Requires-Dist: gcsfs (!=2022.7.1)
 Requires-Dist: geopandas (>=0.14.0,<0.15.0)
 Requires-Dist: gtfs-segments (==0.1.0)
 Requires-Dist: ipython (>=8.9.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pandas (<2)
 Requires-Dist: pandas-gbq (>=0.19.1,<0.20.0)
```

