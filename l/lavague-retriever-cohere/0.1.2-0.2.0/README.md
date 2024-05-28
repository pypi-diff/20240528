# Comparing `tmp/lavague_retriever_cohere-0.1.2.tar.gz` & `tmp/lavague_retriever_cohere-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_retriever_cohere-0.1.2.tar", max compression
+gzip compressed data, was "lavague_retriever_cohere-0.2.0.tar", max compression
```

## Comparing `lavague_retriever_cohere-0.1.2.tar` & `lavague_retriever_cohere-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       30 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/README.md
--rw-r--r--   0        0        0       59 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/__init__.py
--rw-r--r--   0        0        0     1677 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/base.py
--rw-r--r--   0        0        0      971 2024-05-15 21:18:49.639971 lavague_retriever_cohere-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 lavague_retriever_cohere-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-28 08:59:04.860012 lavague_retriever_cohere-0.2.0/README.md
+-rw-r--r--   0        0        0       59 2024-05-28 08:59:04.860768 lavague_retriever_cohere-0.2.0/lavague/retrievers/cohere/__init__.py
+-rw-r--r--   0        0        0     1677 2024-05-28 08:59:04.861021 lavague_retriever_cohere-0.2.0/lavague/retrievers/cohere/base.py
+-rw-r--r--   0        0        0      971 2024-05-28 21:04:47.552904 lavague_retriever_cohere-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 lavague_retriever_cohere-0.2.0/PKG-INFO
```

### Comparing `lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/base.py` & `lavague_retriever_cohere-0.2.0/lavague/retrievers/cohere/base.py`

 * *Files identical despite different names*

### Comparing `lavague_retriever_cohere-0.1.2/pyproject.toml` & `lavague_retriever_cohere-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-retriever-cohere"
-version = "0.1.2"
+version = "0.2.0"
 description = "Cohere retriever for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -17,13 +17,13 @@
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
-lavague-core = "^0.1.1"
+lavague-core = "^0.2.0"
 cohere = "^5.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lavague_retriever_cohere-0.1.2/PKG-INFO` & `lavague_retriever_cohere-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-retriever-cohere
-Version: 0.1.2
+Version: 0.2.0
 Summary: Cohere retriever for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,13 +14,13 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cohere (>=5.4.0,<6.0.0)
-Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
+Requires-Dist: lavague-core (>=0.2.0,<0.3.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
 
 # Cohere retriever for lavague
```

