# Comparing `tmp/milvus_model-0.2.2.tar.gz` & `tmp/milvus_model-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_model-0.2.2.tar", last modified: Fri May 17 12:35:16 2024, max compression
+gzip compressed data, was "milvus_model-0.2.3.tar", last modified: Tue May 28 07:45:53 2024, max compression
```

## Comparing `milvus_model-0.2.2.tar` & `milvus_model-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.246464 milvus_model-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 12:35:09.000000 milvus_model-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 12:35:16.246464 milvus_model-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-17 12:35:09.000000 milvus_model-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-17 12:35:09.000000 milvus_model-0.2.2/_version_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/milvus_model/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/dense/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/jinaai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/hybrid/bge_m3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/reranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/bgereranker.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/cross_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/jinaai.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/sparse/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/lang.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/splade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/dependency_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/lazy_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-17 12:35:09.000000 milvus_model-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:35:16.246464 milvus_model-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.494973 milvus_model-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.486973 milvus_model-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 07:45:41.000000 milvus_model-0.2.3/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-28 07:45:41.000000 milvus_model-0.2.3/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 07:45:41.000000 milvus_model-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 07:45:41.000000 milvus_model-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-28 07:45:53.494973 milvus_model-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 07:45:41.000000 milvus_model-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-28 07:45:41.000000 milvus_model-0.2.3/_version_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/milvus_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/milvus_model/dense/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/dense/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/milvus_model/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/hybrid/bge_m3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/milvus_model/reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/bgereranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/cross_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/reranker/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.490973 milvus_model-0.2.3/milvus_model/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.494973 milvus_model-0.2.3/milvus_model/sparse/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/bm25/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/bm25/lang.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/bm25/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/sparse/splade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.494973 milvus_model-0.2.3/milvus_model/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-28 07:45:41.000000 milvus_model-0.2.3/milvus_model/utils/lazy_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:45:53.494973 milvus_model-0.2.3/milvus_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-28 07:45:53.000000 milvus_model-0.2.3/milvus_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 07:45:53.000000 milvus_model-0.2.3/milvus_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:45:53.000000 milvus_model-0.2.3/milvus_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 07:45:53.000000 milvus_model-0.2.3/milvus_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 07:45:53.000000 milvus_model-0.2.3/milvus_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 07:45:41.000000 milvus_model-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:45:53.494973 milvus_model-0.2.3/setup.cfg
```

### Comparing `milvus_model-0.2.2/.github/workflows/publish_dev_package.yml` & `milvus_model-0.2.3/.github/workflows/publish_dev_package.yml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/.github/workflows/publish_on_release.yml` & `milvus_model-0.2.3/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/LICENSE` & `milvus_model-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/PKG-INFO` & `milvus_model-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.2
+Version: 0.2.3
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: onnxruntime
 Requires-Dist: scipy>=1.10.0
-Requires-Dist: protobuf==3.20.2
+Requires-Dist: protobuf
 Requires-Dist: numpy
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
```

### Comparing `milvus_model-0.2.2/README.md` & `milvus_model-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/_version_helper.py` & `milvus_model-0.2.3/_version_helper.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/base.py` & `milvus_model-0.2.3/milvus_model/base.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/dense/__init__.py` & `milvus_model-0.2.3/milvus_model/dense/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 __all__ = [
     "OpenAIEmbeddingFunction",
     "SentenceTransformerEmbeddingFunction",
     "VoyageEmbeddingFunction",
     "JinaEmbeddingFunction",
     "OnnxEmbeddingFunction",
+    "CohereEmbeddingFunction"
 ]
 
 from milvus_model.utils.lazy_import import LazyImport
 
 jinaai = LazyImport("jinaai", globals(), "milvus_model.dense.jinaai")
 openai = LazyImport("openai", globals(), "milvus_model.dense.openai")
 sentence_transformer = LazyImport("sentence_transformer", globals(), "milvus_model.dense.sentence_transformer")
 voyageai = LazyImport("voyageai", globals(), "milvus_model.dense.voyageai")
 onnx = LazyImport("onnx", globals(), "milvus_model.dense.onnx")
+cohere = LazyImport("cohere", globals(), "milvus_model.dense.cohere")
 
 def JinaEmbeddingFunction(*args, **kwargs):
     return jinaai.JinaEmbeddingFunction(*args, **kwargs)
 
 def OpenAIEmbeddingFunction(*args, **kwargs):
     return openai.OpenAIEmbeddingFunction(*args, **kwargs)
 
@@ -24,7 +26,10 @@
     return sentence_transformer.SentenceTransformerEmbeddingFunction(*args, **kwargs)
 
 def VoyageEmbeddingFunction(*args, **kwargs):
     return voyageai.VoyageEmbeddingFunction(*args, **kwargs)
 
 def OnnxEmbeddingFunction(*args, **kwargs):
     return onnx.OnnxEmbeddingFunction(*args, **kwargs)
