# Comparing `tmp/fastapi_ext_pkg-0.2.0.tar.gz` & `tmp/fastapi_ext_pkg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ext_pkg-0.2.0.tar", last modified: Wed May 15 18:30:01 2024, max compression
+gzip compressed data, was "fastapi_ext_pkg-0.3.0.tar", last modified: Tue May 28 20:23:26 2024, max compression
```

## Comparing `fastapi_ext_pkg-0.2.0.tar` & `fastapi_ext_pkg-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 18:29:35.000000 fastapi_ext_pkg-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 18:30:01.000000 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 18:30:01.000000 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:30:01.000000 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:30:01.000000 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 18:30:01.000000 fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/fastapi_extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.000000 fastapi_ext_pkg-0.2.0/fastapi_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/fastapi_extras/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.000000 fastapi_ext_pkg-0.2.0/fastapi_extras/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 18:29:35.000000 fastapi_ext_pkg-0.2.0/fastapi_extras/middlewares/remove_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 18:29:35.000000 fastapi_ext_pkg-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:30:01.359513 fastapi_ext_pkg-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.681258 fastapi_ext_pkg-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-28 20:23:26.681258 fastapi_ext_pkg-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.677258 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-28 20:23:26.000000 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-28 20:23:26.000000 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:23:26.000000 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 20:23:26.000000 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 20:23:26.000000 fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.677258 fastapi_ext_pkg-0.3.0/fastapi_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.677258 fastapi_ext_pkg-0.3.0/fastapi_extras/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/databases/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.677258 fastapi_ext_pkg-0.3.0/fastapi_extras/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/middlewares/remove_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:26.677258 fastapi_ext_pkg-0.3.0/fastapi_extras/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/fastapi_extras/security/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-28 20:23:00.000000 fastapi_ext_pkg-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:23:26.681258 fastapi_ext_pkg-0.3.0/setup.cfg
```

### Comparing `fastapi_ext_pkg-0.2.0/PKG-INFO` & `fastapi_ext_pkg-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-ext-pkg
-Version: 0.2.0
+Version: 0.3.0
 Summary: A well-tailored utility set for FastAPI.
 Author-email: Dotz Developers <devs-dotz@dotz.com>
 Project-URL: Repository, https://github.com/DotzInc/fastapi-ext-pkg
 Keywords: fastapi,utilities
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
+Requires-Dist: httpx
 
 # FastAPI Extension Package
 
 ![Tests](https://github.com/DotzInc/fastapi-ext-pkg/actions/workflows/tests.yml/badge.svg?event=push)
 ![PyPI - Version](https://img.shields.io/pypi/v/fastapi-ext-pkg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-ext-pkg)
```

### Comparing `fastapi_ext_pkg-0.2.0/fastapi_ext_pkg.egg-info/PKG-INFO` & `fastapi_ext_pkg-0.3.0/fastapi_ext_pkg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-ext-pkg
-Version: 0.2.0
+Version: 0.3.0
 Summary: A well-tailored utility set for FastAPI.
 Author-email: Dotz Developers <devs-dotz@dotz.com>
 Project-URL: Repository, https://github.com/DotzInc/fastapi-ext-pkg
 Keywords: fastapi,utilities
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
+Requires-Dist: httpx
 
 # FastAPI Extension Package
 
 ![Tests](https://github.com/DotzInc/fastapi-ext-pkg/actions/workflows/tests.yml/badge.svg?event=push)
 ![PyPI - Version](https://img.shields.io/pypi/v/fastapi-ext-pkg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-ext-pkg)
```

### Comparing `fastapi_ext_pkg-0.2.0/pyproject.toml` & `fastapi_ext_pkg-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi-ext-pkg"
-version = "0.2.0"
+version = "0.3.0"
 description = "A well-tailored utility set for FastAPI."
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "Dotz Developers", email = "devs-dotz@dotz.com"},
 ]
 keywords = ["fastapi", "utilities"]
 classifiers = [
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet",
     "Topic :: Software Development",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.8"
-dependencies = ["fastapi"]
+dependencies = ["fastapi", "httpx"]
 
 [project.urls]
 Repository = "https://github.com/DotzInc/fastapi-ext-pkg"
 
 [tool.ruff]
 exclude = [
     ".git",
```

