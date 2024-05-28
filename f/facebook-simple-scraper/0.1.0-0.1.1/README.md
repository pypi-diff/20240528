# Comparing `tmp/facebook_simple_scraper-0.1.0.tar.gz` & `tmp/facebook_simple_scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_simple_scraper-0.1.0.tar", last modified: Mon May 27 21:08:48 2024, max compression
+gzip compressed data, was "facebook_simple_scraper-0.1.1.tar", last modified: Tue May 28 11:13:57 2024, max compression
```

## Comparing `facebook_simple_scraper-0.1.0.tar` & `facebook_simple_scraper-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-27 21:08:48.709450 facebook_simple_scraper-0.1.0/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.0/LICENCE
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2102 2024-05-27 21:08:48.709260 facebook_simple_scraper-0.1.0/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.0/README.md
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-27 21:08:48.708088 facebook_simple_scraper-0.1.0/facebook_simple_scraper/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-27 21:04:17.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/credentials_ring.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/default_values.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3291 2024-05-27 18:22:31.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/dependency_builder.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3863 2024-05-27 18:32:28.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/entities.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/error_dict.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-21 22:31:37.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/scraper.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-21 16:26:34.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper/stop_conditions.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-27 21:08:48.709041 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2102 2024-05-27 21:08:48.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      580 2024-05-27 21:08:48.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-27 21:08:48.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-27 21:08:48.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/requires.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-27 21:08:48.000000 facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/top_level.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-27 21:08:48.709489 facebook_simple_scraper-0.1.0/setup.cfg
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      815 2024-05-27 21:08:28.000000 facebook_simple_scraper-0.1.0/setup.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 11:13:57.804267 facebook_simple_scraper-0.1.1/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.1/LICENCE
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2102 2024-05-28 11:13:57.804054 facebook_simple_scraper-0.1.1/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.1/README.md
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 11:13:57.802881 facebook_simple_scraper-0.1.1/facebook_simple_scraper/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-27 21:04:17.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/credentials_ring.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/default_values.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3290 2024-05-27 22:05:24.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/dependency_builder.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3898 2024-05-27 22:04:12.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/entities.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/error_dict.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-21 22:31:37.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/scraper.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-21 16:26:34.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper/stop_conditions.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 11:13:57.803839 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2102 2024-05-28 11:13:57.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      580 2024-05-28 11:13:57.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 11:13:57.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 11:13:57.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/requires.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 11:13:57.000000 facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/top_level.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 11:13:57.804312 facebook_simple_scraper-0.1.1/setup.cfg
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      815 2024-05-28 11:12:01.000000 facebook_simple_scraper-0.1.1/setup.py
```

### Comparing `facebook_simple_scraper-0.1.0/LICENCE` & `facebook_simple_scraper-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/PKG-INFO` & `facebook_simple_scraper-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `facebook_simple_scraper-0.1.0/README.md` & `facebook_simple_scraper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper/dependency_builder.py` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper/dependency_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple, Optional
 
-from facebook_simple_scraper.comments.repository import GraphqlCommentsRepository
+from facebook_simple_scraper.details.repository import GraphqlCommentsRepository
 from facebook_simple_scraper.default_values import DEFAULT_SESSION_DIR
 from facebook_simple_scraper.entities import ScraperOptions, SessionStorage
 from facebook_simple_scraper.login.login import MobileBasicLoginRepository
 from facebook_simple_scraper.login.params import MbasicLoginParamsRepository
 from facebook_simple_scraper.login.session_storage import LocalFileSessionStorage
 from facebook_simple_scraper.posts.summary_extractor import PostSummaryListExtractor
 from facebook_simple_scraper.posts.summary_repository import PostSummaryListRepository, GetPostOptions
```

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper/entities.py` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     text: str
     date: datetime
     image_url: str
     video_url: str
     like_count: int
     comment_count: int
     comments: List[Comment] = []
+    reactions: List[Reaction] = []
 
 
 class PostList(BaseModel):
     posts: List[Post]
     cursor: str
     profile_id: str
```

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper/error_dict.py` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper/error_dict.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper/scraper.py` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper/stop_conditions.py` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/PKG-INFO` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `facebook_simple_scraper-0.1.0/facebook_simple_scraper.egg-info/SOURCES.txt` & `facebook_simple_scraper-0.1.1/facebook_simple_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.0/setup.py` & `facebook_simple_scraper-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facebook_simple_scraper',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'pydantic~=2.7.1',
         'requests~=2.31.0',
         'beautifulsoup4~=4.12.3',
         'python-dateutil~=2.9.0.post0',
         'dateparser~=1.2.0',
```

