# Comparing `tmp/WebSearcher-0.3.9.tar.gz` & `tmp/WebSearcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebSearcher-0.3.9.tar", last modified: Mon Feb 26 03:35:46 2024, max compression
+gzip compressed data, was "WebSearcher-0.4.0.tar", last modified: Tue May 28 02:38:15 2024, max compression
```

## Comparing `WebSearcher-0.3.9.tar` & `WebSearcher-0.4.0.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.262890 WebSearcher-0.3.9/WebSearcher/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/WebSearcher/component_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/ads.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/available_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/general_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge_rhs.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/latest_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/local_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/local_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/map_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/news_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/people_also_ask.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/perspectives.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/scholarly_articles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/searches_related.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/shopping_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/top_image_carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/top_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/view_more_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/result_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/webutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/WebSearcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:38:15.954292 WebSearcher-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 02:38:15.954292 WebSearcher-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:38:15.950292 WebSearcher-0.4.0/WebSearcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:38:15.950292 WebSearcher-0.4.0/WebSearcher/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/classifiers/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/classifiers/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/classifiers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:38:15.954292 WebSearcher-0.4.0/WebSearcher/component_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/available_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/discussions_and_forums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/general_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/knowledge_rhs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/latest_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/local_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/local_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/map_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/news_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/people_also_ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/perspectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/scholarly_articles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/searches_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/shopping_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/top_image_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/top_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/twitter_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/twitter_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/component_parsers/view_more_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/result_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/WebSearcher/webutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:38:15.950292 WebSearcher-0.4.0/WebSearcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 02:38:15.000000 WebSearcher-0.4.0/WebSearcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-28 02:38:15.000000 WebSearcher-0.4.0/WebSearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:38:15.000000 WebSearcher-0.4.0/WebSearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 02:38:15.000000 WebSearcher-0.4.0/WebSearcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 02:38:15.000000 WebSearcher-0.4.0/WebSearcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:38:15.954292 WebSearcher-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-28 02:38:00.000000 WebSearcher-0.4.0/setup.py
```

### Comparing `WebSearcher-0.3.9/LICENSE` & `WebSearcher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/PKG-INFO` & `WebSearcher-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebSearcher
-Version: 0.3.9
+Version: 0.4.0
 Summary: WebSearcher
 Home-page: http://github.com/gitronald/WebSearcher
 Author: Ronald E. Robertson
 Author-email: rer@acm.org
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `WebSearcher-0.3.9/README.md` & `WebSearcher-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,14 @@
   - [Table of Contents](#table-of-contents)
   - [Getting Started](#getting-started)
   - [Usage](#usage)
       - [Prepare a search](#prepare-a-search)
       - [Conduct a search](#conduct-a-search)
     - [Save a Search](#save-a-search)
   - [Localization](#localization)
-      - [Obtain location names](#obtain-location-names)
-      - [Conduct a localized search](#conduct-a-localized-search)
   - [Contributing](#contributing)
     - [Repair or Enhance a Parser](#repair-or-enhance-a-parser)
     - [Add a Parser](#add-a-parser)
     - [Testing](#testing)
   - [Recent Changes](#recent-changes)
   - [Similar Packages](#similar-packages)
   - [License](#license)
@@ -116,127 +114,29 @@
 ```python
 se.save_serp(save_dir='./serps')
 ```
 
 ---  
 ## Localization
 
-Conduct web searches from a location of choice.
+<!-- Conduct web searches from a location of choice. -->
 
-#### Obtain location names
+To conduct localized searches--from a location of your choice--you only need one additional data point: The __"Canonical Name"__ of each location.   
+These are available online, and can be downloaded using a built in function (`ws.download_locations()`) that checks for the most recent version.  
 
-To conduct localized searches, you only need one additional data point: The __"Canonical Name"__ of each location.   
-These are available online, and can be downloaded using a built in function that checks for the most recent version. 
+A brief guide on how to select a canonical name and use it to conduct a localized search is available in a [jupyter notebook here](https://gist.github.com/gitronald/45bad10ca2b78cf4ec1197b542764e05).  
 
-```python
-# Set save location  
-data_dir = './location_data'
-
-# Download latest data; checks for local version before downloading
-ws.download_locations(data_dir)
-
-f  = os.listdir(data_dir)[-1]  # Last file
-fp = os.path.join(data_dir, f) # File path
-locs = pd.read_csv(fp)         # Read
-locs.info()
-```
-```
-<class 'pandas.core.frame.DataFrame'>
-RangeIndex: 102029 entries, 0 to 102028
-Data columns (total 7 columns):
-Criteria ID       102029 non-null int64
-Name              102029 non-null object
-Canonical Name    102029 non-null object
-Parent ID         101788 non-null float64
-Country Code      102013 non-null object
-Target Type       102029 non-null object
-Status            102029 non-null object
-dtypes: float64(1), int64(1), object(5)
-memory usage: 5.4+ MB
-```
-```python
-# Take a look at the first row
-locs.iloc[0]
-```
-```
-Criteria ID                       1000002
-Name                                Kabul
-Canonical Name    Kabul,Kabul,Afghanistan
-Parent ID                     9.07539e+06
-Country Code                           AF
-Target Type                          City
-Status                             Active
-Name: 0, dtype: object
-```
-
-__Looking for Canonical Names__. In order to search from a given location, you must find the corresponding canonical name.
-
-```python
-# Filter for names containing "Boston" and "Massachusetts"
-regex = r'(?=.*Boston)(?=.*Massachusetts)' 
-str_mask = locs['Canonical Name'].str.contains(regex)
-locs[str_mask]
-```
-```
-15849                                Boston,Massachusetts,United States
-15908                           East Boston,Massachusetts,United States
-66033    Boston Logan International Airport,Massachusetts,United States
-84817                        Boston College,Massachusetts,United States
-85985                          South Boston,Massachusetts,United States
-Name: Canonical Name, dtype: object
-```
-
-#### Conduct a localized search
 
-After picking one, say `'Boston,Massachusetts,United States'`, you just add this to your `se.search()` call:
-
-```python
-# Conduct Search
-qry = 'pizza'
-loc = 'Boston,Massachusetts,United States'
-se.search(qry, location=loc)
-
-# Parse Results
-se.parse_results()
-
-# Shape as dataframe
-results = pd.DataFrame(se.results)
-
-# Show details of local results returned 
-results[results.type=='local_results']['details'].tolist()
-```
-
-```
-[{
-    'rating': 4.0,
-    'n_reviews': 152,
-    'sub_type': 'Pizza',
-    'contact': '226 N Market St'
-},
-{
-    'rating': 4.6,
-    'n_reviews': 752,
-    'sub_type': 'Pizza',
-    'contact': '69 Salem St'
-},
-{
-    'sub_type': 'Pizza', 
-    'contact': 'McCormack Building, 1 Ashburton Pl'
-}]
-```
 
 ---
 ## Contributing
 
-Happy to have help! If you see a component that we aren't covering yet, please add it using the process below. If you have other improvements, feel free to add them any way you can.
+Happy to have help! If you see a component that we aren't covering yet, please add it using the process below. If you have other improvements, feel free to add them any way you can.  
 
 
-Coming next:  
-    - Functions for using multiprocessing to parse SERPs.  
-
 ### Repair or Enhance a Parser
 
 1. Examine parser names in `/component_parsers/__init__.py`
 2. Find parser file as `/component_parsers/{cmpt_name}.py`.
 
 ### Add a Parser
 
@@ -264,14 +164,19 @@
 ```
 pytest -k "1684837514.html"
 ```
 
 ---
 ## Recent Changes
 
+`0.3.10` - Updated component classifier for images, added exportable header text mappings, added gist on localized searches.
+
+`0.3.9` - Small fixes for video url parsing
+
+`0.3.8` - Using SERP pydantic model, added github pip publishing workflow
 
 `0.3.7` - Fixed localization, parser and classifier updates and fixes, image subtypes, changed rhs component handling.
 
 `0.3.0` - `0.3.6` - Parser updates for SERPs from 2022 and 2023, standalone extractors file, added pydantic, reduced redundancies in outputs.
 
 `2020.0.0`, `2022.12.18`, `2023.01.04` - Various updates, attempt at date versioning that seemed like a good idea at the time ¯\\\_(ツ)\_/¯
```

### Comparing `WebSearcher-0.3.9/WebSearcher/component_classifier.py` & `WebSearcher-0.4.0/WebSearcher/classifiers/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,284 +1,191 @@
-"""SERP component classifiers
-"""
-
-from . import webutils
+from .headers import ClassifyByHeader
+from .. import webutils
 import bs4
 
