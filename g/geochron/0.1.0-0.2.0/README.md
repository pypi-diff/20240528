# Comparing `tmp/geochron-0.1.0.tar.gz` & `tmp/geochron-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geochron-0.1.0.tar", last modified: Wed May 22 00:38:14 2024, max compression
+gzip compressed data, was "geochron-0.2.0.tar", last modified: Tue May 28 14:41:03 2024, max compression
```

## Comparing `geochron-0.1.0.tar` & `geochron-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:38:14.164051 geochron-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 00:37:32.000000 geochron-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 00:38:14.160051 geochron-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-22 00:37:32.000000 geochron-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:38:14.160051 geochron-0.1.0/geochron/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/chronnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/geotimehash.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/time_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-22 00:37:32.000000 geochron-0.1.0/geochron/timehex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:38:14.160051 geochron-0.1.0/geochron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 00:38:14.000000 geochron-0.1.0/geochron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 00:38:14.000000 geochron-0.1.0/geochron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:38:14.000000 geochron-0.1.0/geochron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 00:38:14.000000 geochron-0.1.0/geochron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 00:38:14.000000 geochron-0.1.0/geochron.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:38:14.164051 geochron-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 00:37:32.000000 geochron-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:38:14.160051 geochron-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-22 00:37:32.000000 geochron-0.1.0/tests/test_chronnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-22 00:37:32.000000 geochron-0.1.0/tests/test_geotimehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 00:37:32.000000 geochron-0.1.0/tests/test_time_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 00:37:32.000000 geochron-0.1.0/tests/test_timehex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:41:03.204396 geochron-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 14:40:21.000000 geochron-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-28 14:41:03.204396 geochron-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-28 14:40:21.000000 geochron-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:41:03.204396 geochron-0.2.0/geochron/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/chronnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/geosynchnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/geotimehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/time_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-28 14:40:21.000000 geochron-0.2.0/geochron/timehex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:41:03.204396 geochron-0.2.0/geochron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-28 14:41:03.000000 geochron-0.2.0/geochron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-28 14:41:03.000000 geochron-0.2.0/geochron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:41:03.000000 geochron-0.2.0/geochron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 14:41:03.000000 geochron-0.2.0/geochron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 14:41:03.000000 geochron-0.2.0/geochron.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:41:03.204396 geochron-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-28 14:40:21.000000 geochron-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:41:03.204396 geochron-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-28 14:40:21.000000 geochron-0.2.0/tests/test_chronnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-28 14:40:21.000000 geochron-0.2.0/tests/test_geosynchnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-28 14:40:21.000000 geochron-0.2.0/tests/test_geotimehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-28 14:40:21.000000 geochron-0.2.0/tests/test_time_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 14:40:21.000000 geochron-0.2.0/tests/test_timehex.py
```

### Comparing `geochron-0.1.0/LICENSE` & `geochron-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/PKG-INFO` & `geochron-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geochron
-Version: 0.1.0
+Version: 0.2.0
 Summary: A companion package to geostructures enabling geo-spatial-temporal data structures.
 Home-page: https://github.com/etalbert/geochron
 Author: Eli Talbert
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -37,16 +37,17 @@
 
 ### Overview
 
 Geotime enables various ways of displaying and structuring geo-spatial-temporal data
 
 The methods currently supported are:
 * time hexes H3 Geohashes with second dimension time (Original Niemeyer can also be used)
