# Comparing `tmp/tidal_algorithmic_mixes-0.1.0.tar.gz` & `tmp/tidal_algorithmic_mixes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_algorithmic_mixes-0.1.0.tar", max compression
+gzip compressed data, was "tidal_algorithmic_mixes-0.1.1.tar", max compression
```

## Comparing `tidal_algorithmic_mixes-0.1.0.tar` & `tidal_algorithmic_mixes-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11341 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/LICENSE
--rw-r--r--   0        0        0     1030 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/README.md
--rw-r--r--   0        0        0     1199 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/__init__.py
--rw-r--r--   0        0        0        1 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/__init__.py
--rw-r--r--   0        0        0     2897 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/daily_update_transformation.py
--rw-r--r--   0        0        0     1775 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/observed_tracks_aggregator_transformation.py
--rw-r--r--   0        0        0     9362 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/post_processor_transformation.py
--rw-r--r--   0        0        0     4634 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/sasrec_model_transformation.py
--rw-r--r--   0        0        0     1481 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/etl_model.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/__init__.py
--rw-r--r--   0        0        0     1475 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/config.py
--rw-r--r--   0        0        0     1361 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/constants.py
--rw-r--r--   0        0        0     2573 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/mix_utils.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/__init__.py
--rw-r--r--   0        0        0      780 2024-03-01 12:57:51.390596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/artist_index_enricher_transformer.py
--rw-r--r--   0        0        0     1399 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/artist_top_tracks_mix_output_transformer.py
--rw-r--r--   0        0        0      830 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_artist_cluster.py
--rw-r--r--   0        0        0     1155 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_similar_artist.py
--rw-r--r--   0        0        0     1590 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/main_artist_compound_mapping_transformer.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/blacklist/__init__.py
--rw-r--r--   0        0        0     4077 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/blacklist/user_blacklist_filter_transformer.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/__init__.py
--rw-r--r--   0        0        0     1293 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_output_transformer.py
--rw-r--r--   0        0        0     1404 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_sort_transformer.py
--rw-r--r--   0        0        0     2179 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/flag_known_artists_transformer.py
--rw-r--r--   0        0        0     2177 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/split_by_known_artists_transformer.py
--rw-r--r--   0        0        0     2760 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/diversity_sort_transformer.py
--rw-r--r--   0        0        0      932 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/posexplode_transformer.py
--rw-r--r--   0        0        0        0 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/__init__.py
--rw-r--r--   0        0        0     1278 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/enrich_user_transformer.py
--rw-r--r--   0        0        0      927 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_albums_transformer.py
--rw-r--r--   0        0        0     2218 2024-03-01 12:57:51.394596 tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_tracks_transformer.py
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 tidal_algorithmic_mixes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-05-28 07:45:37.597262 tidal_algorithmic_mixes-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1053 2024-05-28 07:45:37.597262 tidal_algorithmic_mixes-0.1.1/README.md
+-rw-r--r--   0        0        0     1200 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/daily_update_transformation.py
+-rw-r--r--   0        0        0     1775 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/observed_tracks_aggregator_transformation.py
+-rw-r--r--   0        0        0     9362 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/post_processor_transformation.py
+-rw-r--r--   0        0        0     4634 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/sasrec_model_transformation.py
+-rw-r--r--   0        0        0     1481 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/etl_model.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/config.py
+-rw-r--r--   0        0        0     1361 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/constants.py
+-rw-r--r--   0        0        0     2573 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/mix_utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/__init__.py
+-rw-r--r--   0        0        0      780 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/artist_index_enricher_transformer.py
+-rw-r--r--   0        0        0     1399 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/artist_top_tracks_mix_output_transformer.py
+-rw-r--r--   0        0        0      830 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_artist_cluster.py
+-rw-r--r--   0        0        0     1155 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_similar_artist.py
+-rw-r--r--   0        0        0     1590 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/main_artist_compound_mapping_transformer.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/blacklist/__init__.py
+-rw-r--r--   0        0        0     4077 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/blacklist/user_blacklist_filter_transformer.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.601263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/__init__.py
+-rw-r--r--   0        0        0     1293 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_output_transformer.py
+-rw-r--r--   0        0        0     1404 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_sort_transformer.py
+-rw-r--r--   0        0        0     2179 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/flag_known_artists_transformer.py
+-rw-r--r--   0        0        0     2177 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/split_by_known_artists_transformer.py
+-rw-r--r--   0        0        0     2760 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/diversity_sort_transformer.py
+-rw-r--r--   0        0        0      932 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/posexplode_transformer.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/__init__.py
+-rw-r--r--   0        0        0     1278 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/enrich_user_transformer.py
+-rw-r--r--   0        0        0      927 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_albums_transformer.py
+-rw-r--r--   0        0        0     2218 2024-05-28 07:45:37.605263 tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_tracks_transformer.py
+-rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 tidal_algorithmic_mixes-0.1.1/PKG-INFO
```

### Comparing `tidal_algorithmic_mixes-0.1.0/LICENSE` & `tidal_algorithmic_mixes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/pyproject.toml` & `tidal_algorithmic_mixes-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
-requires-python = ">=3.12"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Apache License V 2.0",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/tidal-music/tidal-algorithmic-mixes"
 
 [tool.poetry]
 name = "tidal_algorithmic_mixes"
