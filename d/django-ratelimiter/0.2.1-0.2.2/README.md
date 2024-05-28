# Comparing `tmp/django_ratelimiter-0.2.1.tar.gz` & `tmp/django_ratelimiter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ratelimiter-0.2.1.tar", max compression
+gzip compressed data, was "django_ratelimiter-0.2.2.tar", max compression
```

## Comparing `django_ratelimiter-0.2.1.tar` & `django_ratelimiter-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/LICENSE
--rw-r--r--   0        0        0     4855 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/README.md
--rw-r--r--   0        0        0      144 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/__init__.py
--rw-r--r--   0        0        0     2502 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/decorator.py
--rw-r--r--   0        0        0     2221 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/middleware.py
--rw-r--r--   0        0        0        0 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/py.typed
--rw-r--r--   0        0        0     1666 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/storage.py
--rw-r--r--   0        0        0      315 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/types.py
--rw-r--r--   0        0        0     1950 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/django_ratelimiter/utils.py
--rw-r--r--   0        0        0     1214 2024-04-23 17:03:09.953274 django_ratelimiter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 django_ratelimiter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4855 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/README.md
+-rw-r--r--   0        0        0      144 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/__init__.py
+-rw-r--r--   0        0        0     2502 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/decorator.py
+-rw-r--r--   0        0        0     2221 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/py.typed
+-rw-r--r--   0        0        0     1666 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/storage.py
+-rw-r--r--   0        0        0      315 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/types.py
+-rw-r--r--   0        0        0     1950 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/django_ratelimiter/utils.py
+-rw-r--r--   0        0        0     1239 2024-05-28 15:46:59.109405 django_ratelimiter-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 django_ratelimiter-0.2.2/PKG-INFO
```

### Comparing `django_ratelimiter-0.2.1/LICENSE` & `django_ratelimiter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/README.md` & `django_ratelimiter-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/django_ratelimiter/decorator.py` & `django_ratelimiter-0.2.2/django_ratelimiter/decorator.py`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/django_ratelimiter/middleware.py` & `django_ratelimiter-0.2.2/django_ratelimiter/middleware.py`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/django_ratelimiter/storage.py` & `django_ratelimiter-0.2.2/django_ratelimiter/storage.py`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/django_ratelimiter/utils.py` & `django_ratelimiter-0.2.2/django_ratelimiter/utils.py`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.2.1/pyproject.toml` & `django_ratelimiter-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ratelimiter"
-version = "0.2.1"
+version = "0.2.2"
 description = "Rate-limiting for django"
 authors = ["Andrii Kohut <kogut.andriy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://andriykohut.github.io/django-ratelimiter/"
 repository = "https://github.com/andriykohut/django-ratelimiter"
 documentation = "https://andriykohut.github.io/django-ratelimiter/"
@@ -14,29 +14,29 @@
 python = ">=3.9"
 django = "*"
 limits = ">=3.10"
 typing-extensions = { version = "^4.11.0", python = "3.9" }
 
 
 [tool.poetry.group.dev.dependencies]
-django-stubs = "^4.2.7"
+django-stubs = ">=4.2.7,<6.0.0"
 mypy = "^1.9.0"
 black = "^24.4.0"
-ruff = "^0.3.5"
+ruff = ">=0.3.5,<0.5.0"
 pytest = "^8.1.1"
 freezegun = "^1.4.0"
 pymemcache = "^4.0.0"
 redis = "^5.0.3"
 pytest-cov = "^5.0.0"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.18"
 djangorestframework = "^3.15.1"
 django-ninja = "^1.1.0"
 pytest-django = "^4.8.0"
-mkdocstrings = { extras = ["python"], version = "^0.24.3" }
+mkdocstrings = { extras = ["python"], version = ">=0.24.3,<0.26.0" }
 mike = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `django_ratelimiter-0.2.1/PKG-INFO` & `django_ratelimiter-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ratelimiter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rate-limiting for django
 Home-page: https://andriykohut.github.io/django-ratelimiter/
 License: MIT
 Keywords: rate-limit,django
 Author: Andrii Kohut
 Author-email: kogut.andriy@gmail.com
 Requires-Python: >=3.9
```

