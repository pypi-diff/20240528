# Comparing `tmp/lavague_contexts_openai-0.1.3.tar.gz` & `tmp/lavague_contexts_openai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_openai-0.1.3.tar", max compression
+gzip compressed data, was "lavague_contexts_openai-0.2.0.tar", max compression
```

## Comparing `lavague_contexts_openai-0.1.3.tar` & `lavague_contexts_openai-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-22 18:18:44.473928 lavague_contexts_openai-0.1.3/README.md
--rw-r--r--   0        0        0       75 2024-05-22 18:18:44.474112 lavague_contexts_openai-0.1.3/lavague/contexts/openai/__init__.py
--rw-r--r--   0        0        0     2186 2024-05-24 06:43:44.648233 lavague_contexts_openai-0.1.3/lavague/contexts/openai/base.py
--rw-r--r--   0        0        0     1171 2024-05-24 11:05:35.199763 lavague_contexts_openai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-28 08:59:04.856425 lavague_contexts_openai-0.2.0/README.md
+-rw-r--r--   0        0        0       75 2024-05-28 08:59:04.856610 lavague_contexts_openai-0.2.0/lavague/contexts/openai/__init__.py
+-rw-r--r--   0        0        0     2186 2024-05-28 08:59:04.856683 lavague_contexts_openai-0.2.0/lavague/contexts/openai/base.py
+-rw-r--r--   0        0        0     1171 2024-05-28 21:04:15.435260 lavague_contexts_openai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.2.0/PKG-INFO
```

### Comparing `lavague_contexts_openai-0.1.3/lavague/contexts/openai/base.py` & `lavague_contexts_openai-0.2.0/lavague/contexts/openai/base.py`

 * *Files identical despite different names*

### Comparing `lavague_contexts_openai-0.1.3/pyproject.toml` & `lavague_contexts_openai-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-openai"
-version = "0.1.3"
+version = "0.2.0"
 description = "Openai integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -17,15 +17,15 @@
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
-lavague-core = "^0.1.1"
+lavague-core = "^0.2.0"
 llama-index-llms-openai = "^0.1.9"
 llama-index-embeddings-openai = "^0.1.9"
 llama-index-llms-azure-openai = "^0.1.8"
 llama-index-multi-modal-llms-openai = "^0.1.6"
 llama-index-multi-modal-llms-azure-openai = "^0.1.4"
 
 [build-system]
```

### Comparing `lavague_contexts_openai-0.1.3/PKG-INFO` & `lavague_contexts_openai-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-openai
-Version: 0.1.3
+Version: 0.2.0
 Summary: Openai integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
+Requires-Dist: lavague-core (>=0.2.0,<0.3.0)
 Requires-Dist: llama-index-embeddings-openai (>=0.1.9,<0.2.0)
 Requires-Dist: llama-index-llms-azure-openai (>=0.1.8,<0.2.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.9,<0.2.0)
 Requires-Dist: llama-index-multi-modal-llms-azure-openai (>=0.1.4,<0.2.0)
 Requires-Dist: llama-index-multi-modal-llms-openai (>=0.1.6,<0.2.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
```

