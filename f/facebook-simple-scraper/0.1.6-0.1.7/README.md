# Comparing `tmp/facebook_simple_scraper-0.1.6.tar.gz` & `tmp/facebook_simple_scraper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_simple_scraper-0.1.6.tar", last modified: Tue May 28 13:31:36 2024, max compression
+gzip compressed data, was "facebook_simple_scraper-0.1.7.tar", last modified: Tue May 28 14:03:36 2024, max compression
```

## Comparing `facebook_simple_scraper-0.1.6.tar` & `facebook_simple_scraper-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363836 facebook_simple_scraper-0.1.6/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.6/LICENCE
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 13:31:36.363645 facebook_simple_scraper-0.1.6/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.6/README.md
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.359367 facebook_simple_scraper-0.1.6/facebook_simple_scraper/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       54 2024-05-28 13:31:04.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/credentials_ring.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/default_values.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3290 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/dependency_builder.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.360586 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     6742 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/extractor.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     4633 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/repository.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3973 2024-05-28 13:14:01.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/entities.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/error_dict.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.362019 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1028 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/domain.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     7520 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/login.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1872 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/params.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1315 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/session_storage.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      108 2024-05-19 20:11:09.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/urls.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3133 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/user_info.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.362599 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     6807 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_extractor.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3713 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_repository.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363161 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/__init__.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1243 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/headers.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     3231 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/requester.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2489 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/scraper.py
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper/stop_conditions.py
-drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:31:36.363417 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hectoroliveros   (501) staff       (20)     1289 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/requires.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 13:31:36.000000 facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/top_level.txt
--rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 13:31:36.363878 facebook_simple_scraper-0.1.6/setup.cfg
--rw-r--r--   0 hectoroliveros   (501) staff       (20)      929 2024-05-28 13:30:53.000000 facebook_simple_scraper-0.1.6/setup.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.178919 facebook_simple_scraper-0.1.7/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1055 2024-05-27 21:08:24.000000 facebook_simple_scraper-0.1.7/LICENCE
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 14:03:36.178745 facebook_simple_scraper-0.1.7/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1455 2024-05-27 21:02:09.000000 facebook_simple_scraper-0.1.7/README.md
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.174566 facebook_simple_scraper-0.1.7/facebook_simple_scraper/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       54 2024-05-28 14:03:34.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      497 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/credentials_ring.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      202 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/default_values.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3429 2024-05-28 14:02:29.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/dependency_builder.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.175782 facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     6742 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/extractor.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     4633 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/repository.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3973 2024-05-28 13:14:01.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/entities.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      727 2024-05-21 19:24:05.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/error_dict.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.177218 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1028 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/domain.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     7520 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/login.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1872 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/params.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1315 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/session_storage.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      108 2024-05-19 20:11:09.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/urls.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3133 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/user_info.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.177715 facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     6807 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/summary_extractor.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3713 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/summary_repository.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.178232 facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 13:19:48.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/__init__.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1243 2024-05-21 22:19:56.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/headers.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     3231 2024-05-28 13:08:33.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/requester.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2604 2024-05-28 14:02:29.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/scraper.py
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2898 2024-05-28 13:08:43.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper/stop_conditions.py
+drwxr-xr-x   0 hectoroliveros   (501) staff       (20)        0 2024-05-28 14:03:36.178514 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     2115 2024-05-28 14:03:36.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)     1289 2024-05-28 14:03:36.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)        1 2024-05-28 14:03:36.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      103 2024-05-28 14:03:36.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/requires.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       24 2024-05-28 14:03:36.000000 facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/top_level.txt
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)       38 2024-05-28 14:03:36.178956 facebook_simple_scraper-0.1.7/setup.cfg
+-rw-r--r--   0 hectoroliveros   (501) staff       (20)      929 2024-05-28 14:03:34.000000 facebook_simple_scraper-0.1.7/setup.py
```

### Comparing `facebook_simple_scraper-0.1.6/LICENCE` & `facebook_simple_scraper-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/PKG-INFO` & `facebook_simple_scraper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.6/README.md` & `facebook_simple_scraper-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/dependency_builder.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/dependency_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from facebook_simple_scraper.entities import ScraperOptions, SessionStorage
 from facebook_simple_scraper.login.login import MobileBasicLoginRepository
 from facebook_simple_scraper.login.params import MbasicLoginParamsRepository
 from facebook_simple_scraper.login.session_storage import LocalFileSessionStorage
 from facebook_simple_scraper.posts.summary_extractor import PostSummaryListExtractor
 from facebook_simple_scraper.posts.summary_repository import PostSummaryListRepository, GetPostOptions
 from facebook_simple_scraper.requester import requester
