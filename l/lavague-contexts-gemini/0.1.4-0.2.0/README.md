# Comparing `tmp/lavague_contexts_gemini-0.1.4.tar.gz` & `tmp/lavague_contexts_gemini-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_gemini-0.1.4.tar", max compression
+gzip compressed data, was "lavague_contexts_gemini-0.2.0.tar", max compression
```

## Comparing `lavague_contexts_gemini-0.1.4.tar` & `lavague_contexts_gemini-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-16 14:49:01.030627 lavague_contexts_gemini-0.1.4/README.md
--rw-r--r--   0        0        0       55 2024-05-16 14:49:01.030627 lavague_contexts_gemini-0.1.4/lavague/contexts/gemini/__init__.py
--rw-r--r--   0        0        0     1115 2024-05-21 21:06:53.305594 lavague_contexts_gemini-0.1.4/lavague/contexts/gemini/base.py
--rw-r--r--   0        0        0     1108 2024-05-21 23:05:31.830269 lavague_contexts_gemini-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-28 08:59:04.855620 lavague_contexts_gemini-0.2.0/README.md
+-rw-r--r--   0        0        0       55 2024-05-28 08:59:04.855805 lavague_contexts_gemini-0.2.0/lavague/contexts/gemini/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-28 08:59:04.855900 lavague_contexts_gemini-0.2.0/lavague/contexts/gemini/base.py
+-rw-r--r--   0        0        0     1108 2024-05-28 21:04:02.659149 lavague_contexts_gemini-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.2.0/PKG-INFO
```

### Comparing `lavague_contexts_gemini-0.1.4/lavague/contexts/gemini/base.py` & `lavague_contexts_gemini-0.2.0/lavague/contexts/gemini/base.py`

 * *Files identical despite different names*

### Comparing `lavague_contexts_gemini-0.1.4/pyproject.toml` & `lavague_contexts_gemini-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-gemini"
-version = "0.1.4"
+version = "0.2.0"
 description = "gemini integration for lavague"
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
 llama-index-llms-gemini = "^0.1.8"
 llama-index-embeddings-gemini = "^0.1.6"
 llama-index-multi-modal-llms-gemini = "^0.1.6"
 google-generativeai = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lavague_contexts_gemini-0.1.4/PKG-INFO` & `lavague_contexts_gemini-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-gemini
-Version: 0.1.4
+Version: 0.2.0
 Summary: gemini integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
-Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
+Requires-Dist: lavague-core (>=0.2.0,<0.3.0)
 Requires-Dist: llama-index-embeddings-gemini (>=0.1.6,<0.2.0)
 Requires-Dist: llama-index-llms-gemini (>=0.1.8,<0.2.0)
 Requires-Dist: llama-index-multi-modal-llms-gemini (>=0.1.6,<0.2.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
```

