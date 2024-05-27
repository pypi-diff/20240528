# Comparing `tmp/acrclient-0.4.5.tar.gz` & `tmp/acrclient-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrclient-0.4.5.tar", max compression
+gzip compressed data, was "acrclient-0.4.6.tar", max compression
```

## Comparing `acrclient-0.4.5.tar` & `acrclient-0.4.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2287 2024-04-12 09:06:39.845582 acrclient-0.4.5/README.md
--rw-r--r--   0        0        0      322 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/__init__.py
--rw-r--r--   0        0        0     5367 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/client.py
--rw-r--r--   0        0        0      819 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/models.py
--rw-r--r--   0        0        0        0 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/py.typed
--rw-r--r--   0        0        0     1284 2024-04-12 09:06:54.197681 acrclient-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 acrclient-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     2287 2024-05-27 21:58:05.794185 acrclient-0.4.6/README.md
+-rw-r--r--   0        0        0      322 2024-05-27 21:58:05.794185 acrclient-0.4.6/acrclient/__init__.py
+-rw-r--r--   0        0        0     5367 2024-05-27 21:58:05.794185 acrclient-0.4.6/acrclient/client.py
+-rw-r--r--   0        0        0      819 2024-05-27 21:58:05.794185 acrclient-0.4.6/acrclient/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:58:05.794185 acrclient-0.4.6/acrclient/py.typed
+-rw-r--r--   0        0        0     1292 2024-05-27 21:58:20.530057 acrclient-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 acrclient-0.4.6/PKG-INFO
```

### Comparing `acrclient-0.4.5/README.md` & `acrclient-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.5/acrclient/client.py` & `acrclient-0.4.6/acrclient/client.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.5/acrclient/models.py` & `acrclient-0.4.6/acrclient/models.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.5/pyproject.toml` & `acrclient-0.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrclient"
-version = "v0.4.5"
+version = "v0.4.6"
 description = "API wrapper for the v2 ACRCloud API"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-v3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -18,27 +18,27 @@
 python = "^3.11"
 requests = ">=2.28.2"
 cachecontrol = ">=0.13,<0.15"
 
 [tool.poetry.group.dev.dependencies]
 freezegun = "^1.2.2"
 Markdown = "^3.3"
-mkdocstrings = {extras = ["python"], version = ">=0.21.2,<0.25.0"}
+mkdocstrings = {extras = ["python"], version = ">=0.21.2,<0.26.0"}
 mkdocs-material = "^9.1"
 mkdocs = "^1.4.2"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 pytest = ">=8.1.1,<9.0.0"
 pytest-cov = ">=4,<6"
 pytest-mypy = "^0.10.3"
 pytest-random-order = "^1.1.0"
 pytest-ruff = "^0.3.1"
 requests-mock = "^1.10.0"
-ruff = "^0.3.2"
+ruff = ">=0.3.2,<0.5.0"
 types-requests = "^2.28.11"
 wheel = ">=0.40,<0.44"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=acrclient --cov-fail-under=100 --ignore=docs/ --ruff --mypy"
 filterwarnings = [
```

### Comparing `acrclient-0.4.5/PKG-INFO` & `acrclient-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrclient
-Version: 0.4.5
+Version: 0.4.6
 Summary: API wrapper for the v2 ACRCloud API
 License: AGPL-v3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

