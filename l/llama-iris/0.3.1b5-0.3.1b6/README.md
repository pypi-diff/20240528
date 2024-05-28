# Comparing `tmp/llama_iris-0.3.1b5.tar.gz` & `tmp/llama_iris-0.3.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_iris-0.3.1b5.tar", max compression
+gzip compressed data, was "llama_iris-0.3.1b6.tar", max compression
```

## Comparing `llama_iris-0.3.1b5.tar` & `llama_iris-0.3.1b6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-05-09 02:30:35.048595 llama_iris-0.3.1b5/LICENSE
--rw-r--r--   0        0        0     1108 2024-05-09 02:30:35.048595 llama_iris-0.3.1b5/README.md
--rw-r--r--   0        0        0      224 2024-05-09 02:30:35.048595 llama_iris-0.3.1b5/llama_iris/__init__.py
--rw-r--r--   0        0        0    10429 2024-05-09 02:30:35.048595 llama_iris-0.3.1b5/llama_iris/vectorstore.py
--rw-r--r--   0        0        0     1060 2024-05-09 02:30:51.824482 llama_iris-0.3.1b5/pyproject.toml
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 llama_iris-0.3.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 15:40:32.944281 llama_iris-0.3.1b6/LICENSE
+-rw-r--r--   0        0        0     1108 2024-05-28 15:40:32.944281 llama_iris-0.3.1b6/README.md
+-rw-r--r--   0        0        0      224 2024-05-28 15:40:32.944281 llama_iris-0.3.1b6/llama_iris/__init__.py
+-rw-r--r--   0        0        0    10429 2024-05-28 15:40:32.944281 llama_iris-0.3.1b6/llama_iris/vectorstore.py
+-rw-r--r--   0        0        0     1060 2024-05-28 15:40:49.644309 llama_iris-0.3.1b6/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 llama_iris-0.3.1b6/PKG-INFO
```

### Comparing `llama_iris-0.3.1b5/LICENSE` & `llama_iris-0.3.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b5/README.md` & `llama_iris-0.3.1b6/README.md`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b5/llama_iris/vectorstore.py` & `llama_iris-0.3.1b6/llama_iris/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b5/pyproject.toml` & `llama_iris-0.3.1b6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 [tool.poetry]
 name = "llama-iris"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.3.1b5"
+version = "0.3.1b6"
 description = "Interface between LLMs and your data"
 authors = ["Dmitry Maslennikov <dmitry@caretdev.com>"]
 keywords = ["LLM", "NLP", "RAG", "data", "devtools", "index", "retrieval", "iris"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "llama_iris"}]
 repository = "https://github.com/caretdev/llama-iris"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 SQLAlchemy = {extras = ["asyncio"], version = ">=1.4.49"}
 llama-index = "^0.9.46"
 pandas = "^2.2.0"
-sqlalchemy-iris = "^0.13.0"
+sqlalchemy-iris = "^0.14.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.2.1"
 pytest-asyncio = "0.21.0"
 pytest-dotenv = "0.5.2"
 pytest-mock = "3.11.1"
 testcontainers-iris = "^1.1.0"
```

### Comparing `llama_iris-0.3.1b5/PKG-INFO` & `llama_iris-0.3.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-iris
-Version: 0.3.1b5
+Version: 0.3.1b6
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/caretdev/llama-iris
 License: MIT
 Keywords: LLM,NLP,RAG,data,devtools,index,retrieval,iris
 Author: Dmitry Maslennikov
 Author-email: dmitry@caretdev.com
 Requires-Python: >=3.9,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: SQLAlchemy[asyncio] (>=1.4.49)
 Requires-Dist: llama-index (>=0.9.46,<0.10.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: sqlalchemy-iris (>=0.13.0,<0.14.0)
+Requires-Dist: sqlalchemy-iris (>=0.14.0,<0.15.0)
 Project-URL: Repository, https://github.com/caretdev/llama-iris
 Description-Content-Type: text/markdown
 
 # Llama-index with InterSystems IRIS
 
 [Llama-index](https://github.com/run-llama/llama_index) with support for InterSystems IRIS
```

