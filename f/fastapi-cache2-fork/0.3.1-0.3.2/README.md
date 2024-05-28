# Comparing `tmp/fastapi_cache2_fork-0.3.1.tar.gz` & `tmp/fastapi_cache2_fork-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cache2_fork-0.3.1.tar", max compression
+gzip compressed data, was "fastapi_cache2_fork-0.3.2.tar", max compression
```

## Comparing `fastapi_cache2_fork-0.3.1.tar` & `fastapi_cache2_fork-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11338 2023-11-28 08:51:24.085360 fastapi_cache2_fork-0.3.1/LICENSE
--rw-r--r--   0        0        0     8414 2023-11-28 08:51:24.085360 fastapi_cache2_fork-0.3.1/README.md
--rw-r--r--   0        0        0     3033 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/__init__.py
--rw-r--r--   0        0        0      625 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/backends/__init__.py
--rw-r--r--   0        0        0     3392 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/backends/dynamodb.py
--rw-r--r--   0        0        0     1582 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/backends/inmemory.py
--rw-r--r--   0        0        0      672 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/backends/memcached.py
--rw-r--r--   0        0        0     1325 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/backends/redis.py
--rw-r--r--   0        0        0     3877 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/coder.py
--rw-r--r--   0        0        0     7955 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/decorator.py
--rw-r--r--   0        0        0      553 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/key_builder.py
--rw-r--r--   0        0        0        0 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/py.typed
--rw-r--r--   0        0        0     1015 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/fastapi_cache/types.py
--rw-r--r--   0        0        0     3037 2023-11-28 08:51:24.089360 fastapi_cache2_fork-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9664 1970-01-01 00:00:00.000000 fastapi_cache2_fork-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-11-28 03:34:37.840046 fastapi_cache2_fork-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8414 2023-11-28 08:31:12.442297 fastapi_cache2_fork-0.3.2/README.md
+-rw-r--r--   0        0        0     3033 2023-11-28 08:31:08.936610 fastapi_cache2_fork-0.3.2/fastapi_cache/__init__.py
+-rw-r--r--   0        0        0      625 2023-11-28 03:34:37.841394 fastapi_cache2_fork-0.3.2/fastapi_cache/backends/__init__.py
+-rw-r--r--   0        0        0     3392 2023-11-28 03:49:33.208925 fastapi_cache2_fork-0.3.2/fastapi_cache/backends/dynamodb.py
+-rw-r--r--   0        0        0     1582 2023-11-28 03:49:33.208157 fastapi_cache2_fork-0.3.2/fastapi_cache/backends/inmemory.py
+-rw-r--r--   0        0        0      672 2023-11-28 03:49:33.208112 fastapi_cache2_fork-0.3.2/fastapi_cache/backends/memcached.py
+-rw-r--r--   0        0        0     2090 2024-05-28 11:30:22.097721 fastapi_cache2_fork-0.3.2/fastapi_cache/backends/redis.py
+-rw-r--r--   0        0        0     3877 2023-11-28 05:08:34.692856 fastapi_cache2_fork-0.3.2/fastapi_cache/coder.py
+-rw-r--r--   0        0        0     7955 2023-11-28 08:32:40.563077 fastapi_cache2_fork-0.3.2/fastapi_cache/decorator.py
+-rw-r--r--   0        0        0      553 2023-11-28 03:49:33.208558 fastapi_cache2_fork-0.3.2/fastapi_cache/key_builder.py
+-rw-r--r--   0        0        0        0 2023-11-28 03:34:37.842169 fastapi_cache2_fork-0.3.2/fastapi_cache/py.typed
+-rw-r--r--   0        0        0     1015 2023-11-28 04:09:40.445265 fastapi_cache2_fork-0.3.2/fastapi_cache/types.py
+-rw-r--r--   0        0        0     2914 2024-05-28 11:29:29.045889 fastapi_cache2_fork-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 fastapi_cache2_fork-0.3.2/PKG-INFO
```

### Comparing `fastapi_cache2_fork-0.3.1/LICENSE` & `fastapi_cache2_fork-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/README.md` & `fastapi_cache2_fork-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/__init__.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/backends/__init__.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/backends/dynamodb.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/backends/inmemory.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/backends/inmemory.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/backends/memcached.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/coder.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/coder.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/decorator.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/decorator.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/key_builder.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/key_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/fastapi_cache/types.py` & `fastapi_cache2_fork-0.3.2/fastapi_cache/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_cache2_fork-0.3.1/pyproject.toml` & `fastapi_cache2_fork-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 [tool.poetry]
 name = "fastapi-cache2-fork"
