# Comparing `tmp/djpress-0.3.2.tar.gz` & `tmp/djpress-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.3.2.tar", last modified: Mon May 27 13:05:06 2024, max compression
+gzip compressed data, was "djpress-0.3.3.tar", last modified: Tue May 28 08:16:30 2024, max compression
```

## Comparing `djpress-0.3.2.tar` & `djpress-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.593070 djpress-0.3.2/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.3.2/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.3.2/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     3907 2024-05-27 13:05:06.592801 djpress-0.3.2/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1208 2024-05-25 22:35:25.000000 djpress-0.3.2/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.585769 djpress-0.3.2/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      784 2024-05-27 13:00:19.000000 djpress-0.3.2/djpress/app_settings.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)     1154 2024-05-27 13:00:19.000000 djpress-0.3.2/djpress/conf.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.587271 djpress-0.3.2/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2929 2024-05-27 10:44:59.000000 djpress-0.3.2/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      358 2024-05-27 10:44:59.000000 djpress-0.3.2/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.587774 djpress-0.3.2/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.581971 djpress-0.3.2/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.582022 djpress-0.3.2/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.588332 djpress-0.3.2/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)     3325 2024-05-27 10:57:47.000000 djpress-0.3.2/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)     2449 2024-05-27 10:58:33.000000 djpress-0.3.2/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.582139 djpress-0.3.2/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.588637 djpress-0.3.2/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2150 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.589280 djpress-0.3.2/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8228 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2196 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/helpers.py
--rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.592249 djpress-0.3.2/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     3907 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1002 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       71 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.589451 djpress-0.3.2/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.3.2/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     2064 2024-05-27 13:00:19.000000 djpress-0.3.2/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-27 13:05:06.593120 djpress-0.3.2/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       69 2024-05-27 09:29:30.000000 djpress-0.3.2/setup.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.591874 djpress-0.3.2/tests/
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14772 2024-05-25 22:18:09.000000 djpress-0.3.2/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.3.2/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.3.2/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4686 2024-05-27 13:00:19.000000 djpress-0.3.2/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 08:16:23.000000 djpress-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 08:16:23.000000 djpress-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-28 08:16:30.514467 djpress-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 08:16:23.000000 djpress-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/feeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/static/djpress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/static/djpress/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/static/djpress/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/templates/djpress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templates/djpress/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/djpress_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/djpress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 08:16:23.000000 djpress-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 08:16:23.000000 djpress-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:16:30.514467 djpress-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 08:16:23.000000 djpress-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_category_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_djpress_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_post_authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_published_posts_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_views.py
```

### Comparing `djpress-0.3.2/LICENSE` & `djpress-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/PKG-INFO` & `djpress-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.2
+Version: 0.3.3
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,19 +36,20 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: markdown
 Requires-Dist: pygments
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `djpress-0.3.2/README.md` & `djpress-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/app_settings.py` & `djpress-0.3.3/djpress/app_settings.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/conf.py` & `djpress-0.3.3/djpress/conf.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/feeds.py` & `djpress-0.3.3/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/migrations/0001_initial.py` & `djpress-0.3.3/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/models/category.py` & `djpress-0.3.3/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/models/post.py` & `djpress-0.3.3/djpress/models/post.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/signals.py` & `djpress-0.3.3/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/static/djpress/css/style.css` & `djpress-0.3.3/djpress/static/djpress/css/style.css`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/static/djpress/css/style.min.css` & `djpress-0.3.3/djpress/static/djpress/css/style.min.css`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/templates/djpress/index.html` & `djpress-0.3.3/djpress/templates/djpress/index.html`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/templatetags/djpress_tags.py` & `djpress-0.3.3/djpress/templatetags/djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/templatetags/helpers.py` & `djpress-0.3.3/djpress/templatetags/helpers.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/urls.py` & `djpress-0.3.3/djpress/urls.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/utils.py` & `djpress-0.3.3/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress/views.py` & `djpress-0.3.3/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/djpress.egg-info/PKG-INFO` & `djpress-0.3.3/djpress.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.2
+Version: 0.3.3
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,19 +36,20 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: markdown
 Requires-Dist: pygments
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `djpress-0.3.2/djpress.egg-info/SOURCES.txt` & `djpress-0.3.3/djpress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/pyproject.toml` & `djpress-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.3.2"
+version = "0.3.3"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dependencies = ["django", "markdown", "pygments"]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 keywords = ["django", "blog", "cms", "markdown", "wordpress"]
```

### Comparing `djpress-0.3.2/tests/test_category_cache.py` & `djpress-0.3.3/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_djpress_tags.py` & `djpress-0.3.3/tests/test_djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_feeds.py` & `djpress-0.3.3/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_models.py` & `djpress-0.3.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_post_authors.py` & `djpress-0.3.3/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_published_posts_cache.py` & `djpress-0.3.3/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.2/tests/test_views.py` & `djpress-0.3.3/tests/test_views.py`

 * *Files identical despite different names*