-def classify_type(cmpt: bs4.element.Tag):
-    """Component classifier
+class ClassifyMain:
+    """Classify a component from the main section based on its bs4.element.Tag """
 
-    Args:
-        cmpt (bs4.element.Tag): A search component
+    @staticmethod
+    def classify(cmpt: bs4.element.Tag) -> str:
 
-    Returns:
-        str: A classification of the component type (default: "unknown")
-    """
-    
-    # Default unknown
-    cmpt_type = "unknown"
-    
-   # Component type classifiers (order matters)
-    component_classifiers = [
-        classify_top_stories,        # Check top stories
-        classify_header_lvl2,        # Check level 2 header text
-        classify_header_lvl3,        # Check level 3 header text
-        classify_img_cards,          # Check image cards
-        classify_images,             # Check images
-        classify_knowledge_panel,    # Check knowledge panel
-        classify_knowledge_block,    # Check knowledge components
-        classify_banner,             # Check for banners
-        classify_finance_panel,      # Check finance panel (classify as knowledge)
-        classify_map_result,         # Check for map results
-        classify_general_questions,  # Check hybrid general questions
-        classify_twitter,            # Check twitter cards and results
-        classify_general,            # Check general components
-        classify_general_subresult,  # Check general result with submenu
-        classify_people_also_ask,    # Check people also ask
-        classify_knowledge_box,      # Check flights, maps, hotels, events, jobs
-        classify_hidden_survey,      # Check for hidden surveys
-        classify_local_results,      # Check for local results
-    ]
-    for classifier in component_classifiers:
-        if cmpt_type != "unknown":  break  # Exit if successful classification
-        cmpt_type = classifier(cmpt)
-
-        # Ad-hoc check for available on divs
-        if "/Available on" in cmpt.text:
-            cmpt_type = "available_on"
-    
-    return cmpt_type
-
-
-def classify_header_lvl2(cmpt: bs4.element.Tag):
-    # Wrapper for header level 2
-    return classify_header(cmpt, level=2)
-
-def classify_header_lvl3(cmpt: bs4.element.Tag):
-    # Wrapper for header level 2
-    return classify_header(cmpt, level=3)
-
-def classify_header(cmpt: bs4.element.Tag, level):
-    """Check text in common headers for dict matches"""
-
-    # Find headers
-    if level == 2:
-        header_dict = {
-            'Calculator Result': 'knowledge',
-            'Directions': 'directions',
-            'Featured snippet from the web': 'knowledge',
-            'Finance Results': 'knowledge',
-            'Jobs': 'jobs',
-            'Knowledge Result': 'knowledge',
-            'Local Results': 'local_results',
-            'Map Results': 'map_results',
-            'People also ask': 'people_also_ask',
-            'Perspectives & opinions': 'perspectives',
-            'Perspectives': 'perspectives',
-            'Related searches': 'searches_related',
-            'Resultado de traducción': 'knowledge',
-            'Resultados de la Web': 'general',
-            'Sports Results': 'knowledge',
-            'Top stories': 'top_stories',
-            'Local news': 'local_news',
-            'Translation Result': 'knowledge',
-            'Twitter Results': 'twitter',
-            'Unit Converter': 'knowledge',
-            'Weather Result': 'knowledge',
-            'Web Result with Site Links': 'general',
-            'Web results': 'general',
-            'Complementary Results': 'general',
-            'Videos': 'videos',
-        }
-    elif level == 3:
-        header_dict = {
-            'Images for': 'images',
-            'Latest from': 'latest_from',
-            'Popular products': 'products',
-            'Quotes in the news': 'news_quotes',
-            'Recipes': 'recipes',
-            'Related searches': 'searches_related',
-            'Scholarly articles for': 'scholarly_articles',
-            'Top stories': 'top_stories',
-            'Videos': 'videos',
-            'View more news': 'view_more_news',
-            'View more videos': 'view_more_videos'
-        }
-
-    # Find headers, eg for level 2: <h2> or <div aria-level="2" role="heading">
-    header_list = []
-    header_list.extend(cmpt.find_all(f"h{level}", {"role":"heading"}))
-    header_list.extend(cmpt.find_all("div", {'aria-level':f"{level}", "role":"heading"}))
-
-   # Check for string matches in header text e.g. `h2.text`
-    for header in filter(None, header_list):
-        for text, label in header_dict.items():
-            if header.text.strip().startswith(text):
-                return label
-
-    # Return unknown if no matches
-    return "unknown"
-
-
-def classify_top_stories(cmpt: bs4.element.Tag):
-    """Classify top stories components
-    
-    Checks for g-scrolling-carousel & div id, not all top stories have an h3 tag
-    
-    """
-    conditions = [cmpt.find("g-scrolling-carousel"), 
-                  cmpt.find("div", {"id": "tvcap"})]
-    return 'top_stories' if all(conditions) else "unknown"
-
-
-def classify_img_cards(cmpt: bs4.element.Tag):
-    """Classify image cards components"""
-    if "class" in cmpt.attrs:
-        conditions = [
-            any(s in ["hlcw0c", "MjjYud"] for s in cmpt.attrs["class"]),
-            cmpt.find("block-component"),
+        # Ordered list of classifiers to try
+        component_classifiers = [
+            ClassifyMain.top_stories,        # Check top stories
+            ClassifyByHeader.classify,       # Check levels 2 & 3 header text
+            ClassifyMain.img_cards,          # Check image cards
+            ClassifyMain.images,             # Check images
+            ClassifyMain.knowledge_panel,    # Check knowledge panel
+            ClassifyMain.knowledge_block,    # Check knowledge components
+            ClassifyMain.banner,             # Check for banners
+            ClassifyMain.finance_panel,      # Check finance panel (classify as knowledge)
+            ClassifyMain.map_result,         # Check for map results
+            ClassifyMain.general_questions,  # Check hybrid general questions
+            ClassifyMain.twitter,            # Check twitter cards and results
+            ClassifyMain.general,            # Check general components
+            ClassifyMain.people_also_ask,    # Check people also ask
+            ClassifyMain.knowledge_box,      # Check flights, maps, hotels, events, jobs
+            ClassifyMain.local_results,      # Check for local results
+            ClassifyMain.available_on,       # Check for available on
         ]
-        return 'img_cards' if all(conditions) else "unknown"
-    else:
-        return "unknown"
-
-
-def classify_images(cmpt: bs4.element.Tag):
-    img_box = cmpt.find("div", {"id": "imagebox_bigimages"})
-    return 'images' if img_box else "unknown"
-
 
-def classify_knowledge_panel(cmpt: bs4.element.Tag):
-    condition = cmpt.find("div", {"class": ["knowledge-panel", "knavi", "kp-blk"]})
-    return 'knowledge' if condition else "unknown"
-
-
-def classify_finance_panel(cmpt: bs4.element.Tag):
-    condition = cmpt.find("div", {"id": "knowledge-finance-wholepage__entity-summary"})
-    return 'knowledge' if condition else "unknown"
-
-
-def classify_general_questions(cmpt: bs4.element.Tag):
-    hybrid = cmpt.find("div", {"class": "ifM9O"})
-    g_accordian = cmpt.find("g-accordion")
-    return 'general_questions' if hybrid and g_accordian else "unknown"
+        # Default unknown, exit on first successful classification
+        cmpt_type = "unknown"
+        for classifier in component_classifiers:
+            if cmpt_type != "unknown":  break
+            cmpt_type = classifier(cmpt)
+        
+        return cmpt_type
+
+
+    @staticmethod
+    def available_on(cmpt: bs4.element.Tag) -> str:
+        conditions = [("/Available on" in webutils.get_text(cmpt))]
+        return "available_on" if any(conditions) else "unknown"
 
+    @staticmethod
+    def banner(cmpt: bs4.element.Tag) -> str:
+        conditions = [
+            "ULSxyf" in cmpt.attrs.get("class", []),
+            cmpt.find("div", {"class": "uzjuFc"}),
+        ]
+        return 'banner' if all(conditions) else "unknown"
 
-def classify_twitter(cmpt: bs4.element.Tag):
-    cmpt_type = 'twitter' if cmpt.find('div', {'class': 'eejeod'}) else "unknown"
-    cmpt_type = classify_twitter_type(cmpt, cmpt_type)
-    return cmpt_type
+    @staticmethod
+    def finance_panel(cmpt: bs4.element.Tag) -> str:
+        condition = cmpt.find("div", {"id": "knowledge-finance-wholepage__entity-summary"})
+        return 'knowledge' if condition else "unknown"
+
+    @staticmethod
+    def general(cmpt: bs4.element.Tag) -> str:
+        """Classify general components"""
+
+        if "class" in cmpt.attrs:
+            conditions_dict = {
+                "format-01": cmpt.attrs["class"] == ["g"],
+                "format-02": ( ("g" in cmpt.attrs["class"]) &                            
+                               any(s in ["Ww4FFb"] for s in cmpt.attrs["class"]) ),
+                "format-03": any(s in ["hlcw0c", "MjjYud"] for s in cmpt.attrs["class"]),
+                "format-04": cmpt.find('div', {'class': ['g', 'Ww4FFb']}),
+            }
+        else: 
+            conditions_dict = {
+                'format-05': all(cmpt.find("div", {"class": c}) for c in ["g", "d4rhi"]),
+            }
+
+        layout_matches = [k for k, v in conditions_dict.items() if v]
+        # log.debug(f"general layout: {layout_matches}")
+        
+        return 'general' if any(layout_matches) else "unknown"
+
+    @staticmethod
+    def general_questions(cmpt: bs4.element.Tag) -> str:
+        hybrid = cmpt.find("div", {"class": "ifM9O"})
+        g_accordian = cmpt.find("g-accordion")
+        return 'general_questions' if hybrid and g_accordian else "unknown"
+
+    @staticmethod
+    def img_cards(cmpt: bs4.element.Tag) -> str:
+        """Classify image cards components"""
+        if "class" in cmpt.attrs:
+            conditions = [
+                any(s in ["hlcw0c", "MjjYud"] for s in cmpt.attrs["class"]),
+                cmpt.find("block-component"),
+            ]
+            return 'img_cards' if all(conditions) else "unknown"
+        else:
+            return "unknown"
 
+    @staticmethod
+    def images(cmpt: bs4.element.Tag) -> str:
+        conditions = [
+            cmpt.find("div", {"id": "imagebox_bigimages"}),  
+            cmpt.find("div", {"id":"iur"})
+        ]
+        return 'images' if any(conditions) else "unknown"
 
-def classify_twitter_type(cmpt: bs4.element.Tag, cmpt_type="unknown"):
-    """ Distinguish twitter types ('twitter_cards', 'twitter_result')"""
-    conditions = [
-        (cmpt_type == 'twitter'),                         # Check if already classified as twitter (header text)
-        (cmpt.find_previous().text == "Twitter Results")  # Check for twitter results text
-    ]
-    if any(conditions):
-        # Differentiate twitter cards (carousel) and twitter result (single)
-        carousel = cmpt.find("g-scrolling-carousel")
-        cmpt_type = "twitter_cards" if carousel else "twitter_result"
-    
-    return cmpt_type
+    @staticmethod
+    def knowledge_block(cmpt: bs4.element.Tag) -> str:
+        """Classify knowledge block components"""
+        conditions = [
+            webutils.check_dict_value(cmpt.attrs, "class", ["ULSxyf"]),
+            cmpt.find('block-component'),
+        ]
+        return 'knowledge' if all(conditions) else "unknown"
 
+    @staticmethod
+    def knowledge_box(cmpt: bs4.element.Tag) -> str:
+        """Classify knowledge component types"""
+        attrs = cmpt.attrs
+        condition = {}
+        condition['flights'] = (
+            (webutils.check_dict_value(attrs, "jscontroller", "Z2bSc")) |
+            bool(cmpt.find("div", {"jscontroller": "Z2bSc"}))
+        )
+        condition['maps'] = webutils.check_dict_value(attrs, "data-hveid", "CAMQAA")
+        condition['hotels'] = cmpt.find("div", {"class": "zd2Jbb"})
+        condition['events'] = cmpt.find("g-card", {"class": "URhAHe"})
+        condition['jobs'] = cmpt.find("g-card", {"class": "cvoI5e"})
+        text_list = list(cmpt.stripped_strings)
+        if text_list:
+            condition['covid_alert'] = (text_list[0] == "COVID-19 alert")
+        for condition_type, conditions in condition.items():
+            if conditions:
+                return condition_type
+        return "unknown"
 
-def classify_general(cmpt: bs4.element.Tag):
-    """Classify general components"""
-    if "class" in cmpt.attrs:
+    @staticmethod
+    def knowledge_panel(cmpt: bs4.element.Tag) -> str:
         conditions = [
-            cmpt.attrs["class"] == ["g"],                                # Only class is 'g'
-            (("g" in cmpt.attrs["class"]) &                              # OR contains 'g' and 'Ww4FFb'
-            any(s in ["Ww4FFb"] for s in cmpt.attrs["class"])),
-            any(s in ["hlcw0c", "MjjYud"] for s in cmpt.attrs["class"]), # OR contains 'hlcw0c' or 'MjjYud'
-            cmpt.find('div', {'class': ['g', 'Ww4FFb']}),                # OR contains 'g' and 'Ww4FFb' element
+            cmpt.find("div", {"class": ["knowledge-panel", "knavi", "kp-blk", "kp-wholepage-osrp"]}),
+            cmpt.find("div", {"aria-label": "Featured results", "role": "complementary"}),
         ]
-        return 'general' if any(conditions) else "unknown"
-    else:
-        return "unknown"
+        return 'knowledge' if any(conditions) else "unknown"
 
+    @staticmethod
+    def local_results(cmpt: bs4.element.Tag) -> str:
+        conditions = [
+            cmpt.find("div", {"class": "Qq3Lb"}),  # Places
+            cmpt.find("div", {"class": "VkpGBb"})  # Local Results
+        ]
+        return 'local_results' if any(conditions) else "unknown"
 
-def classify_general_subresult(cmpt: bs4.element.Tag):
-    # A general result followed by an indented result from the same domain
-    mask_class1 = cmpt.find_all('div', {'class':'g'})
-    mask_class2 = cmpt.find_all('div', {'class':'d4rhi'})
-    mask_sum = len(mask_class1) + len(mask_class2)
-    return 'general_subresult' if mask_sum > 1 else "unknown"
-
-
-def classify_banner(cmpt: bs4.element.Tag):
-    conditions = [
-        webutils.check_dict_value(cmpt.attrs, "class", ["ULSxyf"]),
-        cmpt.find("div", {"class": "uzjuFc"}),
-    ]
-    return 'banner' if all(conditions) else "unknown"
-
-
-def classify_hidden_survey(cmpt: bs4.element.Tag):
-    """Classify hidden survey components"""
-    conditions = [
-        webutils.check_dict_value(cmpt.attrs, "class", ["ULSxyf"]),
-        cmpt.find('promo-throttler'),
-    ]
-    return 'hidden_survey' if all(conditions) else "unknown"
-
-
-def classify_knowledge_block(cmpt: bs4.element.Tag):
-    """Classify knowledge block components"""
-    conditions = [
-        webutils.check_dict_value(cmpt.attrs, "class", ["ULSxyf"]),
-        cmpt.find('block-component'),
-    ]
-    return 'knowledge' if all(conditions) else "unknown"
-
-
-def classify_people_also_ask(cmpt: bs4.element.Tag):
-    """Secondary check for people also ask, see classify_header for primary"""
-    class_list = ["g", "kno-kp", "mnr-c", "g-blk"]
-    conditions = webutils.check_dict_value(cmpt.attrs, "class", class_list)
-    return 'people_also_ask' if conditions else "unknown"
-
-
-def classify_map_result(cmpt):
-    condition = cmpt.find("div", {"class": "lu_map_section"})
-    return 'map_results' if condition else "unknown"
-
-
-def classify_local_results(cmpt):
-    conditions = [
-        cmpt.find("div", {"class": "Qq3Lb"}),  # Places
-        cmpt.find("div", {"class": "VkpGBb"})  # Local Results
-    ]
-    return 'local_results' if any(conditions) else "unknown"
-
-
-def classify_knowledge_box(cmpt: bs4.element.Tag):
-    """Classify knowledge component types
-    
-    Creates conditions for each label in a dictionary then assigns the 
-    label as the component type if it's conditions are met using one, or some 
-    combination, of the following three methods:
-
-    1. Check if a component has a specific attribute value
-    2. Check if a component contains a specific div
-    3. Check if a component has a matching string in its text
-    
-    """
-    attrs = cmpt.attrs
-
-    condition = {}
-    condition['flights'] = (
-        (webutils.check_dict_value(attrs, "jscontroller", "Z2bSc")) |
-        bool(cmpt.find("div", {"jscontroller": "Z2bSc"}))
-    )
-    condition['maps'] = webutils.check_dict_value(attrs, "data-hveid", "CAMQAA")
-    condition['hotels'] = cmpt.find("div", {"class": "zd2Jbb"})
-    condition['events'] = cmpt.find("g-card", {"class": "URhAHe"})
-    condition['jobs'] = cmpt.find("g-card", {"class": "cvoI5e"})
-
-    text_list = list(cmpt.stripped_strings)
-    if text_list:
-        condition['covid_alert'] = (text_list[0] == "COVID-19 alert")
+    @staticmethod
+    def map_result(cmpt: bs4.element.Tag) -> str:
+        condition = cmpt.find("div", {"class": "lu_map_section"})
+        return 'map_results' if condition else "unknown"
+
+    @staticmethod
+    def people_also_ask(cmpt: bs4.element.Tag) -> str:
+        """Secondary check for people also ask, see classify_header for primary"""
+        class_list = ["g", "kno-kp", "mnr-c", "g-blk"]
+        conditions = webutils.check_dict_value(cmpt.attrs, "class", class_list)
+        return 'people_also_ask' if conditions else "unknown"
+
+    @staticmethod
+    def top_stories(cmpt: bs4.element.Tag) -> str:
+        """Classify top stories components"""
+        conditions = [
+            cmpt.find("g-scrolling-carousel"), 
+            cmpt.find("div", {"id": "tvcap"})
+        ]
+        return 'top_stories' if all(conditions) else "unknown"
 
-    for condition_type, conditions in condition.items():
-        return condition_type if conditions else "unknown"
+    @staticmethod
+    def twitter(cmpt: bs4.element.Tag) -> str:
+        cmpt_type = 'twitter' if cmpt.find('div', {'class': 'eejeod'}) else "unknown"
+        cmpt_type = ClassifyMain.twitter_type(cmpt, cmpt_type)
+        return cmpt_type
+
+    @staticmethod
+    def twitter_type(cmpt: bs4.element.Tag, cmpt_type="unknown") -> str:
+        """ Distinguish twitter types ('twitter_cards', 'twitter_result')"""
+        cmpt_prev = cmpt.find_previous()
+        conditions = [
+            (cmpt_type == 'twitter'),                                # Check type (header text)
+            webutils.get_text(cmpt, strip=True) == "Twitter Results" # Check text
+        ]
+        if any(conditions):
+            # Differentiate twitter cards (carousel) and twitter result (single)
+            carousel = cmpt.find("g-scrolling-carousel")
+            cmpt_type = "twitter_cards" if carousel else "twitter_result"
+        return cmpt_type
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/ads.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/images.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,114 @@
-from .. import webutils
+from ..models import BaseResult
+from ..webutils import get_text, get_link
 
-def parse_ads(cmpt):
-    """Parse ads from ad component"""
 
-    if cmpt.find_all('li', {'class':'ads-ad'}):
-        # Check for legacy ad format
-        subs = cmpt.find_all('li', {'class':'ads-ad'})
-        parser = parse_ad_legacy
-    elif cmpt.find_all('li', {'class':'ads-fr'}):
-        # Check for secondary ad format
-        subs = cmpt.find_all('li', {'class':'ads-fr'})
-        parser = parse_ad_secondary
-    else:
-        # Check for latest ad format
-        subs = cmpt.find_all('div', {'class':'uEierd'})
-        parser = parse_ad
-
-    return [parser(sub, sub_rank) for sub_rank, sub in enumerate(subs)]
-
-
-
-def parse_ad(sub, sub_rank=0, visible=None):
-    """Parse details of a single ad subcomponent, similar to general"""
-
-    parsed = {'type':'ad', 'sub_rank': sub_rank}
+def parse_images(cmpt):
+    """Parse an image component
     
-    submenu = parse_ad_menu(sub)
-    parsed['sub_type'] = 'submenu' if submenu else 'standard'
+    Args:
+        cmpt (bs4 object): an image component
     
-    parsed['title'] = webutils.get_text(sub, 'div', {'role':'heading'})
-    parsed['url'] = webutils.get_link(sub, {"class":"sVXRqc"})
-    parsed['cite'] = webutils.get_text(sub, 'span', {"role":"text"})
-    parsed['text'] = webutils.get_text(sub, 'div', {'class':'yDYNvb'})
-    parsed['details'] = parse_ad_menu(sub)
+    Returns:
+        list: list of parsed subcomponent dictionaries
+    """
+
+    parsed = []
+
+    # Small images: thumbnails with text labels
+    if cmpt.find('g-expandable-container'):
+        subs_small = cmpt.find_all('a', {'class': 'dgdd6c'})
+        parsed_small = [parse_image_small(div, sub_rank) for sub_rank, div in enumerate(subs_small)]
+        parsed.extend(parsed_small)
+
+    if cmpt.find('g-scrolling-carousel'):
+        # Medium images or video previews, no text labels
+        subs = cmpt.find_all('div', {'class':'eA0Zlc'})
+        _parsed = [parse_image_multimedia(sub, sub_rank + len(parsed)) for sub_rank, sub in enumerate(subs)]
+        parsed.extend(_parsed)
+    else:
+        # Medium images with titles and urls
+        subs = cmpt.find_all('div', {'class':'eA0Zlc'})
+        _parsed = [parse_image_medium(sub, sub_rank + len(parsed)) for sub_rank, sub in enumerate(subs)]
+        parsed.extend(_parsed)
+
+    # Filter empty results
+    parsed = [p for p in parsed if p['title']]
+            
     return parsed
 
 
-def parse_ad_menu(sub):
-    """Parse menu items for a large ad with additional subresults"""
+def parse_image_multimedia(sub, sub_rank=0):
+    """Parse an image subcomponent
+    
+    Args:
+        sub (bs4 object): an image subcomponent
+    
+    Returns:
+        dict : parsed subresult
+    """
+
+    parsed = BaseResult(
+        type="images",
+        sub_type="multimedia",
+        sub_rank=sub_rank,
+        title=get_img_alt(sub),
+        # url=get_img_url(sub), # dynamic load, no source url via requests
+    )
+    return parsed.model_dump()
 
-    parsed_list = []
-    menu_items = sub.find_all('div', {'class':'MhgNwc'})
-    for item in menu_items:
-        parsed = {}
-        item_divs = item.find_all('div', {'class':'MUxGbd'})
-        for div in item_divs:
-            if webutils.check_dict_value(div.attrs, 'role', 'listitem'):
-                parsed['url'] = webutils.get_link(div)
-                parsed['title'] = webutils.get_text(div)
-            else:
-                parsed['text'] = webutils.get_text(div)
-        parsed_list.append(parsed)
-    return parsed_list if parsed_list else None
-
-
-def parse_ad_secondary(sub, sub_rank=0, visible=None):
-    """Parse details of a single ad subcomponent, similar to general"""
-
-    parsed = {'type':'ad', 'sub_rank':sub_rank}
-    parsed['title'] = sub.find('div', {'role':'heading'}).text
-    parsed['url'] = sub.find('div', {'class':'d5oMvf'}).find('a')['href']
-    parsed['cite'] = sub.find('span', {'class':'gBIQub'}).text
-
-    # Take the top div with this class, should be main result abstract
-    text_divs = sub.find_all('div', {'class':'yDYNvb'})
-    parsed['text'] = '|'.join([d.text for d in text_divs]) if text_divs else ''
-    
-    bottom_section = sub.find('div', {'role':'list'})
-    if bottom_section:
-        list_items = sub.find_all('div', {'role':'listitem'})
-        if list_items:
-            parsed['details'] = [i.find('a')['href'] for i in list_items]
-
-    elif sub.find('div', {'class':'bOeY0b'}):
-        bottom_alinks = sub.find('div', {'class':'bOeY0b'}).find_all('a')
-        if bottom_alinks:
-            parsed['details'] = [a.attrs['href'] for a in bottom_alinks]
 
-    return parsed
+def parse_image_medium(sub, sub_rank=0):
+    """Parse an image subcomponent
+    
+    Args:
+        sub (bs4 object): an image subcomponent
+    
+    Returns:
+        dict : parsed subresult
+    """
 
-def parse_ad_legacy(sub, sub_rank=0, visible=None):
-    """[legacy] Parse details of a single ad subcomponent, similar to general"""
+    
+    parsed = BaseResult(
+        type="images",
+        sub_type="medium",
+        sub_rank=sub_rank,
+        title=get_text(sub, 'a', {'class':'EZAeBe'}),
+        url=get_link(sub, {'class':'EZAeBe'}),
+        cite=get_text(sub, 'div', {'class':'ptes9b'})
+    )
+    return parsed.model_dump()
 
-    parsed = {'type':'ad', 'sub_rank':sub_rank}
-    header = sub.find('div', {'class':'ad_cclk'})
-    parsed['title'] = header.find('h3').text
-    parsed['url'] = header.find('cite').text
-    parsed['text'] = sub.find('div', {'class':'ads-creative'}).text
-    
-    bottom_text = sub.find('ul')
-    if bottom_text:
-        bottom_li = bottom_text.find_all('li')
-        parsed['details'] = [li.get_text(separator=' ') for li in bottom_li]
 
-    return parsed
+def parse_image_small(sub, sub_rank=0):
+    """Parse an image subcomponent
+    
+    Args:
+        sub (bs4 object): an image subcomponent
+    
+    Returns:
+        dict : parsed subresult
+    """
+
+    parsed = BaseResult(
+        type="images",
+        sub_type="small",
+        sub_rank=sub_rank,
+        title=get_text(sub, 'div', {'class':'xlY4q'})
+    )
+    return parsed.model_dump()
+
+
+def get_img_url(soup):
+    """Get image source"""
+    try:
+        return soup.find('img').attrs['src']
+    except Exception:
+        return None
+
+
+def get_img_alt(soup):
+    """Get image alt text"""
+    try:
+        return f"alt-text: {soup.find('img').attrs['alt']}"
+    except Exception:
+        return None
```

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/available_on.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/available_on.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/banner.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/banner.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/general.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-import re
-from ..models import BaseResult
-from ..webutils import get_text, get_link
-
-def parse_general_results(cmpt):
-    """Parse a general component
-
-    The ubiquitous blue title, green citation, and black text summary results.
-    Sometimes grouped into components of multiple general results. The
-    subcomponent general results tend to have a similar theme.
-    
-    Args:
-        cmpt (bs4 object): A general component
-    
-    Returns:
-        list : list of parsed subcomponent dictionaries
-    """
-
-    # Legacy compatibility
-    subs = cmpt.find_all('div', {'class':'g'})
-
-    # 2023.05.09 - finds subs
-    additional = cmpt.find_all('div', {'class': 'd4rhi'})
-    if additional:
-        # Catch general_subresult
-        # this means that there is a sub-element, with class d4rhi
-        # the first div child of the div.g is the first sub element
-        first = cmpt.find('div')
-        subs = [first] + additional
-
-    # 2023.05.09 - handles duplicate .g tags within one component
-    if cmpt.find('div', {'class':'g'}):
-        parent_g = cmpt.find('div', {'class':'g'})
-        if parent_g.find_all('div', {'class':'g'}):
-            # this means that there is a .g element inside of another .g element,
-            # and it would otherwise get double-counted
-            # we just want to keep the parent .g element in this case
-            subs = [parent_g]
-    subs = subs if subs else [cmpt]
-
-    parsed = [parse_general_result(sub, sub_rank) for sub_rank, sub in enumerate(subs)]
-    return parsed
-   
-
-def parse_general_result(sub, sub_rank=0):
-    """Parse a general subcomponent
-    
-    Args:
-        sub (bs4 object): A general subcomponent
-    
-    Returns:
-        dict : parsed subresult
-    """
-    
-    if is_general_video(sub):
-        return parse_general_video(sub, sub_rank=sub_rank)
-
-    # Get title and text body divs
-    title_div = sub.find('div', {'class':'rc'}) or sub.find('div', {'class':'yuRUbf'})
-    body_div = sub.find('span', {'class':'st'}) or sub.find('div', {'class': 'VwiC3b'})
-
-    parsed = BaseResult(
-        type='general',
-        sub_rank=sub_rank,
-        title=get_text(title_div, 'h3') if title_div else '',
-        url=get_link(title_div) if title_div else '',
-        text=get_text(body_div) if body_div else '',
-        cite=get_text(sub, 'cite')
-    )
-
-    # Get subtype details
-    parsed = parse_subtype_details(sub, parsed)
-    return parsed.model_dump()
-
-
-def parse_alink(a): 
-    return {'text':a.text,'url':a.attrs['href']}
-
-
-def parse_alink_list(alinks):
-    return [parse_alink(a) for a in alinks if 'href' in a.attrs]
-
-
-def parse_subtype_details(sub, parsed):
-    # Check for subtype and parse details
-
-    details = {}
-
-    # If top menu with children, ignore URLs and get correct title URL
-    top_menu = sub.find('div', {'class':'yWc32e'})    
-    if top_menu:
-        has_children = list(top_menu.children)
-        if has_children: 
-            for child in top_menu.children:
-                child.decompose()
-            if sub.find('h3'):
-                parsed.url = sub.find('h3').find('a')['href']
-
-    # Subtype specific detail parsing
-    if 'class' in sub.attrs:
-        if sub.attrs['class'] == 'd4rhi':
-            parsed.sub_type == 'subresult'
-    
-    # Submenu - rating
-    elif sub.find('g-review-stars'):
-        parsed.sub_type = 'submenu_rating'
-        sibling = sub.find('g-review-stars').next_sibling
-        if sibling:
-            text = str(sibling).strip()
-            if len(text):
-                ratings = parse_ratings(text.split('-'))
-                details.update(ratings)
-    
-    # Submenu - list format
-    elif sub.find('div', {'class': ['P1usbc', 'IThcWe']}):
-        parsed.sub_type = 'submenu'
-        submenu_div = sub.find('div', {'class': ['P1usbc', 'IThcWe']})
-        if submenu_div:
-            alinks = submenu_div.find_all('a')
-            details['links'] = parse_alink_list(alinks)
-
-    # Submenu - table format
-    elif sub.find('table'):
-        parsed.sub_type = 'submenu'
-        alinks = sub.find('table').find_all('a')
-        details['links'] = parse_alink_list(alinks)
-
-    # Mini submenu
-    elif sub.find('div', {'class': ['osl', 'jYOxx']}):
-        parsed.sub_type = 'submenu_mini'  
-        alinks = sub.find('div', {'class':['osl','jYOxx']}).find_all('a')
-        details['links'] = parse_alink_list(alinks)
-
-    elif sub.find('div', {'class': re.compile('fG8Fp')}):
-
-        # Scholar results
-        alinks = sub.find('div', {'class': re.compile('fG8Fp')}).find_all('a')
-        if len(alinks) and 'Cited by' in alinks[0].text:
-            parsed.sub_type = 'submenu_scholarly'
-            details['links'] = parse_alink_list(alinks)
-
-        # Product results
-        text = get_text(sub, 'div', {'class': re.compile('fG8Fp')})
-        if not alinks and '$' in text:
-            parsed.sub_type = 'submenu_product'
-            product_details = parse_product(text) 
-            details.update(product_details)
-    
-    parsed.details = details if details else None          
-    return parsed
-
-
-def parse_ratings(text):
-    """Parse ratings that appear below some general components"""
-
-    text = [t.strip() for t in text]
-    numeric = re.compile('^\d*[.]?\d*$')
-    rating = re.split('Rating: ', text[0])[-1]
-    if numeric.match(rating):
-        details = {'rating': float(rating)}
-    else:
-        details = {'rating': rating}
-    
-    if len(text) > 1:
-        str_match_0 = re.compile(' vote[s]?| review[s]?')
-        str_match_1 = re.compile('Review by')
-        if str_match_0.search(text[1]):
-            reviews = re.split(str_match_0, text[1])[0]
-            reviews = reviews.replace(',','')[1:] # [1:] drops unicode char
-            details['reviews'] = int(reviews)
-        elif str_match_1.search(text[1]):
-            details['reviews'] = 1
-        
-    # could parse other fields
-    # (price, os, category) for products
-    # (time, cals) for recipes
-
-    return details
-
-def parse_product(text):
-    """Parse price and stock that appears below some general components"""
-    split_match = re.compile('-|·')
-    text = re.split(split_match, text)
-    if len(text) == 1:
-        return {'price': text[0].strip()[1:]}
-    else:
-        return {'price': text[0].strip()[1:], 'stock': text[1].strip()[1:]}
-
-
-# ------------------------------------------------------------------------------
-# General Video Results
-
-
-def is_general_video(cmpt):
-    """Check for a unique class name specific to video results"""
-    class_list = cmpt.get('class', [])
-    return 'PmEWq' in class_list
-
-
-def parse_general_video(sub, sub_rank: int = 0):
-    """Parse a general video component
-
-    Args:
-        cmpt (bs4 object): A general video component
-    
-    Returns:
-        VideoResult: Parsed information of the video
-    """
-
-    video_result = BaseResult(
-        type='general',
-        sub_type='video',
-        sub_rank=sub_rank,
-        title=get_result_text(sub, 'h3.LC20lb'),
-        url=sub.select_one('a[href]').get('href', '') if sub.select_one('a[href]') else '',
-        text=get_result_text(sub, '.ITZIwc'),
-        cite=get_result_text(sub, 'cite', strip=False),
-        details=get_result_details(sub),
-    )
-    return video_result.model_dump()
-
-
-def get_result_text(cmpt, selector, strip=True):
-    element = cmpt.select_one(selector)
-    return element.get_text(strip=strip) if element else ''
-
-
-def get_result_details(cmpt):
-    details = {"source": get_result_text(cmpt, '.gqF9jc', strip=False),
-               "duration": get_result_text(cmpt, '.JIv15d')}
+import re
+from ..models import BaseResult
+from ..webutils import get_text, get_link
+
+def parse_general_results(cmpt):
+    """Parse a general component
+
+    The ubiquitous blue title, green citation, and black text summary results.
+    Sometimes grouped into components of multiple general results. The
+    subcomponent general results tend to have a similar theme.
+    
+    Args:
+        cmpt (bs4 object): A general component
+    
+    Returns:
+        list : list of parsed subcomponent dictionaries
+    """
+
+    # Legacy compatibility
+    subs = cmpt.find_all('div', {'class':'g'})
+
+    # 2023.05.09 - finds subs
+    additional = cmpt.find_all('div', {'class': 'd4rhi'})
+    if additional:
+        # Catch general_subresult
+        # this means that there is a sub-element, with class d4rhi
+        # the first div child of the div.g is the first sub element
+        first = cmpt.find('div')
+        subs = [first] + additional
+
+    # 2023.05.09 - handles duplicate .g tags within one component
+    if cmpt.find('div', {'class':'g'}):
+        parent_g = cmpt.find('div', {'class':'g'})
+        if parent_g.find_all('div', {'class':'g'}):
+            # this means that there is a .g element inside of another .g element,
+            # and it would otherwise get double-counted
+            # we just want to keep the parent .g element in this case
+            subs = [parent_g]
+    subs = subs if subs else [cmpt]
+
+    parsed = [parse_general_result(sub, sub_rank) for sub_rank, sub in enumerate(subs)]
+    return parsed
+   
+
+def parse_general_result(sub, sub_rank=0):
+    """Parse a general subcomponent
+    
+    Args:
+        sub (bs4 object): A general subcomponent
+    
+    Returns:
+        dict : parsed subresult
+    """
+    
+    if is_general_video(sub):
+        return parse_general_video(sub, sub_rank=sub_rank)
+
+    # Get title and text body divs
+    title_div = sub.find('div', {'class':'rc'}) or sub.find('div', {'class':'yuRUbf'})
+    body_div = sub.find('span', {'class':'st'}) or sub.find('div', {'class': 'VwiC3b'})
+
+    parsed = BaseResult(
+        type='general',
+        sub_rank=sub_rank,
+        title=get_text(title_div, 'h3') if title_div else '',
+        url=get_link(title_div) if title_div else '',
+        text=get_text(body_div) if body_div else '',
+        cite=get_text(sub, 'cite')
+    )
+
+    # Get subtype details
+    parsed = parse_subtype_details(sub, parsed)
+    return parsed.model_dump()
+
+
+def parse_alink(a): 
+    return {'text':a.text,'url':a.attrs['href']}
+
+
+def parse_alink_list(alinks):
+    return [parse_alink(a) for a in alinks if 'href' in a.attrs]
+
+
+def parse_subtype_details(sub, parsed):
+    # Check for subtype and parse details
+
+    details = {}
+
+    # If top menu with children, ignore URLs and get correct title URL
+    top_menu = sub.find('div', {'class':'yWc32e'})    
+    if top_menu:
+        has_children = list(top_menu.children)
+        if has_children: 
+            for child in top_menu.children:
+                child.decompose()
+            if sub.find('h3'):
+                parsed.url = sub.find('h3').find('a')['href']
+
+    # Subtype specific detail parsing
+    if 'class' in sub.attrs:
+        if sub.attrs['class'] == 'd4rhi':
+            parsed.sub_type == 'subresult'
+    
+    # Submenu - rating
+    elif sub.find('g-review-stars'):
+        parsed.sub_type = 'submenu_rating'
+        sibling = sub.find('g-review-stars').next_sibling
+        if sibling:
+            text = str(sibling).strip()
+            if len(text):
+                ratings = parse_ratings(text.split('-'))
+                details.update(ratings)
+    
+    # Submenu - list format
+    elif sub.find('div', {'class': ['P1usbc', 'IThcWe']}):
+        parsed.sub_type = 'submenu'
+        submenu_div = sub.find('div', {'class': ['P1usbc', 'IThcWe']})
+        if submenu_div:
+            alinks = submenu_div.find_all('a')
+            details['links'] = parse_alink_list(alinks)
+
+    # Submenu - table format
+    elif sub.find('table'):
+        parsed.sub_type = 'submenu'
+        alinks = sub.find('table').find_all('a')
+        details['links'] = parse_alink_list(alinks)
+
+    # Mini submenu
+    elif sub.find('div', {'class': ['osl', 'jYOxx']}):
+        parsed.sub_type = 'submenu_mini'  
+        alinks = sub.find('div', {'class':['osl','jYOxx']}).find_all('a')
+        details['links'] = parse_alink_list(alinks)
+
+    elif sub.find('div', {'class': re.compile('fG8Fp')}):
+
+        # Scholar results
+        alinks = sub.find('div', {'class': re.compile('fG8Fp')}).find_all('a')
+        if len(alinks) and 'Cited by' in alinks[0].text:
+            parsed.sub_type = 'submenu_scholarly'
+            details['links'] = parse_alink_list(alinks)
+
+        # Product results
+        text = get_text(sub, 'div', {'class': re.compile('fG8Fp')})
+        if not alinks and '$' in text:
+            parsed.sub_type = 'submenu_product'
+            product_details = parse_product(text) 
+            details.update(product_details)
+    
+    parsed.details = details if details else None          
+    return parsed
+
+
+def parse_ratings(text):
+    """Parse ratings that appear below some general components"""
+
+    text = [t.strip() for t in text]
+    numeric = re.compile(r'^\d*[.]?\d*$')
+    rating = re.split('Rating: ', text[0])[-1]
+    if numeric.match(rating):
+        details = {'rating': float(rating)}
+    else:
+        details = {'rating': rating}
+    
+    if len(text) > 1:
+        str_match_0 = re.compile(' vote[s]?| review[s]?')
+        str_match_1 = re.compile('Review by')
+        if str_match_0.search(text[1]):
+            reviews = re.split(str_match_0, text[1])[0]
+            reviews = reviews.replace(',','')[1:] # [1:] drops unicode char
+            details['reviews'] = int(reviews)
+        elif str_match_1.search(text[1]):
+            details['reviews'] = 1
+        
+    # could parse other fields
+    # (price, os, category) for products
+    # (time, cals) for recipes
+
+    return details
+
+def parse_product(text):
+    """Parse price and stock that appears below some general components"""
+    split_match = re.compile('-|·')
+    text = re.split(split_match, text)
+    if len(text) == 1:
+        return {'price': text[0].strip()[1:]}
+    else:
+        return {'price': text[0].strip()[1:], 'stock': text[1].strip()[1:]}
+
+
+# ------------------------------------------------------------------------------
+# General Video Results
+
+
+def is_general_video(cmpt):
+    """Check for a unique class name specific to video results"""
+    class_list = cmpt.get('class', [])
+    return 'PmEWq' in class_list
+
+
+def parse_general_video(sub, sub_rank: int = 0):
+    """Parse a general video component
+
+    Args:
+        cmpt (bs4 object): A general video component
+    
+    Returns:
+        VideoResult: Parsed information of the video
+    """
+
+    video_result = BaseResult(
+        type='general',
+        sub_type='video',
+        sub_rank=sub_rank,
+        title=get_result_text(sub, 'h3.LC20lb'),
+        url=sub.select_one('a[href]').get('href', '') if sub.select_one('a[href]') else '',
+        text=get_result_text(sub, '.ITZIwc'),
+        cite=get_result_text(sub, 'cite', strip=False),
+        details=get_result_details(sub),
+    )
+    return video_result.model_dump()
+
+
+def get_result_text(cmpt, selector, strip=True):
+    element = cmpt.select_one(selector)
+    return element.get_text(strip=strip) if element else ''
+
+
+def get_result_details(cmpt):
+    details = {"source": get_result_text(cmpt, '.gqF9jc', strip=False),
+               "duration": get_result_text(cmpt, '.JIv15d')}
     return details
```

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/general_questions.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/general_questions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from . import parse_general_results
-from . import parse_people_also_ask
-
-def parse_general_questions(cmpt):
-    """Parse a General + People Also Ask hybrid component
-
-    These components consist of a general result followed by a people also
-    ask component with 3 subresults (questions).
-    
-    Args:
-        cmpt (bs4 object): A latest from component
-    
-    Returns:
-        dict : parsed result
-    """
-
-    result = parse_general_results(cmpt)
-    questions = parse_people_also_ask(cmpt)
-    result[0]['details'] = questions[0]['details']
-    result[0]['type'] = 'general_questions'
-    return result
-
-
+from .general import parse_general_results
+from .people_also_ask import parse_people_also_ask
+
+def parse_general_questions(cmpt):
+    """Parse a General + People Also Ask hybrid component
+
+    These components consist of a general result followed by a people also
+    ask component with 3 subresults (questions).
+    
+    Args:
+        cmpt (bs4 object): A latest from component
+    
+    Returns:
+        dict : parsed result
+    """
+
+    result = parse_general_results(cmpt)
+    questions = parse_people_also_ask(cmpt)
+    result[0]['details'] = questions[0]['details']
+    result[0]['type'] = 'general_questions'
+    return result
+
+
```

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge_rhs.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/knowledge_rhs.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/map_results.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/map_results.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/news_quotes.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/news_quotes.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/people_also_ask.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/people_also_ask.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/scholarly_articles.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/scholarly_articles.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/shopping_ads.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/shopping_ads.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/top_image_carousel.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/top_image_carousel.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/top_stories.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/top_stories.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_result.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/twitter_result.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/videos.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/videos.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/component_parsers/view_more_news.py` & `WebSearcher-0.4.0/WebSearcher/component_parsers/view_more_news.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/locations.py` & `WebSearcher-0.4.0/WebSearcher/locations.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,28 +49,29 @@
 
     Returns:
         None: Saves to file in the default or selected data_dir
 
     """
     os.makedirs(data_dir, exist_ok=True)
 
-    full_url = get_latest_url(url)
-    fp = os.path.join(data_dir, full_url.split('/')[-1])
+    url_latest = get_latest_url(url)
+    fp = os.path.join(data_dir, url_latest.split('/')[-1])
     fp_unzip = fp.replace('.zip', '')
 
     # Check if the current version already exists
     if os.path.exists(fp):
         print(f"Version up to date: {fp}")
     elif os.path.exists(fp_unzip):
         print(f"Version up to date: {fp_unzip}")
     else:
+        print(f"Version out of date")
         # Download and save
         try:
-            print(f'Getting: {full_url}')
-            response = requests.get(full_url)
+            print(f'getting: {url_latest}')
+            response = requests.get(url_latest)
         except Exception:
             log.exception('Failed to retrieve location data')
 
         if fp.endswith('.zip'):
             save_zip_response(response, fp_unzip)
         else:
             lines = response.content.decode('utf-8').split('\n')
@@ -83,27 +84,21 @@
         html = requests.get(url).content
         soup = wu.make_soup(html)
         url_list = [url for url in wu.get_link_list(soup) if url and url != '']
         geo_urls = [url for url in url_list if 'geotargets' in url]
 
         # Get current CSV url and use as filename
         geo_url = sorted(geo_urls)[-1]
-        full_url = 'https://developers.google.com' + geo_url
-        return full_url
+        url_latest = 'https://developers.google.com' + geo_url
+        return url_latest
 
     except Exception:
         log.exception("Failed to retrieve location data url")
 
 
-def get_all_urls(soup):
-    a_divs = soup.find_all('a')
-    all_urls = {a.attrs['href'] for a in a_divs if 'href' in a.attrs}    
-    return all_urls
-
-
 def save_zip_response(response: requests.Response, fp: str) -> None:
     with zipfile.ZipFile(io.BytesIO(response.content)) as zip_ref:
         for member in zip_ref.namelist():
             if member.endswith('.csv'):
                 with zip_ref.open(member) as csv_file:
                     reader = csv.reader(io.TextIOWrapper(csv_file, 'utf-8'))
                     write_csv(fp, reader=reader)
```

### Comparing `WebSearcher-0.3.9/WebSearcher/logger.py` & `WebSearcher-0.4.0/WebSearcher/logger.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/models.py` & `WebSearcher-0.4.0/WebSearcher/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from pydantic import BaseModel
-from typing import Any, Dict, Optional
+from typing import Any, Optional
+
 
 class BaseResult(BaseModel):
+    sub_rank: int = 0
     type: str = 'unclassified'
     sub_type: Optional[str] = None
-    sub_rank: int = 0
     title: Optional[str] = None
     url: Optional[str] = None
     text: Optional[str] = None
     cite: Optional[str] = None
     details: Optional[Any] = None
+    error: Optional[str] = None
+
 
 class BaseSERP(BaseModel):
     qry: str                   # Search query 
     loc: Optional[str] = None  # Location if set, "Canonical Name"
     url: str                   # URL of SERP   
     html: str                  # Raw HTML of SERP
-    # headers: Dict[str, str]    # HTTP headers
     timestamp: str             # Timestamp of crawl
     response_code: int         # HTTP response code
     user_agent: str            # User agent used for the crawl
     serp_id: str               # Search Engine Results Page (SERP) ID
     crawl_id: str              # Crawl ID for grouping SERPs
     version: str               # WebSearcher version
+
```

### Comparing `WebSearcher-0.3.9/WebSearcher/result_collector.py` & `WebSearcher-0.4.0/WebSearcher/result_collector.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/searchers.py` & `WebSearcher-0.4.0/WebSearcher/searchers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from .models import BaseSERP
 
 import os
 import time
 import brotli
 import requests
 import subprocess
-import pkg_resources
-from datetime import datetime
+from importlib import metadata
+from datetime import datetime, timezone
 from typing import Any, Dict, Optional
 
 # Current version
-WS_VERSION = pkg_resources.get_distribution('WebSearcher').version
+WS_VERSION = metadata.version('WebSearcher')
 
 # Default headers to send with requests (i.e. device fingerprint)
 DEFAULT_HEADERS = {
     'Host': 'www.google.com',
     'Referer': 'https://www.google.com/',
     'Accept': '*/*',
     'Accept-Encoding': 'gzip,deflate,br',
@@ -57,17 +57,18 @@
         self.base_url: str = 'https://www.google.com/search'
         self.headers: Dict[str, str] = headers
         self.sesh: requests.Session = sesh if sesh else wu.start_sesh(headers=self.headers)
         self.ssh_tunnel: subprocess.Popen = ssh_tunnel
         self.unzip: bool = unzip
         self.params: Dict[str, Any] = {}
 
-        # Initialize search data
+        # Initialize search details
         self.qry: str = None
         self.loc: str = None
+        self.num_results = None
         self.url: str = None
         self.timestamp: str = None
         self.serp_id: str = None
         self.crawl_id: str = None
         self.response: requests.Response = None
         self.html: str = None
         self.results: list = []
@@ -78,42 +79,46 @@
             console_level=log_level,
             file_name=log_fp, 
             file_mode=log_mode,
             file_level=log_level,
         ).start(__name__)
 
 
-    def search(self, qry: str, location: str = '', serp_id: str = '', crawl_id: str = ''):
+    def search(self, qry: str, location: str = '', num_results: int = None, serp_id: str = '', crawl_id: str = ''):
         """Conduct a search and save HTML
         
         Args:
             qry (str): The search query
             location (str, optional): A location's Canonical Name.
+            num_results (int, optional): The number of results to return.
             serp_id (str, optional): A unique identifier for this SERP
             crawl_id (str, optional): An identifier for this crawl
         """
-        self.prepare_search(qry, location)
-        self.conduct_search(serp_id, crawl_id)
+        self.prepare_search(qry=qry, location=location, num_results=num_results)
+        self.conduct_search(serp_id=serp_id, crawl_id=crawl_id)
         self.handle_response()
 
 
-    def prepare_search(self, qry: str, location: str = ''):
+    def prepare_search(self, qry: str, location: str = '', num_results: int = None):
         """Prepare a search URL and metadata for the given query and location"""
         self.qry = str(qry)
         self.loc = str(location)
+        self.num_results = num_results
         self.params = {}
         self.params['q'] = wu.encode_param_value(self.qry)
+        if num_results is not None:
+            self.params['num'] = self.num_results
         if location:
             self.params['uule'] = locations.get_location_id(canonical_name=self.loc)
 
 
     def conduct_search(self, serp_id: str = '', crawl_id: str = ''):
         """Send a search request and handle errors"""
 
-        self.timestamp = datetime.utcnow().isoformat()
+        self.timestamp = datetime.now(timezone.utc).replace(tzinfo=None).isoformat()
         self.serp_id = serp_id if serp_id else utils.hash_id(self.qry + self.loc + self.timestamp)
         self.crawl_id = crawl_id
         try:
             self.send_request()
         except requests.exceptions.ConnectionError:
             self.log.exception(f'SERP | Connection error | {self.serp_id}')
             self.reset_ssh_tunnel()
@@ -137,24 +142,19 @@
             self.ssh_tunnel.open_tunnel()
             self.log.info(f'SERP | Restarted SSH tunnel | {self.serp_id}')
             time.sleep(10) # Allow time to establish connection
 
 
     def handle_response(self):
         try:
-            # Unzip string if True
             if self.unzip:  
                 self.unzip_html()
             else:
-                # Get response string
                 self.html = self.response.content
-
-            # Decode string
             self.html = self.html.decode('utf-8', 'ignore')
-        
         except Exception:
             self.log.exception(f'Response handling error')
 
 
     def unzip_html(self):
         """Unzip brotli zipped html 
 
@@ -176,15 +176,15 @@
 
 
     def parse_results(self):
         """Parse a SERP - see parsers.py"""
 
         assert self.html, "No HTML found"
         try:
-            self.results = parsers.parse_serp(self.html, serp_id=self.serp_id, make_soup=True)
+            self.results = parsers.parse_serp(self.html)
         except Exception:
             self.log.exception(f'Parsing error | serp_id : {self.serp_id}')
 
 
     def save_serp(self, save_dir: str = '', append_to: str = ""):
         """Save SERP to file
```

### Comparing `WebSearcher-0.3.9/WebSearcher/utils.py` & `WebSearcher-0.4.0/WebSearcher/utils.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.9/WebSearcher/webutils.py` & `WebSearcher-0.4.0/WebSearcher/webutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from . import utils
 from . import logger
 log = logger.Logger().start(__name__)
 
 import os
 import re
 import atexit
+import brotli
 import requests
 import subprocess
 import tldextract
 import urllib.parse as urlparse
 from bs4 import BeautifulSoup
 
 
 def load_html(fp, zipped=False):
     """Load html file, with option for brotli decompression"""
+    read_func = lambda i: brotli.decompress(i.read()) if zipped else i.read()
     read_type = 'rb' if zipped else 'r'
     with open(fp, read_type) as infile:
-        return infile.read()
+        return read_func(infile)
 
 
 def load_soup(fp, zipped=False):
     return make_soup(load_html(fp, zipped))
 
 
 def start_sesh(headers=None, proxy_port=None):
@@ -57,15 +59,18 @@
 
 def strip_html_tags(string):
     """Strips HTML <tags>"""
     return re.sub('<[^<]+?>', '', string)
 
 def make_soup(html, parser='lxml'):
     """Create soup object"""
-    return BeautifulSoup(html, parser)
+    if isinstance(html, BeautifulSoup):
+        return html
+    else:
+        return BeautifulSoup(html, parser)
 
 def has_captcha(soup):
     """Boolean for 'CAPTCHA' appearance in soup"""
     return True if soup.find(text=re.compile('CAPTCHA')) else False
 
 def get_html_language(soup):
     try:
@@ -92,40 +97,51 @@
 
 # Get divs, links, and text ----------------------------------------------------
 
 def get_div(soup: BeautifulSoup, name: str, attrs: dict = {}) -> BeautifulSoup:
     """Utility for `soup.find(name)` with null attrs handling"""
     return soup.find(name, attrs) if attrs else soup.find(name)
 
-def get_text(soup, name: str=None, attrs: dict={}, separator:str=" ") -> str:
+def get_text(soup: BeautifulSoup, name: str=None, attrs: dict={}, separator:str=" ", strip=False) -> str:
     """Utility for `soup.find(name).text` with null name handling"""
+    if not soup:
+        return None
     div = get_div(soup, name, attrs) if name else soup
-    return div.get_text(separator=separator) if div else None
+    if not div:
+        return None
+    text = div.get_text(separator=separator)
+    return text.strip() if strip else text
+
+
 
 def get_link(soup: BeautifulSoup, attrs: dict = {}, key: str = 'href') -> str:
     """Utility for `soup.find('a')['href']` with null key handling"""
     link = get_div(soup, 'a', attrs)
     return link.attrs.get(key, None) if link else None
 
-def get_link_list(soup: BeautifulSoup, attrs: dict = {}, key: str = 'href') -> list:
+def get_link_list(soup: BeautifulSoup, attrs: dict = {}, key: str = 'href', filter_empty: bool = True) -> list:
     """Utility for `soup.find_all('a')['href']` with null key handling"""
-    links = find_all_divs(soup, 'a', attrs)
+    links = find_all_divs(soup, 'a', attrs, filter_empty)
     return [link.attrs.get(key, None) for link in links] if links else None
 
 def find_all_divs(soup: BeautifulSoup, name: str, attrs: dict = {}, filter_empty: bool = True) -> list:
     divs = soup.find_all(name, attrs) if attrs else soup.find_all(name)
     if filter_empty:
         divs = [c for c in divs if c]
         divs = [c for c in divs if c.text != '']
     return divs
 
-def find_children(soup, name: str, attrs: dict = {}) -> list:
+def find_children(soup, name: str, attrs: dict = {}, filter_empty: bool = False):
     """Find all children of a div with a given name and attribute"""
     div = get_div(soup, name, attrs)
-    return div.children if div else []
+    divs = div.children if div else []
+    if divs and filter_empty:
+        divs = [c for c in divs if c]
+        divs = [c for c in divs if c.text != '']
+    return divs
 
 
 # URLs -------------------------------------------------------------------------
 
 def join_url_quote(quote_dict):
     return '&'.join([f'{k}={v}' for k, v in quote_dict.items()])
```

### Comparing `WebSearcher-0.3.9/WebSearcher.egg-info/PKG-INFO` & `WebSearcher-0.4.0/WebSearcher.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebSearcher
-Version: 0.3.9
+Version: 0.4.0
 Summary: WebSearcher
 Home-page: http://github.com/gitronald/WebSearcher
 Author: Ronald E. Robertson
 Author-email: rer@acm.org
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `WebSearcher-0.3.9/WebSearcher.egg-info/SOURCES.txt` & `WebSearcher-0.4.0/WebSearcher.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 WebSearcher/__init__.py
-WebSearcher/component_classifier.py
+WebSearcher/components.py
 WebSearcher/extractors.py
 WebSearcher/locations.py
 WebSearcher/logger.py
 WebSearcher/models.py
 WebSearcher/parsers.py
 WebSearcher/result_collector.py
 WebSearcher/searchers.py
 WebSearcher/utils.py
 WebSearcher/webutils.py
 WebSearcher.egg-info/PKG-INFO
 WebSearcher.egg-info/SOURCES.txt
 WebSearcher.egg-info/dependency_links.txt
 WebSearcher.egg-info/requires.txt
 WebSearcher.egg-info/top_level.txt
+WebSearcher/classifiers/__init__.py
+WebSearcher/classifiers/footer.py
+WebSearcher/classifiers/headers.py
+WebSearcher/classifiers/main.py
 WebSearcher/component_parsers/__init__.py
 WebSearcher/component_parsers/ads.py
 WebSearcher/component_parsers/available_on.py
 WebSearcher/component_parsers/banner.py
+WebSearcher/component_parsers/discussions_and_forums.py
 WebSearcher/component_parsers/footer.py
 WebSearcher/component_parsers/general.py
 WebSearcher/component_parsers/general_questions.py
 WebSearcher/component_parsers/images.py
 WebSearcher/component_parsers/knowledge.py
 WebSearcher/component_parsers/knowledge_rhs.py
 WebSearcher/component_parsers/latest_from.py
```

### Comparing `WebSearcher-0.3.9/setup.py` & `WebSearcher-0.4.0/setup.py`

 * *Files identical despite different names*

