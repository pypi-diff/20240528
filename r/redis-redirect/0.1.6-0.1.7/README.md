# Comparing `tmp/redis_redirect-0.1.6.tar.gz` & `tmp/redis_redirect-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_redirect-0.1.6.tar", last modified: Tue May 28 15:20:05 2024, max compression
+gzip compressed data, was "redis_redirect-0.1.7.tar", last modified: Tue May 28 16:11:38 2024, max compression
```

## Comparing `redis_redirect-0.1.6.tar` & `redis_redirect-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:20:05.933371 redis_redirect-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 15:20:05.933371 redis_redirect-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 15:20:05.933371 redis_redirect-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:20:05.929371 redis_redirect-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:20:05.933371 redis_redirect-0.1.6/src/redis_redirect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 15:20:05.000000 redis_redirect-0.1.6/src/redis_redirect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 15:20:05.000000 redis_redirect-0.1.6/src/redis_redirect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:20:05.000000 redis_redirect-0.1.6/src/redis_redirect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 15:20:05.000000 redis_redirect-0.1.6/src/redis_redirect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:20:05.000000 redis_redirect-0.1.6/src/redis_redirect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:20:05.933371 redis_redirect-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/tests/test_aioredis_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-28 15:19:57.000000 redis_redirect-0.1.6/tests/test_redis_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:11:38.475684 redis_redirect-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 16:11:38.475684 redis_redirect-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 16:11:38.475684 redis_redirect-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:11:38.471684 redis_redirect-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:11:38.475684 redis_redirect-0.1.7/src/redis_redirect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 16:11:38.000000 redis_redirect-0.1.7/src/redis_redirect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-28 16:11:38.000000 redis_redirect-0.1.7/src/redis_redirect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:11:38.000000 redis_redirect-0.1.7/src/redis_redirect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 16:11:38.000000 redis_redirect-0.1.7/src/redis_redirect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:11:38.000000 redis_redirect-0.1.7/src/redis_redirect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:11:38.475684 redis_redirect-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/tests/test_aioredis_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-28 16:11:25.000000 redis_redirect-0.1.7/tests/test_redis_wrapper.py
```

### Comparing `redis_redirect-0.1.6/LICENSE.txt` & `redis_redirect-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redis_redirect-0.1.6/PKG-INFO` & `redis_redirect-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-redirect
-Version: 0.1.6
+Version: 0.1.7
 Summary: (aio)REDIS wrapper to deal with cluster redirect exceptions (`MOVED`).
 Home-page: https://github.com/andgineer/redis-redirect
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: redis asyncio wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `redis_redirect-0.1.6/README.md` & `redis_redirect-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `redis_redirect-0.1.6/setup.py` & `redis_redirect-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `redis_redirect-0.1.6/src/redis_redirect.egg-info/PKG-INFO` & `redis_redirect-0.1.7/src/redis_redirect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-redirect
-Version: 0.1.6
+Version: 0.1.7
 Summary: (aio)REDIS wrapper to deal with cluster redirect exceptions (`MOVED`).
 Home-page: https://github.com/andgineer/redis-redirect
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: redis asyncio wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `redis_redirect-0.1.6/tests/test_aioredis_wrapper.py` & `redis_redirect-0.1.7/tests/test_aioredis_wrapper.py`

 * *Files identical despite different names*

### Comparing `redis_redirect-0.1.6/tests/test_redis_wrapper.py` & `redis_redirect-0.1.7/tests/test_redis_wrapper.py`

 * *Files identical despite different names*