-* chron-nets (https://www.nature.com/articles/s41467-020-17634-2)
+* chron-net (https://www.nature.com/articles/s41467-020-17634-2)
 * geotimehash (https://isprs-annals.copernicus.org/articles/IV-4-W2/31/2017/isprs-annals-IV-4-W2-31-2017.pdf)
+* geosynchnet (geographic synchronous networks)
 
 
 #### Basic Functionality
 The primary and simplest use case is converting a geostructures FeatureCollection to another datastructure.
 Geostructures FeatureCollections can take most major geospatial standards like shapefiles and geopandas. See geostructures documentation. 
 ```python
 import datetime as dt
@@ -60,14 +61,17 @@
 
 chronnet_output = convert_chronnet(fcol=Feature_Collection_of_time_shapes,
 time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection, self_loop = True, mode = "directed")
 
 geotimehash_output = convert_geotimehash(fcol=Feature_Collection_of_time_shapes, precision = 8,
 hash_func= hasher.hash_collection)
 
+geosynchnet_output = convert_geosynchnet(fcol=Feature_Collection_of_time_shapes, 
+time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection)
+
 ```
 
 
 ## More Information
 
 For an more in-depth introduction, please review our collection of [Jupyter notebooks](./notebooks).
```

### Comparing `geochron-0.1.0/README.md` & `geochron-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 ### Overview
 
 Geotime enables various ways of displaying and structuring geo-spatial-temporal data
 
 The methods currently supported are:
 * time hexes H3 Geohashes with second dimension time (Original Niemeyer can also be used)
-* chron-nets (https://www.nature.com/articles/s41467-020-17634-2)
+* chron-net (https://www.nature.com/articles/s41467-020-17634-2)
 * geotimehash (https://isprs-annals.copernicus.org/articles/IV-4-W2/31/2017/isprs-annals-IV-4-W2-31-2017.pdf)
+* geosynchnet (geographic synchronous networks)
 
 
 #### Basic Functionality
 The primary and simplest use case is converting a geostructures FeatureCollection to another datastructure.
 Geostructures FeatureCollections can take most major geospatial standards like shapefiles and geopandas. See geostructures documentation. 
 ```python
 import datetime as dt
@@ -43,14 +44,17 @@
 
 chronnet_output = convert_chronnet(fcol=Feature_Collection_of_time_shapes,
 time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection, self_loop = True, mode = "directed")
 
 geotimehash_output = convert_geotimehash(fcol=Feature_Collection_of_time_shapes, precision = 8,
 hash_func= hasher.hash_collection)
 
+geosynchnet_output = convert_geosynchnet(fcol=Feature_Collection_of_time_shapes, 
+time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection)
+
 ```
 
 
 ## More Information
 
 For an more in-depth introduction, please review our collection of [Jupyter notebooks](./notebooks).
```

### Comparing `geochron-0.1.0/geochron/__init__.py` & `geochron-0.2.0/geochron/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import sys
 
 from geochron._version import __version__  # noqa: F401
 from geochron.utils.conditional_imports import ConditionalPackageInterceptor
 from geochron.chronnet import convert_chronnet
 from geochron.timehex import convert_timehex
 from geochron.geotimehash import convert_geotimehash
+from geochron.geosynchnet import convert_geosynchnet
 
 ConditionalPackageInterceptor.permit_packages(
     {
         'networkx': 'networkx>=3.0,<4.0',
         'plotly': 'plotly>=5,<6',
         'timehash': 'timehash>=1.2,<2',
     }
 )
 sys.meta_path.append(ConditionalPackageInterceptor)  # type: ignore
 
 __all__ = [
     'convert_chronnet',
     'convert_timehex',
-    'convert_geotimehash' 
+    'convert_geotimehash',
+    'convert_geosynchnet' 
 ]
```

### Comparing `geochron-0.1.0/geochron/chronnet.py` & `geochron-0.2.0/geochron/chronnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Representation as chronnets """
 from datetime import  timedelta
 import itertools
 from typing import Callable, List
-import networkx as nx # type: ignore
 import numpy as np
 import pandas as pd
 
 from geostructures.collections import  FeatureCollection,Track
 from geochron.time_slicing import get_timestamp_intervals, time_slice_track
 
 
@@ -45,26 +44,29 @@
 
     return df
 
 
 def chronnet_create(df: pd.DataFrame, self_loops: bool, mode= str):
     """
     Converts a properly formatted pandas dataframe with the columns
-    of cell and time to a networkx network. 
+    of cell and time to a networkx network where nodes are locations
+    and edges are formed between nodes with consecutive times. 
     
     Args:
         df: a pandas dataframe withe two columns cell and time
 
         self_loops: whether self loops are included in the network
 
         mode: whether the network is directed or undirected
 
     Returns:
         A networkx network
     """
+    # pylint: disable=import-outside-toplevel
+    import networkx as nx # type: ignore
     time_seq = sorted(np.unique(df['time']))
     if len(time_seq) < 2: # pragma: no cover
         print("The total time interval in the dataset should be larger than two.")
     links = pd.DataFrame()
     cells_before=[]
     cells_after=[]
     weights = []
```

### Comparing `geochron-0.1.0/geochron/geotimehash.py` & `geochron-0.2.0/geochron/geotimehash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Geotime hash representation"""
 from typing import Callable, List
 from collections import Counter
 from datetime import  datetime, timedelta
-import timehash
 from geostructures.structures import GeoShape
 from geostructures.time import TimeInterval
 from geostructures import FeatureCollection, Track
 
 def precision_delta(precision: int):
     """
     Translates a timehash precision into the corresponding timedelta. 
@@ -81,14 +80,16 @@
 
         precision: the desired precision of the timehash precision higher
         then 10 is not supported
 
     Returns:
         A timehash list
     """
+    # pylint: disable=import-outside-toplevel
+    import timehash
     timehash_list = []
     assert isinstance(geoshape.dt, TimeInterval)
     start_time = geoshape.dt.start
     end_time = geoshape.dt.end
 
     time_list = generate_times(start_time, end_time, precision)
```

### Comparing `geochron-0.1.0/geochron/time_slicing.py` & `geochron-0.2.0/geochron/time_slicing.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/geochron/timehex.py` & `geochron-0.2.0/geochron/timehex.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/geochron.egg-info/PKG-INFO` & `geochron-0.2.0/geochron.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geochron
-Version: 0.1.0
+Version: 0.2.0
 Summary: A companion package to geostructures enabling geo-spatial-temporal data structures.
 Home-page: https://github.com/etalbert/geochron
 Author: Eli Talbert
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -37,16 +37,17 @@
 
 ### Overview
 
 Geotime enables various ways of displaying and structuring geo-spatial-temporal data
 
 The methods currently supported are:
 * time hexes H3 Geohashes with second dimension time (Original Niemeyer can also be used)
-* chron-nets (https://www.nature.com/articles/s41467-020-17634-2)
+* chron-net (https://www.nature.com/articles/s41467-020-17634-2)
 * geotimehash (https://isprs-annals.copernicus.org/articles/IV-4-W2/31/2017/isprs-annals-IV-4-W2-31-2017.pdf)
+* geosynchnet (geographic synchronous networks)
 
 
 #### Basic Functionality
 The primary and simplest use case is converting a geostructures FeatureCollection to another datastructure.
 Geostructures FeatureCollections can take most major geospatial standards like shapefiles and geopandas. See geostructures documentation. 
 ```python
 import datetime as dt
@@ -60,14 +61,17 @@
 
 chronnet_output = convert_chronnet(fcol=Feature_Collection_of_time_shapes,
 time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection, self_loop = True, mode = "directed")
 
 geotimehash_output = convert_geotimehash(fcol=Feature_Collection_of_time_shapes, precision = 8,
 hash_func= hasher.hash_collection)
 
+geosynchnet_output = convert_geosynchnet(fcol=Feature_Collection_of_time_shapes, 
+time_delta= dt.timedelta(hours=1), hash_func= hasher.hash_collection)
+
 ```
 
 
 ## More Information
 
 For an more in-depth introduction, please review our collection of [Jupyter notebooks](./notebooks).
```

### Comparing `geochron-0.1.0/setup.py` & `geochron-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/tests/test_chronnet.py` & `geochron-0.2.0/tests/test_chronnet.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/tests/test_geotimehash.py` & `geochron-0.2.0/tests/test_geotimehash.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/tests/test_time_slicing.py` & `geochron-0.2.0/tests/test_time_slicing.py`

 * *Files identical despite different names*

### Comparing `geochron-0.1.0/tests/test_timehex.py` & `geochron-0.2.0/tests/test_timehex.py`

 * *Files identical despite different names*