-version = "0.1.0"
+version = "0.1.1"
 description = "common transformers used by the tidal personalization team."
 authors = [
     "Loay <loay@squareup.com>",
     "Tao <tma@squareup.com>",
     "Thomas <talmenningen@squareup.com>",
     "Yuhua <yuhua@squareup.com>"
 ]
 
 license = "Apache License V 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.12.0"
+python = ">=3.10.13"
 pyspark = ">=3.5.0,<=3.6.0"
 numpy = ">=1.16.4"
 s3fs = "2022.11.0"
 boto3 = "1.24.59"
 pandas = ">=1.4.2"
 great-expectations = "0.16.15"
 scikit-learn = "1.4.0"
```

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/daily_update_transformation.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/daily_update_transformation.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/observed_tracks_aggregator_transformation.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/observed_tracks_aggregator_transformation.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/post_processor_transformation.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/post_processor_transformation.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/discovery_mix/sasrec_model_transformation.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/discovery_mix/sasrec_model_transformation.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/etl_model.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/etl_model.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/config.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/config.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/constants.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/mix_utils.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/mix_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/artist_index_enricher_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/artist_index_enricher_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/artist_top_tracks_mix_output_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/artist_top_tracks_mix_output_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_artist_cluster.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_artist_cluster.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_similar_artist.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/enrich_with_similar_artist.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/artist/main_artist_compound_mapping_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/artist/main_artist_compound_mapping_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/blacklist/user_blacklist_filter_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/blacklist/user_blacklist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_output_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_output_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_sort_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/discovery_mix_sort_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/flag_known_artists_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/flag_known_artists_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/discovery_mix/split_by_known_artists_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/discovery_mix/split_by_known_artists_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/diversity_sort_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/diversity_sort_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/posexplode_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/posexplode_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/enrich_user_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/enrich_user_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_albums_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_albums_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_tracks_transformer.py` & `tidal_algorithmic_mixes-0.1.1/tidal_algorithmic_mixes/utils/transformers/user/filter_streamed_tracks_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_algorithmic_mixes-0.1.0/PKG-INFO` & `tidal_algorithmic_mixes-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: tidal_algorithmic_mixes
-Version: 0.1.0
+Version: 0.1.1
 Summary: common transformers used by the tidal personalization team.
 License: Apache License V 2.0
 Author: Loay
 Author-email: loay@squareup.com
-Requires-Python: >=3.12.0
+Requires-Python: >=3.10.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alphabet-detector (==0.0.7)
 Requires-Dist: boto3 (==1.24.59)
 Requires-Dist: great-expectations (==0.16.15)
 Requires-Dist: mlflow (==2.10.2)
 Requires-Dist: numpy (>=1.16.4)
 Requires-Dist: pandas (>=1.4.2)
@@ -28,16 +29,16 @@
 This contains the logic of how tidal create its algorithmic offline mixes,
 how it utilizes different machine learning models, 
 alongside business rules to create different mixes for different use cases, 
 included personalized mixes (like my mix, my new arrivals and daily discovery)
 and non-personalized like track radio and artist radio.
 
 - Make sure you have pyenv and [pyenv](https://github.com/pyenv/pyenv) amd [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) installed on your local environment.
-- Install python 3.8.16 with pyenv `pyenv install 3.12.0`.
-- Set up a new virtual env `pyenv virtualenv 3.12.0 mixes`
+- Install python 3.10.13 with pyenv `pyenv install 3.11.13`.
+- Set up a new virtual env `pyenv virtualenv 3.10.13 mixes`
 - Set local pyenv version `pyenv local mixes`
 - Activate the virtual pyenv using `pyenv activate mixes`
-- Upgrade the pip package installer `pip install --upgrade pip`
-- Install poetry for package management `pip install poetry==1.7.1`
+- Upgrade the pip package installer `python -m pip install --upgrade pip`
+- Install poetry for package management `python -m pip install poetry==1.7.1`
 - Install dependencies from the lock file `poetry install --no-root` 
 
 [pyproject.toml](pyproject.toml)[pyproject.toml](pyproject.toml)
```

