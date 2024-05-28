# Comparing `tmp/facebook_simple_scraper-0.1.5.tar.gz` & `tmp/facebook_simple_scraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_simple_scraper-0.1.5.tar", last modified: Tue May 28 12:55:10 2024, max compression
+gzip compressed data, was "facebook_simple_scraper-0.1.6.tar", last modified: Tue May 28 13:31:36 2024, max compression
```

## Comparing `facebook_simple_scraper-0.1.5.tar` & `facebook_simple_scraper-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,41 @@
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:55:10.327731 facebook_simple_scraper-0.1.5/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.5/LICENCE
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:55:10.327537 facebook_simple_scraper-0.1.5/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.5/README.md
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:55:10.327311 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:55:10.000000 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      420 2024-05-28 12:55:10.000000 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 12:55:10.000000 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 12:55:10.000000 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/requires.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        4 2024-05-28 12:55:10.000000 facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/top_level.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 12:55:10.327917 facebook_simple_scraper-0.1.5/setup.cfg
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      857 2024-05-28 12:55:09.000000 facebook_simple_scraper-0.1.5/setup.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:55:10.327048 facebook_simple_scraper-0.1.5/src/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       54 2024-05-28 12:54:47.000000 facebook_simple_scraper-0.1.5/src/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      477 2024-05-28 12:52:32.000000 facebook_simple_scraper-0.1.5/src/credentials_ring.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.5/src/default_values.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3110 2024-05-28 12:52:32.000000 facebook_simple_scraper-0.1.5/src/dependency_builder.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3933 2024-05-28 12:52:55.000000 facebook_simple_scraper-0.1.5/src/entities.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.5/src/error_dict.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2429 2024-05-28 12:52:32.000000 facebook_simple_scraper-0.1.5/src/scraper.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2878 2024-05-28 12:52:32.000000 facebook_simple_scraper-0.1.5/src/stop_conditions.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363836 facebook_simple_scraper-0.1.6/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.6/LICENCE
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 13:31:36.363645 facebook_simple_scraper-0.1.6/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.6/README.md
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.359367 facebook_simple_scraper-0.1.6/facebook_simple_scraper/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       54 2024-05-28 13:31:04.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/credentials_ring.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/default_values.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3290 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/dependency_builder.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.360586 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     6742 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/extractor.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     4633 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/repository.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3973 2024-05-28 13:14:01.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/entities.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/error_dict.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.362019 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1028 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/domain.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     7520 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/login.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1872 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/params.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1315 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/session_storage.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      108 2024-05-19 20:11:09.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/urls.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3133 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/user_info.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.362599 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     6807 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_extractor.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3713 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_repository.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363161 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1243 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/headers.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3231 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/requester.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/scraper.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/stop_conditions.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363417 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1289 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/requires.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/top_level.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 13:31:36.363878 facebook_simple_scraper-0.1.6/setup.cfg
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      929 2024-05-28 13:30:53.000000 facebook_simple_scraper-0.1.6/setup.py
```

### Comparing `facebook_simple_scraper-0.1.5/LICENCE` & `facebook_simple_scraper-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.5/PKG-INFO` & `facebook_simple_scraper-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.5/README.md` & `facebook_simple_scraper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.5/facebook_simple_scraper.egg-info/PKG-INFO` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.5/setup.py` & `facebook_simple_scraper-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facebook_simple_scraper',
-    version='0.1.5',
-    packages=["src"],
+    version='0.1.6',
+    packages=find_packages(include=['facebook_simple_scraper', 'facebook_simple_scraper.*']),
     include_package_data=True,
     install_requires=[
         'pydantic~=2.7.1',
         'requests~=2.31.0',
         'beautifulsoup4~=4.12.3',
         'python-dateutil~=2.9.0.post0',
         'dateparser~=1.2.0',
```

### Comparing `facebook_simple_scraper-0.1.5/src/dependency_builder.py` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper/dependency_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Tuple, Optional
 
-from src.details.repository import GraphqlCommentsRepository
-from src.default_values import DEFAULT_SESSION_DIR
-from src.entities import ScraperOptions, SessionStorage
-from src.login.login import MobileBasicLoginRepository
-from src.login.params import MbasicLoginParamsRepository
-from src.login.session_storage import LocalFileSessionStorage
-from src.posts.summary_extractor import PostSummaryListExtractor
-from src.posts.summary_repository import PostSummaryListRepository, GetPostOptions
-from src.requester import requester
+from facebook_simple_scraper.details.repository import GraphqlCommentsRepository
+from facebook_simple_scraper.default_values import DEFAULT_SESSION_DIR
+from facebook_simple_scraper.entities import ScraperOptions, SessionStorage
+from facebook_simple_scraper.login.login import MobileBasicLoginRepository
+from facebook_simple_scraper.login.params import MbasicLoginParamsRepository
+from facebook_simple_scraper.login.session_storage import LocalFileSessionStorage
+from facebook_simple_scraper.posts.summary_extractor import PostSummaryListExtractor
+from facebook_simple_scraper.posts.summary_repository import PostSummaryListRepository, GetPostOptions
+from facebook_simple_scraper.requester import requester
 
 
 class AbstractScraperDependencyBuilder:
     """Abstract class for building dependencies for a web scraper."""
 
     @staticmethod
     def build_deps(opts: ScraperOptions) -> Tuple[MobileBasicLoginRepository, PostSummaryListRepository]:
```

### Comparing `facebook_simple_scraper-0.1.5/src/entities.py` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import BaseModel, HttpUrl
 
-from src.default_values import DEFAULT_MAX_COMMENTS_PER_POST, DEFAULT_SLEEP_TIME_MAX, \
+from facebook_simple_scraper.default_values import DEFAULT_MAX_COMMENTS_PER_POST, DEFAULT_SLEEP_TIME_MAX, \
     DEFAULT_SLEEP_TIME_MIN
-from src.requester import requester
+from facebook_simple_scraper.requester import requester
 
 
 class MediaQuality(Enum):
     LOW = 'low'
     MEDIUM = 'medium'
     HIGH = 'high'
```

### Comparing `facebook_simple_scraper-0.1.5/src/error_dict.py` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper/error_dict.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.5/src/scraper.py` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Iterable
 
-from src.credentials_ring import CredentialsRingBuffer
-from src.dependency_builder import AbstractScraperDependencyBuilder, DefaultScraperDependencyBuilder
-from src.entities import ScraperOptions, Post
+from facebook_simple_scraper.credentials_ring import CredentialsRingBuffer
+from facebook_simple_scraper.dependency_builder import AbstractScraperDependencyBuilder, DefaultScraperDependencyBuilder
+from facebook_simple_scraper.entities import ScraperOptions, Post
 
 
 class Scraper:
     """Main scraper class responsible for scraping posts from an account."""
 
     def __init__(self, opts: ScraperOptions, deps_builder: Optional[AbstractScraperDependencyBuilder] = None):
         """Initialize the scraper with options and dependencies builder.
```

### Comparing `facebook_simple_scraper-0.1.5/src/stop_conditions.py` & `facebook_simple_scraper-0.1.6/facebook_simple_scraper/stop_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from typing import List
 
-from src.entities import Post, StopCondition
+from facebook_simple_scraper.entities import Post, StopCondition
 
 
 class StopAfterNPosts(StopCondition):
     """Stop condition that stops scraping after a specified number of posts."""
 
     def __init__(self, n: int):
         """
```