+
+def CohereEmbeddingFunction(*args, **kwargs):
+    return cohere.CohereEmbeddingFunction(*args, **kwargs)
```

### Comparing `milvus_model-0.2.2/milvus_model/dense/jinaai.py` & `milvus_model-0.2.3/milvus_model/dense/jinaai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/dense/onnx.py` & `milvus_model-0.2.3/milvus_model/dense/onnx.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/dense/openai.py` & `milvus_model-0.2.3/milvus_model/dense/openai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/dense/sentence_transformer.py` & `milvus_model-0.2.3/milvus_model/dense/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/dense/voyageai.py` & `milvus_model-0.2.3/milvus_model/dense/voyageai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/hybrid/bge_m3.py` & `milvus_model-0.2.3/milvus_model/hybrid/bge_m3.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/__init__.py` & `milvus_model-0.2.3/milvus_model/reranker/__init__.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/bgereranker.py` & `milvus_model-0.2.3/milvus_model/reranker/bgereranker.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/cohere.py` & `milvus_model-0.2.3/milvus_model/reranker/cohere.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/cross_encoder.py` & `milvus_model-0.2.3/milvus_model/reranker/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/jinaai.py` & `milvus_model-0.2.3/milvus_model/reranker/jinaai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/reranker/voyageai.py` & `milvus_model-0.2.3/milvus_model/reranker/voyageai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/sparse/bm25/__init__.py` & `milvus_model-0.2.3/milvus_model/sparse/bm25/__init__.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/sparse/bm25/bm25.py` & `milvus_model-0.2.3/milvus_model/sparse/bm25/bm25.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from collections import defaultdict
 from multiprocessing import Pool, cpu_count
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import requests
 from scipy.sparse import csr_array, vstack
+import numpy as np
 
 from milvus_model.base import BaseEmbeddingFunction
 from milvus_model.sparse.bm25.tokenizers import Analyzer, build_default_analyzer
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 console_handler = logging.StreamHandler()
@@ -130,15 +131,15 @@
         terms = self.analyzer(query)
         values, rows, cols = [], [], []
         for term in terms:
             if term in self.idf:
                 values.append(self.idf[term][0])
                 rows.append(0)
                 cols.append(self.idf[term][1])
-        return csr_array((values, (rows, cols)), shape=(1, len(self.idf)))
+        return csr_array((values, (rows, cols)), shape=(1, len(self.idf))).astype(np.float32)
 
     def _encode_document(self, doc: str) -> csr_array:
         terms = self.analyzer(doc)
         frequencies = defaultdict(int)
         doc_len = len(terms)
         term_set = set()
         for term in terms:
@@ -152,15 +153,15 @@
                     term_freq
                     * (self.k1 + 1)
                     / (term_freq + self.k1 * (1 - self.b + self.b * doc_len / self.avgdl))
                 )
                 rows.append(0)
                 cols.append(self.idf[term][1])
                 values.append(value)
-        return csr_array((values, (rows, cols)), shape=(1, len(self.idf)))
+        return csr_array((values, (rows, cols)), shape=(1, len(self.idf))).astype(np.float32)
 
     def encode_queries(self, queries: List[str]) -> csr_array:
         sparse_embs = [self._encode_query(query) for query in queries]
         return vstack(sparse_embs).tocsr()
 
     def __call__(self, texts: List[str]) -> csr_array:
         error_message = "Unsupported function called, please check the documentation of 'BM25EmbeddingFunction'."
```

### Comparing `milvus_model-0.2.2/milvus_model/sparse/bm25/lang.yaml` & `milvus_model-0.2.3/milvus_model/sparse/bm25/lang.yaml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/sparse/bm25/tokenizers.py` & `milvus_model-0.2.3/milvus_model/sparse/bm25/tokenizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 
     def apply(self, text: str):
         return self.pattern.sub(self._replacement_function, text)
 
 
 @register_class("StandardTokenizer")
 class StandardTokenizer:
+    def __init__(self):
+        try:
+           word_tokenize("this is a simple test.") 
+        except LookupError:
+            nltk.download("punkt")
     def tokenize(self, text: str):
         return word_tokenize(text)
 
 
 class TextFilter:
     def apply(self, tokens: List[str]):
         error_message = "Each filter must implement the 'apply' method."
```

### Comparing `milvus_model-0.2.2/milvus_model/sparse/splade.py` & `milvus_model-0.2.3/milvus_model/sparse/splade.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/utils/__init__.py` & `milvus_model-0.2.3/milvus_model/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/utils/dependency_control.py` & `milvus_model-0.2.3/milvus_model/utils/dependency_control.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model/utils/lazy_import.py` & `milvus_model-0.2.3/milvus_model/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.2/milvus_model.egg-info/PKG-INFO` & `milvus_model-0.2.3/milvus_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.2
+Version: 0.2.3
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: onnxruntime
 Requires-Dist: scipy>=1.10.0
-Requires-Dist: protobuf==3.20.2
+Requires-Dist: protobuf
 Requires-Dist: numpy
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
```

### Comparing `milvus_model-0.2.2/milvus_model.egg-info/SOURCES.txt` & `milvus_model-0.2.3/milvus_model.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 milvus_model/base.py
 milvus_model.egg-info/PKG-INFO
 milvus_model.egg-info/SOURCES.txt
 milvus_model.egg-info/dependency_links.txt
 milvus_model.egg-info/requires.txt
 milvus_model.egg-info/top_level.txt
 milvus_model/dense/__init__.py
+milvus_model/dense/cohere.py
 milvus_model/dense/jinaai.py
 milvus_model/dense/onnx.py
 milvus_model/dense/openai.py
 milvus_model/dense/sentence_transformer.py
 milvus_model/dense/voyageai.py
 milvus_model/hybrid/__init__.py
 milvus_model/hybrid/bge_m3.py
```

### Comparing `milvus_model-0.2.2/pyproject.toml` & `milvus_model-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires-python = ">=3.8"
 description = "Model components for PyMilvus, the Python SDK for Milvus"
 readme = "README.md"
 dependencies = [
     "transformers >= 4.36.0",
     "onnxruntime",
     "scipy >= 1.10.0",
-    "protobuf==3.20.2",
+    "protobuf",
     "numpy"
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

