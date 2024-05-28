# Comparing `tmp/ipulse_shared_ai_ftredge-1.2.tar.gz` & `tmp/ipulse_shared_ai_ftredge-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipulse_shared_ai_ftredge-1.2.tar", last modified: Fri Apr  5 13:33:48 2024, max compression
+gzip compressed data, was "ipulse_shared_ai_ftredge-1.3.tar", last modified: Tue May 28 12:36:19 2024, max compression
```

## Comparing `ipulse_shared_ai_ftredge-1.2.tar` & `ipulse_shared_ai_ftredge-1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:19.265802 ipulse_shared_ai_ftredge-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-28 12:36:19.265802 ipulse_shared_ai_ftredge-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:36:19.265802 ipulse_shared_ai_ftredge-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:19.261802 ipulse_shared_ai_ftredge-1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:19.261802 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:19.265802 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/mlmodel_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/mlmodel_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-28 12:36:09.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:36:19.265802 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-28 12:36:19.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 12:36:19.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:36:19.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 12:36:19.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 12:36:19.000000 ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/top_level.txt
```

### Comparing `ipulse_shared_ai_ftredge-1.2/LICENCE` & `ipulse_shared_ai_ftredge-1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.2/setup.py` & `ipulse_shared_ai_ftredge-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipulse_shared_ai_ftredge',
-    version='1.2',
+    version='1.3',
     package_dir={'': 'src'},  # Specify the source directory
     packages=find_packages(where='src'),  # Look for packages in 'src'
     install_requires=[
         # List your dependencies here
         'pydantic[email]~=2.5',
         'python-dateutil~=2.8',
         'pytest~=7.1',
```

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/common_utils.py` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/common_utils.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_abstract.py` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_abstract.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series.py` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         return value
  
     data_domain: str #oracle/historical/ or oracle/predictions/ or gym/historical
     asset_category: str  # indices,  crypto, stocks , commodities, real_estate, forex, options, bonds, funds, watches, cars, art, wine, collectibles, weather, other
  
     @validator('asset_category')
     def validate_asset_category(cls, value):
-        valid_categories = ["indcs", "crypto", "stocks", "commdts", "rel_est", "forex", 
-                            "options", "bonds", "funds", "corpfundam", "economcs","energy", "luxury", "art", "wine", 
-                            "clctbls", "weather", "climate", "sports", "health", "transprt", "astronmcl", "simultn", "other" ]
+        valid_categories = ["indices", "crypto", "stocks", "comdts", "realest", "forex", 
+                            "options", "bonds", "funds", "economcs", "luxury", "arts", "wine", 
+                            "cllctbls", "climate", "sports", "health", "transprt", "astronmcl", "simultn", "other" ]
         if value not in valid_categories:
             raise ValueError(f"asset_category '{value}' is not valid. Must be one of: {', '.join(valid_categories)}")
         return value
     
     series_main_origin_short: Optional[str]= None #brief description of the source
     @validator('series_main_origin_short')
     def validate_series_main_origin_short(cls, value):
```

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt` & `ipulse_shared_ai_ftredge-1.3/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