+from facebook_simple_scraper.requester.requester import Requester
 
 
 class AbstractScraperDependencyBuilder:
     """Abstract class for building dependencies for a web scraper."""
 
     @staticmethod
     def build_deps(opts: ScraperOptions) -> Tuple[MobileBasicLoginRepository, PostSummaryListRepository]:
@@ -27,27 +28,28 @@
     You can extend this class to create a custom implementation.
     For example you can:
         - Change session storage so that it stores the session in a database instead of a file.
         - Change the requester to use a proxy.
     """
 
     @staticmethod
-    def build_deps(opts: ScraperOptions) -> Tuple[MobileBasicLoginRepository, PostSummaryListRepository]:
+    def build_deps(opts: ScraperOptions, req: Optional[Requester] = None) -> Tuple[
+        MobileBasicLoginRepository, PostSummaryListRepository]:
         """Build the default dependencies for the scraper.
 
         Args:
             opts (ScraperOptions): The options/configuration for the scraper.
 
         Returns:
             Tuple[MobileBasicLoginRepository, PostSummaryListRepository]: A tuple
             containing the login repository and post summary repository.
         """
-
-        # Create a requester for Facebook sessions
-        req = requester.FacebookSessionBasedRequester()
+        if req is None:
+            # Create a requester for Facebook sessions
+            req = requester.FacebookSessionBasedRequester()
 
         # Create a repository for login parameters
         params_repo = MbasicLoginParamsRepository(req)
 
         session_storage: Optional[SessionStorage] = None
         # Determine session storage mechanism
         if opts.session_storage is None:
```

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/extractor.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/extractor.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/details/repository.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/details/repository.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/entities.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/entities.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/error_dict.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/error_dict.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/domain.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/domain.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/login.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/login.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/params.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/params.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/session_storage.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/session_storage.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/login/user_info.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/login/user_info.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_extractor.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/summary_extractor.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/posts/summary_repository.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/posts/summary_repository.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/headers.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/headers.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/requester/requester.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/requester/requester.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/scraper.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         """
         # Build the necessary dependencies
         login_repo, post_repo = self.deps_builder.build_deps(self.opts)
 
         # Iterate through the credentials in a ring buffer fashion
         for cred in self.creds_ring.next():
             # Login using the current credential
-            login_repo.login(cred.username, cred.password)
+            login_resp = login_repo.login(cred.username, cred.password)
+            login_repo, post_repo = self.deps_builder.build_deps(self.opts, req=login_resp.requester)
 
             # Get posts using the post repository and stop conditions
             gen = post_repo.get_posts(account_ids, self.opts.stop_conditions)
 
             # Yield each post
             for post in gen:
                 yield post
```

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper/stop_conditions.py` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/PKG-INFO` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_simple_scraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple scraper for Facebook
 Home-page: https://github.com/Eitol/facebook_simple_scraper
 Author: Hector Oliveros
 Author-email: hector.oliveros.leon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook_simple_scraper-0.1.6/facebook_simple_scraper.egg-info/SOURCES.txt` & `facebook_simple_scraper-0.1.7/facebook_simple_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook_simple_scraper-0.1.6/setup.py` & `facebook_simple_scraper-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facebook_simple_scraper',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(include=['facebook_simple_scraper', 'facebook_simple_scraper.*']),
     include_package_data=True,
     install_requires=[
         'pydantic~=2.7.1',
         'requests~=2.31.0',
         'beautifulsoup4~=4.12.3',
         'python-dateutil~=2.9.0.post0',
```