-version = "0.3.1"
+version = "0.3.2"
 description = "Cache for FastAPI. An opinionated fork of fastapi-cache library that uses msgspec for json encoding/decoding where possible"
 authors = ["long2ice <long2ice@gmail.com>", "Yolley <comingreal@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Yolley/fastapi-cache"
 repository = "https://github.com/Yolley/fastapi-cache.git"
 documentation = "https://github.com/Yolley/fastapi-cache"
 keywords = ["fastapi", "cache", "caching"]
 packages = [{ include = "fastapi_cache" }]
 include = ["LICENSE", "README.md"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fastapi = "*"
-uvicorn = "*"
-redis = { version = ">=5,<6", optional = true }
-aiomcache = { version = "*", optional = true }
-pendulum = { version = "^3.0.0b1", allow-prereleases = true }
 aiobotocore = { version = ">=1.4.1,<3.0.0", optional = true }
+aiomcache = { version = "*", optional = true }
+fastapi-slim = "*"
 msgspec = "^0.18.4"
 pydantic = "^2.5.2"
+redis = { version = ">=5,<6", optional = true }
+uvicorn = "*"
 
-[tool.poetry.group.linting]
-optional = true
-
-[tool.poetry.group.linting.dependencies]
+[tool.poetry.group.dev.dependencies]
+coverage = ">=6.5,<8.0"
+httpx = "*"
 mypy = "^1.5.1"
+pendulum = "^3.0.0"
 pyright = "^1.1.306"
-types-aiobotocore = { extras = ["dynamodb"], version = "^2.7.0" }
-types-redis = "^4.6.0.10"
-ruff = "^0.1.5"
-
-[tool.poetry.group.dev.dependencies]
 pytest = "*"
 requests = "*"
-coverage = ">=6.5,<8.0"
-httpx = "*"
-tox = "^4.11.3"
+ruff = "^0.1.5"
 towncrier = "^22.12.0"
+tox = "^4.11.3"
+types-aiobotocore = { extras = ["dynamodb"], version = "^2.7.0" }
+types-redis = "^4.6.0.10"
 
 [tool.poetry.group.distributing]
 optional = true
 
 [tool.poetry.group.distributing.dependencies]
 twine = "^4.0.2"
 
@@ -91,15 +86,15 @@
 pythonVersion = "3.11"
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings"
 
 [tool.ruff]
 ignore = ["E501"]
-line-length = 80
+line-length = 120
 select = [
     "B",  # flake8-bugbear
     "C4", # flake8-comprehensions
     "E",  # pycodestyle errors
     "F",  # pyflakes
     "I",  # isort
     "S",  # flake8-bandit
```

### Comparing `fastapi_cache2_fork-0.3.1/PKG-INFO` & `fastapi_cache2_fork-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cache2-fork
-Version: 0.3.1
+Version: 0.3.2
 Summary: Cache for FastAPI. An opinionated fork of fastapi-cache library that uses msgspec for json encoding/decoding where possible
 Home-page: https://github.com/Yolley/fastapi-cache
 License: Apache-2.0
 Keywords: fastapi,cache,caching
 Author: long2ice
 Author-email: long2ice@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -14,17 +14,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: dynamodb
 Provides-Extra: memcache
 Provides-Extra: redis
 Requires-Dist: aiobotocore (>=1.4.1,<3.0.0) ; extra == "dynamodb" or extra == "all"
 Requires-Dist: aiomcache ; extra == "memcache" or extra == "all"
-Requires-Dist: fastapi
+Requires-Dist: fastapi-slim
 Requires-Dist: msgspec (>=0.18.4,<0.19.0)
-Requires-Dist: pendulum (>=3.0.0b1,<4.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: redis (>=5,<6) ; extra == "redis" or extra == "all"
 Requires-Dist: uvicorn
 Project-URL: Documentation, https://github.com/Yolley/fastapi-cache
 Project-URL: Repository, https://github.com/Yolley/fastapi-cache.git
 Description-Content-Type: text/markdown
```

