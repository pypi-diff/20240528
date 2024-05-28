# Comparing `tmp/facebook_simple_scraper-0.1.3.tar.gz` & `tmp/facebook_simple_scraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_simple_scraper-0.1.3.tar", last modified: Tue May 28 12:47:01 2024, max compression
+gzip compressed data, was "facebook_simple_scraper-0.1.4.tar", last modified: Tue May 28 12:51:05 2024, max compression
```

## Comparing `facebook_simple_scraper-0.1.3.tar` & `facebook_simple_scraper-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:47:01.381416 facebook_simple_scraper-0.1.3/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.3/LICENCE
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:47:01.381223 facebook_simple_scraper-0.1.3/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.3/README.md
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:47:01.380213 facebook_simple_scraper-0.1.3/facebook_simple_scraper/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       53 2024-05-28 12:45:46.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/credentials_ring.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/default_values.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3290 2024-05-27 22:05:24.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/dependency_builder.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3973 2024-05-28 11:49:34.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/entities.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/error_dict.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-21 22:31:37.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/scraper.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-21 16:26:34.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper/stop_conditions.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:47:01.381001 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:47:01.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      580 2024-05-28 12:47:01.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 12:47:01.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 12:47:01.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/requires.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 12:47:01.000000 facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/top_level.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 12:47:01.381455 facebook_simple_scraper-0.1.3/setup.cfg
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      877 2024-05-28 12:46:37.000000 facebook_simple_scraper-0.1.3/setup.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:51:05.814032 facebook_simple_scraper-0.1.4/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.4/LICENCE
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:51:05.813803 facebook_simple_scraper-0.1.4/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.4/README.md
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:51:05.812710 facebook_simple_scraper-0.1.4/facebook_simple_scraper/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       53 2024-05-28 12:51:03.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/credentials_ring.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/default_values.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3290 2024-05-27 22:05:24.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/dependency_builder.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3925 2024-05-28 12:50:49.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/entities.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/error_dict.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-21 22:31:37.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/scraper.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-21 16:26:34.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper/stop_conditions.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 12:51:05.813574 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 12:51:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      580 2024-05-28 12:51:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 12:51:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 12:51:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/requires.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 12:51:05.000000 facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/top_level.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 12:51:05.814083 facebook_simple_scraper-0.1.4/setup.cfg
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      877 2024-05-28 12:51:03.000000 facebook_simple_scraper-0.1.4/setup.py
```

### Comparing `facebook_simple_scraper-0.1.3/LICENCE` & `facebook_simple_scraper-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/PKG-INFO` & `facebook_simple_scraper-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.3/README.md` & `facebook_simple_scraper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper/dependency_builder.py` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper/dependency_builder.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper/entities.py` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import BaseModel, HttpUrl
 
-from facebook_simple_scraper.default_values import DEFAULT_MAX_COMMENTS_PER_POST, DEFAULT_SLEEP_TIME_MAX, \
+from default_values import DEFAULT_MAX_COMMENTS_PER_POST, DEFAULT_SLEEP_TIME_MAX, \
     DEFAULT_SLEEP_TIME_MIN
-from facebook_simple_scraper.requester import requester
+from requester import requester
 
 
 class MediaQuality(Enum):
     LOW = 'low'
     MEDIUM = 'medium'
     HIGH = 'high'
```

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper/error_dict.py` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper/error_dict.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper/scraper.py` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper/stop_conditions.py` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/PKG-INFO` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.3/facebook_simple_scraper.egg-info/SOURCES.txt` & `facebook_simple_scraper-0.1.4/facebook_simple_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.3/setup.py` & `facebook_simple_scraper-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facebook_simple_scraper',
-    version='0.1.3',
+    version='0.1.4',
     packages=["facebook_simple_scraper"],
     include_package_data=True,
     install_requires=[
         'pydantic~=2.7.1',
         'requests~=2.31.0',
         'beautifulsoup4~=4.12.3',
         'python-dateutil~=2.9.0.post0',
```

