# Comparing `tmp/indox-0.1.4.tar.gz` & `tmp/Indox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indox-0.1.4.tar", last modified: Tue May 21 15:54:06 2024, max compression
+gzip compressed data, was "Indox-0.1.5.tar", last modified: Tue May 28 07:16:44 2024, max compression
```

## Comparing `indox-0.1.4.tar` & `Indox-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.145660 indox-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.113031 indox-0.1.4/Indox/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.129691 indox-0.1.4/Indox/DataLoaderSplitter/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.133662 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/
--rw-rw-rw-   0        0        0     6348 2024-05-11 13:44:58.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py
--rw-rw-rw-   0        0        0     2074 2024-05-13 06:41:26.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py
--rw-rw-rw-   0        0        0     4781 2024-05-13 08:12:00.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py
--rw-rw-rw-   0        0        0     2856 2024-05-13 06:27:35.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py
--rw-rw-rw-   0        0        0       35 2024-05-14 14:02:48.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/__init__.py
--rw-rw-rw-   0        0        0     4078 2024-05-14 14:21:32.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/split.py
--rw-rw-rw-   0        0        0     6425 2024-05-13 08:09:25.000000 indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.135662 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/
--rw-rw-rw-   0        0        0       45 2024-05-14 14:02:48.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/__init__.py
--rw-rw-rw-   0        0        0     2453 2024-05-15 14:05:13.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py
--rw-rw-rw-   0        0        0     3596 2024-05-15 08:19:59.000000 indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py
--rw-rw-rw-   0        0        0      108 2024-05-14 14:18:27.000000 indox-0.1.4/Indox/DataLoaderSplitter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.136662 indox-0.1.4/Indox/Embeddings/
--rw-rw-rw-   0        0        0       67 2024-05-12 16:34:51.000000 indox-0.1.4/Indox/Embeddings/__init__.py
--rw-rw-rw-   0        0        0      441 2024-05-21 05:20:09.000000 indox-0.1.4/Indox/Embeddings/embedding_models.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.139661 indox-0.1.4/Indox/Evaluation/
--rw-rw-rw-   0        0        0       28 2024-05-13 12:54:42.000000 indox-0.1.4/Indox/Evaluation/__init__.py
--rw-rw-rw-   0        0        0     8003 2024-05-21 05:20:09.000000 indox-0.1.4/Indox/Evaluation/eval.py
--rw-rw-rw-   0        0        0     2906 2024-05-13 12:39:30.000000 indox-0.1.4/Indox/Evaluation/metrics.py
--rw-rw-rw-   0        0        0     4719 2024-05-19 08:29:16.000000 indox-0.1.4/Indox/Evaluation/similarity.py
--rw-rw-rw-   0        0        0    10059 2024-05-13 12:39:30.000000 indox-0.1.4/Indox/Evaluation/unieval.py
--rw-rw-rw-   0        0        0     2453 2024-05-11 13:44:58.000000 indox-0.1.4/Indox/Graph.py
--rw-rw-rw-   0        0        0     8869 2024-05-16 15:16:32.000000 indox-0.1.4/Indox/Indox.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.140662 indox-0.1.4/Indox/QaModels/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.141661 indox-0.1.4/Indox/QaModels/Dspy_Cot/
--rw-rw-rw-   0        0        0       27 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/Dspy_Cot/__init__.py
--rw-rw-rw-   0        0        0     2604 2024-05-20 11:24:22.000000 indox-0.1.4/Indox/QaModels/Dspy_Cot/dspy.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.142662 indox-0.1.4/Indox/QaModels/Mistral/
--rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/Mistral/__init__.py
--rw-rw-rw-   0        0        0     2684 2024-05-20 11:34:09.000000 indox-0.1.4/Indox/QaModels/Mistral/mistral.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.143664 indox-0.1.4/Indox/QaModels/OpenAi/
--rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.4/Indox/QaModels/OpenAi/__init__.py
--rw-rw-rw-   0        0        0     2185 2024-05-20 11:23:53.000000 indox-0.1.4/Indox/QaModels/OpenAi/openai.py
--rw-rw-rw-   0        0        0       95 2024-05-14 13:59:17.000000 indox-0.1.4/Indox/QaModels/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.143664 indox-0.1.4/Indox/Splitter/
--rw-rw-rw-   0        0        0       60 2024-05-15 04:55:56.000000 indox-0.1.4/Indox/Splitter/__init__.py
--rw-rw-rw-   0        0        0      377 2024-05-14 14:16:18.000000 indox-0.1.4/Indox/Splitter/semantic_text_splitter.py
--rw-rw-rw-   0        0        0       66 2024-05-12 15:34:14.000000 indox-0.1.4/Indox/__init__.py
--rw-rw-rw-   0        0        0      960 2024-05-14 11:18:39.000000 indox-0.1.4/Indox/config.yaml
--rw-rw-rw-   0        0        0     2738 2024-05-15 06:17:01.000000 indox-0.1.4/Indox/utils.py
--rw-rw-rw-   0        0        0     8896 2024-05-13 14:07:14.000000 indox-0.1.4/Indox/vectorstore.py
--rw-rw-rw-   0        0        0     2562 2024-05-16 15:16:32.000000 indox-0.1.4/Indox/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:54:06.144661 indox-0.1.4/Indox.egg-info/
--rw-rw-rw-   0        0        0     8261 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 15:54:04.000000 indox-0.1.4/Indox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-11 13:44:58.000000 indox-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8261 2024-05-21 15:54:06.145660 indox-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2024-05-20 09:59:26.000000 indox-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 15:54:06.146660 indox-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1307 2024-05-21 14:19:39.000000 indox-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.227386 Indox-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.225398 Indox-0.1.5/Indox.egg-info/
+-rw-rw-rw-   0        0        0     9896 2024-05-28 07:16:43.000000 Indox-0.1.5/Indox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1453 2024-05-28 07:16:43.000000 Indox-0.1.5/Indox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:16:43.000000 Indox-0.1.5/Indox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2024-05-28 07:16:43.000000 Indox-0.1.5/Indox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 07:16:43.000000 Indox-0.1.5/Indox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-28 06:52:32.000000 Indox-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-05-28 06:52:32.000000 Indox-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9896 2024-05-28 07:16:44.226389 Indox-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8551 2024-05-28 06:52:32.000000 Indox-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:43.935858 Indox-0.1.5/indox/
+-rw-rw-rw-   0        0        0     2453 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/Graph.py
+-rw-rw-rw-   0        0        0       66 2024-05-28 06:55:37.000000 Indox-0.1.5/indox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:43.945865 Indox-0.1.5/indox/data_loader_splitter/
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.026345 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/
+-rw-rw-rw-   0        0        0     6348 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Clustering.py
+-rw-rw-rw-   0        0        0     2044 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Embed.py
+-rw-rw-rw-   0        0        0    10291 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/EmbedClusterSummarize.py
+-rw-rw-rw-   0        0        0     2684 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Summary.py
+-rw-rw-rw-   0        0        0       35 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/__init__.py
+-rw-rw-rw-   0        0        0     3825 2024-05-28 06:59:33.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/split.py
+-rw-rw-rw-   0        0        0     6425 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.061701 Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/
+-rw-rw-rw-   0        0        0       45 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/__init__.py
+-rw-rw-rw-   0        0        0     2453 2024-05-28 06:59:33.000000 Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/loader.py
+-rw-rw-rw-   0        0        0     3578 2024-05-28 07:09:47.000000 Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/split.py
+-rw-rw-rw-   0        0        0      108 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/data_loader_splitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.074317 Indox-0.1.5/indox/embeddings/
+-rw-rw-rw-   0        0        0       88 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     3333 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/embeddings/embedding_models.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.166694 Indox-0.1.5/indox/evaluation/
+-rw-rw-rw-   0        0        0       28 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     8003 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/evaluation/eval.py
+-rw-rw-rw-   0        0        0     2906 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/evaluation/metrics.py
+-rw-rw-rw-   0        0        0     4719 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/evaluation/similarity.py
+-rw-rw-rw-   0        0        0    10059 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/evaluation/unieval.py
+-rw-rw-rw-   0        0        0     8978 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/indox.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.178387 Indox-0.1.5/indox/qa_models/
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.179383 Indox-0.1.5/indox/qa_models/Dspy_Cot/
+-rw-rw-rw-   0        0        0       27 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/Dspy_Cot/__init__.py
+-rw-rw-rw-   0        0        0     2604 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/Dspy_Cot/dspy.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.191386 Indox-0.1.5/indox/qa_models/Mistral/
+-rw-rw-rw-   0        0        0       30 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/Mistral/__init__.py
+-rw-rw-rw-   0        0        0     2684 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/Mistral/mistral.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.212383 Indox-0.1.5/indox/qa_models/OpenAi/
+-rw-rw-rw-   0        0        0       76 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/OpenAi/__init__.py
+-rw-rw-rw-   0        0        0     2113 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/OpenAi/openai.py
+-rw-rw-rw-   0        0        0     2248 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/OpenAi/openai_indox_api.py
+-rw-rw-rw-   0        0        0      131 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/qa_models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:16:44.224385 Indox-0.1.5/indox/splitter/
+-rw-rw-rw-   0        0        0       60 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/splitter/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/splitter/semantic_text_splitter.py
+-rw-rw-rw-   0        0        0     2738 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/utils.py
+-rw-rw-rw-   0        0        0     8896 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/vectorstore.py
+-rw-rw-rw-   0        0        0     2562 2024-05-28 06:52:32.000000 Indox-0.1.5/indox/visualization.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:16:44.227386 Indox-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-05-28 07:15:56.000000 Indox-0.1.5/setup.py
```

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py` & `Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Clustering.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py` & `Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Embed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 import pandas as pd
 from typing import List
 
 from .Clustering import perform_clustering
 
 
-def embed(texts: List[str], embeddings) -> np.ndarray:
+def embed(texts, embeddings) -> np.ndarray:
     """
     Generate embeddings for a list of text documents using a provided embeddings object.
 
     Parameters:
-    - texts: List[str], a list of text documents to be embedded.
+    - texts, a list of text documents to be embedded.
     - embeddings: An object capable of generating embeddings, must have an `embed_documents` method.
 
     Returns:
     - numpy.ndarray: An array of embeddings for the given text documents.
     """
     text_embeddings = embeddings.embed_documents(texts)
 
@@ -32,20 +32,16 @@
     Parameters:
     - texts: List[str], a list of text documents to be processed.
     - embeddings: An object capable of generating embeddings, must have an `embed_documents` method.
 
     Returns:
     - pandas.DataFrame: A DataFrame containing the original texts, their embeddings, and the assigned cluster labels.
     """
-    text_embeddings_np = embed(
-        texts, embeddings
-    )  # Generate embeddings using the provided embeddings object
-    cluster_labels = perform_clustering(
-        text_embeddings_np,
-        dim=dim,
-        threshold=threshold,
-    )  # Perform clustering on the embeddings
+    text_embeddings_np = embed(texts, embeddings)  # Generate embeddings using the provided embeddings object
+    cluster_labels = perform_clustering(text_embeddings_np, dim=dim,
+                                        threshold=threshold)  # Perform clustering on the embeddings
     df = pd.DataFrame()  # Initialize a DataFrame to store the results
     df["text"] = texts  # Store original texts
     df["embd"] = list(text_embeddings_np)  # Store embeddings as a list in the DataFrame
     df["cluster"] = cluster_labels  # Store cluster labels
     return df
+
```

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py` & `Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/Summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,16 @@
                         "role": "user",
                         "content": f"{context}",
                     },
                 ],
                 max_tokens=config["summary_model"]["max_tokens"],
                 model="gpt-3.5-turbo-0125",
             )
-            input_tokens = response.usage.prompt_tokens
-            output_tokens = response.usage.total_tokens - response.usage.prompt_tokens
-            return response.choices[0].message.content.replace("\n", " "), input_tokens, output_tokens
+
+            return response.choices[0].message.content.replace("\n", " ")
         else:
             hf_model = SummarizationModelHuggingFace(
                 config["summary_model"]["model_name"],
                 max_len=config["summary_model"]["max_tokens"],
                 min_len=config["summary_model"]["min_len"],
             )
             return hf_model.summarize(context), 0, None
```

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/split.py` & `Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/split.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from Indox.DataLoaderSplitter.ClusteredSplit.EmbedClusterSummarize import recursive_embed_cluster_summarize
-from Indox.DataLoaderSplitter.ClusteredSplit.utils import get_all_texts, split_text, create_document
-from Indox.DataLoaderSplitter.utils.clean import remove_stopwords_chunk
+from indox.data_loader_splitter.ClusteredSplit.EmbedClusterSummarize import recursive_embed_cluster_summarize
+from indox.data_loader_splitter.ClusteredSplit.utils import get_all_texts, split_text, create_document
+from indox.data_loader_splitter.utils.clean import remove_stopwords_chunk
 from typing import Optional, List, Tuple
 
 
 def get_chunks(docs, embeddings, threshold, dim, chunk_size, overlap,
                re_chunk, remove_sword):
     """
     Extract chunks from the provided documents using an embedding function. Optionally, recursively cluster
@@ -18,16 +18,15 @@
     - re_chunk (bool, optional): Whether to re-chunk the clustered data for smaller summarization. Defaults to `False`.
     - remove_sword (bool, optional): If `True`, remove stopwords from the chunks. Defaults to `False`.
 
     Returns:
     - Tuple or List:
       - If `do_clustering` is `True`, returns a tuple containing:
         - `all_chunks` (List[str]): A list of all document chunks (leaf and extra).
-        - `input_tokens_all` (int): The total number of input tokens used.
-        - `output_tokens_all` (int): The total number of output tokens received.
+
       - Otherwise, returns a list of leaf chunks without further clustering.
 
     Raises:
     - Exception: Any errors occurring during the chunking, clustering, or summarization process.
 
     Notes:
     - The function creates document chunks, optionally applies stopword removal, and clusters chunks based on the
@@ -43,22 +42,21 @@
         for i in range(len(leaf_chunks)):
             leaf_chunks[i] = leaf_chunks[i].replace("\n", " ")
 
         # Optionally remove stopwords from the chunks
         if remove_sword:
             leaf_chunks = remove_stopwords_chunk(leaf_chunks)
 
-        results, input_tokens_all, output_tokens_all = recursive_embed_cluster_summarize(
+        results = recursive_embed_cluster_summarize(
             texts=leaf_chunks, embeddings=embeddings, dim=dim, threshold=threshold, level=1, n_levels=3,
             re_chunk=re_chunk, max_chunk=int(chunk_size / 2), remove_sword=remove_sword
         )
         all_chunks = get_all_texts(results=results, texts=leaf_chunks)
 
         print("End Chunking & Clustering process.")
-        # return all_chunks, input_tokens_all, output_tokens_all
         return all_chunks
 
 
     except Exception as e:
         print(f"Failed at step with error: {e}")
         raise e
```

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/ClusteredSplit/utils.py` & `Indox-0.1.5/indox/data_loader_splitter/ClusteredSplit/utils.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py` & `Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import importlib
-from Indox.utils import convert_latex_to_md
+from indox.utils import convert_latex_to_md
 
 
 def import_unstructured_partition(content_type):
     # Import appropriate partition function from the `unstructured` library
     module_name = f"unstructured.partition.{content_type}"
     module = importlib.import_module(module_name)
     partition_function_name = f"partition_{content_type}"
```

### Comparing `indox-0.1.4/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py` & `Indox-0.1.5/indox/data_loader_splitter/UnstructuredLoadAndSplit/split.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from Indox.DataLoaderSplitter.UnstructuredLoadAndSplit.loader import create_documents_unstructured
-from Indox.DataLoaderSplitter.utils.clean import remove_stopwords
+from indox.data_loader_splitter.UnstructuredLoadAndSplit.loader import create_documents_unstructured
+from indox.data_loader_splitter.utils.clean import remove_stopwords
 from unstructured.chunking.title import chunk_by_title
-from langchain_community.vectorstores.utils import filter_complex_metadata
+from langchain_community.vectorstores.utils import c
 from typing import List, Tuple, Optional, Any, Dict
 from langchain_core.documents import Document
 
 
 def get_chunks_unstructured(file_path, chunk_size, remove_sword, splitter):
     """
     Extract chunks from an unstructured document file using an unstructured data processing library.
```

### Comparing `indox-0.1.4/Indox/Evaluation/eval.py` & `Indox-0.1.5/indox/evaluation/eval.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/Evaluation/metrics.py` & `Indox-0.1.5/indox/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/Evaluation/similarity.py` & `Indox-0.1.5/indox/evaluation/similarity.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/Evaluation/unieval.py` & `Indox-0.1.5/indox/evaluation/unieval.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/Graph.py` & `Indox-0.1.5/indox/Graph.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/Indox.py` & `Indox-0.1.5/indox/indox.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
              """
         self.input_tokens_all = 0
         self.embedding_tokens = 0
         self.output_tokens_all = 0
         self.db = None
         self.config = None
-        self.qa_model = None
+        # self.qa_model = None
         self.config = read_config()
-        self.test = None
         self.qa_history = []
 
     def update_config(self):
         """
         Calls `update_config` to update the configuration, then loads
         """
         # Update the configuration
@@ -95,42 +94,47 @@
         except RuntimeError as re:
             print(f"Runtime error while storing in the vector store: {re}")
             return None
         except Exception as e:
             print(f"Unexpected error while storing in the vector store: {e}")
             return None
 
-    def answer_question(self, qa_model, query: str, top_k: int = 5, document_relevancy_filter: bool = False):
+    def answer_question(self, qa_model, query: str, db=None, top_k: int = 5, document_relevancy_filter: bool = False):
         """
         Answer a query using the QA model, finding the most relevant document chunks in the database.
 
         Parameters:
         - query (str): The question or search query to answer.
         - top_k (int): The number of top results to retrieve from the vector store.
         - document_relevancy_filter (bool, optional): If `True`, apply additional filtering using a RAG graph for
           document relevancy. Default is `False`.
-
+        -db : vector database
         Returns:
         - Tuple[str, Tuple[List[str], List[float]]]: A tuple containing the answer and the retrieved context:
             - `answer` (str): The answer provided by the QA model.
             - `retrieve_context` (Tuple[List[str], List[float]]): A tuple of the retrieved documents and their scores.
 
         Raises:
         - RuntimeError: If the vector store database is not initialized or fails to retrieve relevant documents.
         - ValueError: If the input query is empty.
         - Exception: Any other unexpected errors that occur while retrieving documents or generating the answer.
         """
+        vector_database = None
         if not query:
             raise ValueError("Query string cannot be empty.")
-
-        if self.db is None:
+        if db:
+            vector_database = db
+        elif self.db:
+            vector_database = self.db
+        if self.db and db is None:
             raise RuntimeError("Vector store database is not initialized.")
 
         try:
-            context, scores = self.db.retrieve(query, top_k=top_k)
+            context, scores = vector_database.retrieve(query, top_k=top_k)
+
             if not document_relevancy_filter:
                 # TODO: Add cost of embedding and qa_model
                 # response = qa_model.answer_question(context=context, question=query)
                 # self.output_tokens += response.usage.completion_tokens
                 # self.input_tokens += response.usage.prompt_tokens
                 answer = qa_model.answer_question(context=context, question=query)
             else:
@@ -187,23 +191,23 @@
     #     Displays the following token counts:
     #     - `input_tokens_all`: Number of input tokens sent to GPT-3.5 Turbo for summarization.
     #     - `output_tokens_all`: Number of output tokens received from GPT-3.5 Turbo.
     #     - `embedding_tokens`: Number of tokens used in the embedding process and sent to the database.
     #
     #     If no output tokens were used, only the embedding token information is displayed.
     #     """
-        # if self.output_tokens_all > 0:
-        #     print(
-        #         f"""
-        #         Overview of All Tokens Used:
-        #         Input tokens sent to GPT-3.5 Turbo (Model ID: 0125) for summarizing: {self.input_tokens_all}
-        #         Output tokens received from GPT-3.5 Turbo (Model ID: 0125): {self.output_tokens_all}
-        #         Tokens used in the embedding section that were sent to the database: {self.embedding_tokens}
-        #         """
-        #     )
-        # else:
-        #     print(
-        #         f"""
-        #         Overview of All Tokens Used:
-        #         Tokens used in the embedding section that were sent to the database: {self.embedding_tokens}
-        #         """
-        #     )
+    # if self.output_tokens_all > 0:
+    #     print(
+    #         f"""
+    #         Overview of All Tokens Used:
+    #         Input tokens sent to GPT-3.5 Turbo (Model ID: 0125) for summarizing: {self.input_tokens_all}
+    #         Output tokens received from GPT-3.5 Turbo (Model ID: 0125): {self.output_tokens_all}
+    #         Tokens used in the embedding section that were sent to the database: {self.embedding_tokens}
+    #         """
+    #     )
+    # else:
+    #     print(
+    #         f"""
+    #         Overview of All Tokens Used:
+    #         Tokens used in the embedding section that were sent to the database: {self.embedding_tokens}
+    #         """
+    #     )
```

### Comparing `indox-0.1.4/Indox/QaModels/Dspy_Cot/dspy.py` & `Indox-0.1.5/indox/qa_models/Dspy_Cot/dspy.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/QaModels/Mistral/mistral.py` & `Indox-0.1.5/indox/qa_models/Mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/QaModels/OpenAi/openai.py` & `Indox-0.1.5/indox/qa_models/OpenAi/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class OpenAiQA:
     def __init__(self, api_key, model):
         """
         Initializes the GPT-3 model with the specified model version.
 
         Args:
-            model (str, optional): The GPT-3 model version to use for generating summaries. Defaults to "text-davinci-003".
+            model (str, optional): The GPT-3 model.
         """
         self.model = model
         self.client = OpenAI(api_key=api_key)
 
     @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
     def _attempt_answer_question(
             self, context, question, max_tokens=150, stop_sequence=None, temperature=0
```

### Comparing `indox-0.1.4/Indox/utils.py` & `Indox-0.1.5/indox/utils.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/vectorstore.py` & `Indox-0.1.5/indox/vectorstore.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox/visualization.py` & `Indox-0.1.5/indox/visualization.py`

 * *Files identical despite different names*

### Comparing `indox-0.1.4/Indox.egg-info/PKG-INFO` & `Indox-0.1.5/Indox.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2049 6e64  : 2.1..Name: Ind
 00000020: 6f78 0d0a 5665 7273 696f 6e3a 2030 2e31  ox..Version: 0.1
-00000030: 2e34 0d0a 5375 6d6d 6172 793a 2049 6e64  .4..Summary: Ind
+00000030: 2e35 0d0a 5375 6d6d 6172 793a 2049 6e64  .5..Summary: Ind
 00000040: 6f78 2052 6574 7269 6576 616c 2041 7567  ox Retrieval Aug
 00000050: 6d65 6e74 6174 696f 6e0d 0a48 6f6d 652d  mentation..Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f6f 736c 6c6d 6169  thub.com/osllmai
 00000080: 2f69 6e44 6f78 0d0a 4175 7468 6f72 3a20  /inDox..Author: 
 00000090: 6e65 7264 7374 7564 696f 0d0a 4175 7468  nerdstudio..Auth
 000000a0: 6f72 2d65 6d61 696c 3a20 6173 686b 616e  or-email: ashkan
@@ -35,37 +35,37 @@
 00000220: 3a20 332e 3130 0d0a 436c 6173 7369 6669  : 3.10..Classifi
 00000230: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
 00000240: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000250: 6f6e 203a 3a20 332e 3131 0d0a 5265 7175  on :: 3.11..Requ
 00000260: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000270: 2e39 0d0a 4465 7363 7269 7074 696f 6e2d  .9..Description-
 00000280: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000290: 7874 2f6d 6172 6b64 6f77 6e0d 0a52 6571  xt/markdown..Req
-000002a0: 7569 7265 732d 4469 7374 3a20 6265 7274  uires-Dist: bert
-000002b0: 5f73 636f 7265 0d0a 5265 7175 6972 6573  _score..Requires
-000002c0: 2d44 6973 743a 2066 6169 7373 5f63 7075  -Dist: faiss_cpu
-000002d0: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-000002e0: 206c 616e 6763 6861 696e 0d0a 5265 7175   langchain..Requ
-000002f0: 6972 6573 2d44 6973 743a 206c 616e 6763  ires-Dist: langc
-00000300: 6861 696e 5f63 6f6d 6d75 6e69 7479 0d0a  hain_community..
-00000310: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
-00000320: 616e 6763 6861 696e 5f63 6f72 650d 0a52  angchain_core..R
-00000330: 6571 7569 7265 732d 4469 7374 3a20 6c61  equires-Dist: la
-00000340: 6e67 6368 6169 6e5f 6f70 656e 6169 0d0a  ngchain_openai..
-00000350: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
-00000360: 616e 6767 7261 7068 0d0a 5265 7175 6972  anggraph..Requir
-00000370: 6573 2d44 6973 743a 206c 6174 6578 326d  es-Dist: latex2m
-00000380: 6172 6b64 6f77 6e0d 0a52 6571 7569 7265  arkdown..Require
-00000390: 732d 4469 7374 3a20 6e6c 746b 0d0a 5265  s-Dist: nltk..Re
-000003a0: 7175 6972 6573 2d44 6973 743a 206e 756d  quires-Dist: num
-000003b0: 7079 0d0a 5265 7175 6972 6573 2d44 6973  py..Requires-Dis
-000003c0: 743a 2070 616e 6461 730d 0a52 6571 7569  t: pandas..Requi
-000003d0: 7265 732d 4469 7374 3a20 5079 5044 4632  res-Dist: PyPDF2
+00000290: 7874 2f6d 6172 6b64 6f77 6e0d 0a4c 6963  xt/markdown..Lic
+000002a0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000002b0: 5345 0d0a 5265 7175 6972 6573 2d44 6973  SE..Requires-Dis
+000002c0: 743a 2062 6572 745f 7363 6f72 650d 0a52  t: bert_score..R
+000002d0: 6571 7569 7265 732d 4469 7374 3a20 6661  equires-Dist: fa
+000002e0: 6973 735f 6370 750d 0a52 6571 7569 7265  iss_cpu..Require
+000002f0: 732d 4469 7374 3a20 6c61 6e67 6368 6169  s-Dist: langchai
+00000300: 6e0d 0a52 6571 7569 7265 732d 4469 7374  n..Requires-Dist
+00000310: 3a20 6c61 6e67 6368 6169 6e5f 636f 6d6d  : langchain_comm
+00000320: 756e 6974 790d 0a52 6571 7569 7265 732d  unity..Requires-
+00000330: 4469 7374 3a20 6c61 6e67 6368 6169 6e5f  Dist: langchain_
+00000340: 636f 7265 0d0a 5265 7175 6972 6573 2d44  core..Requires-D
+00000350: 6973 743a 206c 616e 6763 6861 696e 5f6f  ist: langchain_o
+00000360: 7065 6e61 690d 0a52 6571 7569 7265 732d  penai..Requires-
+00000370: 4469 7374 3a20 6c61 6e67 6772 6170 680d  Dist: langgraph.
+00000380: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000390: 6c61 7465 7832 6d61 726b 646f 776e 0d0a  latex2markdown..
+000003a0: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
+000003b0: 6c74 6b0d 0a52 6571 7569 7265 732d 4469  ltk..Requires-Di
+000003c0: 7374 3a20 6e75 6d70 790d 0a52 6571 7569  st: numpy..Requi
+000003d0: 7265 732d 4469 7374 3a20 7061 6e64 6173  res-Dist: pandas
 000003e0: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-000003f0: 2050 7959 414d 4c0d 0a52 6571 7569 7265   PyYAML..Require
+000003f0: 2050 7950 4446 320d 0a52 6571 7569 7265   PyPDF2..Require
 00000400: 732d 4469 7374 3a20 5079 5941 4d4c 0d0a  s-Dist: PyYAML..
 00000410: 5265 7175 6972 6573 2d44 6973 743a 2052  Requires-Dist: R
 00000420: 6571 7565 7374 730d 0a52 6571 7569 7265  equests..Require
 00000430: 732d 4469 7374 3a20 7363 696b 6974 5f6c  s-Dist: scikit_l
 00000440: 6561 726e 0d0a 5265 7175 6972 6573 2d44  earn..Requires-D
 00000450: 6973 743a 2073 656e 7465 6e63 655f 7472  ist: sentence_tr
 00000460: 616e 7366 6f72 6d65 7273 0d0a 5265 7175  ansformers..Requ
@@ -78,440 +78,542 @@
 000004d0: 7273 0d0a 5265 7175 6972 6573 2d44 6973  rs..Requires-Dis
 000004e0: 743a 2074 6f72 6368 0d0a 5265 7175 6972  t: torch..Requir
 000004f0: 6573 2d44 6973 743a 2074 7261 6e73 666f  es-Dist: transfo
 00000500: 726d 6572 730d 0a52 6571 7569 7265 732d  rmers..Requires-
 00000510: 4469 7374 3a20 756d 6170 5f6c 6561 726e  Dist: umap_learn
 00000520: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
 00000530: 2075 6e73 7472 7563 7475 7265 640d 0a0d   unstructured...
-00000540: 0a23 2069 6e44 6f78 3a20 4164 7661 6e63  .# inDox: Advanc
-00000550: 6564 2053 6561 7263 6820 616e 6420 5265  ed Search and Re
-00000560: 7472 6965 7661 6c20 4175 676d 656e 7461  trieval Augmenta
-00000570: 7469 6f6e 2047 656e 6572 6174 6976 650d  tion Generative.
-00000580: 0a0d 0a2a 2a49 6e64 6f78 2052 6574 7269  ...**Indox Retri
-00000590: 6576 616c 2041 7567 6d65 6e74 6174 696f  eval Augmentatio
-000005a0: 6e2a 2a20 6973 2061 6e20 696e 6e6f 7661  n** is an innova
-000005b0: 7469 7665 2061 7070 6c69 6361 7469 6f6e  tive application
-000005c0: 2064 6573 6967 6e65 6420 746f 2073 7472   designed to str
-000005d0: 6561 6d6c 696e 6520 696e 666f 726d 6174  eamline informat
-000005e0: 696f 6e20 6578 7472 6163 7469 6f6e 2066  ion extraction f
-000005f0: 726f 6d20 6120 7769 6465 0d0a 7261 6e67  rom a wide..rang
-00000600: 6520 6f66 2064 6f63 756d 656e 7420 7479  e of document ty
-00000610: 7065 732c 2069 6e63 6c75 6469 6e67 2074  pes, including t
-00000620: 6578 7420 6669 6c65 732c 2050 4446 2c20  ext files, PDF, 
-00000630: 4854 4d4c 2c20 4d61 726b 646f 776e 2c20  HTML, Markdown, 
-00000640: 616e 6420 4c61 5465 582e 2057 6865 7468  and LaTeX. Wheth
-00000650: 6572 2073 7472 7563 7475 7265 6420 6f72  er structured or
-00000660: 2075 6e73 7472 7563 7475 7265 642c 2049   unstructured, I
-00000670: 6e64 6f78 0d0a 7072 6f76 6964 6573 2075  ndox..provides u
-00000680: 7365 7273 2077 6974 6820 6120 706f 7765  sers with a powe
-00000690: 7266 756c 2074 6f6f 6c73 6574 2074 6f20  rful toolset to 
-000006a0: 6566 6669 6369 656e 746c 7920 6578 7472  efficiently extr
-000006b0: 6163 7420 7265 6c65 7661 6e74 2064 6174  act relevant dat
-000006c0: 612e 0d0a 0d0a 496e 646f 7820 5265 7472  a.....Indox Retr
-000006d0: 6965 7661 6c20 4175 676d 656e 7461 7469  ieval Augmentati
-000006e0: 6f6e 2069 7320 616e 2069 6e6e 6f76 6174  on is an innovat
-000006f0: 6976 6520 6170 706c 6963 6174 696f 6e20  ive application 
-00000700: 6465 7369 676e 6564 2074 6f20 7374 7265  designed to stre
-00000710: 616d 6c69 6e65 2069 6e66 6f72 6d61 7469  amline informati
-00000720: 6f6e 2065 7874 7261 6374 696f 6e20 6672  on extraction fr
-00000730: 6f6d 2061 2077 6964 650d 0a72 616e 6765  om a wide..range
-00000740: 206f 6620 646f 6375 6d65 6e74 2074 7970   of document typ
-00000750: 6573 2c20 696e 636c 7564 696e 6720 7465  es, including te
-00000760: 7874 2066 696c 6573 2c20 5044 462c 2048  xt files, PDF, H
-00000770: 544d 4c2c 204d 6172 6b64 6f77 6e2c 2061  TML, Markdown, a
-00000780: 6e64 204c 6154 6558 2e20 5768 6574 6865  nd LaTeX. Whethe
-00000790: 7220 7374 7275 6374 7572 6564 206f 7220  r structured or 
-000007a0: 756e 7374 7275 6374 7572 6564 2c20 496e  unstructured, In
-000007b0: 646f 780d 0a70 726f 7669 6465 7320 7573  dox..provides us
-000007c0: 6572 7320 7769 7468 2061 2070 6f77 6572  ers with a power
-000007d0: 6675 6c20 746f 6f6c 7365 7420 746f 2065  ful toolset to e
-000007e0: 6666 6963 6965 6e74 6c79 2065 7874 7261  fficiently extra
-000007f0: 6374 2072 656c 6576 616e 7420 6461 7461  ct relevant data
-00000800: 2e20 4f6e 6520 6f66 2069 7473 206b 6579  . One of its key
-00000810: 2066 6561 7475 7265 7320 6973 2074 6865   features is the
-00000820: 2061 6269 6c69 7479 2074 6f0d 0a69 6e74   ability to..int
-00000830: 656c 6c69 6765 6e74 6c79 2063 6c75 7374  elligently clust
-00000840: 6572 2070 7269 6d61 7279 2063 6875 6e6b  er primary chunk
-00000850: 7320 746f 2066 6f72 6d20 6d6f 7265 2072  s to form more r
-00000860: 6f62 7573 7420 6772 6f75 7069 6e67 732c  obust groupings,
-00000870: 2065 6e68 616e 6369 6e67 2074 6865 2071   enhancing the q
-00000880: 7561 6c69 7479 2061 6e64 2072 656c 6576  uality and relev
-00000890: 616e 6365 206f 6620 7468 6520 6578 7472  ance of the extr
-000008a0: 6163 7465 640d 0a69 6e66 6f72 6d61 7469  acted..informati
-000008b0: 6f6e 2e0d 0a57 6974 6820 6120 666f 6375  on...With a focu
-000008c0: 7320 6f6e 2061 6461 7074 6162 696c 6974  s on adaptabilit
-000008d0: 7920 616e 6420 7573 6572 2d63 656e 7472  y and user-centr
-000008e0: 6963 2064 6573 6967 6e2c 2049 6e64 6f78  ic design, Indox
-000008f0: 2061 696d 7320 746f 2064 656c 6976 6572   aims to deliver
-00000900: 2066 7574 7572 652d 7265 6164 7920 6675   future-ready fu
-00000910: 6e63 7469 6f6e 616c 6974 7920 7769 7468  nctionality with
-00000920: 206d 6f72 650d 0a66 6561 7475 7265 7320   more..features 
-00000930: 706c 616e 6e65 6420 666f 7220 7570 636f  planned for upco
-00000940: 6d69 6e67 2072 656c 6561 7365 732e 204a  ming releases. J
-00000950: 6f69 6e20 7573 2069 6e20 6578 706c 6f72  oin us in explor
-00000960: 696e 6720 686f 7720 496e 646f 7820 6361  ing how Indox ca
-00000970: 6e20 7265 766f 6c75 7469 6f6e 697a 6520  n revolutionize 
-00000980: 796f 7572 2064 6f63 756d 656e 7420 7072  your document pr
-00000990: 6f63 6573 7369 6e67 0d0a 776f 726b 666c  ocessing..workfl
-000009a0: 6f77 2c20 6272 696e 6769 6e67 2063 6c61  ow, bringing cla
-000009b0: 7269 7479 2061 6e64 206f 7267 616e 697a  rity and organiz
-000009c0: 6174 696f 6e20 746f 2079 6f75 7220 6461  ation to your da
-000009d0: 7461 2072 6574 7269 6576 616c 206e 6565  ta retrieval nee
-000009e0: 6473 2e0d 0a0d 0a23 2320 5072 6572 6571  ds.....## Prereq
-000009f0: 7569 7369 7465 730d 0a0d 0a42 6566 6f72  uisites....Befor
-00000a00: 6520 7275 6e6e 696e 6720 7468 6973 2070  e running this p
-00000a10: 726f 6a65 6374 2c20 656e 7375 7265 2074  roject, ensure t
-00000a20: 6861 7420 796f 7520 6861 7665 2074 6865  hat you have the
-00000a30: 2066 6f6c 6c6f 7769 6e67 2069 6e73 7461   following insta
-00000a40: 6c6c 6564 3a0d 0a0d 0a2d 202a 2a50 7974  lled:....- **Pyt
-00000a50: 686f 6e20 332e 382b 2a2a 3a20 5265 7175  hon 3.8+**: Requ
-00000a60: 6972 6564 2066 6f72 2072 756e 6e69 6e67  ired for running
-00000a70: 2074 6865 2050 7974 686f 6e20 6261 636b   the Python back
-00000a80: 656e 642e 0d0a 2d20 2a2a 506f 7374 6772  end...- **Postgr
-00000a90: 6553 514c 2a2a 3a20 4e65 6564 6564 2069  eSQL**: Needed i
-00000aa0: 6620 796f 7520 7769 7368 2074 6f20 7374  f you wish to st
-00000ab0: 6f72 6520 796f 7572 2064 6174 6120 696e  ore your data in
-00000ac0: 2061 2050 6f73 7467 7265 5351 4c20 6461   a PostgreSQL da
-00000ad0: 7461 6261 7365 2e0d 0a2d 202a 2a4f 7065  tabase...- **Ope
-00000ae0: 6e41 4920 4150 4920 4b65 792a 2a3a 204e  nAI API Key**: N
-00000af0: 6563 6573 7361 7279 2069 6620 796f 7520  ecessary if you 
-00000b00: 6172 6520 7573 696e 6720 7468 6520 4f70  are using the Op
-00000b10: 656e 4149 2065 6d62 6564 6469 6e67 206d  enAI embedding m
-00000b20: 6f64 656c 2e0d 0a2d 202a 2a48 7567 6769  odel...- **Huggi
-00000b30: 6e67 4661 6365 2041 5049 204b 6579 2a2a  ngFace API Key**
-00000b40: 3a20 4e65 6365 7373 6172 7920 6966 2079  : Necessary if y
-00000b50: 6f75 2061 7265 2075 7369 6e67 2074 6865  ou are using the
-00000b60: 2048 7567 6769 6e67 4661 6365 206c 6c6d   HuggingFace llm
-00000b70: 732e 0d0a 0d0a 456e 7375 7265 2079 6f75  s.....Ensure you
-00000b80: 7220 7379 7374 656d 2061 6c73 6f20 6d65  r system also me
-00000b90: 6574 7320 7468 6573 6520 7265 7175 6972  ets these requir
-00000ba0: 656d 656e 7473 3a0d 0a0d 0a2d 2041 6363  ements:....- Acc
-00000bb0: 6573 7320 746f 2065 6e76 6972 6f6e 6d65  ess to environme
-00000bc0: 6e74 616c 2076 6172 6961 626c 6573 2066  ntal variables f
-00000bd0: 6f72 2068 616e 646c 696e 6720 7365 6e73  or handling sens
-00000be0: 6974 6976 6520 696e 666f 726d 6174 696f  itive informatio
-00000bf0: 6e20 6c69 6b65 2041 5049 206b 6579 732e  n like API keys.
-00000c00: 0d0a 2d20 5375 6974 6162 6c65 2068 6172  ..- Suitable har
-00000c10: 6477 6172 6520 6361 7061 626c 6520 6f66  dware capable of
-00000c20: 2073 7570 706f 7274 696e 6720 696e 7465   supporting inte
-00000c30: 6e73 6976 6520 636f 6d70 7574 6174 696f  nsive computatio
-00000c40: 6e61 6c20 7461 736b 732e 0d0a 0d0a 2323  nal tasks.....##
-00000c50: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
-00000c60: 0a43 6c6f 6e65 2074 6865 2072 6570 6f73  .Clone the repos
-00000c70: 6974 6f72 7920 616e 6420 6e61 7669 6761  itory and naviga
-00000c80: 7465 2074 6f20 7468 6520 6469 7265 6374  te to the direct
-00000c90: 6f72 793a 0d0a 0d0a 6060 6062 6173 680d  ory:....```bash.
-00000ca0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
-00000cb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f73  ://github.com/os
-00000cc0: 6c6c 6d61 692f 696e 446f 782e 6769 740d  llmai/inDox.git.
-00000cd0: 0a63 6420 696e 446f 780d 0a60 6060 0d0a  .cd inDox..```..
-00000ce0: 0d0a 496e 7374 616c 6c20 7468 6520 7265  ..Install the re
-00000cf0: 7175 6972 6564 2050 7974 686f 6e20 7061  quired Python pa
-00000d00: 636b 6167 6573 3a0d 0a0d 0a60 6060 6261  ckages:....```ba
-00000d10: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
-00000d20: 2d72 2072 6571 7569 7265 6d65 6e74 732e  -r requirements.
-00000d30: 7478 740d 0a60 6060 0d0a 0d0a 2323 2043  txt..```....## C
-00000d40: 6f6e 6669 6775 7261 7469 6f6e 0d0a 0d0a  onfiguration....
-00000d50: 2323 2320 456e 7669 726f 6e6d 656e 7420  ### Environment 
-00000d60: 5661 7269 6162 6c65 730d 0a0d 0a53 6574  Variables....Set
-00000d70: 2079 6f75 7220 604f 5045 4e41 495f 4150   your `OPENAI_AP
-00000d80: 495f 4b45 5960 206f 7220 6048 465f 4150  I_KEY` or `HF_AP
-00000d90: 495f 4b45 5960 2069 6e20 796f 7572 2065  I_KEY` in your e
-00000da0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00000db0: 626c 6573 2066 6f72 2073 6563 7572 6520  bles for secure 
-00000dc0: 6163 6365 7373 2e0d 0a0d 0a23 2323 2044  access.....### D
-00000dd0: 6174 6162 6173 6520 5365 7475 700d 0a0d  atabase Setup...
-00000de0: 0a45 6e73 7572 6520 796f 7572 2050 6f73  .Ensure your Pos
-00000df0: 7467 7265 5351 4c20 6461 7461 6261 7365  tgreSQL database
-00000e00: 2069 7320 7570 2061 6e64 2072 756e 6e69   is up and runni
-00000e10: 6e67 2c20 616e 6420 6163 6365 7373 6962  ng, and accessib
-00000e20: 6c65 2066 726f 6d20 796f 7572 2061 7070  le from your app
-00000e30: 6c69 6361 7469 6f6e 2e20 5468 6973 2069  lication. This i
-00000e40: 7320 6e65 6365 7373 6172 7920 6966 2079  s necessary if y
-00000e50: 6f75 2070 6c61 6e20 746f 2075 7365 2070  ou plan to use p
-00000e60: 6776 6563 746f 7220 6173 2079 6f75 7220  gvector as your 
-00000e70: 7665 6374 6f72 2073 746f 7265 2e0d 0a0d  vector store....
-00000e80: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
-00000e90: 796f 7520 6361 6e20 7573 6520 4368 726f  you can use Chro
-00000ea0: 6d61 206f 7220 4661 6973 7320 6173 2079  ma or Faiss as y
-00000eb0: 6f75 7220 7665 6374 6f72 2073 746f 7265  our vector store
-00000ec0: 2e20 4d61 6b65 2073 7572 6520 746f 2073  . Make sure to s
-00000ed0: 7065 6369 6679 2079 6f75 7220 6368 6f69  pecify your choi
-00000ee0: 6365 2061 6e64 2074 6865 206e 6563 6573  ce and the neces
-00000ef0: 7361 7279 2063 6f6e 6669 6775 7261 7469  sary configurati
-00000f00: 6f6e 7320 696e 2074 6865 2063 6f6e 6669  ons in the confi
-00000f10: 672e 7961 6d6c 2066 696c 652e 0d0a 0d0a  g.yaml file.....
-00000f20: 2323 2055 7361 6765 0d0a 0d0a 2323 2320  ## Usage....### 
-00000f30: 5072 6570 6172 696e 6720 596f 7572 2044  Preparing Your D
-00000f40: 6174 610d 0a0d 0a31 2e20 2a2a 4465 6669  ata....1. **Defi
-00000f50: 6e65 2074 6865 2046 696c 6520 5061 7468  ne the File Path
-00000f60: 2a2a 3a20 5370 6563 6966 7920 7468 6520  **: Specify the 
-00000f70: 7061 7468 2074 6f20 796f 7572 2074 6578  path to your tex
-00000f80: 7420 6f72 2050 4446 2066 696c 652e 0d0a  t or PDF file...
-00000f90: 322e 202a 2a4c 6f61 6420 456d 6265 6464  2. **Load Embedd
-00000fa0: 696e 6720 4d6f 6465 6c73 2a2a 3a20 496e  ing Models**: In
-00000fb0: 6974 6961 6c69 7a65 2079 6f75 7220 656d  itialize your em
-00000fc0: 6265 6464 696e 6720 6d6f 6465 6c20 6672  bedding model fr
-00000fd0: 6f6d 204f 7065 6e41 4927 7320 7365 6c65  om OpenAI's sele
-00000fe0: 6374 696f 6e20 6f66 2070 7265 2d74 7261  ction of pre-tra
-00000ff0: 696e 6564 206d 6f64 656c 732e 0d0a 0d0a  ined models.....
-00001000: 2320 5175 6963 6b20 5374 6172 7420 0d0a  # Quick Start ..
-00001010: 0d0a 2323 2049 6d70 6f72 7420 496e 646f  ..## Import Indo
-00001020: 7820 5061 636b 6167 650d 0a0d 0a49 6d70  x Package....Imp
-00001030: 6f72 7420 7468 6520 6e65 6365 7373 6172  ort the necessar
-00001040: 7920 636c 6173 7365 7320 6672 6f6d 2074  y classes from t
-00001050: 6865 2049 6e64 6f78 2070 6163 6b61 6765  he Indox package
-00001060: 2e0d 0a0d 0a60 6060 2070 7974 686f 6e0d  .....``` python.
-00001070: 0a66 726f 6d20 496e 646f 7820 696d 706f  .from Indox impo
-00001080: 7274 2049 6e64 6f78 5265 7472 6965 7661  rt IndoxRetrieva
-00001090: 6c41 7567 6d65 6e74 6174 696f 6e0d 0a60  lAugmentation..`
-000010a0: 6060 0d0a 0d0a 2323 2320 496e 6974 6961  ``....### Initia
-000010b0: 6c69 7a65 2049 6e64 6f78 0d0a 0d0a 4372  lize Indox....Cr
-000010c0: 6561 7465 2061 6e20 696e 7374 616e 6365  eate an instance
-000010d0: 206f 6620 496e 646f 7852 6574 7269 6576   of IndoxRetriev
-000010e0: 616c 4175 676d 656e 7461 7469 6f6e 2e0d  alAugmentation..
-000010f0: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a49  ...``` python..I
-00001100: 6e64 6f78 203d 2049 6e64 6f78 5265 7472  ndox = IndoxRetr
-00001110: 6965 7661 6c41 7567 6d65 6e74 6174 696f  ievalAugmentatio
-00001120: 6e28 290d 0a60 6060 0d0a 2323 2049 6e69  n()..```..## Ini
-00001130: 7469 616c 2043 6f6e 6669 6775 7261 7469  tial Configurati
-00001140: 6f6e 0d0a 0d0a 2d20 2a2a 436f 6e66 6967  on....- **Config
-00001150: 7572 6174 696f 6e20 4669 6c65 2a2a 3a20  uration File**: 
-00001160: 456e 7375 7265 2079 6f75 206c 6f63 6174  Ensure you locat
-00001170: 6520 616e 6420 6d6f 6469 6679 2074 6865  e and modify the
-00001180: 2060 496e 646f 782e 636f 6e66 6967 6020   `Indox.config` 
-00001190: 5941 4d4c 2066 696c 6520 6163 636f 7264  YAML file accord
-000011a0: 696e 6720 746f 2079 6f75 7220 6e65 6564  ing to your need
-000011b0: 7320 6265 666f 7265 0d0a 2020 7374 6172  s before..  star
-000011c0: 7469 6e67 2074 6865 2061 7070 6c69 6361  ting the applica
-000011d0: 7469 6f6e 2e0d 0a0d 0a23 2320 4479 6e61  tion.....## Dyna
-000011e0: 6d69 6320 436f 6e66 6967 7572 6174 696f  mic Configuratio
-000011f0: 6e20 4368 616e 6765 730d 0a0d 0a46 6f72  n Changes....For
-00001200: 2063 6861 6e67 6573 2074 6861 7420 6e65   changes that ne
-00001210: 6564 2074 6f20 6265 2061 7070 6c69 6564  ed to be applied
-00001220: 2061 6674 6572 2074 6865 2069 6e69 7469   after the initi
-00001230: 616c 2073 6574 7570 206f 7220 6475 7269  al setup or duri
-00001240: 6e67 2072 756e 7469 6d65 3a0d 0a0d 0a2d  ng runtime:....-
-00001250: 202a 2a4d 6f64 6966 7969 6e67 2043 6f6e   **Modifying Con
-00001260: 6669 6775 7261 7469 6f6e 732a 2a3a 2055  figurations**: U
-00001270: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00001280: 2050 7974 686f 6e20 736e 6970 7065 7420   Python snippet 
-00001290: 746f 2075 7064 6174 6520 796f 7572 2073  to update your s
-000012a0: 6574 7469 6e67 7320 6479 6e61 6d69 6361  ettings dynamica
-000012b0: 6c6c 793a 0d0a 2020 6060 6070 7974 686f  lly:..  ```pytho
-000012c0: 6e0d 0a20 2049 6e64 6f78 2e63 6f6e 6669  n..  Indox.confi
-000012d0: 675b 2279 6f75 725f 7365 7474 696e 675f  g["your_setting_
-000012e0: 7468 6174 5f6e 6565 645f 746f 5f63 6861  that_need_to_cha
-000012f0: 6e67 6522 5d20 3d20 226e 6577 5f73 6574  nge"] = "new_set
-00001300: 7469 6e67 220d 0a20 2049 6e64 6f78 2e75  ting"..  Indox.u
-00001310: 7064 6174 655f 636f 6e66 6967 2829 0d0a  pdate_config()..
-00001320: 0d0a 2323 2043 6f6e 6669 6775 7261 7469  ..## Configurati
-00001330: 6f6e 2044 6574 6169 6c73 0d0a 0d0a 4865  on Details....He
-00001340: 7265 2773 2061 2062 7265 616b 646f 776e  re's a breakdown
-00001350: 206f 6620 7468 6520 636f 6e66 6967 2064   of the config d
-00001360: 6963 7469 6f6e 6172 7920 616e 6420 6974  ictionary and it
-00001370: 7320 7072 6f70 6572 7469 6573 3a0d 0a0d  s properties:...
-00001380: 0a23 2323 2050 6f73 7467 7265 5351 4c0d  .### PostgreSQL.
-00001390: 0a0d 0a2d 2060 636f 6e6e 5f73 7472 696e  ...- `conn_strin
-000013a0: 6760 3a20 596f 7572 2050 6f73 7467 7265  g`: Your Postgre
-000013b0: 5351 4c20 6461 7461 6261 7365 2063 7265  SQL database cre
-000013c0: 6465 6e74 6961 6c73 2e0d 0a0d 0a23 2323  dentials.....###
-000013d0: 2053 756d 6d61 7279 204d 6f64 656c 0d0a   Summary Model..
-000013e0: 0d0a 2d20 606d 6178 5f74 6f6b 656e 7360  ..- `max_tokens`
-000013f0: 3a20 4d61 7869 6d75 6d20 746f 6b65 6e20  : Maximum token 
-00001400: 636f 756e 7420 7468 6520 7375 6d6d 6172  count the summar
-00001410: 7920 6d6f 6465 6c20 6361 6e20 6765 6e65  y model can gene
-00001420: 7261 7465 2e0d 0a2d 2060 6d69 6e5f 6c65  rate...- `min_le
-00001430: 6e60 3a20 4d69 6e69 6d75 6d20 746f 6b65  n`: Minimum toke
-00001440: 6e20 636f 756e 7420 7468 6520 7375 6d6d  n count the summ
-00001450: 6172 7920 6d6f 6465 6c20 6765 6e65 7261  ary model genera
-00001460: 7465 732e 0d0a 2d20 606d 6f64 656c 5f6e  tes...- `model_n
-00001470: 616d 6560 3a20 4465 6661 756c 7420 6973  ame`: Default is
-00001480: 2060 6770 742d 332e 352d 7475 7262 6f2d   `gpt-3.5-turbo-
-00001490: 3031 3235 602c 2062 7574 2069 7420 6361  0125`, but it ca
-000014a0: 6e20 6265 2072 6570 6c61 6365 6420 7769  n be replaced wi
-000014b0: 7468 2061 6e79 2048 7567 6769 6e67 2046  th any Hugging F
-000014c0: 6163 6520 6d6f 6465 6c20 7375 7070 6f72  ace model suppor
-000014d0: 7469 6e67 2074 6865 0d0a 2020 7375 6d6d  ting the..  summ
-000014e0: 6172 697a 6174 696f 6e20 7069 7065 6c69  arization pipeli
-000014f0: 6e65 2e0d 0a0d 0a23 2323 2050 6f73 7467  ne.....### Postg
-00001500: 7265 5351 4c20 5365 7475 7020 7769 7468  reSQL Setup with
-00001510: 2070 6776 6563 746f 720d 0a0d 0a49 6620   pgvector....If 
-00001520: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00001530: 506f 7374 6772 6553 514c 2066 6f72 2076  PostgreSQL for v
-00001540: 6563 746f 7220 7374 6f72 6167 652c 2079  ector storage, y
-00001550: 6f75 2073 686f 756c 6420 7065 7266 6f72  ou should perfor
-00001560: 6d20 7468 6520 666f 6c6c 6f77 696e 6720  m the following 
-00001570: 7374 6570 733a 0d0a 0d0a 312e 202a 2a49  steps:....1. **I
-00001580: 6e73 7461 6c6c 2070 6776 6563 746f 722a  nstall pgvector*
-00001590: 2a3a 2054 6f20 696e 7374 616c 6c20 6070  *: To install `p
-000015a0: 6776 6563 746f 7260 206f 6e20 796f 7572  gvector` on your
-000015b0: 2050 6f73 7467 7265 5351 4c20 7365 7276   PostgreSQL serv
-000015c0: 6572 2c20 666f 6c6c 6f77 2074 6865 2064  er, follow the d
-000015d0: 6574 6169 6c65 6420 696e 7374 616c 6c61  etailed installa
-000015e0: 7469 6f6e 2069 6e73 7472 7563 7469 6f6e  tion instruction
-000015f0: 730d 0a20 2020 6176 6169 6c61 626c 6520  s..   available 
-00001600: 6f6e 2074 6865 206f 6666 6963 6961 6c20  on the official 
-00001610: 7067 7665 6374 6f72 2047 6974 4875 6220  pgvector GitHub 
-00001620: 7265 706f 7369 746f 7279 3a0d 0a20 2020  repository:..   
-00001630: 5b70 6776 6563 746f 7220 496e 7374 616c  [pgvector Instal
-00001640: 6c61 7469 6f6e 2049 6e73 7472 7563 7469  lation Instructi
-00001650: 6f6e 735d 2868 7474 7073 3a2f 2f67 6974  ons](https://git
-00001660: 6875 622e 636f 6d2f 7067 7665 6374 6f72  hub.com/pgvector
-00001670: 2f70 6776 6563 746f 7229 0d0a 0d0a 322e  /pgvector)....2.
-00001680: 202a 2a41 6464 2056 6563 746f 7220 4578   **Add Vector Ex
-00001690: 7465 6e73 696f 6e2a 2a3a 0d0a 2020 2043  tension**:..   C
-000016a0: 6f6e 6e65 6374 2074 6f20 796f 7572 2050  onnect to your P
-000016b0: 6f73 7467 7265 5351 4c20 6461 7461 6261  ostgreSQL databa
-000016c0: 7365 2061 6e64 2065 7865 6375 7465 2074  se and execute t
-000016d0: 6865 2066 6f6c 6c6f 7769 6e67 2053 514c  he following SQL
-000016e0: 2063 6f6d 6d61 6e64 2074 6f20 6372 6561   command to crea
-000016f0: 7465 2074 6865 2060 7067 7665 6374 6f72  te the `pgvector
-00001700: 6020 6578 7465 6e73 696f 6e3a 0d0a 0d0a  ` extension:....
-00001710: 2020 2060 6060 7371 6c0d 0a20 2020 2d2d     ```sql..   --
-00001720: 2043 6f6e 6e65 6374 2074 6f20 796f 7572   Connect to your
-00001730: 2064 6174 6162 6173 650d 0a20 2020 7073   database..   ps
-00001740: 716c 202d 5520 7573 6572 6e61 6d65 202d  ql -U username -
-00001750: 6420 6461 7461 6261 7365 5f6e 616d 650d  d database_name.
-00001760: 0a0d 0a20 2020 2d2d 2052 756e 2069 6e73  ...   -- Run ins
-00001770: 6964 6520 796f 7572 2070 7371 6c20 7465  ide your psql te
-00001780: 726d 696e 616c 0d0a 2020 2043 5245 4154  rminal..   CREAT
-00001790: 4520 4558 5445 4e53 494f 4e20 7665 6374  E EXTENSION vect
-000017a0: 6f72 3b0d 0a20 2020 2320 5265 706c 6163  or;..   # Replac
-000017b0: 6520 7468 6520 706c 6163 6568 6f6c 6465  e the placeholde
-000017c0: 7273 2077 6974 6820 796f 7572 2061 6374  rs with your act
-000017d0: 7561 6c20 506f 7374 6772 6553 514c 2063  ual PostgreSQL c
-000017e0: 7265 6465 6e74 6961 6c73 2061 6e64 2064  redentials and d
-000017f0: 6574 6169 6c73 0d0a 0d0a 4164 6469 7469  etails....Additi
-00001800: 6f6e 616c 6c79 2c20 666f 7220 7468 6f73  onally, for thos
-00001810: 6520 696e 7465 7265 7374 6564 2069 6e20  e interested in 
-00001820: 6578 706c 6f72 696e 6720 6f74 6865 7220  exploring other 
-00001830: 7665 6374 6f72 2064 6174 6162 6173 6520  vector database 
-00001840: 6f70 7469 6f6e 732c 2079 6f75 2063 616e  options, you can
-00001850: 2063 6f6e 7369 6465 7220 7573 696e 6720   consider using 
-00001860: 2a2a 4368 726f 6d61 2a2a 206f 7220 2a0d  **Chroma** or *.
-00001870: 0a2a 4661 6973 732a 2a2e 2054 6865 7365  .*Faiss**. These
-00001880: 2070 726f 7669 6465 2061 6c74 6572 6e61   provide alterna
-00001890: 7469 7665 2061 7070 726f 6163 6865 7320  tive approaches 
-000018a0: 746f 2076 6563 746f 7220 7374 6f72 6167  to vector storag
-000018b0: 6520 616e 6420 7265 7472 6965 7661 6c20  e and retrieval 
-000018c0: 7468 6174 206d 6179 2062 6574 7465 7220  that may better 
-000018d0: 7375 6974 2073 7065 6369 6669 6320 7573  suit specific us
-000018e0: 6520 6361 7365 730d 0a6f 7220 7065 7266  e cases..or perf
-000018f0: 6f72 6d61 6e63 6520 7265 7175 6972 656d  ormance requirem
-00001900: 656e 7473 2e0d 0a0d 0a23 2323 2049 6d70  ents.....### Imp
-00001910: 6f72 7469 6e67 2051 4120 616e 6420 456d  orting QA and Em
-00001920: 6265 6464 696e 6720 4d6f 6465 6c73 0d0a  bedding Models..
-00001930: 0d0a 6060 6020 7079 7468 6f6e 0d0a 6672  ..``` python..fr
-00001940: 6f6d 2049 6e64 6f78 2e51 614d 6f64 656c  om Indox.QaModel
-00001950: 7320 696d 706f 7274 204f 7065 6e41 6951  s import OpenAiQ
-00001960: 410d 0a60 6060 0d0a 0d0a 6060 6020 7079  A..```....``` py
-00001970: 7468 6f6e 0d0a 6672 6f6d 2049 6e64 6f78  thon..from Indox
-00001980: 2e45 6d62 6564 6469 6e67 7320 696d 706f  .Embeddings impo
-00001990: 7274 204f 7065 6e41 6945 6d62 6564 6469  rt OpenAiEmbeddi
-000019a0: 6e67 0d0a 6060 600d 0a0d 0a0d 0a60 6060  ng..```......```
-000019b0: 2070 7974 686f 6e0d 0a6f 7065 6e61 695f   python..openai_
-000019c0: 7161 203d 204f 7065 6e41 6951 4128 6170  qa = OpenAiQA(ap
-000019d0: 695f 6b65 793d 4f50 454e 4149 5f41 5049  i_key=OPENAI_API
-000019e0: 5f4b 4559 2c6d 6f64 656c 3d22 6770 742d  _KEY,model="gpt-
-000019f0: 332e 352d 7475 7262 6f2d 3031 3235 2229  3.5-turbo-0125")
-00001a00: 0d0a 6f70 656e 6169 5f65 6d62 6564 6469  ..openai_embeddi
-00001a10: 6e67 7320 3d20 4f70 656e 4169 456d 6265  ngs = OpenAiEmbe
-00001a20: 6464 696e 6728 6d6f 6465 6c3d 2274 6578  dding(model="tex
-00001a30: 742d 656d 6265 6464 696e 672d 332d 736d  t-embedding-3-sm
-00001a40: 616c 6c22 2c6f 7065 6e61 695f 6170 695f  all",openai_api_
-00001a50: 6b65 793d 4f50 454e 4149 5f41 5049 5f4b  key=OPENAI_API_K
-00001a60: 4559 290d 0a60 6060 0d0a 0d0a 2323 204d  EY)..```....## M
-00001a70: 6f64 6966 7969 6e67 2043 6f6e 6669 6775  odifying Configu
-00001a80: 7261 7469 6f6e 2053 6574 7469 6e67 730d  ration Settings.
-00001a90: 0a0d 0a54 6f20 6368 616e 6765 2061 2063  ...To change a c
-00001aa0: 6f6e 6669 6775 7261 7469 6f6e 2073 6574  onfiguration set
-00001ab0: 7469 6e67 2c20 796f 7520 6361 6e20 6469  ting, you can di
-00001ac0: 7265 6374 6c79 206d 6f64 6966 7920 7468  rectly modify th
-00001ad0: 650d 0a60 496e 646f 782e 636f 6e66 6967  e..`Indox.config
-00001ae0: 6020 6469 6374 696f 6e61 7279 2e20 4865  ` dictionary. He
-00001af0: 7265 2069 7320 616e 2065 7861 6d70 6c65  re is an example
-00001b00: 206f 6620 686f 7720 796f 7520 6361 6e20   of how you can 
-00001b10: 7570 6461 7465 2061 0d0a 636f 6e66 6967  update a..config
-00001b20: 7572 6174 696f 6e20 7365 7474 696e 673a  uration setting:
-00001b30: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
-00001b40: 2320 4578 616d 706c 6520 6f66 206d 6f64  # Example of mod
-00001b50: 6966 7969 6e67 2061 2063 6f6e 6669 6775  ifying a configu
-00001b60: 7261 7469 6f6e 2073 6574 7469 6e67 0d0a  ration setting..
-00001b70: 496e 646f 782e 636f 6e66 6967 5b22 6f6c  Indox.config["ol
-00001b80: 645f 636f 6e66 6967 225d 203d 2022 6e65  d_config"] = "ne
-00001b90: 775f 636f 6e66 6967 220d 0a0d 0a23 2041  w_config"....# A
-00001ba0: 7070 6c79 696e 6720 7468 6520 7570 6461  pplying the upda
-00001bb0: 7465 6420 636f 6e66 6967 7572 6174 696f  ted configuratio
-00001bc0: 6e0d 0a49 6e64 6f78 2e75 7064 6174 655f  n..Indox.update_
-00001bd0: 636f 6e66 6967 2829 0d0a 6060 600d 0a0d  config()..```...
-00001be0: 0a0d 0a57 6520 7461 6b65 2061 6476 616e  ...We take advan
-00001bf0: 7461 6765 206f 6620 7468 6520 6075 6e73  tage of the `uns
-00001c00: 7472 7563 7475 7265 6460 206c 6962 7261  tructured` libra
-00001c10: 7279 2074 6f20 6c6f 6164 0d0a 646f 6375  ry to load..docu
-00001c20: 6d65 6e74 7320 616e 6420 7370 6c69 7420  ments and split 
-00001c30: 7468 656d 2069 6e74 6f20 6368 756e 6b73  them into chunks
-00001c40: 2062 7920 7469 746c 652e 2054 6869 7320   by title. This 
-00001c50: 6d65 7468 6f64 2068 656c 7073 2069 6e0d  method helps in.
-00001c60: 0a6f 7267 616e 697a 696e 6720 7468 6d65  .organizing thme
-00001c70: 2064 6f63 756d 656e 7420 696e 746f 206d   document into m
-00001c80: 616e 6167 6561 626c 6520 7365 6374 696f  anageable sectio
-00001c90: 6e73 2066 6f72 2066 7572 7468 6572 0d0a  ns for further..
-00001ca0: 7072 6f63 6573 7369 6e67 2e0d 0a0d 0a60  processing.....`
-00001cb0: 6060 2070 7974 686f 6e0d 0a66 726f 6d20  `` python..from 
-00001cc0: 496e 646f 782e 4461 7461 4c6f 6164 6572  Indox.DataLoader
-00001cd0: 5370 6c69 7474 6572 2069 6d70 6f72 7420  Splitter import 
-00001ce0: 556e 7374 7275 6374 7572 6564 4c6f 6164  UnstructuredLoad
-00001cf0: 416e 6453 706c 6974 0d0a 6060 600d 0a0d  AndSplit..```...
-00001d00: 0a60 6060 2070 7974 686f 6e0d 0a64 6f63  .``` python..doc
-00001d10: 735f 756e 7374 7275 6374 7572 6564 203d  s_unstructured =
-00001d20: 2055 6e73 7472 7563 7475 7265 644c 6f61   UnstructuredLoa
-00001d30: 6441 6e64 5370 6c69 7428 6669 6c65 5f70  dAndSplit(file_p
-00001d40: 6174 683d 6669 6c65 5f70 6174 6829 0d0a  ath=file_path)..
-00001d50: 6060 600d 0a0d 0a20 2020 2053 7461 7274  ```....    Start
-00001d60: 696e 6720 7072 6f63 6573 7369 6e67 2e2e  ing processing..
-00001d70: 2e0d 0a20 2020 2045 6e64 2043 6875 6e6b  ...    End Chunk
-00001d80: 696e 6720 7072 6f63 6573 732e 0d0a 0d0a  ing process.....
-00001d90: 5374 6f72 696e 6720 646f 6375 6d65 6e74  Storing document
-00001da0: 2063 6875 6e6b 7320 696e 2061 2076 6563   chunks in a vec
-00001db0: 746f 7220 7374 6f72 6520 6973 2063 7275  tor store is cru
-00001dc0: 6369 616c 2066 6f72 2065 6e61 626c 696e  cial for enablin
-00001dd0: 670d 0a65 6666 6963 6965 6e74 2072 6574  g..efficient ret
-00001de0: 7269 6576 616c 2061 6e64 2073 6561 7263  rieval and searc
-00001df0: 6820 6f70 6572 6174 696f 6e73 2e20 4279  h operations. By
-00001e00: 2063 6f6e 7665 7274 696e 6720 7465 7874   converting text
-00001e10: 2064 6174 6120 696e 746f 0d0a 7665 6374   data into..vect
-00001e20: 6f72 2072 6570 7265 7365 6e74 6174 696f  or representatio
-00001e30: 6e73 2061 6e64 2073 746f 7269 6e67 2074  ns and storing t
-00001e40: 6865 6d20 696e 2061 2076 6563 746f 7220  hem in a vector 
-00001e50: 7374 6f72 652c 2079 6f75 2063 616e 0d0a  store, you can..
-00001e60: 7065 7266 6f72 6d20 7261 7069 6420 7369  perform rapid si
-00001e70: 6d69 6c61 7269 7479 2073 6561 7263 6865  milarity searche
-00001e80: 7320 616e 6420 6f74 6865 7220 7665 6374  s and other vect
-00001e90: 6f72 2d62 6173 6564 206f 7065 7261 7469  or-based operati
-00001ea0: 6f6e 732e 0d0a 0d0a 6060 6020 7079 7468  ons.....``` pyth
-00001eb0: 6f6e 0d0a 496e 646f 782e 636f 6e6e 6563  on..Indox.connec
-00001ec0: 745f 746f 5f76 6563 746f 7273 746f 7265  t_to_vectorstore
-00001ed0: 2863 6f6c 6c65 6374 696f 6e5f 6e61 6d65  (collection_name
-00001ee0: 3d22 7361 6d70 6c65 222c 656d 6265 6464  ="sample",embedd
-00001ef0: 696e 6773 3d6f 7065 6e61 695f 656d 6265  ings=openai_embe
-00001f00: 6464 696e 6773 290d 0a49 6e64 6f78 2e73  ddings)..Indox.s
-00001f10: 746f 7265 5f69 6e5f 7665 6374 6f72 7374  tore_in_vectorst
-00001f20: 6f72 6528 6368 756e 6b73 3d64 6f63 735f  ore(chunks=docs_
-00001f30: 756e 7374 7275 6374 7572 6564 290d 0a60  unstructured)..`
-00001f40: 6060 0d0a 0d0a 2323 2051 7565 7269 6e67  ``....## Quering
-00001f50: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
-00001f60: 7175 6572 7920 3d20 2279 6f75 7220 7175  query = "your qu
-00001f70: 6572 7921 213f 3f22 0d0a 6060 600d 0a0d  ery!!??"..```...
-00001f80: 0a60 6060 2070 7974 686f 6e0d 0a72 6573  .``` python..res
-00001f90: 706f 6e73 655f 6f70 656e 6169 203d 2049  ponse_openai = I
-00001fa0: 6e64 6f78 2e61 6e73 7765 725f 7175 6573  ndox.answer_ques
-00001fb0: 7469 6f6e 2871 7565 7279 3d71 7565 7279  tion(query=query
-00001fc0: 2c71 615f 6d6f 6465 6c3d 6f70 656e 6169  ,qa_model=openai
-00001fd0: 5f71 6129 0d0a 6060 600d 0a0d 0a60 6060  _qa)..```....```
-00001fe0: 2070 7974 686f 6e0d 0a61 6e73 7765 7220   python..answer 
-00001ff0: 3d20 7265 7370 6f6e 7365 5f6f 7065 6e61  = response_opena
-00002000: 695b 305d 0d0a 6060 600d 0a0d 0a60 6060  i[0]..```....```
-00002010: 2070 7974 686f 6e0d 0a63 6f6e 7465 7874   python..context
-00002020: 2c20 7363 6f72 6520 3d20 7265 7370 6f6e  , score = respon
-00002030: 7365 5f6f 7065 6e61 695b 315d 0d0a 6060  se_openai[1]..``
-00002040: 600d 0a0d 0a                             `....
+00000540: 0a0d 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000550: 7465 7222 3e0d 0a0d 0a0d 0a3c 6833 2061  ter">......<h3 a
+00000560: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
+00000570: 2020 2020 3c69 6d67 2073 7263 3d22 646f      <img src="do
+00000580: 6373 2f6c 6974 652d 6c6f 676f 2031 2e70  cs/lite-logo 1.p
+00000590: 6e67 2220 616c 743d 224c 6f67 6f22 2073  ng" alt="Logo" s
+000005a0: 7479 6c65 3d22 7769 6474 683a 2038 3025  tyle="width: 80%
+000005b0: 3b20 6f70 6163 6974 793a 2030 2e37 3b22  ; opacity: 0.7;"
+000005c0: 2f3e 0d0a 0d0a 3c2f 6833 3e0d 0a0d 0a0d  />....</h3>.....
+000005d0: 0a3c 6469 7620 7374 796c 653d 2270 6f73  .<div style="pos
+000005e0: 6974 696f 6e3a 2072 656c 6174 6976 653b  ition: relative;
+000005f0: 2077 6964 7468 3a20 3130 3025 3b20 7465   width: 100%; te
+00000600: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00000610: 3b22 3e0d 0a3c 6831 3e0d 0a69 6e44 6f78  ;">..<h1>..inDox
+00000620: 200d 0a3c 7020 616c 6967 6e3d 2263 656e   ..<p align="cen
+00000630: 7465 7222 3e41 6476 616e 6365 6420 5365  ter">Advanced Se
+00000640: 6172 6368 2061 6e64 2052 6574 7269 6576  arch and Retriev
+00000650: 616c 2041 7567 6d65 6e74 6174 696f 6e20  al Augmentation 
+00000660: 4765 6e65 7261 7469 7665 0d0a 3c2f 703e  Generative..</p>
+00000670: 0d0a 0d0a 3c2f 6831 3e0d 0a0d 0a5b 215b  ....</h1>....[![
+00000680: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+00000690: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000006a0: 6769 7468 7562 2f6c 6963 656e 7365 2f6f  github/license/o
+000006b0: 736c 6c6d 6169 2f69 6e44 6f78 295d 2868  sllmai/inDox)](h
+000006c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006d0: 6d2f 6f73 6c6c 6d61 692f 696e 446f 782f  m/osllmai/inDox/
+000006e0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000006f0: 4529 0d0a 5b21 5b50 7950 495d 2868 7474  E)..[![PyPI](htt
+00000700: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+00000710: 696f 2f70 792f 496e 646f 782e 7376 6729  io/py/Indox.svg)
+00000720: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000730: 7267 2f70 726f 6a65 6374 2f49 6e64 6f78  rg/project/Indox
+00000740: 2f30 2e31 2e34 2f29 0d0a 5b21 5b50 7974  /0.1.4/)..[![Pyt
+00000750: 686f 6e5d 2868 7474 7073 3a2f 2f69 6d67  hon](https://img
+00000760: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000770: 2f70 7976 6572 7369 6f6e 732f 496e 646f  /pyversions/Indo
+00000780: 782e 7376 6729 5d28 6874 7470 733a 2f2f  x.svg)](https://
+00000790: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000007a0: 2f49 6e64 6f78 2f30 2e31 2e34 2f29 0d0a  /Indox/0.1.4/)..
+000007b0: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+000007c0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+000007d0: 792e 7465 6368 2f62 6164 6765 2f69 6e64  y.tech/badge/ind
+000007e0: 6f78 295d 2868 7474 7073 3a2f 2f70 6570  ox)](https://pep
+000007f0: 792e 7465 6368 2f70 726f 6a65 6374 2f69  y.tech/project/i
+00000800: 6e64 6f78 290d 0a0d 0a5b 215b 4469 7363  ndox)....[![Disc
+00000810: 6f72 645d 2868 7474 7073 3a2f 2f69 6d67  ord](https://img
+00000820: 2e73 6869 656c 6473 2e69 6f2f 6469 7363  .shields.io/disc
+00000830: 6f72 642f 3132 3233 3836 3733 3832 3436  ord/122386738246
+00000840: 3035 3739 3936 313f 6c61 6265 6c3d 4469  0579961?label=Di
+00000850: 7363 6f72 6426 6c6f 676f 3d44 6973 636f  scord&logo=Disco
+00000860: 7264 2673 7479 6c65 3d73 6f63 6961 6c29  rd&style=social)
+00000870: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+00000880: 642e 636f 6d2f 696e 7669 7465 2f6f 7373  d.com/invite/oss
+00000890: 6c6c 6d61 6929 0d0a 5b21 5b47 6974 4875  llmai)..[![GitHu
+000008a0: 6220 7374 6172 735d 2868 7474 7073 3a2f  b stars](https:/
+000008b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000008c0: 6769 7468 7562 2f73 7461 7273 2f6f 736c  github/stars/osl
+000008d0: 6c6d 6169 2f69 6e44 6f78 3f73 7479 6c65  lmai/inDox?style
+000008e0: 3d73 6f63 6961 6c29 5d28 6874 7470 733a  =social)](https:
+000008f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
+00000900: 6c6d 6169 2f69 6e44 6f78 290d 0a0d 0a0d  lmai/inDox).....
+00000910: 0a0d 0a0d 0a3c 7020 616c 6967 6e3d 2263  .....<p align="c
+00000920: 656e 7465 7222 3e0d 0a20 203c 6120 6872  enter">..  <a hr
+00000930: 6566 3d22 6874 7470 733a 2f2f 6f73 6c6c  ef="https://osll
+00000940: 6d2e 6169 223e 4f66 6669 6369 616c 2057  m.ai">Official W
+00000950: 6562 7369 7465 3c2f 613e 2026 6275 6c6c  ebsite</a> &bull
+00000960: 3b20 3c61 2068 7265 663d 2268 7474 7073  ; <a href="https
+00000970: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f73  ://github.com/os
+00000980: 6c6c 6d61 692f 696e 446f 782f 7769 6b69  llmai/inDox/wiki
+00000990: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+000009a0: 2f61 3e20 2662 756c 6c3b 203c 6120 6872  /a> &bull; <a hr
+000009b0: 6566 3d22 6874 7470 733a 2f2f 6469 7363  ef="https://disc
+000009c0: 6f72 642e 6767 2f71 7243 6335 365a 5222  ord.gg/qrCc56ZR"
+000009d0: 3e44 6973 636f 7264 3c2f 613e 0d0a 3c2f  >Discord</a>..</
+000009e0: 703e 0d0a 0d0a 0d0a 3c70 2061 6c69 676e  p>......<p align
+000009f0: 3d22 6365 6e74 6572 223e 0d0a 2020 3c62  ="center">..  <b
+00000a00: 3e4e 4557 3a3c 2f62 3e20 3c61 2068 7265  >NEW:</b> <a hre
+00000a10: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00000a20: 676f 6f67 6c65 2e63 6f6d 2f66 6f72 6d73  google.com/forms
+00000a30: 2f64 2f31 4351 584a 7678 4c55 714c 4253  /d/1CQXJvxLUqLBS
+00000a40: 586e 6a71 516d 5270 4f79 5a71 4436 6e72  XnjqQmRpOyZqD6nr
+00000a50: 4b75 624c 7a32 5754 6349 4a33 3766 552f  KubLz2WTcIJ37fU/
+00000a60: 7072 6566 696c 6c22 3e53 7562 7363 7269  prefill">Subscri
+00000a70: 6265 2074 6f20 6f75 7220 6d61 696c 696e  be to our mailin
+00000a80: 6720 6c69 7374 3c2f 613e 2066 6f72 2075  g list</a> for u
+00000a90: 7064 6174 6573 2061 6e64 206e 6577 7321  pdates and news!
+00000aa0: 0d0a 3c2f 703e 0d0a 0d0a 0d0a 0d0a 2a2a  ..</p>........**
+00000ab0: 496e 646f 7820 5265 7472 6965 7661 6c20  Indox Retrieval 
+00000ac0: 4175 676d 656e 7461 7469 6f6e 2a2a 2069  Augmentation** i
+00000ad0: 7320 616e 2069 6e6e 6f76 6174 6976 6520  s an innovative 
+00000ae0: 6170 706c 6963 6174 696f 6e20 6465 7369  application desi
+00000af0: 676e 6564 2074 6f20 7374 7265 616d 6c69  gned to streamli
+00000b00: 6e65 2069 6e66 6f72 6d61 7469 6f6e 2065  ne information e
+00000b10: 7874 7261 6374 696f 6e20 6672 6f6d 2061  xtraction from a
+00000b20: 2077 6964 650d 0a72 616e 6765 206f 6620   wide..range of 
+00000b30: 646f 6375 6d65 6e74 2074 7970 6573 2c20  document types, 
+00000b40: 696e 636c 7564 696e 6720 7465 7874 2066  including text f
+00000b50: 696c 6573 2c20 5044 462c 2048 544d 4c2c  iles, PDF, HTML,
+00000b60: 204d 6172 6b64 6f77 6e2c 2061 6e64 204c   Markdown, and L
+00000b70: 6154 6558 2e20 5768 6574 6865 7220 7374  aTeX. Whether st
+00000b80: 7275 6374 7572 6564 206f 7220 756e 7374  ructured or unst
+00000b90: 7275 6374 7572 6564 2c20 496e 646f 780d  ructured, Indox.
+00000ba0: 0a70 726f 7669 6465 7320 7573 6572 7320  .provides users 
+00000bb0: 7769 7468 2061 2070 6f77 6572 6675 6c20  with a powerful 
+00000bc0: 746f 6f6c 7365 7420 746f 2065 6666 6963  toolset to effic
+00000bd0: 6965 6e74 6c79 2065 7874 7261 6374 2072  iently extract r
+00000be0: 656c 6576 616e 7420 6461 7461 2e0d 0a0d  elevant data....
+00000bf0: 0a49 6e64 6f78 2052 6574 7269 6576 616c  .Indox Retrieval
+00000c00: 2041 7567 6d65 6e74 6174 696f 6e20 6973   Augmentation is
+00000c10: 2061 6e20 696e 6e6f 7661 7469 7665 2061   an innovative a
+00000c20: 7070 6c69 6361 7469 6f6e 2064 6573 6967  pplication desig
+00000c30: 6e65 6420 746f 2073 7472 6561 6d6c 696e  ned to streamlin
+00000c40: 6520 696e 666f 726d 6174 696f 6e20 6578  e information ex
+00000c50: 7472 6163 7469 6f6e 2066 726f 6d20 6120  traction from a 
+00000c60: 7769 6465 0d0a 7261 6e67 6520 6f66 2064  wide..range of d
+00000c70: 6f63 756d 656e 7420 7479 7065 732c 2069  ocument types, i
+00000c80: 6e63 6c75 6469 6e67 2074 6578 7420 6669  ncluding text fi
+00000c90: 6c65 732c 2050 4446 2c20 4854 4d4c 2c20  les, PDF, HTML, 
+00000ca0: 4d61 726b 646f 776e 2c20 616e 6420 4c61  Markdown, and La
+00000cb0: 5465 582e 2057 6865 7468 6572 2073 7472  TeX. Whether str
+00000cc0: 7563 7475 7265 6420 6f72 2075 6e73 7472  uctured or unstr
+00000cd0: 7563 7475 7265 642c 2049 6e64 6f78 0d0a  uctured, Indox..
+00000ce0: 7072 6f76 6964 6573 2075 7365 7273 2077  provides users w
+00000cf0: 6974 6820 6120 706f 7765 7266 756c 2074  ith a powerful t
+00000d00: 6f6f 6c73 6574 2074 6f20 6566 6669 6369  oolset to effici
+00000d10: 656e 746c 7920 6578 7472 6163 7420 7265  ently extract re
+00000d20: 6c65 7661 6e74 2064 6174 612e 204f 6e65  levant data. One
+00000d30: 206f 6620 6974 7320 6b65 7920 6665 6174   of its key feat
+00000d40: 7572 6573 2069 7320 7468 6520 6162 696c  ures is the abil
+00000d50: 6974 7920 746f 0d0a 696e 7465 6c6c 6967  ity to..intellig
+00000d60: 656e 746c 7920 636c 7573 7465 7220 7072  ently cluster pr
+00000d70: 696d 6172 7920 6368 756e 6b73 2074 6f20  imary chunks to 
+00000d80: 666f 726d 206d 6f72 6520 726f 6275 7374  form more robust
+00000d90: 2067 726f 7570 696e 6773 2c20 656e 6861   groupings, enha
+00000da0: 6e63 696e 6720 7468 6520 7175 616c 6974  ncing the qualit
+00000db0: 7920 616e 6420 7265 6c65 7661 6e63 6520  y and relevance 
+00000dc0: 6f66 2074 6865 2065 7874 7261 6374 6564  of the extracted
+00000dd0: 0d0a 696e 666f 726d 6174 696f 6e2e 0d0a  ..information...
+00000de0: 5769 7468 2061 2066 6f63 7573 206f 6e20  With a focus on 
+00000df0: 6164 6170 7461 6269 6c69 7479 2061 6e64  adaptability and
+00000e00: 2075 7365 722d 6365 6e74 7269 6320 6465   user-centric de
+00000e10: 7369 676e 2c20 496e 646f 7820 6169 6d73  sign, Indox aims
+00000e20: 2074 6f20 6465 6c69 7665 7220 6675 7475   to deliver futu
+00000e30: 7265 2d72 6561 6479 2066 756e 6374 696f  re-ready functio
+00000e40: 6e61 6c69 7479 2077 6974 6820 6d6f 7265  nality with more
+00000e50: 0d0a 6665 6174 7572 6573 2070 6c61 6e6e  ..features plann
+00000e60: 6564 2066 6f72 2075 7063 6f6d 696e 6720  ed for upcoming 
+00000e70: 7265 6c65 6173 6573 2e20 4a6f 696e 2075  releases. Join u
+00000e80: 7320 696e 2065 7870 6c6f 7269 6e67 2068  s in exploring h
+00000e90: 6f77 2049 6e64 6f78 2063 616e 2072 6576  ow Indox can rev
+00000ea0: 6f6c 7574 696f 6e69 7a65 2079 6f75 7220  olutionize your 
+00000eb0: 646f 6375 6d65 6e74 2070 726f 6365 7373  document process
+00000ec0: 696e 670d 0a77 6f72 6b66 6c6f 772c 2062  ing..workflow, b
+00000ed0: 7269 6e67 696e 6720 636c 6172 6974 7920  ringing clarity 
+00000ee0: 616e 6420 6f72 6761 6e69 7a61 7469 6f6e  and organization
+00000ef0: 2074 6f20 796f 7572 2064 6174 6120 7265   to your data re
+00000f00: 7472 6965 7661 6c20 6e65 6564 732e 0d0a  trieval needs...
+00000f10: 0d0a 2323 2044 6570 656e 6465 6e63 7920  ..## Dependency 
+00000f20: 5265 7175 6972 656d 656e 7473 0d0a 0d0a  Requirements....
+00000f30: 4265 666f 7265 2072 756e 6e69 6e67 2074  Before running t
+00000f40: 6869 7320 7072 6f6a 6563 742c 2065 6e73  his project, ens
+00000f50: 7572 6520 7468 6174 2079 6f75 2068 6176  ure that you hav
+00000f60: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00000f70: 696e 7374 616c 6c65 643a 0d0a 0d0a 2d20  installed:....- 
+00000f80: 2a2a 5079 7468 6f6e 2033 2e38 2b2a 2a3a  **Python 3.8+**:
+00000f90: 2052 6571 7569 7265 6420 666f 7220 7275   Required for ru
+00000fa0: 6e6e 696e 6720 7468 6520 5079 7468 6f6e  nning the Python
+00000fb0: 2062 6163 6b65 6e64 2e0d 0a2d 202a 2a50   backend...- **P
+00000fc0: 6f73 7467 7265 5351 4c2a 2a3a 204e 6565  ostgreSQL**: Nee
+00000fd0: 6465 6420 6966 2079 6f75 2077 6973 6820  ded if you wish 
+00000fe0: 746f 2073 746f 7265 2079 6f75 7220 6461  to store your da
+00000ff0: 7461 2069 6e20 6120 506f 7374 6772 6553  ta in a PostgreS
+00001000: 514c 2064 6174 6162 6173 652e 0d0a 2d20  QL database...- 
+00001010: 2a2a 4f70 656e 4149 2041 5049 204b 6579  **OpenAI API Key
+00001020: 2a2a 3a20 4e65 6365 7373 6172 7920 6966  **: Necessary if
+00001030: 2079 6f75 2061 7265 2075 7369 6e67 2074   you are using t
+00001040: 6865 204f 7065 6e41 4920 656d 6265 6464  he OpenAI embedd
+00001050: 696e 6720 6d6f 6465 6c2e 0d0a 2d20 2a2a  ing model...- **
+00001060: 4875 6767 696e 6746 6163 6520 4150 4920  HuggingFace API 
+00001070: 4b65 792a 2a3a 204e 6563 6573 7361 7279  Key**: Necessary
+00001080: 2069 6620 796f 7520 6172 6520 7573 696e   if you are usin
+00001090: 6720 7468 6520 4875 6767 696e 6746 6163  g the HuggingFac
+000010a0: 6520 6c6c 6d73 2e0d 0a0d 0a45 6e73 7572  e llms.....Ensur
+000010b0: 6520 796f 7572 2073 7973 7465 6d20 616c  e your system al
+000010c0: 736f 206d 6565 7473 2074 6865 7365 2072  so meets these r
+000010d0: 6571 7569 7265 6d65 6e74 733a 0d0a 0d0a  equirements:....
+000010e0: 2d20 4163 6365 7373 2074 6f20 656e 7669  - Access to envi
+000010f0: 726f 6e6d 656e 7461 6c20 7661 7269 6162  ronmental variab
+00001100: 6c65 7320 666f 7220 6861 6e64 6c69 6e67  les for handling
+00001110: 2073 656e 7369 7469 7665 2069 6e66 6f72   sensitive infor
+00001120: 6d61 7469 6f6e 206c 696b 6520 4150 4920  mation like API 
+00001130: 6b65 7973 2e0d 0a2d 2053 7569 7461 626c  keys...- Suitabl
+00001140: 6520 6861 7264 7761 7265 2063 6170 6162  e hardware capab
+00001150: 6c65 206f 6620 7375 7070 6f72 7469 6e67  le of supporting
+00001160: 2069 6e74 656e 7369 7665 2063 6f6d 7075   intensive compu
+00001170: 7461 7469 6f6e 616c 2074 6173 6b73 2e0d  tational tasks..
+00001180: 0a0d 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00001190: 6f6e 0d0a 0d0a 0d0a 2323 2047 6574 7469  on......## Getti
+000011a0: 6e67 2053 7461 7274 6564 0d0a 0d0a 5468  ng Started....Th
+000011b0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+000011c0: 616e 6420 7769 6c6c 2069 6e73 7461 6c6c  and will install
+000011d0: 2074 6865 206c 6174 6573 7420 7374 6162   the latest stab
+000011e0: 6c65 2069 6e44 6f78 0d0a 0d0a 6060 600d  le inDox....```.
+000011f0: 0a70 6970 2069 6e73 7461 6c6c 2049 6e64  .pip install Ind
+00001200: 6f78 0d0a 6060 600d 0a0d 0a54 6f20 696e  ox..```....To in
+00001210: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
+00001220: 2064 6576 656c 6f70 6d65 6e74 2076 6572   development ver
+00001230: 7369 6f6e 2c20 796f 7520 6d61 7920 7275  sion, you may ru
+00001240: 6e0d 0a0d 0a60 6060 0d0a 7069 7020 696e  n....```..pip in
+00001250: 7374 616c 6c20 6769 742b 6874 7470 733a  stall git+https:
+00001260: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
+00001270: 6c6d 6169 2f69 6e44 6f78 406d 6169 6e0d  lmai/inDox@main.
+00001280: 0a60 6060 0d0a 0d0a 546f 2063 6f6e 6669  .```....To confi
+00001290: 6775 7265 2074 6865 2043 4c49 2c20 7275  gure the CLI, ru
+000012a0: 6e0d 0a0d 0a60 6060 0d0a 696e 646f 7820  n....```..indox 
+000012b0: 636f 6e66 6967 7572 650d 0a60 6060 0d0a  configure..```..
+000012c0: 0d0a 0d0a 436c 6f6e 6520 7468 6520 7265  ....Clone the re
+000012d0: 706f 7369 746f 7279 2061 6e64 206e 6176  pository and nav
+000012e0: 6967 6174 6520 746f 2074 6865 2064 6972  igate to the dir
+000012f0: 6563 746f 7279 3a0d 0a0d 0a60 6060 6261  ectory:....```ba
+00001300: 7368 0d0a 6769 7420 636c 6f6e 6520 6874  sh..git clone ht
+00001310: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001320: 2f6f 736c 6c6d 6169 2f69 6e44 6f78 2e67  /osllmai/inDox.g
+00001330: 6974 0d0a 6364 2069 6e44 6f78 0d0a 6060  it..cd inDox..``
+00001340: 600d 0a0d 0a49 6e73 7461 6c6c 2074 6865  `....Install the
+00001350: 2072 6571 7569 7265 6420 5079 7468 6f6e   required Python
+00001360: 2070 6163 6b61 6765 733a 0d0a 0d0a 6060   packages:....``
+00001370: 6062 6173 680d 0a70 6970 2069 6e73 7461  `bash..pip insta
+00001380: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
+00001390: 7473 2e74 7874 0d0a 6060 600d 0a0d 0a23  ts.txt..```....#
+000013a0: 2320 436f 6e66 6967 7572 6174 696f 6e0d  # Configuration.
+000013b0: 0a0d 0a23 2323 2045 6e76 6972 6f6e 6d65  ...### Environme
+000013c0: 6e74 2056 6172 6961 626c 6573 0d0a 0d0a  nt Variables....
+000013d0: 5365 7420 796f 7572 2060 4f50 454e 4149  Set your `OPENAI
+000013e0: 5f41 5049 5f4b 4559 6020 6f72 2060 4846  _API_KEY` or `HF
+000013f0: 5f41 5049 5f4b 4559 6020 696e 2079 6f75  _API_KEY` in you
+00001400: 7220 656e 7669 726f 6e6d 656e 7420 7661  r environment va
+00001410: 7269 6162 6c65 7320 666f 7220 7365 6375  riables for secu
+00001420: 7265 2061 6363 6573 732e 0d0a 0d0a 2323  re access.....##
+00001430: 2320 4461 7461 6261 7365 2053 6574 7570  # Database Setup
+00001440: 0d0a 0d0a 456e 7375 7265 2079 6f75 7220  ....Ensure your 
+00001450: 506f 7374 6772 6553 514c 2064 6174 6162  PostgreSQL datab
+00001460: 6173 6520 6973 2075 7020 616e 6420 7275  ase is up and ru
+00001470: 6e6e 696e 672c 2061 6e64 2061 6363 6573  nning, and acces
+00001480: 7369 626c 6520 6672 6f6d 2079 6f75 7220  sible from your 
+00001490: 6170 706c 6963 6174 696f 6e2e 2054 6869  application. Thi
+000014a0: 7320 6973 206e 6563 6573 7361 7279 2069  s is necessary i
+000014b0: 6620 796f 7520 706c 616e 2074 6f20 7573  f you plan to us
+000014c0: 6520 7067 7665 6374 6f72 2061 7320 796f  e pgvector as yo
+000014d0: 7572 2076 6563 746f 7220 7374 6f72 652e  ur vector store.
+000014e0: 0d0a 0d0a 416c 7465 726e 6174 6976 656c  ....Alternativel
+000014f0: 792c 2079 6f75 2063 616e 2075 7365 2043  y, you can use C
+00001500: 6872 6f6d 6120 6f72 2046 6169 7373 2061  hroma or Faiss a
+00001510: 7320 796f 7572 2076 6563 746f 7220 7374  s your vector st
+00001520: 6f72 652e 204d 616b 6520 7375 7265 2074  ore. Make sure t
+00001530: 6f20 7370 6563 6966 7920 796f 7572 2063  o specify your c
+00001540: 686f 6963 6520 616e 6420 7468 6520 6e65  hoice and the ne
+00001550: 6365 7373 6172 7920 636f 6e66 6967 7572  cessary configur
+00001560: 6174 696f 6e73 2069 6e20 7468 6520 636f  ations in the co
+00001570: 6e66 6967 2e79 616d 6c20 6669 6c65 2e0d  nfig.yaml file..
+00001580: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a23  ...## Usage....#
+00001590: 2323 2050 7265 7061 7269 6e67 2059 6f75  ## Preparing You
+000015a0: 7220 4461 7461 0d0a 0d0a 312e 202a 2a44  r Data....1. **D
+000015b0: 6566 696e 6520 7468 6520 4669 6c65 2050  efine the File P
+000015c0: 6174 682a 2a3a 2053 7065 6369 6679 2074  ath**: Specify t
+000015d0: 6865 2070 6174 6820 746f 2079 6f75 7220  he path to your 
+000015e0: 7465 7874 206f 7220 5044 4620 6669 6c65  text or PDF file
+000015f0: 2e0d 0a32 2e20 2a2a 4c6f 6164 2045 6d62  ...2. **Load Emb
+00001600: 6564 6469 6e67 204d 6f64 656c 732a 2a3a  edding Models**:
+00001610: 2049 6e69 7469 616c 697a 6520 796f 7572   Initialize your
+00001620: 2065 6d62 6564 6469 6e67 206d 6f64 656c   embedding model
+00001630: 2066 726f 6d20 4f70 656e 4149 2773 2073   from OpenAI's s
+00001640: 656c 6563 7469 6f6e 206f 6620 7072 652d  election of pre-
+00001650: 7472 6169 6e65 6420 6d6f 6465 6c73 2e0d  trained models..
+00001660: 0a0d 0a23 2051 7569 636b 2053 7461 7274  ...# Quick Start
+00001670: 200d 0a0d 0a23 2320 496d 706f 7274 2049   ....## Import I
+00001680: 6e64 6f78 2050 6163 6b61 6765 0d0a 0d0a  ndox Package....
+00001690: 496d 706f 7274 2074 6865 206e 6563 6573  Import the neces
+000016a0: 7361 7279 2063 6c61 7373 6573 2066 726f  sary classes fro
+000016b0: 6d20 7468 6520 496e 646f 7820 7061 636b  m the Indox pack
+000016c0: 6167 652e 0d0a 0d0a 6060 6020 7079 7468  age.....``` pyth
+000016d0: 6f6e 0d0a 6672 6f6d 2049 6e64 6f78 2069  on..from Indox i
+000016e0: 6d70 6f72 7420 496e 646f 7852 6574 7269  mport IndoxRetri
+000016f0: 6576 616c 4175 676d 656e 7461 7469 6f6e  evalAugmentation
+00001700: 0d0a 6060 600d 0a0d 0a23 2323 2049 6e69  ..```....### Ini
+00001710: 7469 616c 697a 6520 496e 646f 780d 0a0d  tialize Indox...
+00001720: 0a43 7265 6174 6520 616e 2069 6e73 7461  .Create an insta
+00001730: 6e63 6520 6f66 2049 6e64 6f78 5265 7472  nce of IndoxRetr
+00001740: 6965 7661 6c41 7567 6d65 6e74 6174 696f  ievalAugmentatio
+00001750: 6e2e 0d0a 0d0a 6060 6020 7079 7468 6f6e  n.....``` python
+00001760: 0d0a 496e 646f 7820 3d20 496e 646f 7852  ..Indox = IndoxR
+00001770: 6574 7269 6576 616c 4175 676d 656e 7461  etrievalAugmenta
+00001780: 7469 6f6e 2829 0d0a 6060 600d 0a23 2320  tion()..```..## 
+00001790: 496e 6974 6961 6c20 436f 6e66 6967 7572  Initial Configur
+000017a0: 6174 696f 6e0d 0a0d 0a2d 202a 2a43 6f6e  ation....- **Con
+000017b0: 6669 6775 7261 7469 6f6e 2046 696c 652a  figuration File*
+000017c0: 2a3a 2045 6e73 7572 6520 796f 7520 6c6f  *: Ensure you lo
+000017d0: 6361 7465 2061 6e64 206d 6f64 6966 7920  cate and modify 
+000017e0: 7468 6520 6049 6e64 6f78 2e63 6f6e 6669  the `Indox.confi
+000017f0: 6760 2059 414d 4c20 6669 6c65 2061 6363  g` YAML file acc
+00001800: 6f72 6469 6e67 2074 6f20 796f 7572 206e  ording to your n
+00001810: 6565 6473 2062 6566 6f72 650d 0a20 2073  eeds before..  s
+00001820: 7461 7274 696e 6720 7468 6520 6170 706c  tarting the appl
+00001830: 6963 6174 696f 6e2e 0d0a 0d0a 2323 2044  ication.....## D
+00001840: 796e 616d 6963 2043 6f6e 6669 6775 7261  ynamic Configura
+00001850: 7469 6f6e 2043 6861 6e67 6573 0d0a 0d0a  tion Changes....
+00001860: 466f 7220 6368 616e 6765 7320 7468 6174  For changes that
+00001870: 206e 6565 6420 746f 2062 6520 6170 706c   need to be appl
+00001880: 6965 6420 6166 7465 7220 7468 6520 696e  ied after the in
+00001890: 6974 6961 6c20 7365 7475 7020 6f72 2064  itial setup or d
+000018a0: 7572 696e 6720 7275 6e74 696d 653a 0d0a  uring runtime:..
+000018b0: 0d0a 2d20 2a2a 4d6f 6469 6679 696e 6720  ..- **Modifying 
+000018c0: 436f 6e66 6967 7572 6174 696f 6e73 2a2a  Configurations**
+000018d0: 3a20 5573 6520 7468 6520 666f 6c6c 6f77  : Use the follow
+000018e0: 696e 6720 5079 7468 6f6e 2073 6e69 7070  ing Python snipp
+000018f0: 6574 2074 6f20 7570 6461 7465 2079 6f75  et to update you
+00001900: 7220 7365 7474 696e 6773 2064 796e 616d  r settings dynam
+00001910: 6963 616c 6c79 3a0d 0a20 2060 6060 7079  ically:..  ```py
+00001920: 7468 6f6e 0d0a 2020 496e 646f 782e 636f  thon..  Indox.co
+00001930: 6e66 6967 5b22 796f 7572 5f73 6574 7469  nfig["your_setti
+00001940: 6e67 5f74 6861 745f 6e65 6564 5f74 6f5f  ng_that_need_to_
+00001950: 6368 616e 6765 225d 203d 2022 6e65 775f  change"] = "new_
+00001960: 7365 7474 696e 6722 0d0a 2020 496e 646f  setting"..  Indo
+00001970: 782e 7570 6461 7465 5f63 6f6e 6669 6728  x.update_config(
+00001980: 290d 0a0d 0a23 2320 436f 6e66 6967 7572  )....## Configur
+00001990: 6174 696f 6e20 4465 7461 696c 730d 0a0d  ation Details...
+000019a0: 0a48 6572 6527 7320 6120 6272 6561 6b64  .Here's a breakd
+000019b0: 6f77 6e20 6f66 2074 6865 2063 6f6e 6669  own of the confi
+000019c0: 6720 6469 6374 696f 6e61 7279 2061 6e64  g dictionary and
+000019d0: 2069 7473 2070 726f 7065 7274 6965 733a   its properties:
+000019e0: 0d0a 0d0a 2323 2320 506f 7374 6772 6553  ....### PostgreS
+000019f0: 514c 0d0a 0d0a 2d20 6063 6f6e 6e5f 7374  QL....- `conn_st
+00001a00: 7269 6e67 603a 2059 6f75 7220 506f 7374  ring`: Your Post
+00001a10: 6772 6553 514c 2064 6174 6162 6173 6520  greSQL database 
+00001a20: 6372 6564 656e 7469 616c 732e 0d0a 0d0a  credentials.....
+00001a30: 2323 2320 5375 6d6d 6172 7920 4d6f 6465  ### Summary Mode
+00001a40: 6c0d 0a0d 0a2d 2060 6d61 785f 746f 6b65  l....- `max_toke
+00001a50: 6e73 603a 204d 6178 696d 756d 2074 6f6b  ns`: Maximum tok
+00001a60: 656e 2063 6f75 6e74 2074 6865 2073 756d  en count the sum
+00001a70: 6d61 7279 206d 6f64 656c 2063 616e 2067  mary model can g
+00001a80: 656e 6572 6174 652e 0d0a 2d20 606d 696e  enerate...- `min
+00001a90: 5f6c 656e 603a 204d 696e 696d 756d 2074  _len`: Minimum t
+00001aa0: 6f6b 656e 2063 6f75 6e74 2074 6865 2073  oken count the s
+00001ab0: 756d 6d61 7279 206d 6f64 656c 2067 656e  ummary model gen
+00001ac0: 6572 6174 6573 2e0d 0a2d 2060 6d6f 6465  erates...- `mode
+00001ad0: 6c5f 6e61 6d65 603a 2044 6566 6175 6c74  l_name`: Default
+00001ae0: 2069 7320 6067 7074 2d33 2e35 2d74 7572   is `gpt-3.5-tur
+00001af0: 626f 2d30 3132 3560 2c20 6275 7420 6974  bo-0125`, but it
+00001b00: 2063 616e 2062 6520 7265 706c 6163 6564   can be replaced
+00001b10: 2077 6974 6820 616e 7920 4875 6767 696e   with any Huggin
+00001b20: 6720 4661 6365 206d 6f64 656c 2073 7570  g Face model sup
+00001b30: 706f 7274 696e 6720 7468 650d 0a20 2073  porting the..  s
+00001b40: 756d 6d61 7269 7a61 7469 6f6e 2070 6970  ummarization pip
+00001b50: 656c 696e 652e 0d0a 0d0a 2323 2320 506f  eline.....### Po
+00001b60: 7374 6772 6553 514c 2053 6574 7570 2077  stgreSQL Setup w
+00001b70: 6974 6820 7067 7665 6374 6f72 0d0a 0d0a  ith pgvector....
+00001b80: 4966 2079 6f75 2077 616e 7420 746f 2075  If you want to u
+00001b90: 7365 2050 6f73 7467 7265 5351 4c20 666f  se PostgreSQL fo
+00001ba0: 7220 7665 6374 6f72 2073 746f 7261 6765  r vector storage
+00001bb0: 2c20 796f 7520 7368 6f75 6c64 2070 6572  , you should per
+00001bc0: 666f 726d 2074 6865 2066 6f6c 6c6f 7769  form the followi
+00001bd0: 6e67 2073 7465 7073 3a0d 0a0d 0a31 2e20  ng steps:....1. 
+00001be0: 2a2a 496e 7374 616c 6c20 7067 7665 6374  **Install pgvect
+00001bf0: 6f72 2a2a 3a20 546f 2069 6e73 7461 6c6c  or**: To install
+00001c00: 2060 7067 7665 6374 6f72 6020 6f6e 2079   `pgvector` on y
+00001c10: 6f75 7220 506f 7374 6772 6553 514c 2073  our PostgreSQL s
+00001c20: 6572 7665 722c 2066 6f6c 6c6f 7720 7468  erver, follow th
+00001c30: 6520 6465 7461 696c 6564 2069 6e73 7461  e detailed insta
+00001c40: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
+00001c50: 696f 6e73 0d0a 2020 2061 7661 696c 6162  ions..   availab
+00001c60: 6c65 206f 6e20 7468 6520 6f66 6669 6369  le on the offici
+00001c70: 616c 2070 6776 6563 746f 7220 4769 7448  al pgvector GitH
+00001c80: 7562 2072 6570 6f73 6974 6f72 793a 0d0a  ub repository:..
+00001c90: 2020 205b 7067 7665 6374 6f72 2049 6e73     [pgvector Ins
+00001ca0: 7461 6c6c 6174 696f 6e20 496e 7374 7275  tallation Instru
+00001cb0: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
+00001cc0: 6769 7468 7562 2e63 6f6d 2f70 6776 6563  github.com/pgvec
+00001cd0: 746f 722f 7067 7665 6374 6f72 290d 0a0d  tor/pgvector)...
+00001ce0: 0a32 2e20 2a2a 4164 6420 5665 6374 6f72  .2. **Add Vector
+00001cf0: 2045 7874 656e 7369 6f6e 2a2a 3a0d 0a20   Extension**:.. 
+00001d00: 2020 436f 6e6e 6563 7420 746f 2079 6f75    Connect to you
+00001d10: 7220 506f 7374 6772 6553 514c 2064 6174  r PostgreSQL dat
+00001d20: 6162 6173 6520 616e 6420 6578 6563 7574  abase and execut
+00001d30: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001d40: 5351 4c20 636f 6d6d 616e 6420 746f 2063  SQL command to c
+00001d50: 7265 6174 6520 7468 6520 6070 6776 6563  reate the `pgvec
+00001d60: 746f 7260 2065 7874 656e 7369 6f6e 3a0d  tor` extension:.
+00001d70: 0a0d 0a20 2020 6060 6073 716c 0d0a 2020  ...   ```sql..  
+00001d80: 202d 2d20 436f 6e6e 6563 7420 746f 2079   -- Connect to y
+00001d90: 6f75 7220 6461 7461 6261 7365 0d0a 2020  our database..  
+00001da0: 2070 7371 6c20 2d55 2075 7365 726e 616d   psql -U usernam
+00001db0: 6520 2d64 2064 6174 6162 6173 655f 6e61  e -d database_na
+00001dc0: 6d65 0d0a 0d0a 2020 202d 2d20 5275 6e20  me....   -- Run 
+00001dd0: 696e 7369 6465 2079 6f75 7220 7073 716c  inside your psql
+00001de0: 2074 6572 6d69 6e61 6c0d 0a20 2020 4352   terminal..   CR
+00001df0: 4541 5445 2045 5854 454e 5349 4f4e 2076  EATE EXTENSION v
+00001e00: 6563 746f 723b 0d0a 2020 2023 2052 6570  ector;..   # Rep
+00001e10: 6c61 6365 2074 6865 2070 6c61 6365 686f  lace the placeho
+00001e20: 6c64 6572 7320 7769 7468 2079 6f75 7220  lders with your 
+00001e30: 6163 7475 616c 2050 6f73 7467 7265 5351  actual PostgreSQ
+00001e40: 4c20 6372 6564 656e 7469 616c 7320 616e  L credentials an
+00001e50: 6420 6465 7461 696c 730d 0a0d 0a41 6464  d details....Add
+00001e60: 6974 696f 6e61 6c6c 792c 2066 6f72 2074  itionally, for t
+00001e70: 686f 7365 2069 6e74 6572 6573 7465 6420  hose interested 
+00001e80: 696e 2065 7870 6c6f 7269 6e67 206f 7468  in exploring oth
+00001e90: 6572 2076 6563 746f 7220 6461 7461 6261  er vector databa
+00001ea0: 7365 206f 7074 696f 6e73 2c20 796f 7520  se options, you 
+00001eb0: 6361 6e20 636f 6e73 6964 6572 2075 7369  can consider usi
+00001ec0: 6e67 202a 2a43 6872 6f6d 612a 2a20 6f72  ng **Chroma** or
+00001ed0: 202a 0d0a 2a46 6169 7373 2a2a 2e20 5468   *..*Faiss**. Th
+00001ee0: 6573 6520 7072 6f76 6964 6520 616c 7465  ese provide alte
+00001ef0: 726e 6174 6976 6520 6170 7072 6f61 6368  rnative approach
+00001f00: 6573 2074 6f20 7665 6374 6f72 2073 746f  es to vector sto
+00001f10: 7261 6765 2061 6e64 2072 6574 7269 6576  rage and retriev
+00001f20: 616c 2074 6861 7420 6d61 7920 6265 7474  al that may bett
+00001f30: 6572 2073 7569 7420 7370 6563 6966 6963  er suit specific
+00001f40: 2075 7365 2063 6173 6573 0d0a 6f72 2070   use cases..or p
+00001f50: 6572 666f 726d 616e 6365 2072 6571 7569  erformance requi
+00001f60: 7265 6d65 6e74 732e 0d0a 0d0a 2323 2320  rements.....### 
+00001f70: 496d 706f 7274 696e 6720 5141 2061 6e64  Importing QA and
+00001f80: 2045 6d62 6564 6469 6e67 204d 6f64 656c   Embedding Model
+00001f90: 730d 0a0d 0a60 6060 2070 7974 686f 6e0d  s....``` python.
+00001fa0: 0a66 726f 6d20 496e 646f 782e 5161 4d6f  .from Indox.QaMo
+00001fb0: 6465 6c73 2069 6d70 6f72 7420 4f70 656e  dels import Open
+00001fc0: 4169 5141 0d0a 6060 600d 0a0d 0a60 6060  AiQA..```....```
+00001fd0: 2070 7974 686f 6e0d 0a66 726f 6d20 496e   python..from In
+00001fe0: 646f 782e 456d 6265 6464 696e 6773 2069  dox.Embeddings i
+00001ff0: 6d70 6f72 7420 4f70 656e 4169 456d 6265  mport OpenAiEmbe
+00002000: 6464 696e 670d 0a60 6060 0d0a 0d0a 0d0a  dding..```......
+00002010: 6060 6020 7079 7468 6f6e 0d0a 6f70 656e  ``` python..open
+00002020: 6169 5f71 6120 3d20 4f70 656e 4169 5141  ai_qa = OpenAiQA
+00002030: 2861 7069 5f6b 6579 3d4f 5045 4e41 495f  (api_key=OPENAI_
+00002040: 4150 495f 4b45 592c 6d6f 6465 6c3d 2267  API_KEY,model="g
+00002050: 7074 2d33 2e35 2d74 7572 626f 2d30 3132  pt-3.5-turbo-012
+00002060: 3522 290d 0a6f 7065 6e61 695f 656d 6265  5")..openai_embe
+00002070: 6464 696e 6773 203d 204f 7065 6e41 6945  ddings = OpenAiE
+00002080: 6d62 6564 6469 6e67 286d 6f64 656c 3d22  mbedding(model="
+00002090: 7465 7874 2d65 6d62 6564 6469 6e67 2d33  text-embedding-3
+000020a0: 2d73 6d61 6c6c 222c 6f70 656e 6169 5f61  -small",openai_a
+000020b0: 7069 5f6b 6579 3d4f 5045 4e41 495f 4150  pi_key=OPENAI_AP
+000020c0: 495f 4b45 5929 0d0a 6060 600d 0a0d 0a23  I_KEY)..```....#
+000020d0: 2320 4d6f 6469 6679 696e 6720 436f 6e66  # Modifying Conf
+000020e0: 6967 7572 6174 696f 6e20 5365 7474 696e  iguration Settin
+000020f0: 6773 0d0a 0d0a 546f 2063 6861 6e67 6520  gs....To change 
+00002100: 6120 636f 6e66 6967 7572 6174 696f 6e20  a configuration 
+00002110: 7365 7474 696e 672c 2079 6f75 2063 616e  setting, you can
+00002120: 2064 6972 6563 746c 7920 6d6f 6469 6679   directly modify
+00002130: 2074 6865 0d0a 6049 6e64 6f78 2e63 6f6e   the..`Indox.con
+00002140: 6669 6760 2064 6963 7469 6f6e 6172 792e  fig` dictionary.
+00002150: 2048 6572 6520 6973 2061 6e20 6578 616d   Here is an exam
+00002160: 706c 6520 6f66 2068 6f77 2079 6f75 2063  ple of how you c
+00002170: 616e 2075 7064 6174 6520 610d 0a63 6f6e  an update a..con
+00002180: 6669 6775 7261 7469 6f6e 2073 6574 7469  figuration setti
+00002190: 6e67 3a0d 0a0d 0a60 6060 2070 7974 686f  ng:....``` pytho
+000021a0: 6e0d 0a23 2045 7861 6d70 6c65 206f 6620  n..# Example of 
+000021b0: 6d6f 6469 6679 696e 6720 6120 636f 6e66  modifying a conf
+000021c0: 6967 7572 6174 696f 6e20 7365 7474 696e  iguration settin
+000021d0: 670d 0a49 6e64 6f78 2e63 6f6e 6669 675b  g..Indox.config[
+000021e0: 226f 6c64 5f63 6f6e 6669 6722 5d20 3d20  "old_config"] = 
+000021f0: 226e 6577 5f63 6f6e 6669 6722 0d0a 0d0a  "new_config"....
+00002200: 2320 4170 706c 7969 6e67 2074 6865 2075  # Applying the u
+00002210: 7064 6174 6564 2063 6f6e 6669 6775 7261  pdated configura
+00002220: 7469 6f6e 0d0a 496e 646f 782e 7570 6461  tion..Indox.upda
+00002230: 7465 5f63 6f6e 6669 6728 290d 0a60 6060  te_config()..```
+00002240: 0d0a 0d0a 0d0a 5765 2074 616b 6520 6164  ......We take ad
+00002250: 7661 6e74 6167 6520 6f66 2074 6865 2060  vantage of the `
+00002260: 756e 7374 7275 6374 7572 6564 6020 6c69  unstructured` li
+00002270: 6272 6172 7920 746f 206c 6f61 640d 0a64  brary to load..d
+00002280: 6f63 756d 656e 7473 2061 6e64 2073 706c  ocuments and spl
+00002290: 6974 2074 6865 6d20 696e 746f 2063 6875  it them into chu
+000022a0: 6e6b 7320 6279 2074 6974 6c65 2e20 5468  nks by title. Th
+000022b0: 6973 206d 6574 686f 6420 6865 6c70 7320  is method helps 
+000022c0: 696e 0d0a 6f72 6761 6e69 7a69 6e67 2074  in..organizing t
+000022d0: 686d 6520 646f 6375 6d65 6e74 2069 6e74  hme document int
+000022e0: 6f20 6d61 6e61 6765 6162 6c65 2073 6563  o manageable sec
+000022f0: 7469 6f6e 7320 666f 7220 6675 7274 6865  tions for furthe
+00002300: 720d 0a70 726f 6365 7373 696e 672e 0d0a  r..processing...
+00002310: 0d0a 6060 6020 7079 7468 6f6e 0d0a 6672  ..``` python..fr
+00002320: 6f6d 2049 6e64 6f78 2e44 6174 614c 6f61  om Indox.DataLoa
+00002330: 6465 7253 706c 6974 7465 7220 696d 706f  derSplitter impo
+00002340: 7274 2055 6e73 7472 7563 7475 7265 644c  rt UnstructuredL
+00002350: 6f61 6441 6e64 5370 6c69 740d 0a60 6060  oadAndSplit..```
+00002360: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
+00002370: 646f 6373 5f75 6e73 7472 7563 7475 7265  docs_unstructure
+00002380: 6420 3d20 556e 7374 7275 6374 7572 6564  d = Unstructured
+00002390: 4c6f 6164 416e 6453 706c 6974 2866 696c  LoadAndSplit(fil
+000023a0: 655f 7061 7468 3d66 696c 655f 7061 7468  e_path=file_path
+000023b0: 290d 0a60 6060 0d0a 0d0a 2020 2020 5374  )..```....    St
+000023c0: 6172 7469 6e67 2070 726f 6365 7373 696e  arting processin
+000023d0: 672e 2e2e 0d0a 2020 2020 456e 6420 4368  g.....    End Ch
+000023e0: 756e 6b69 6e67 2070 726f 6365 7373 2e0d  unking process..
+000023f0: 0a0d 0a53 746f 7269 6e67 2064 6f63 756d  ...Storing docum
+00002400: 656e 7420 6368 756e 6b73 2069 6e20 6120  ent chunks in a 
+00002410: 7665 6374 6f72 2073 746f 7265 2069 7320  vector store is 
+00002420: 6372 7563 6961 6c20 666f 7220 656e 6162  crucial for enab
+00002430: 6c69 6e67 0d0a 6566 6669 6369 656e 7420  ling..efficient 
+00002440: 7265 7472 6965 7661 6c20 616e 6420 7365  retrieval and se
+00002450: 6172 6368 206f 7065 7261 7469 6f6e 732e  arch operations.
+00002460: 2042 7920 636f 6e76 6572 7469 6e67 2074   By converting t
+00002470: 6578 7420 6461 7461 2069 6e74 6f0d 0a76  ext data into..v
+00002480: 6563 746f 7220 7265 7072 6573 656e 7461  ector representa
+00002490: 7469 6f6e 7320 616e 6420 7374 6f72 696e  tions and storin
+000024a0: 6720 7468 656d 2069 6e20 6120 7665 6374  g them in a vect
+000024b0: 6f72 2073 746f 7265 2c20 796f 7520 6361  or store, you ca
+000024c0: 6e0d 0a70 6572 666f 726d 2072 6170 6964  n..perform rapid
+000024d0: 2073 696d 696c 6172 6974 7920 7365 6172   similarity sear
+000024e0: 6368 6573 2061 6e64 206f 7468 6572 2076  ches and other v
+000024f0: 6563 746f 722d 6261 7365 6420 6f70 6572  ector-based oper
+00002500: 6174 696f 6e73 2e0d 0a0d 0a60 6060 2070  ations.....``` p
+00002510: 7974 686f 6e0d 0a49 6e64 6f78 2e63 6f6e  ython..Indox.con
+00002520: 6e65 6374 5f74 6f5f 7665 6374 6f72 7374  nect_to_vectorst
+00002530: 6f72 6528 636f 6c6c 6563 7469 6f6e 5f6e  ore(collection_n
+00002540: 616d 653d 2273 616d 706c 6522 2c65 6d62  ame="sample",emb
+00002550: 6564 6469 6e67 733d 6f70 656e 6169 5f65  eddings=openai_e
+00002560: 6d62 6564 6469 6e67 7329 0d0a 496e 646f  mbeddings)..Indo
+00002570: 782e 7374 6f72 655f 696e 5f76 6563 746f  x.store_in_vecto
+00002580: 7273 746f 7265 2863 6875 6e6b 733d 646f  rstore(chunks=do
+00002590: 6373 5f75 6e73 7472 7563 7475 7265 6429  cs_unstructured)
+000025a0: 0d0a 6060 600d 0a0d 0a23 2320 5175 6572  ..```....## Quer
+000025b0: 696e 670d 0a0d 0a60 6060 2070 7974 686f  ing....``` pytho
+000025c0: 6e0d 0a71 7565 7279 203d 2022 796f 7572  n..query = "your
+000025d0: 2071 7565 7279 2121 3f3f 220d 0a60 6060   query!!??"..```
+000025e0: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
+000025f0: 7265 7370 6f6e 7365 5f6f 7065 6e61 6920  response_openai 
+00002600: 3d20 496e 646f 782e 616e 7377 6572 5f71  = Indox.answer_q
+00002610: 7565 7374 696f 6e28 7175 6572 793d 7175  uestion(query=qu
+00002620: 6572 792c 7161 5f6d 6f64 656c 3d6f 7065  ery,qa_model=ope
+00002630: 6e61 695f 7161 290d 0a60 6060 0d0a 0d0a  nai_qa)..```....
+00002640: 6060 6020 7079 7468 6f6e 0d0a 616e 7377  ``` python..answ
+00002650: 6572 203d 2072 6573 706f 6e73 655f 6f70  er = response_op
+00002660: 656e 6169 5b30 5d0d 0a60 6060 0d0a 0d0a  enai[0]..```....
+00002670: 6060 6020 7079 7468 6f6e 0d0a 636f 6e74  ``` python..cont
+00002680: 6578 742c 2073 636f 7265 203d 2072 6573  ext, score = res
+00002690: 706f 6e73 655f 6f70 656e 6169 5b31 5d0d  ponse_openai[1].
+000026a0: 0a60 6060 0d0a 0d0a                      .```....
```

### Comparing `indox-0.1.4/PKG-INFO` & `Indox-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2049 6e64  : 2.1..Name: Ind
 00000020: 6f78 0d0a 5665 7273 696f 6e3a 2030 2e31  ox..Version: 0.1
-00000030: 2e34 0d0a 5375 6d6d 6172 793a 2049 6e64  .4..Summary: Ind
+00000030: 2e35 0d0a 5375 6d6d 6172 793a 2049 6e64  .5..Summary: Ind
 00000040: 6f78 2052 6574 7269 6576 616c 2041 7567  ox Retrieval Aug
 00000050: 6d65 6e74 6174 696f 6e0d 0a48 6f6d 652d  mentation..Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f6f 736c 6c6d 6169  thub.com/osllmai
 00000080: 2f69 6e44 6f78 0d0a 4175 7468 6f72 3a20  /inDox..Author: 
 00000090: 6e65 7264 7374 7564 696f 0d0a 4175 7468  nerdstudio..Auth
 000000a0: 6f72 2d65 6d61 696c 3a20 6173 686b 616e  or-email: ashkan
@@ -35,37 +35,37 @@
 00000220: 3a20 332e 3130 0d0a 436c 6173 7369 6669  : 3.10..Classifi
 00000230: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
 00000240: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000250: 6f6e 203a 3a20 332e 3131 0d0a 5265 7175  on :: 3.11..Requ
 00000260: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000270: 2e39 0d0a 4465 7363 7269 7074 696f 6e2d  .9..Description-
 00000280: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000290: 7874 2f6d 6172 6b64 6f77 6e0d 0a52 6571  xt/markdown..Req
-000002a0: 7569 7265 732d 4469 7374 3a20 6265 7274  uires-Dist: bert
-000002b0: 5f73 636f 7265 0d0a 5265 7175 6972 6573  _score..Requires
-000002c0: 2d44 6973 743a 2066 6169 7373 5f63 7075  -Dist: faiss_cpu
-000002d0: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-000002e0: 206c 616e 6763 6861 696e 0d0a 5265 7175   langchain..Requ
-000002f0: 6972 6573 2d44 6973 743a 206c 616e 6763  ires-Dist: langc
-00000300: 6861 696e 5f63 6f6d 6d75 6e69 7479 0d0a  hain_community..
-00000310: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
-00000320: 616e 6763 6861 696e 5f63 6f72 650d 0a52  angchain_core..R
-00000330: 6571 7569 7265 732d 4469 7374 3a20 6c61  equires-Dist: la
-00000340: 6e67 6368 6169 6e5f 6f70 656e 6169 0d0a  ngchain_openai..
-00000350: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
-00000360: 616e 6767 7261 7068 0d0a 5265 7175 6972  anggraph..Requir
-00000370: 6573 2d44 6973 743a 206c 6174 6578 326d  es-Dist: latex2m
-00000380: 6172 6b64 6f77 6e0d 0a52 6571 7569 7265  arkdown..Require
-00000390: 732d 4469 7374 3a20 6e6c 746b 0d0a 5265  s-Dist: nltk..Re
-000003a0: 7175 6972 6573 2d44 6973 743a 206e 756d  quires-Dist: num
-000003b0: 7079 0d0a 5265 7175 6972 6573 2d44 6973  py..Requires-Dis
-000003c0: 743a 2070 616e 6461 730d 0a52 6571 7569  t: pandas..Requi
-000003d0: 7265 732d 4469 7374 3a20 5079 5044 4632  res-Dist: PyPDF2
+00000290: 7874 2f6d 6172 6b64 6f77 6e0d 0a4c 6963  xt/markdown..Lic
+000002a0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000002b0: 5345 0d0a 5265 7175 6972 6573 2d44 6973  SE..Requires-Dis
+000002c0: 743a 2062 6572 745f 7363 6f72 650d 0a52  t: bert_score..R
+000002d0: 6571 7569 7265 732d 4469 7374 3a20 6661  equires-Dist: fa
+000002e0: 6973 735f 6370 750d 0a52 6571 7569 7265  iss_cpu..Require
+000002f0: 732d 4469 7374 3a20 6c61 6e67 6368 6169  s-Dist: langchai
+00000300: 6e0d 0a52 6571 7569 7265 732d 4469 7374  n..Requires-Dist
+00000310: 3a20 6c61 6e67 6368 6169 6e5f 636f 6d6d  : langchain_comm
+00000320: 756e 6974 790d 0a52 6571 7569 7265 732d  unity..Requires-
+00000330: 4469 7374 3a20 6c61 6e67 6368 6169 6e5f  Dist: langchain_
+00000340: 636f 7265 0d0a 5265 7175 6972 6573 2d44  core..Requires-D
+00000350: 6973 743a 206c 616e 6763 6861 696e 5f6f  ist: langchain_o
+00000360: 7065 6e61 690d 0a52 6571 7569 7265 732d  penai..Requires-
+00000370: 4469 7374 3a20 6c61 6e67 6772 6170 680d  Dist: langgraph.
+00000380: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000390: 6c61 7465 7832 6d61 726b 646f 776e 0d0a  latex2markdown..
+000003a0: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
+000003b0: 6c74 6b0d 0a52 6571 7569 7265 732d 4469  ltk..Requires-Di
+000003c0: 7374 3a20 6e75 6d70 790d 0a52 6571 7569  st: numpy..Requi
+000003d0: 7265 732d 4469 7374 3a20 7061 6e64 6173  res-Dist: pandas
 000003e0: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-000003f0: 2050 7959 414d 4c0d 0a52 6571 7569 7265   PyYAML..Require
+000003f0: 2050 7950 4446 320d 0a52 6571 7569 7265   PyPDF2..Require
 00000400: 732d 4469 7374 3a20 5079 5941 4d4c 0d0a  s-Dist: PyYAML..
 00000410: 5265 7175 6972 6573 2d44 6973 743a 2052  Requires-Dist: R
 00000420: 6571 7565 7374 730d 0a52 6571 7569 7265  equests..Require
 00000430: 732d 4469 7374 3a20 7363 696b 6974 5f6c  s-Dist: scikit_l
 00000440: 6561 726e 0d0a 5265 7175 6972 6573 2d44  earn..Requires-D
 00000450: 6973 743a 2073 656e 7465 6e63 655f 7472  ist: sentence_tr
 00000460: 616e 7366 6f72 6d65 7273 0d0a 5265 7175  ansformers..Requ
@@ -78,440 +78,542 @@
 000004d0: 7273 0d0a 5265 7175 6972 6573 2d44 6973  rs..Requires-Dis
 000004e0: 743a 2074 6f72 6368 0d0a 5265 7175 6972  t: torch..Requir
 000004f0: 6573 2d44 6973 743a 2074 7261 6e73 666f  es-Dist: transfo
 00000500: 726d 6572 730d 0a52 6571 7569 7265 732d  rmers..Requires-
 00000510: 4469 7374 3a20 756d 6170 5f6c 6561 726e  Dist: umap_learn
 00000520: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
 00000530: 2075 6e73 7472 7563 7475 7265 640d 0a0d   unstructured...
-00000540: 0a23 2069 6e44 6f78 3a20 4164 7661 6e63  .# inDox: Advanc
-00000550: 6564 2053 6561 7263 6820 616e 6420 5265  ed Search and Re
-00000560: 7472 6965 7661 6c20 4175 676d 656e 7461  trieval Augmenta
-00000570: 7469 6f6e 2047 656e 6572 6174 6976 650d  tion Generative.
-00000580: 0a0d 0a2a 2a49 6e64 6f78 2052 6574 7269  ...**Indox Retri
-00000590: 6576 616c 2041 7567 6d65 6e74 6174 696f  eval Augmentatio
-000005a0: 6e2a 2a20 6973 2061 6e20 696e 6e6f 7661  n** is an innova
-000005b0: 7469 7665 2061 7070 6c69 6361 7469 6f6e  tive application
-000005c0: 2064 6573 6967 6e65 6420 746f 2073 7472   designed to str
-000005d0: 6561 6d6c 696e 6520 696e 666f 726d 6174  eamline informat
-000005e0: 696f 6e20 6578 7472 6163 7469 6f6e 2066  ion extraction f
-000005f0: 726f 6d20 6120 7769 6465 0d0a 7261 6e67  rom a wide..rang
-00000600: 6520 6f66 2064 6f63 756d 656e 7420 7479  e of document ty
-00000610: 7065 732c 2069 6e63 6c75 6469 6e67 2074  pes, including t
-00000620: 6578 7420 6669 6c65 732c 2050 4446 2c20  ext files, PDF, 
-00000630: 4854 4d4c 2c20 4d61 726b 646f 776e 2c20  HTML, Markdown, 
-00000640: 616e 6420 4c61 5465 582e 2057 6865 7468  and LaTeX. Wheth
-00000650: 6572 2073 7472 7563 7475 7265 6420 6f72  er structured or
-00000660: 2075 6e73 7472 7563 7475 7265 642c 2049   unstructured, I
-00000670: 6e64 6f78 0d0a 7072 6f76 6964 6573 2075  ndox..provides u
-00000680: 7365 7273 2077 6974 6820 6120 706f 7765  sers with a powe
-00000690: 7266 756c 2074 6f6f 6c73 6574 2074 6f20  rful toolset to 
-000006a0: 6566 6669 6369 656e 746c 7920 6578 7472  efficiently extr
-000006b0: 6163 7420 7265 6c65 7661 6e74 2064 6174  act relevant dat
-000006c0: 612e 0d0a 0d0a 496e 646f 7820 5265 7472  a.....Indox Retr
-000006d0: 6965 7661 6c20 4175 676d 656e 7461 7469  ieval Augmentati
-000006e0: 6f6e 2069 7320 616e 2069 6e6e 6f76 6174  on is an innovat
-000006f0: 6976 6520 6170 706c 6963 6174 696f 6e20  ive application 
-00000700: 6465 7369 676e 6564 2074 6f20 7374 7265  designed to stre
-00000710: 616d 6c69 6e65 2069 6e66 6f72 6d61 7469  amline informati
-00000720: 6f6e 2065 7874 7261 6374 696f 6e20 6672  on extraction fr
-00000730: 6f6d 2061 2077 6964 650d 0a72 616e 6765  om a wide..range
-00000740: 206f 6620 646f 6375 6d65 6e74 2074 7970   of document typ
-00000750: 6573 2c20 696e 636c 7564 696e 6720 7465  es, including te
-00000760: 7874 2066 696c 6573 2c20 5044 462c 2048  xt files, PDF, H
-00000770: 544d 4c2c 204d 6172 6b64 6f77 6e2c 2061  TML, Markdown, a
-00000780: 6e64 204c 6154 6558 2e20 5768 6574 6865  nd LaTeX. Whethe
-00000790: 7220 7374 7275 6374 7572 6564 206f 7220  r structured or 
-000007a0: 756e 7374 7275 6374 7572 6564 2c20 496e  unstructured, In
-000007b0: 646f 780d 0a70 726f 7669 6465 7320 7573  dox..provides us
-000007c0: 6572 7320 7769 7468 2061 2070 6f77 6572  ers with a power
-000007d0: 6675 6c20 746f 6f6c 7365 7420 746f 2065  ful toolset to e
-000007e0: 6666 6963 6965 6e74 6c79 2065 7874 7261  fficiently extra
-000007f0: 6374 2072 656c 6576 616e 7420 6461 7461  ct relevant data
-00000800: 2e20 4f6e 6520 6f66 2069 7473 206b 6579  . One of its key
-00000810: 2066 6561 7475 7265 7320 6973 2074 6865   features is the
-00000820: 2061 6269 6c69 7479 2074 6f0d 0a69 6e74   ability to..int
-00000830: 656c 6c69 6765 6e74 6c79 2063 6c75 7374  elligently clust
-00000840: 6572 2070 7269 6d61 7279 2063 6875 6e6b  er primary chunk
-00000850: 7320 746f 2066 6f72 6d20 6d6f 7265 2072  s to form more r
-00000860: 6f62 7573 7420 6772 6f75 7069 6e67 732c  obust groupings,
-00000870: 2065 6e68 616e 6369 6e67 2074 6865 2071   enhancing the q
-00000880: 7561 6c69 7479 2061 6e64 2072 656c 6576  uality and relev
-00000890: 616e 6365 206f 6620 7468 6520 6578 7472  ance of the extr
-000008a0: 6163 7465 640d 0a69 6e66 6f72 6d61 7469  acted..informati
-000008b0: 6f6e 2e0d 0a57 6974 6820 6120 666f 6375  on...With a focu
-000008c0: 7320 6f6e 2061 6461 7074 6162 696c 6974  s on adaptabilit
-000008d0: 7920 616e 6420 7573 6572 2d63 656e 7472  y and user-centr
-000008e0: 6963 2064 6573 6967 6e2c 2049 6e64 6f78  ic design, Indox
-000008f0: 2061 696d 7320 746f 2064 656c 6976 6572   aims to deliver
-00000900: 2066 7574 7572 652d 7265 6164 7920 6675   future-ready fu
-00000910: 6e63 7469 6f6e 616c 6974 7920 7769 7468  nctionality with
-00000920: 206d 6f72 650d 0a66 6561 7475 7265 7320   more..features 
-00000930: 706c 616e 6e65 6420 666f 7220 7570 636f  planned for upco
-00000940: 6d69 6e67 2072 656c 6561 7365 732e 204a  ming releases. J
-00000950: 6f69 6e20 7573 2069 6e20 6578 706c 6f72  oin us in explor
-00000960: 696e 6720 686f 7720 496e 646f 7820 6361  ing how Indox ca
-00000970: 6e20 7265 766f 6c75 7469 6f6e 697a 6520  n revolutionize 
-00000980: 796f 7572 2064 6f63 756d 656e 7420 7072  your document pr
-00000990: 6f63 6573 7369 6e67 0d0a 776f 726b 666c  ocessing..workfl
-000009a0: 6f77 2c20 6272 696e 6769 6e67 2063 6c61  ow, bringing cla
-000009b0: 7269 7479 2061 6e64 206f 7267 616e 697a  rity and organiz
-000009c0: 6174 696f 6e20 746f 2079 6f75 7220 6461  ation to your da
-000009d0: 7461 2072 6574 7269 6576 616c 206e 6565  ta retrieval nee
-000009e0: 6473 2e0d 0a0d 0a23 2320 5072 6572 6571  ds.....## Prereq
-000009f0: 7569 7369 7465 730d 0a0d 0a42 6566 6f72  uisites....Befor
-00000a00: 6520 7275 6e6e 696e 6720 7468 6973 2070  e running this p
-00000a10: 726f 6a65 6374 2c20 656e 7375 7265 2074  roject, ensure t
-00000a20: 6861 7420 796f 7520 6861 7665 2074 6865  hat you have the
-00000a30: 2066 6f6c 6c6f 7769 6e67 2069 6e73 7461   following insta
-00000a40: 6c6c 6564 3a0d 0a0d 0a2d 202a 2a50 7974  lled:....- **Pyt
-00000a50: 686f 6e20 332e 382b 2a2a 3a20 5265 7175  hon 3.8+**: Requ
-00000a60: 6972 6564 2066 6f72 2072 756e 6e69 6e67  ired for running
-00000a70: 2074 6865 2050 7974 686f 6e20 6261 636b   the Python back
-00000a80: 656e 642e 0d0a 2d20 2a2a 506f 7374 6772  end...- **Postgr
-00000a90: 6553 514c 2a2a 3a20 4e65 6564 6564 2069  eSQL**: Needed i
-00000aa0: 6620 796f 7520 7769 7368 2074 6f20 7374  f you wish to st
-00000ab0: 6f72 6520 796f 7572 2064 6174 6120 696e  ore your data in
-00000ac0: 2061 2050 6f73 7467 7265 5351 4c20 6461   a PostgreSQL da
-00000ad0: 7461 6261 7365 2e0d 0a2d 202a 2a4f 7065  tabase...- **Ope
-00000ae0: 6e41 4920 4150 4920 4b65 792a 2a3a 204e  nAI API Key**: N
-00000af0: 6563 6573 7361 7279 2069 6620 796f 7520  ecessary if you 
-00000b00: 6172 6520 7573 696e 6720 7468 6520 4f70  are using the Op
-00000b10: 656e 4149 2065 6d62 6564 6469 6e67 206d  enAI embedding m
-00000b20: 6f64 656c 2e0d 0a2d 202a 2a48 7567 6769  odel...- **Huggi
-00000b30: 6e67 4661 6365 2041 5049 204b 6579 2a2a  ngFace API Key**
-00000b40: 3a20 4e65 6365 7373 6172 7920 6966 2079  : Necessary if y
-00000b50: 6f75 2061 7265 2075 7369 6e67 2074 6865  ou are using the
-00000b60: 2048 7567 6769 6e67 4661 6365 206c 6c6d   HuggingFace llm
-00000b70: 732e 0d0a 0d0a 456e 7375 7265 2079 6f75  s.....Ensure you
-00000b80: 7220 7379 7374 656d 2061 6c73 6f20 6d65  r system also me
-00000b90: 6574 7320 7468 6573 6520 7265 7175 6972  ets these requir
-00000ba0: 656d 656e 7473 3a0d 0a0d 0a2d 2041 6363  ements:....- Acc
-00000bb0: 6573 7320 746f 2065 6e76 6972 6f6e 6d65  ess to environme
-00000bc0: 6e74 616c 2076 6172 6961 626c 6573 2066  ntal variables f
-00000bd0: 6f72 2068 616e 646c 696e 6720 7365 6e73  or handling sens
-00000be0: 6974 6976 6520 696e 666f 726d 6174 696f  itive informatio
-00000bf0: 6e20 6c69 6b65 2041 5049 206b 6579 732e  n like API keys.
-00000c00: 0d0a 2d20 5375 6974 6162 6c65 2068 6172  ..- Suitable har
-00000c10: 6477 6172 6520 6361 7061 626c 6520 6f66  dware capable of
-00000c20: 2073 7570 706f 7274 696e 6720 696e 7465   supporting inte
-00000c30: 6e73 6976 6520 636f 6d70 7574 6174 696f  nsive computatio
-00000c40: 6e61 6c20 7461 736b 732e 0d0a 0d0a 2323  nal tasks.....##
-00000c50: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
-00000c60: 0a43 6c6f 6e65 2074 6865 2072 6570 6f73  .Clone the repos
-00000c70: 6974 6f72 7920 616e 6420 6e61 7669 6761  itory and naviga
-00000c80: 7465 2074 6f20 7468 6520 6469 7265 6374  te to the direct
-00000c90: 6f72 793a 0d0a 0d0a 6060 6062 6173 680d  ory:....```bash.
-00000ca0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
-00000cb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f73  ://github.com/os
-00000cc0: 6c6c 6d61 692f 696e 446f 782e 6769 740d  llmai/inDox.git.
-00000cd0: 0a63 6420 696e 446f 780d 0a60 6060 0d0a  .cd inDox..```..
-00000ce0: 0d0a 496e 7374 616c 6c20 7468 6520 7265  ..Install the re
-00000cf0: 7175 6972 6564 2050 7974 686f 6e20 7061  quired Python pa
-00000d00: 636b 6167 6573 3a0d 0a0d 0a60 6060 6261  ckages:....```ba
-00000d10: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
-00000d20: 2d72 2072 6571 7569 7265 6d65 6e74 732e  -r requirements.
-00000d30: 7478 740d 0a60 6060 0d0a 0d0a 2323 2043  txt..```....## C
-00000d40: 6f6e 6669 6775 7261 7469 6f6e 0d0a 0d0a  onfiguration....
-00000d50: 2323 2320 456e 7669 726f 6e6d 656e 7420  ### Environment 
-00000d60: 5661 7269 6162 6c65 730d 0a0d 0a53 6574  Variables....Set
-00000d70: 2079 6f75 7220 604f 5045 4e41 495f 4150   your `OPENAI_AP
-00000d80: 495f 4b45 5960 206f 7220 6048 465f 4150  I_KEY` or `HF_AP
-00000d90: 495f 4b45 5960 2069 6e20 796f 7572 2065  I_KEY` in your e
-00000da0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00000db0: 626c 6573 2066 6f72 2073 6563 7572 6520  bles for secure 
-00000dc0: 6163 6365 7373 2e0d 0a0d 0a23 2323 2044  access.....### D
-00000dd0: 6174 6162 6173 6520 5365 7475 700d 0a0d  atabase Setup...
-00000de0: 0a45 6e73 7572 6520 796f 7572 2050 6f73  .Ensure your Pos
-00000df0: 7467 7265 5351 4c20 6461 7461 6261 7365  tgreSQL database
-00000e00: 2069 7320 7570 2061 6e64 2072 756e 6e69   is up and runni
-00000e10: 6e67 2c20 616e 6420 6163 6365 7373 6962  ng, and accessib
-00000e20: 6c65 2066 726f 6d20 796f 7572 2061 7070  le from your app
-00000e30: 6c69 6361 7469 6f6e 2e20 5468 6973 2069  lication. This i
-00000e40: 7320 6e65 6365 7373 6172 7920 6966 2079  s necessary if y
-00000e50: 6f75 2070 6c61 6e20 746f 2075 7365 2070  ou plan to use p
-00000e60: 6776 6563 746f 7220 6173 2079 6f75 7220  gvector as your 
-00000e70: 7665 6374 6f72 2073 746f 7265 2e0d 0a0d  vector store....
-00000e80: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
-00000e90: 796f 7520 6361 6e20 7573 6520 4368 726f  you can use Chro
-00000ea0: 6d61 206f 7220 4661 6973 7320 6173 2079  ma or Faiss as y
-00000eb0: 6f75 7220 7665 6374 6f72 2073 746f 7265  our vector store
-00000ec0: 2e20 4d61 6b65 2073 7572 6520 746f 2073  . Make sure to s
-00000ed0: 7065 6369 6679 2079 6f75 7220 6368 6f69  pecify your choi
-00000ee0: 6365 2061 6e64 2074 6865 206e 6563 6573  ce and the neces
-00000ef0: 7361 7279 2063 6f6e 6669 6775 7261 7469  sary configurati
-00000f00: 6f6e 7320 696e 2074 6865 2063 6f6e 6669  ons in the confi
-00000f10: 672e 7961 6d6c 2066 696c 652e 0d0a 0d0a  g.yaml file.....
-00000f20: 2323 2055 7361 6765 0d0a 0d0a 2323 2320  ## Usage....### 
-00000f30: 5072 6570 6172 696e 6720 596f 7572 2044  Preparing Your D
-00000f40: 6174 610d 0a0d 0a31 2e20 2a2a 4465 6669  ata....1. **Defi
-00000f50: 6e65 2074 6865 2046 696c 6520 5061 7468  ne the File Path
-00000f60: 2a2a 3a20 5370 6563 6966 7920 7468 6520  **: Specify the 
-00000f70: 7061 7468 2074 6f20 796f 7572 2074 6578  path to your tex
-00000f80: 7420 6f72 2050 4446 2066 696c 652e 0d0a  t or PDF file...
-00000f90: 322e 202a 2a4c 6f61 6420 456d 6265 6464  2. **Load Embedd
-00000fa0: 696e 6720 4d6f 6465 6c73 2a2a 3a20 496e  ing Models**: In
-00000fb0: 6974 6961 6c69 7a65 2079 6f75 7220 656d  itialize your em
-00000fc0: 6265 6464 696e 6720 6d6f 6465 6c20 6672  bedding model fr
-00000fd0: 6f6d 204f 7065 6e41 4927 7320 7365 6c65  om OpenAI's sele
-00000fe0: 6374 696f 6e20 6f66 2070 7265 2d74 7261  ction of pre-tra
-00000ff0: 696e 6564 206d 6f64 656c 732e 0d0a 0d0a  ined models.....
-00001000: 2320 5175 6963 6b20 5374 6172 7420 0d0a  # Quick Start ..
-00001010: 0d0a 2323 2049 6d70 6f72 7420 496e 646f  ..## Import Indo
-00001020: 7820 5061 636b 6167 650d 0a0d 0a49 6d70  x Package....Imp
-00001030: 6f72 7420 7468 6520 6e65 6365 7373 6172  ort the necessar
-00001040: 7920 636c 6173 7365 7320 6672 6f6d 2074  y classes from t
-00001050: 6865 2049 6e64 6f78 2070 6163 6b61 6765  he Indox package
-00001060: 2e0d 0a0d 0a60 6060 2070 7974 686f 6e0d  .....``` python.
-00001070: 0a66 726f 6d20 496e 646f 7820 696d 706f  .from Indox impo
-00001080: 7274 2049 6e64 6f78 5265 7472 6965 7661  rt IndoxRetrieva
-00001090: 6c41 7567 6d65 6e74 6174 696f 6e0d 0a60  lAugmentation..`
-000010a0: 6060 0d0a 0d0a 2323 2320 496e 6974 6961  ``....### Initia
-000010b0: 6c69 7a65 2049 6e64 6f78 0d0a 0d0a 4372  lize Indox....Cr
-000010c0: 6561 7465 2061 6e20 696e 7374 616e 6365  eate an instance
-000010d0: 206f 6620 496e 646f 7852 6574 7269 6576   of IndoxRetriev
-000010e0: 616c 4175 676d 656e 7461 7469 6f6e 2e0d  alAugmentation..
-000010f0: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a49  ...``` python..I
-00001100: 6e64 6f78 203d 2049 6e64 6f78 5265 7472  ndox = IndoxRetr
-00001110: 6965 7661 6c41 7567 6d65 6e74 6174 696f  ievalAugmentatio
-00001120: 6e28 290d 0a60 6060 0d0a 2323 2049 6e69  n()..```..## Ini
-00001130: 7469 616c 2043 6f6e 6669 6775 7261 7469  tial Configurati
-00001140: 6f6e 0d0a 0d0a 2d20 2a2a 436f 6e66 6967  on....- **Config
-00001150: 7572 6174 696f 6e20 4669 6c65 2a2a 3a20  uration File**: 
-00001160: 456e 7375 7265 2079 6f75 206c 6f63 6174  Ensure you locat
-00001170: 6520 616e 6420 6d6f 6469 6679 2074 6865  e and modify the
-00001180: 2060 496e 646f 782e 636f 6e66 6967 6020   `Indox.config` 
-00001190: 5941 4d4c 2066 696c 6520 6163 636f 7264  YAML file accord
-000011a0: 696e 6720 746f 2079 6f75 7220 6e65 6564  ing to your need
-000011b0: 7320 6265 666f 7265 0d0a 2020 7374 6172  s before..  star
-000011c0: 7469 6e67 2074 6865 2061 7070 6c69 6361  ting the applica
-000011d0: 7469 6f6e 2e0d 0a0d 0a23 2320 4479 6e61  tion.....## Dyna
-000011e0: 6d69 6320 436f 6e66 6967 7572 6174 696f  mic Configuratio
-000011f0: 6e20 4368 616e 6765 730d 0a0d 0a46 6f72  n Changes....For
-00001200: 2063 6861 6e67 6573 2074 6861 7420 6e65   changes that ne
-00001210: 6564 2074 6f20 6265 2061 7070 6c69 6564  ed to be applied
-00001220: 2061 6674 6572 2074 6865 2069 6e69 7469   after the initi
-00001230: 616c 2073 6574 7570 206f 7220 6475 7269  al setup or duri
-00001240: 6e67 2072 756e 7469 6d65 3a0d 0a0d 0a2d  ng runtime:....-
-00001250: 202a 2a4d 6f64 6966 7969 6e67 2043 6f6e   **Modifying Con
-00001260: 6669 6775 7261 7469 6f6e 732a 2a3a 2055  figurations**: U
-00001270: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00001280: 2050 7974 686f 6e20 736e 6970 7065 7420   Python snippet 
-00001290: 746f 2075 7064 6174 6520 796f 7572 2073  to update your s
-000012a0: 6574 7469 6e67 7320 6479 6e61 6d69 6361  ettings dynamica
-000012b0: 6c6c 793a 0d0a 2020 6060 6070 7974 686f  lly:..  ```pytho
-000012c0: 6e0d 0a20 2049 6e64 6f78 2e63 6f6e 6669  n..  Indox.confi
-000012d0: 675b 2279 6f75 725f 7365 7474 696e 675f  g["your_setting_
-000012e0: 7468 6174 5f6e 6565 645f 746f 5f63 6861  that_need_to_cha
-000012f0: 6e67 6522 5d20 3d20 226e 6577 5f73 6574  nge"] = "new_set
-00001300: 7469 6e67 220d 0a20 2049 6e64 6f78 2e75  ting"..  Indox.u
-00001310: 7064 6174 655f 636f 6e66 6967 2829 0d0a  pdate_config()..
-00001320: 0d0a 2323 2043 6f6e 6669 6775 7261 7469  ..## Configurati
-00001330: 6f6e 2044 6574 6169 6c73 0d0a 0d0a 4865  on Details....He
-00001340: 7265 2773 2061 2062 7265 616b 646f 776e  re's a breakdown
-00001350: 206f 6620 7468 6520 636f 6e66 6967 2064   of the config d
-00001360: 6963 7469 6f6e 6172 7920 616e 6420 6974  ictionary and it
-00001370: 7320 7072 6f70 6572 7469 6573 3a0d 0a0d  s properties:...
-00001380: 0a23 2323 2050 6f73 7467 7265 5351 4c0d  .### PostgreSQL.
-00001390: 0a0d 0a2d 2060 636f 6e6e 5f73 7472 696e  ...- `conn_strin
-000013a0: 6760 3a20 596f 7572 2050 6f73 7467 7265  g`: Your Postgre
-000013b0: 5351 4c20 6461 7461 6261 7365 2063 7265  SQL database cre
-000013c0: 6465 6e74 6961 6c73 2e0d 0a0d 0a23 2323  dentials.....###
-000013d0: 2053 756d 6d61 7279 204d 6f64 656c 0d0a   Summary Model..
-000013e0: 0d0a 2d20 606d 6178 5f74 6f6b 656e 7360  ..- `max_tokens`
-000013f0: 3a20 4d61 7869 6d75 6d20 746f 6b65 6e20  : Maximum token 
-00001400: 636f 756e 7420 7468 6520 7375 6d6d 6172  count the summar
-00001410: 7920 6d6f 6465 6c20 6361 6e20 6765 6e65  y model can gene
-00001420: 7261 7465 2e0d 0a2d 2060 6d69 6e5f 6c65  rate...- `min_le
-00001430: 6e60 3a20 4d69 6e69 6d75 6d20 746f 6b65  n`: Minimum toke
-00001440: 6e20 636f 756e 7420 7468 6520 7375 6d6d  n count the summ
-00001450: 6172 7920 6d6f 6465 6c20 6765 6e65 7261  ary model genera
-00001460: 7465 732e 0d0a 2d20 606d 6f64 656c 5f6e  tes...- `model_n
-00001470: 616d 6560 3a20 4465 6661 756c 7420 6973  ame`: Default is
-00001480: 2060 6770 742d 332e 352d 7475 7262 6f2d   `gpt-3.5-turbo-
-00001490: 3031 3235 602c 2062 7574 2069 7420 6361  0125`, but it ca
-000014a0: 6e20 6265 2072 6570 6c61 6365 6420 7769  n be replaced wi
-000014b0: 7468 2061 6e79 2048 7567 6769 6e67 2046  th any Hugging F
-000014c0: 6163 6520 6d6f 6465 6c20 7375 7070 6f72  ace model suppor
-000014d0: 7469 6e67 2074 6865 0d0a 2020 7375 6d6d  ting the..  summ
-000014e0: 6172 697a 6174 696f 6e20 7069 7065 6c69  arization pipeli
-000014f0: 6e65 2e0d 0a0d 0a23 2323 2050 6f73 7467  ne.....### Postg
-00001500: 7265 5351 4c20 5365 7475 7020 7769 7468  reSQL Setup with
-00001510: 2070 6776 6563 746f 720d 0a0d 0a49 6620   pgvector....If 
-00001520: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00001530: 506f 7374 6772 6553 514c 2066 6f72 2076  PostgreSQL for v
-00001540: 6563 746f 7220 7374 6f72 6167 652c 2079  ector storage, y
-00001550: 6f75 2073 686f 756c 6420 7065 7266 6f72  ou should perfor
-00001560: 6d20 7468 6520 666f 6c6c 6f77 696e 6720  m the following 
-00001570: 7374 6570 733a 0d0a 0d0a 312e 202a 2a49  steps:....1. **I
-00001580: 6e73 7461 6c6c 2070 6776 6563 746f 722a  nstall pgvector*
-00001590: 2a3a 2054 6f20 696e 7374 616c 6c20 6070  *: To install `p
-000015a0: 6776 6563 746f 7260 206f 6e20 796f 7572  gvector` on your
-000015b0: 2050 6f73 7467 7265 5351 4c20 7365 7276   PostgreSQL serv
-000015c0: 6572 2c20 666f 6c6c 6f77 2074 6865 2064  er, follow the d
-000015d0: 6574 6169 6c65 6420 696e 7374 616c 6c61  etailed installa
-000015e0: 7469 6f6e 2069 6e73 7472 7563 7469 6f6e  tion instruction
-000015f0: 730d 0a20 2020 6176 6169 6c61 626c 6520  s..   available 
-00001600: 6f6e 2074 6865 206f 6666 6963 6961 6c20  on the official 
-00001610: 7067 7665 6374 6f72 2047 6974 4875 6220  pgvector GitHub 
-00001620: 7265 706f 7369 746f 7279 3a0d 0a20 2020  repository:..   
-00001630: 5b70 6776 6563 746f 7220 496e 7374 616c  [pgvector Instal
-00001640: 6c61 7469 6f6e 2049 6e73 7472 7563 7469  lation Instructi
-00001650: 6f6e 735d 2868 7474 7073 3a2f 2f67 6974  ons](https://git
-00001660: 6875 622e 636f 6d2f 7067 7665 6374 6f72  hub.com/pgvector
-00001670: 2f70 6776 6563 746f 7229 0d0a 0d0a 322e  /pgvector)....2.
-00001680: 202a 2a41 6464 2056 6563 746f 7220 4578   **Add Vector Ex
-00001690: 7465 6e73 696f 6e2a 2a3a 0d0a 2020 2043  tension**:..   C
-000016a0: 6f6e 6e65 6374 2074 6f20 796f 7572 2050  onnect to your P
-000016b0: 6f73 7467 7265 5351 4c20 6461 7461 6261  ostgreSQL databa
-000016c0: 7365 2061 6e64 2065 7865 6375 7465 2074  se and execute t
-000016d0: 6865 2066 6f6c 6c6f 7769 6e67 2053 514c  he following SQL
-000016e0: 2063 6f6d 6d61 6e64 2074 6f20 6372 6561   command to crea
-000016f0: 7465 2074 6865 2060 7067 7665 6374 6f72  te the `pgvector
-00001700: 6020 6578 7465 6e73 696f 6e3a 0d0a 0d0a  ` extension:....
-00001710: 2020 2060 6060 7371 6c0d 0a20 2020 2d2d     ```sql..   --
-00001720: 2043 6f6e 6e65 6374 2074 6f20 796f 7572   Connect to your
-00001730: 2064 6174 6162 6173 650d 0a20 2020 7073   database..   ps
-00001740: 716c 202d 5520 7573 6572 6e61 6d65 202d  ql -U username -
-00001750: 6420 6461 7461 6261 7365 5f6e 616d 650d  d database_name.
-00001760: 0a0d 0a20 2020 2d2d 2052 756e 2069 6e73  ...   -- Run ins
-00001770: 6964 6520 796f 7572 2070 7371 6c20 7465  ide your psql te
-00001780: 726d 696e 616c 0d0a 2020 2043 5245 4154  rminal..   CREAT
-00001790: 4520 4558 5445 4e53 494f 4e20 7665 6374  E EXTENSION vect
-000017a0: 6f72 3b0d 0a20 2020 2320 5265 706c 6163  or;..   # Replac
-000017b0: 6520 7468 6520 706c 6163 6568 6f6c 6465  e the placeholde
-000017c0: 7273 2077 6974 6820 796f 7572 2061 6374  rs with your act
-000017d0: 7561 6c20 506f 7374 6772 6553 514c 2063  ual PostgreSQL c
-000017e0: 7265 6465 6e74 6961 6c73 2061 6e64 2064  redentials and d
-000017f0: 6574 6169 6c73 0d0a 0d0a 4164 6469 7469  etails....Additi
-00001800: 6f6e 616c 6c79 2c20 666f 7220 7468 6f73  onally, for thos
-00001810: 6520 696e 7465 7265 7374 6564 2069 6e20  e interested in 
-00001820: 6578 706c 6f72 696e 6720 6f74 6865 7220  exploring other 
-00001830: 7665 6374 6f72 2064 6174 6162 6173 6520  vector database 
-00001840: 6f70 7469 6f6e 732c 2079 6f75 2063 616e  options, you can
-00001850: 2063 6f6e 7369 6465 7220 7573 696e 6720   consider using 
-00001860: 2a2a 4368 726f 6d61 2a2a 206f 7220 2a0d  **Chroma** or *.
-00001870: 0a2a 4661 6973 732a 2a2e 2054 6865 7365  .*Faiss**. These
-00001880: 2070 726f 7669 6465 2061 6c74 6572 6e61   provide alterna
-00001890: 7469 7665 2061 7070 726f 6163 6865 7320  tive approaches 
-000018a0: 746f 2076 6563 746f 7220 7374 6f72 6167  to vector storag
-000018b0: 6520 616e 6420 7265 7472 6965 7661 6c20  e and retrieval 
-000018c0: 7468 6174 206d 6179 2062 6574 7465 7220  that may better 
-000018d0: 7375 6974 2073 7065 6369 6669 6320 7573  suit specific us
-000018e0: 6520 6361 7365 730d 0a6f 7220 7065 7266  e cases..or perf
-000018f0: 6f72 6d61 6e63 6520 7265 7175 6972 656d  ormance requirem
-00001900: 656e 7473 2e0d 0a0d 0a23 2323 2049 6d70  ents.....### Imp
-00001910: 6f72 7469 6e67 2051 4120 616e 6420 456d  orting QA and Em
-00001920: 6265 6464 696e 6720 4d6f 6465 6c73 0d0a  bedding Models..
-00001930: 0d0a 6060 6020 7079 7468 6f6e 0d0a 6672  ..``` python..fr
-00001940: 6f6d 2049 6e64 6f78 2e51 614d 6f64 656c  om Indox.QaModel
-00001950: 7320 696d 706f 7274 204f 7065 6e41 6951  s import OpenAiQ
-00001960: 410d 0a60 6060 0d0a 0d0a 6060 6020 7079  A..```....``` py
-00001970: 7468 6f6e 0d0a 6672 6f6d 2049 6e64 6f78  thon..from Indox
-00001980: 2e45 6d62 6564 6469 6e67 7320 696d 706f  .Embeddings impo
-00001990: 7274 204f 7065 6e41 6945 6d62 6564 6469  rt OpenAiEmbeddi
-000019a0: 6e67 0d0a 6060 600d 0a0d 0a0d 0a60 6060  ng..```......```
-000019b0: 2070 7974 686f 6e0d 0a6f 7065 6e61 695f   python..openai_
-000019c0: 7161 203d 204f 7065 6e41 6951 4128 6170  qa = OpenAiQA(ap
-000019d0: 695f 6b65 793d 4f50 454e 4149 5f41 5049  i_key=OPENAI_API
-000019e0: 5f4b 4559 2c6d 6f64 656c 3d22 6770 742d  _KEY,model="gpt-
-000019f0: 332e 352d 7475 7262 6f2d 3031 3235 2229  3.5-turbo-0125")
-00001a00: 0d0a 6f70 656e 6169 5f65 6d62 6564 6469  ..openai_embeddi
-00001a10: 6e67 7320 3d20 4f70 656e 4169 456d 6265  ngs = OpenAiEmbe
-00001a20: 6464 696e 6728 6d6f 6465 6c3d 2274 6578  dding(model="tex
-00001a30: 742d 656d 6265 6464 696e 672d 332d 736d  t-embedding-3-sm
-00001a40: 616c 6c22 2c6f 7065 6e61 695f 6170 695f  all",openai_api_
-00001a50: 6b65 793d 4f50 454e 4149 5f41 5049 5f4b  key=OPENAI_API_K
-00001a60: 4559 290d 0a60 6060 0d0a 0d0a 2323 204d  EY)..```....## M
-00001a70: 6f64 6966 7969 6e67 2043 6f6e 6669 6775  odifying Configu
-00001a80: 7261 7469 6f6e 2053 6574 7469 6e67 730d  ration Settings.
-00001a90: 0a0d 0a54 6f20 6368 616e 6765 2061 2063  ...To change a c
-00001aa0: 6f6e 6669 6775 7261 7469 6f6e 2073 6574  onfiguration set
-00001ab0: 7469 6e67 2c20 796f 7520 6361 6e20 6469  ting, you can di
-00001ac0: 7265 6374 6c79 206d 6f64 6966 7920 7468  rectly modify th
-00001ad0: 650d 0a60 496e 646f 782e 636f 6e66 6967  e..`Indox.config
-00001ae0: 6020 6469 6374 696f 6e61 7279 2e20 4865  ` dictionary. He
-00001af0: 7265 2069 7320 616e 2065 7861 6d70 6c65  re is an example
-00001b00: 206f 6620 686f 7720 796f 7520 6361 6e20   of how you can 
-00001b10: 7570 6461 7465 2061 0d0a 636f 6e66 6967  update a..config
-00001b20: 7572 6174 696f 6e20 7365 7474 696e 673a  uration setting:
-00001b30: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
-00001b40: 2320 4578 616d 706c 6520 6f66 206d 6f64  # Example of mod
-00001b50: 6966 7969 6e67 2061 2063 6f6e 6669 6775  ifying a configu
-00001b60: 7261 7469 6f6e 2073 6574 7469 6e67 0d0a  ration setting..
-00001b70: 496e 646f 782e 636f 6e66 6967 5b22 6f6c  Indox.config["ol
-00001b80: 645f 636f 6e66 6967 225d 203d 2022 6e65  d_config"] = "ne
-00001b90: 775f 636f 6e66 6967 220d 0a0d 0a23 2041  w_config"....# A
-00001ba0: 7070 6c79 696e 6720 7468 6520 7570 6461  pplying the upda
-00001bb0: 7465 6420 636f 6e66 6967 7572 6174 696f  ted configuratio
-00001bc0: 6e0d 0a49 6e64 6f78 2e75 7064 6174 655f  n..Indox.update_
-00001bd0: 636f 6e66 6967 2829 0d0a 6060 600d 0a0d  config()..```...
-00001be0: 0a0d 0a57 6520 7461 6b65 2061 6476 616e  ...We take advan
-00001bf0: 7461 6765 206f 6620 7468 6520 6075 6e73  tage of the `uns
-00001c00: 7472 7563 7475 7265 6460 206c 6962 7261  tructured` libra
-00001c10: 7279 2074 6f20 6c6f 6164 0d0a 646f 6375  ry to load..docu
-00001c20: 6d65 6e74 7320 616e 6420 7370 6c69 7420  ments and split 
-00001c30: 7468 656d 2069 6e74 6f20 6368 756e 6b73  them into chunks
-00001c40: 2062 7920 7469 746c 652e 2054 6869 7320   by title. This 
-00001c50: 6d65 7468 6f64 2068 656c 7073 2069 6e0d  method helps in.
-00001c60: 0a6f 7267 616e 697a 696e 6720 7468 6d65  .organizing thme
-00001c70: 2064 6f63 756d 656e 7420 696e 746f 206d   document into m
-00001c80: 616e 6167 6561 626c 6520 7365 6374 696f  anageable sectio
-00001c90: 6e73 2066 6f72 2066 7572 7468 6572 0d0a  ns for further..
-00001ca0: 7072 6f63 6573 7369 6e67 2e0d 0a0d 0a60  processing.....`
-00001cb0: 6060 2070 7974 686f 6e0d 0a66 726f 6d20  `` python..from 
-00001cc0: 496e 646f 782e 4461 7461 4c6f 6164 6572  Indox.DataLoader
-00001cd0: 5370 6c69 7474 6572 2069 6d70 6f72 7420  Splitter import 
-00001ce0: 556e 7374 7275 6374 7572 6564 4c6f 6164  UnstructuredLoad
-00001cf0: 416e 6453 706c 6974 0d0a 6060 600d 0a0d  AndSplit..```...
-00001d00: 0a60 6060 2070 7974 686f 6e0d 0a64 6f63  .``` python..doc
-00001d10: 735f 756e 7374 7275 6374 7572 6564 203d  s_unstructured =
-00001d20: 2055 6e73 7472 7563 7475 7265 644c 6f61   UnstructuredLoa
-00001d30: 6441 6e64 5370 6c69 7428 6669 6c65 5f70  dAndSplit(file_p
-00001d40: 6174 683d 6669 6c65 5f70 6174 6829 0d0a  ath=file_path)..
-00001d50: 6060 600d 0a0d 0a20 2020 2053 7461 7274  ```....    Start
-00001d60: 696e 6720 7072 6f63 6573 7369 6e67 2e2e  ing processing..
-00001d70: 2e0d 0a20 2020 2045 6e64 2043 6875 6e6b  ...    End Chunk
-00001d80: 696e 6720 7072 6f63 6573 732e 0d0a 0d0a  ing process.....
-00001d90: 5374 6f72 696e 6720 646f 6375 6d65 6e74  Storing document
-00001da0: 2063 6875 6e6b 7320 696e 2061 2076 6563   chunks in a vec
-00001db0: 746f 7220 7374 6f72 6520 6973 2063 7275  tor store is cru
-00001dc0: 6369 616c 2066 6f72 2065 6e61 626c 696e  cial for enablin
-00001dd0: 670d 0a65 6666 6963 6965 6e74 2072 6574  g..efficient ret
-00001de0: 7269 6576 616c 2061 6e64 2073 6561 7263  rieval and searc
-00001df0: 6820 6f70 6572 6174 696f 6e73 2e20 4279  h operations. By
-00001e00: 2063 6f6e 7665 7274 696e 6720 7465 7874   converting text
-00001e10: 2064 6174 6120 696e 746f 0d0a 7665 6374   data into..vect
-00001e20: 6f72 2072 6570 7265 7365 6e74 6174 696f  or representatio
-00001e30: 6e73 2061 6e64 2073 746f 7269 6e67 2074  ns and storing t
-00001e40: 6865 6d20 696e 2061 2076 6563 746f 7220  hem in a vector 
-00001e50: 7374 6f72 652c 2079 6f75 2063 616e 0d0a  store, you can..
-00001e60: 7065 7266 6f72 6d20 7261 7069 6420 7369  perform rapid si
-00001e70: 6d69 6c61 7269 7479 2073 6561 7263 6865  milarity searche
-00001e80: 7320 616e 6420 6f74 6865 7220 7665 6374  s and other vect
-00001e90: 6f72 2d62 6173 6564 206f 7065 7261 7469  or-based operati
-00001ea0: 6f6e 732e 0d0a 0d0a 6060 6020 7079 7468  ons.....``` pyth
-00001eb0: 6f6e 0d0a 496e 646f 782e 636f 6e6e 6563  on..Indox.connec
-00001ec0: 745f 746f 5f76 6563 746f 7273 746f 7265  t_to_vectorstore
-00001ed0: 2863 6f6c 6c65 6374 696f 6e5f 6e61 6d65  (collection_name
-00001ee0: 3d22 7361 6d70 6c65 222c 656d 6265 6464  ="sample",embedd
-00001ef0: 696e 6773 3d6f 7065 6e61 695f 656d 6265  ings=openai_embe
-00001f00: 6464 696e 6773 290d 0a49 6e64 6f78 2e73  ddings)..Indox.s
-00001f10: 746f 7265 5f69 6e5f 7665 6374 6f72 7374  tore_in_vectorst
-00001f20: 6f72 6528 6368 756e 6b73 3d64 6f63 735f  ore(chunks=docs_
-00001f30: 756e 7374 7275 6374 7572 6564 290d 0a60  unstructured)..`
-00001f40: 6060 0d0a 0d0a 2323 2051 7565 7269 6e67  ``....## Quering
-00001f50: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
-00001f60: 7175 6572 7920 3d20 2279 6f75 7220 7175  query = "your qu
-00001f70: 6572 7921 213f 3f22 0d0a 6060 600d 0a0d  ery!!??"..```...
-00001f80: 0a60 6060 2070 7974 686f 6e0d 0a72 6573  .``` python..res
-00001f90: 706f 6e73 655f 6f70 656e 6169 203d 2049  ponse_openai = I
-00001fa0: 6e64 6f78 2e61 6e73 7765 725f 7175 6573  ndox.answer_ques
-00001fb0: 7469 6f6e 2871 7565 7279 3d71 7565 7279  tion(query=query
-00001fc0: 2c71 615f 6d6f 6465 6c3d 6f70 656e 6169  ,qa_model=openai
-00001fd0: 5f71 6129 0d0a 6060 600d 0a0d 0a60 6060  _qa)..```....```
-00001fe0: 2070 7974 686f 6e0d 0a61 6e73 7765 7220   python..answer 
-00001ff0: 3d20 7265 7370 6f6e 7365 5f6f 7065 6e61  = response_opena
-00002000: 695b 305d 0d0a 6060 600d 0a0d 0a60 6060  i[0]..```....```
-00002010: 2070 7974 686f 6e0d 0a63 6f6e 7465 7874   python..context
-00002020: 2c20 7363 6f72 6520 3d20 7265 7370 6f6e  , score = respon
-00002030: 7365 5f6f 7065 6e61 695b 315d 0d0a 6060  se_openai[1]..``
-00002040: 600d 0a0d 0a                             `....
+00000540: 0a0d 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000550: 7465 7222 3e0d 0a0d 0a0d 0a3c 6833 2061  ter">......<h3 a
+00000560: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
+00000570: 2020 2020 3c69 6d67 2073 7263 3d22 646f      <img src="do
+00000580: 6373 2f6c 6974 652d 6c6f 676f 2031 2e70  cs/lite-logo 1.p
+00000590: 6e67 2220 616c 743d 224c 6f67 6f22 2073  ng" alt="Logo" s
+000005a0: 7479 6c65 3d22 7769 6474 683a 2038 3025  tyle="width: 80%
+000005b0: 3b20 6f70 6163 6974 793a 2030 2e37 3b22  ; opacity: 0.7;"
+000005c0: 2f3e 0d0a 0d0a 3c2f 6833 3e0d 0a0d 0a0d  />....</h3>.....
+000005d0: 0a3c 6469 7620 7374 796c 653d 2270 6f73  .<div style="pos
+000005e0: 6974 696f 6e3a 2072 656c 6174 6976 653b  ition: relative;
+000005f0: 2077 6964 7468 3a20 3130 3025 3b20 7465   width: 100%; te
+00000600: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00000610: 3b22 3e0d 0a3c 6831 3e0d 0a69 6e44 6f78  ;">..<h1>..inDox
+00000620: 200d 0a3c 7020 616c 6967 6e3d 2263 656e   ..<p align="cen
+00000630: 7465 7222 3e41 6476 616e 6365 6420 5365  ter">Advanced Se
+00000640: 6172 6368 2061 6e64 2052 6574 7269 6576  arch and Retriev
+00000650: 616c 2041 7567 6d65 6e74 6174 696f 6e20  al Augmentation 
+00000660: 4765 6e65 7261 7469 7665 0d0a 3c2f 703e  Generative..</p>
+00000670: 0d0a 0d0a 3c2f 6831 3e0d 0a0d 0a5b 215b  ....</h1>....[![
+00000680: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+00000690: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000006a0: 6769 7468 7562 2f6c 6963 656e 7365 2f6f  github/license/o
+000006b0: 736c 6c6d 6169 2f69 6e44 6f78 295d 2868  sllmai/inDox)](h
+000006c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006d0: 6d2f 6f73 6c6c 6d61 692f 696e 446f 782f  m/osllmai/inDox/
+000006e0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000006f0: 4529 0d0a 5b21 5b50 7950 495d 2868 7474  E)..[![PyPI](htt
+00000700: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+00000710: 696f 2f70 792f 496e 646f 782e 7376 6729  io/py/Indox.svg)
+00000720: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000730: 7267 2f70 726f 6a65 6374 2f49 6e64 6f78  rg/project/Indox
+00000740: 2f30 2e31 2e34 2f29 0d0a 5b21 5b50 7974  /0.1.4/)..[![Pyt
+00000750: 686f 6e5d 2868 7474 7073 3a2f 2f69 6d67  hon](https://img
+00000760: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000770: 2f70 7976 6572 7369 6f6e 732f 496e 646f  /pyversions/Indo
+00000780: 782e 7376 6729 5d28 6874 7470 733a 2f2f  x.svg)](https://
+00000790: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000007a0: 2f49 6e64 6f78 2f30 2e31 2e34 2f29 0d0a  /Indox/0.1.4/)..
+000007b0: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+000007c0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+000007d0: 792e 7465 6368 2f62 6164 6765 2f69 6e64  y.tech/badge/ind
+000007e0: 6f78 295d 2868 7474 7073 3a2f 2f70 6570  ox)](https://pep
+000007f0: 792e 7465 6368 2f70 726f 6a65 6374 2f69  y.tech/project/i
+00000800: 6e64 6f78 290d 0a0d 0a5b 215b 4469 7363  ndox)....[![Disc
+00000810: 6f72 645d 2868 7474 7073 3a2f 2f69 6d67  ord](https://img
+00000820: 2e73 6869 656c 6473 2e69 6f2f 6469 7363  .shields.io/disc
+00000830: 6f72 642f 3132 3233 3836 3733 3832 3436  ord/122386738246
+00000840: 3035 3739 3936 313f 6c61 6265 6c3d 4469  0579961?label=Di
+00000850: 7363 6f72 6426 6c6f 676f 3d44 6973 636f  scord&logo=Disco
+00000860: 7264 2673 7479 6c65 3d73 6f63 6961 6c29  rd&style=social)
+00000870: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+00000880: 642e 636f 6d2f 696e 7669 7465 2f6f 7373  d.com/invite/oss
+00000890: 6c6c 6d61 6929 0d0a 5b21 5b47 6974 4875  llmai)..[![GitHu
+000008a0: 6220 7374 6172 735d 2868 7474 7073 3a2f  b stars](https:/
+000008b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000008c0: 6769 7468 7562 2f73 7461 7273 2f6f 736c  github/stars/osl
+000008d0: 6c6d 6169 2f69 6e44 6f78 3f73 7479 6c65  lmai/inDox?style
+000008e0: 3d73 6f63 6961 6c29 5d28 6874 7470 733a  =social)](https:
+000008f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
+00000900: 6c6d 6169 2f69 6e44 6f78 290d 0a0d 0a0d  lmai/inDox).....
+00000910: 0a0d 0a0d 0a3c 7020 616c 6967 6e3d 2263  .....<p align="c
+00000920: 656e 7465 7222 3e0d 0a20 203c 6120 6872  enter">..  <a hr
+00000930: 6566 3d22 6874 7470 733a 2f2f 6f73 6c6c  ef="https://osll
+00000940: 6d2e 6169 223e 4f66 6669 6369 616c 2057  m.ai">Official W
+00000950: 6562 7369 7465 3c2f 613e 2026 6275 6c6c  ebsite</a> &bull
+00000960: 3b20 3c61 2068 7265 663d 2268 7474 7073  ; <a href="https
+00000970: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f73  ://github.com/os
+00000980: 6c6c 6d61 692f 696e 446f 782f 7769 6b69  llmai/inDox/wiki
+00000990: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+000009a0: 2f61 3e20 2662 756c 6c3b 203c 6120 6872  /a> &bull; <a hr
+000009b0: 6566 3d22 6874 7470 733a 2f2f 6469 7363  ef="https://disc
+000009c0: 6f72 642e 6767 2f71 7243 6335 365a 5222  ord.gg/qrCc56ZR"
+000009d0: 3e44 6973 636f 7264 3c2f 613e 0d0a 3c2f  >Discord</a>..</
+000009e0: 703e 0d0a 0d0a 0d0a 3c70 2061 6c69 676e  p>......<p align
+000009f0: 3d22 6365 6e74 6572 223e 0d0a 2020 3c62  ="center">..  <b
+00000a00: 3e4e 4557 3a3c 2f62 3e20 3c61 2068 7265  >NEW:</b> <a hre
+00000a10: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00000a20: 676f 6f67 6c65 2e63 6f6d 2f66 6f72 6d73  google.com/forms
+00000a30: 2f64 2f31 4351 584a 7678 4c55 714c 4253  /d/1CQXJvxLUqLBS
+00000a40: 586e 6a71 516d 5270 4f79 5a71 4436 6e72  XnjqQmRpOyZqD6nr
+00000a50: 4b75 624c 7a32 5754 6349 4a33 3766 552f  KubLz2WTcIJ37fU/
+00000a60: 7072 6566 696c 6c22 3e53 7562 7363 7269  prefill">Subscri
+00000a70: 6265 2074 6f20 6f75 7220 6d61 696c 696e  be to our mailin
+00000a80: 6720 6c69 7374 3c2f 613e 2066 6f72 2075  g list</a> for u
+00000a90: 7064 6174 6573 2061 6e64 206e 6577 7321  pdates and news!
+00000aa0: 0d0a 3c2f 703e 0d0a 0d0a 0d0a 0d0a 2a2a  ..</p>........**
+00000ab0: 496e 646f 7820 5265 7472 6965 7661 6c20  Indox Retrieval 
+00000ac0: 4175 676d 656e 7461 7469 6f6e 2a2a 2069  Augmentation** i
+00000ad0: 7320 616e 2069 6e6e 6f76 6174 6976 6520  s an innovative 
+00000ae0: 6170 706c 6963 6174 696f 6e20 6465 7369  application desi
+00000af0: 676e 6564 2074 6f20 7374 7265 616d 6c69  gned to streamli
+00000b00: 6e65 2069 6e66 6f72 6d61 7469 6f6e 2065  ne information e
+00000b10: 7874 7261 6374 696f 6e20 6672 6f6d 2061  xtraction from a
+00000b20: 2077 6964 650d 0a72 616e 6765 206f 6620   wide..range of 
+00000b30: 646f 6375 6d65 6e74 2074 7970 6573 2c20  document types, 
+00000b40: 696e 636c 7564 696e 6720 7465 7874 2066  including text f
+00000b50: 696c 6573 2c20 5044 462c 2048 544d 4c2c  iles, PDF, HTML,
+00000b60: 204d 6172 6b64 6f77 6e2c 2061 6e64 204c   Markdown, and L
+00000b70: 6154 6558 2e20 5768 6574 6865 7220 7374  aTeX. Whether st
+00000b80: 7275 6374 7572 6564 206f 7220 756e 7374  ructured or unst
+00000b90: 7275 6374 7572 6564 2c20 496e 646f 780d  ructured, Indox.
+00000ba0: 0a70 726f 7669 6465 7320 7573 6572 7320  .provides users 
+00000bb0: 7769 7468 2061 2070 6f77 6572 6675 6c20  with a powerful 
+00000bc0: 746f 6f6c 7365 7420 746f 2065 6666 6963  toolset to effic
+00000bd0: 6965 6e74 6c79 2065 7874 7261 6374 2072  iently extract r
+00000be0: 656c 6576 616e 7420 6461 7461 2e0d 0a0d  elevant data....
+00000bf0: 0a49 6e64 6f78 2052 6574 7269 6576 616c  .Indox Retrieval
+00000c00: 2041 7567 6d65 6e74 6174 696f 6e20 6973   Augmentation is
+00000c10: 2061 6e20 696e 6e6f 7661 7469 7665 2061   an innovative a
+00000c20: 7070 6c69 6361 7469 6f6e 2064 6573 6967  pplication desig
+00000c30: 6e65 6420 746f 2073 7472 6561 6d6c 696e  ned to streamlin
+00000c40: 6520 696e 666f 726d 6174 696f 6e20 6578  e information ex
+00000c50: 7472 6163 7469 6f6e 2066 726f 6d20 6120  traction from a 
+00000c60: 7769 6465 0d0a 7261 6e67 6520 6f66 2064  wide..range of d
+00000c70: 6f63 756d 656e 7420 7479 7065 732c 2069  ocument types, i
+00000c80: 6e63 6c75 6469 6e67 2074 6578 7420 6669  ncluding text fi
+00000c90: 6c65 732c 2050 4446 2c20 4854 4d4c 2c20  les, PDF, HTML, 
+00000ca0: 4d61 726b 646f 776e 2c20 616e 6420 4c61  Markdown, and La
+00000cb0: 5465 582e 2057 6865 7468 6572 2073 7472  TeX. Whether str
+00000cc0: 7563 7475 7265 6420 6f72 2075 6e73 7472  uctured or unstr
+00000cd0: 7563 7475 7265 642c 2049 6e64 6f78 0d0a  uctured, Indox..
+00000ce0: 7072 6f76 6964 6573 2075 7365 7273 2077  provides users w
+00000cf0: 6974 6820 6120 706f 7765 7266 756c 2074  ith a powerful t
+00000d00: 6f6f 6c73 6574 2074 6f20 6566 6669 6369  oolset to effici
+00000d10: 656e 746c 7920 6578 7472 6163 7420 7265  ently extract re
+00000d20: 6c65 7661 6e74 2064 6174 612e 204f 6e65  levant data. One
+00000d30: 206f 6620 6974 7320 6b65 7920 6665 6174   of its key feat
+00000d40: 7572 6573 2069 7320 7468 6520 6162 696c  ures is the abil
+00000d50: 6974 7920 746f 0d0a 696e 7465 6c6c 6967  ity to..intellig
+00000d60: 656e 746c 7920 636c 7573 7465 7220 7072  ently cluster pr
+00000d70: 696d 6172 7920 6368 756e 6b73 2074 6f20  imary chunks to 
+00000d80: 666f 726d 206d 6f72 6520 726f 6275 7374  form more robust
+00000d90: 2067 726f 7570 696e 6773 2c20 656e 6861   groupings, enha
+00000da0: 6e63 696e 6720 7468 6520 7175 616c 6974  ncing the qualit
+00000db0: 7920 616e 6420 7265 6c65 7661 6e63 6520  y and relevance 
+00000dc0: 6f66 2074 6865 2065 7874 7261 6374 6564  of the extracted
+00000dd0: 0d0a 696e 666f 726d 6174 696f 6e2e 0d0a  ..information...
+00000de0: 5769 7468 2061 2066 6f63 7573 206f 6e20  With a focus on 
+00000df0: 6164 6170 7461 6269 6c69 7479 2061 6e64  adaptability and
+00000e00: 2075 7365 722d 6365 6e74 7269 6320 6465   user-centric de
+00000e10: 7369 676e 2c20 496e 646f 7820 6169 6d73  sign, Indox aims
+00000e20: 2074 6f20 6465 6c69 7665 7220 6675 7475   to deliver futu
+00000e30: 7265 2d72 6561 6479 2066 756e 6374 696f  re-ready functio
+00000e40: 6e61 6c69 7479 2077 6974 6820 6d6f 7265  nality with more
+00000e50: 0d0a 6665 6174 7572 6573 2070 6c61 6e6e  ..features plann
+00000e60: 6564 2066 6f72 2075 7063 6f6d 696e 6720  ed for upcoming 
+00000e70: 7265 6c65 6173 6573 2e20 4a6f 696e 2075  releases. Join u
+00000e80: 7320 696e 2065 7870 6c6f 7269 6e67 2068  s in exploring h
+00000e90: 6f77 2049 6e64 6f78 2063 616e 2072 6576  ow Indox can rev
+00000ea0: 6f6c 7574 696f 6e69 7a65 2079 6f75 7220  olutionize your 
+00000eb0: 646f 6375 6d65 6e74 2070 726f 6365 7373  document process
+00000ec0: 696e 670d 0a77 6f72 6b66 6c6f 772c 2062  ing..workflow, b
+00000ed0: 7269 6e67 696e 6720 636c 6172 6974 7920  ringing clarity 
+00000ee0: 616e 6420 6f72 6761 6e69 7a61 7469 6f6e  and organization
+00000ef0: 2074 6f20 796f 7572 2064 6174 6120 7265   to your data re
+00000f00: 7472 6965 7661 6c20 6e65 6564 732e 0d0a  trieval needs...
+00000f10: 0d0a 2323 2044 6570 656e 6465 6e63 7920  ..## Dependency 
+00000f20: 5265 7175 6972 656d 656e 7473 0d0a 0d0a  Requirements....
+00000f30: 4265 666f 7265 2072 756e 6e69 6e67 2074  Before running t
+00000f40: 6869 7320 7072 6f6a 6563 742c 2065 6e73  his project, ens
+00000f50: 7572 6520 7468 6174 2079 6f75 2068 6176  ure that you hav
+00000f60: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00000f70: 696e 7374 616c 6c65 643a 0d0a 0d0a 2d20  installed:....- 
+00000f80: 2a2a 5079 7468 6f6e 2033 2e38 2b2a 2a3a  **Python 3.8+**:
+00000f90: 2052 6571 7569 7265 6420 666f 7220 7275   Required for ru
+00000fa0: 6e6e 696e 6720 7468 6520 5079 7468 6f6e  nning the Python
+00000fb0: 2062 6163 6b65 6e64 2e0d 0a2d 202a 2a50   backend...- **P
+00000fc0: 6f73 7467 7265 5351 4c2a 2a3a 204e 6565  ostgreSQL**: Nee
+00000fd0: 6465 6420 6966 2079 6f75 2077 6973 6820  ded if you wish 
+00000fe0: 746f 2073 746f 7265 2079 6f75 7220 6461  to store your da
+00000ff0: 7461 2069 6e20 6120 506f 7374 6772 6553  ta in a PostgreS
+00001000: 514c 2064 6174 6162 6173 652e 0d0a 2d20  QL database...- 
+00001010: 2a2a 4f70 656e 4149 2041 5049 204b 6579  **OpenAI API Key
+00001020: 2a2a 3a20 4e65 6365 7373 6172 7920 6966  **: Necessary if
+00001030: 2079 6f75 2061 7265 2075 7369 6e67 2074   you are using t
+00001040: 6865 204f 7065 6e41 4920 656d 6265 6464  he OpenAI embedd
+00001050: 696e 6720 6d6f 6465 6c2e 0d0a 2d20 2a2a  ing model...- **
+00001060: 4875 6767 696e 6746 6163 6520 4150 4920  HuggingFace API 
+00001070: 4b65 792a 2a3a 204e 6563 6573 7361 7279  Key**: Necessary
+00001080: 2069 6620 796f 7520 6172 6520 7573 696e   if you are usin
+00001090: 6720 7468 6520 4875 6767 696e 6746 6163  g the HuggingFac
+000010a0: 6520 6c6c 6d73 2e0d 0a0d 0a45 6e73 7572  e llms.....Ensur
+000010b0: 6520 796f 7572 2073 7973 7465 6d20 616c  e your system al
+000010c0: 736f 206d 6565 7473 2074 6865 7365 2072  so meets these r
+000010d0: 6571 7569 7265 6d65 6e74 733a 0d0a 0d0a  equirements:....
+000010e0: 2d20 4163 6365 7373 2074 6f20 656e 7669  - Access to envi
+000010f0: 726f 6e6d 656e 7461 6c20 7661 7269 6162  ronmental variab
+00001100: 6c65 7320 666f 7220 6861 6e64 6c69 6e67  les for handling
+00001110: 2073 656e 7369 7469 7665 2069 6e66 6f72   sensitive infor
+00001120: 6d61 7469 6f6e 206c 696b 6520 4150 4920  mation like API 
+00001130: 6b65 7973 2e0d 0a2d 2053 7569 7461 626c  keys...- Suitabl
+00001140: 6520 6861 7264 7761 7265 2063 6170 6162  e hardware capab
+00001150: 6c65 206f 6620 7375 7070 6f72 7469 6e67  le of supporting
+00001160: 2069 6e74 656e 7369 7665 2063 6f6d 7075   intensive compu
+00001170: 7461 7469 6f6e 616c 2074 6173 6b73 2e0d  tational tasks..
+00001180: 0a0d 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00001190: 6f6e 0d0a 0d0a 0d0a 2323 2047 6574 7469  on......## Getti
+000011a0: 6e67 2053 7461 7274 6564 0d0a 0d0a 5468  ng Started....Th
+000011b0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+000011c0: 616e 6420 7769 6c6c 2069 6e73 7461 6c6c  and will install
+000011d0: 2074 6865 206c 6174 6573 7420 7374 6162   the latest stab
+000011e0: 6c65 2069 6e44 6f78 0d0a 0d0a 6060 600d  le inDox....```.
+000011f0: 0a70 6970 2069 6e73 7461 6c6c 2049 6e64  .pip install Ind
+00001200: 6f78 0d0a 6060 600d 0a0d 0a54 6f20 696e  ox..```....To in
+00001210: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
+00001220: 2064 6576 656c 6f70 6d65 6e74 2076 6572   development ver
+00001230: 7369 6f6e 2c20 796f 7520 6d61 7920 7275  sion, you may ru
+00001240: 6e0d 0a0d 0a60 6060 0d0a 7069 7020 696e  n....```..pip in
+00001250: 7374 616c 6c20 6769 742b 6874 7470 733a  stall git+https:
+00001260: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
+00001270: 6c6d 6169 2f69 6e44 6f78 406d 6169 6e0d  lmai/inDox@main.
+00001280: 0a60 6060 0d0a 0d0a 546f 2063 6f6e 6669  .```....To confi
+00001290: 6775 7265 2074 6865 2043 4c49 2c20 7275  gure the CLI, ru
+000012a0: 6e0d 0a0d 0a60 6060 0d0a 696e 646f 7820  n....```..indox 
+000012b0: 636f 6e66 6967 7572 650d 0a60 6060 0d0a  configure..```..
+000012c0: 0d0a 0d0a 436c 6f6e 6520 7468 6520 7265  ....Clone the re
+000012d0: 706f 7369 746f 7279 2061 6e64 206e 6176  pository and nav
+000012e0: 6967 6174 6520 746f 2074 6865 2064 6972  igate to the dir
+000012f0: 6563 746f 7279 3a0d 0a0d 0a60 6060 6261  ectory:....```ba
+00001300: 7368 0d0a 6769 7420 636c 6f6e 6520 6874  sh..git clone ht
+00001310: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001320: 2f6f 736c 6c6d 6169 2f69 6e44 6f78 2e67  /osllmai/inDox.g
+00001330: 6974 0d0a 6364 2069 6e44 6f78 0d0a 6060  it..cd inDox..``
+00001340: 600d 0a0d 0a49 6e73 7461 6c6c 2074 6865  `....Install the
+00001350: 2072 6571 7569 7265 6420 5079 7468 6f6e   required Python
+00001360: 2070 6163 6b61 6765 733a 0d0a 0d0a 6060   packages:....``
+00001370: 6062 6173 680d 0a70 6970 2069 6e73 7461  `bash..pip insta
+00001380: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
+00001390: 7473 2e74 7874 0d0a 6060 600d 0a0d 0a23  ts.txt..```....#
+000013a0: 2320 436f 6e66 6967 7572 6174 696f 6e0d  # Configuration.
+000013b0: 0a0d 0a23 2323 2045 6e76 6972 6f6e 6d65  ...### Environme
+000013c0: 6e74 2056 6172 6961 626c 6573 0d0a 0d0a  nt Variables....
+000013d0: 5365 7420 796f 7572 2060 4f50 454e 4149  Set your `OPENAI
+000013e0: 5f41 5049 5f4b 4559 6020 6f72 2060 4846  _API_KEY` or `HF
+000013f0: 5f41 5049 5f4b 4559 6020 696e 2079 6f75  _API_KEY` in you
+00001400: 7220 656e 7669 726f 6e6d 656e 7420 7661  r environment va
+00001410: 7269 6162 6c65 7320 666f 7220 7365 6375  riables for secu
+00001420: 7265 2061 6363 6573 732e 0d0a 0d0a 2323  re access.....##
+00001430: 2320 4461 7461 6261 7365 2053 6574 7570  # Database Setup
+00001440: 0d0a 0d0a 456e 7375 7265 2079 6f75 7220  ....Ensure your 
+00001450: 506f 7374 6772 6553 514c 2064 6174 6162  PostgreSQL datab
+00001460: 6173 6520 6973 2075 7020 616e 6420 7275  ase is up and ru
+00001470: 6e6e 696e 672c 2061 6e64 2061 6363 6573  nning, and acces
+00001480: 7369 626c 6520 6672 6f6d 2079 6f75 7220  sible from your 
+00001490: 6170 706c 6963 6174 696f 6e2e 2054 6869  application. Thi
+000014a0: 7320 6973 206e 6563 6573 7361 7279 2069  s is necessary i
+000014b0: 6620 796f 7520 706c 616e 2074 6f20 7573  f you plan to us
+000014c0: 6520 7067 7665 6374 6f72 2061 7320 796f  e pgvector as yo
+000014d0: 7572 2076 6563 746f 7220 7374 6f72 652e  ur vector store.
+000014e0: 0d0a 0d0a 416c 7465 726e 6174 6976 656c  ....Alternativel
+000014f0: 792c 2079 6f75 2063 616e 2075 7365 2043  y, you can use C
+00001500: 6872 6f6d 6120 6f72 2046 6169 7373 2061  hroma or Faiss a
+00001510: 7320 796f 7572 2076 6563 746f 7220 7374  s your vector st
+00001520: 6f72 652e 204d 616b 6520 7375 7265 2074  ore. Make sure t
+00001530: 6f20 7370 6563 6966 7920 796f 7572 2063  o specify your c
+00001540: 686f 6963 6520 616e 6420 7468 6520 6e65  hoice and the ne
+00001550: 6365 7373 6172 7920 636f 6e66 6967 7572  cessary configur
+00001560: 6174 696f 6e73 2069 6e20 7468 6520 636f  ations in the co
+00001570: 6e66 6967 2e79 616d 6c20 6669 6c65 2e0d  nfig.yaml file..
+00001580: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a23  ...## Usage....#
+00001590: 2323 2050 7265 7061 7269 6e67 2059 6f75  ## Preparing You
+000015a0: 7220 4461 7461 0d0a 0d0a 312e 202a 2a44  r Data....1. **D
+000015b0: 6566 696e 6520 7468 6520 4669 6c65 2050  efine the File P
+000015c0: 6174 682a 2a3a 2053 7065 6369 6679 2074  ath**: Specify t
+000015d0: 6865 2070 6174 6820 746f 2079 6f75 7220  he path to your 
+000015e0: 7465 7874 206f 7220 5044 4620 6669 6c65  text or PDF file
+000015f0: 2e0d 0a32 2e20 2a2a 4c6f 6164 2045 6d62  ...2. **Load Emb
+00001600: 6564 6469 6e67 204d 6f64 656c 732a 2a3a  edding Models**:
+00001610: 2049 6e69 7469 616c 697a 6520 796f 7572   Initialize your
+00001620: 2065 6d62 6564 6469 6e67 206d 6f64 656c   embedding model
+00001630: 2066 726f 6d20 4f70 656e 4149 2773 2073   from OpenAI's s
+00001640: 656c 6563 7469 6f6e 206f 6620 7072 652d  election of pre-
+00001650: 7472 6169 6e65 6420 6d6f 6465 6c73 2e0d  trained models..
+00001660: 0a0d 0a23 2051 7569 636b 2053 7461 7274  ...# Quick Start
+00001670: 200d 0a0d 0a23 2320 496d 706f 7274 2049   ....## Import I
+00001680: 6e64 6f78 2050 6163 6b61 6765 0d0a 0d0a  ndox Package....
+00001690: 496d 706f 7274 2074 6865 206e 6563 6573  Import the neces
+000016a0: 7361 7279 2063 6c61 7373 6573 2066 726f  sary classes fro
+000016b0: 6d20 7468 6520 496e 646f 7820 7061 636b  m the Indox pack
+000016c0: 6167 652e 0d0a 0d0a 6060 6020 7079 7468  age.....``` pyth
+000016d0: 6f6e 0d0a 6672 6f6d 2049 6e64 6f78 2069  on..from Indox i
+000016e0: 6d70 6f72 7420 496e 646f 7852 6574 7269  mport IndoxRetri
+000016f0: 6576 616c 4175 676d 656e 7461 7469 6f6e  evalAugmentation
+00001700: 0d0a 6060 600d 0a0d 0a23 2323 2049 6e69  ..```....### Ini
+00001710: 7469 616c 697a 6520 496e 646f 780d 0a0d  tialize Indox...
+00001720: 0a43 7265 6174 6520 616e 2069 6e73 7461  .Create an insta
+00001730: 6e63 6520 6f66 2049 6e64 6f78 5265 7472  nce of IndoxRetr
+00001740: 6965 7661 6c41 7567 6d65 6e74 6174 696f  ievalAugmentatio
+00001750: 6e2e 0d0a 0d0a 6060 6020 7079 7468 6f6e  n.....``` python
+00001760: 0d0a 496e 646f 7820 3d20 496e 646f 7852  ..Indox = IndoxR
+00001770: 6574 7269 6576 616c 4175 676d 656e 7461  etrievalAugmenta
+00001780: 7469 6f6e 2829 0d0a 6060 600d 0a23 2320  tion()..```..## 
+00001790: 496e 6974 6961 6c20 436f 6e66 6967 7572  Initial Configur
+000017a0: 6174 696f 6e0d 0a0d 0a2d 202a 2a43 6f6e  ation....- **Con
+000017b0: 6669 6775 7261 7469 6f6e 2046 696c 652a  figuration File*
+000017c0: 2a3a 2045 6e73 7572 6520 796f 7520 6c6f  *: Ensure you lo
+000017d0: 6361 7465 2061 6e64 206d 6f64 6966 7920  cate and modify 
+000017e0: 7468 6520 6049 6e64 6f78 2e63 6f6e 6669  the `Indox.confi
+000017f0: 6760 2059 414d 4c20 6669 6c65 2061 6363  g` YAML file acc
+00001800: 6f72 6469 6e67 2074 6f20 796f 7572 206e  ording to your n
+00001810: 6565 6473 2062 6566 6f72 650d 0a20 2073  eeds before..  s
+00001820: 7461 7274 696e 6720 7468 6520 6170 706c  tarting the appl
+00001830: 6963 6174 696f 6e2e 0d0a 0d0a 2323 2044  ication.....## D
+00001840: 796e 616d 6963 2043 6f6e 6669 6775 7261  ynamic Configura
+00001850: 7469 6f6e 2043 6861 6e67 6573 0d0a 0d0a  tion Changes....
+00001860: 466f 7220 6368 616e 6765 7320 7468 6174  For changes that
+00001870: 206e 6565 6420 746f 2062 6520 6170 706c   need to be appl
+00001880: 6965 6420 6166 7465 7220 7468 6520 696e  ied after the in
+00001890: 6974 6961 6c20 7365 7475 7020 6f72 2064  itial setup or d
+000018a0: 7572 696e 6720 7275 6e74 696d 653a 0d0a  uring runtime:..
+000018b0: 0d0a 2d20 2a2a 4d6f 6469 6679 696e 6720  ..- **Modifying 
+000018c0: 436f 6e66 6967 7572 6174 696f 6e73 2a2a  Configurations**
+000018d0: 3a20 5573 6520 7468 6520 666f 6c6c 6f77  : Use the follow
+000018e0: 696e 6720 5079 7468 6f6e 2073 6e69 7070  ing Python snipp
+000018f0: 6574 2074 6f20 7570 6461 7465 2079 6f75  et to update you
+00001900: 7220 7365 7474 696e 6773 2064 796e 616d  r settings dynam
+00001910: 6963 616c 6c79 3a0d 0a20 2060 6060 7079  ically:..  ```py
+00001920: 7468 6f6e 0d0a 2020 496e 646f 782e 636f  thon..  Indox.co
+00001930: 6e66 6967 5b22 796f 7572 5f73 6574 7469  nfig["your_setti
+00001940: 6e67 5f74 6861 745f 6e65 6564 5f74 6f5f  ng_that_need_to_
+00001950: 6368 616e 6765 225d 203d 2022 6e65 775f  change"] = "new_
+00001960: 7365 7474 696e 6722 0d0a 2020 496e 646f  setting"..  Indo
+00001970: 782e 7570 6461 7465 5f63 6f6e 6669 6728  x.update_config(
+00001980: 290d 0a0d 0a23 2320 436f 6e66 6967 7572  )....## Configur
+00001990: 6174 696f 6e20 4465 7461 696c 730d 0a0d  ation Details...
+000019a0: 0a48 6572 6527 7320 6120 6272 6561 6b64  .Here's a breakd
+000019b0: 6f77 6e20 6f66 2074 6865 2063 6f6e 6669  own of the confi
+000019c0: 6720 6469 6374 696f 6e61 7279 2061 6e64  g dictionary and
+000019d0: 2069 7473 2070 726f 7065 7274 6965 733a   its properties:
+000019e0: 0d0a 0d0a 2323 2320 506f 7374 6772 6553  ....### PostgreS
+000019f0: 514c 0d0a 0d0a 2d20 6063 6f6e 6e5f 7374  QL....- `conn_st
+00001a00: 7269 6e67 603a 2059 6f75 7220 506f 7374  ring`: Your Post
+00001a10: 6772 6553 514c 2064 6174 6162 6173 6520  greSQL database 
+00001a20: 6372 6564 656e 7469 616c 732e 0d0a 0d0a  credentials.....
+00001a30: 2323 2320 5375 6d6d 6172 7920 4d6f 6465  ### Summary Mode
+00001a40: 6c0d 0a0d 0a2d 2060 6d61 785f 746f 6b65  l....- `max_toke
+00001a50: 6e73 603a 204d 6178 696d 756d 2074 6f6b  ns`: Maximum tok
+00001a60: 656e 2063 6f75 6e74 2074 6865 2073 756d  en count the sum
+00001a70: 6d61 7279 206d 6f64 656c 2063 616e 2067  mary model can g
+00001a80: 656e 6572 6174 652e 0d0a 2d20 606d 696e  enerate...- `min
+00001a90: 5f6c 656e 603a 204d 696e 696d 756d 2074  _len`: Minimum t
+00001aa0: 6f6b 656e 2063 6f75 6e74 2074 6865 2073  oken count the s
+00001ab0: 756d 6d61 7279 206d 6f64 656c 2067 656e  ummary model gen
+00001ac0: 6572 6174 6573 2e0d 0a2d 2060 6d6f 6465  erates...- `mode
+00001ad0: 6c5f 6e61 6d65 603a 2044 6566 6175 6c74  l_name`: Default
+00001ae0: 2069 7320 6067 7074 2d33 2e35 2d74 7572   is `gpt-3.5-tur
+00001af0: 626f 2d30 3132 3560 2c20 6275 7420 6974  bo-0125`, but it
+00001b00: 2063 616e 2062 6520 7265 706c 6163 6564   can be replaced
+00001b10: 2077 6974 6820 616e 7920 4875 6767 696e   with any Huggin
+00001b20: 6720 4661 6365 206d 6f64 656c 2073 7570  g Face model sup
+00001b30: 706f 7274 696e 6720 7468 650d 0a20 2073  porting the..  s
+00001b40: 756d 6d61 7269 7a61 7469 6f6e 2070 6970  ummarization pip
+00001b50: 656c 696e 652e 0d0a 0d0a 2323 2320 506f  eline.....### Po
+00001b60: 7374 6772 6553 514c 2053 6574 7570 2077  stgreSQL Setup w
+00001b70: 6974 6820 7067 7665 6374 6f72 0d0a 0d0a  ith pgvector....
+00001b80: 4966 2079 6f75 2077 616e 7420 746f 2075  If you want to u
+00001b90: 7365 2050 6f73 7467 7265 5351 4c20 666f  se PostgreSQL fo
+00001ba0: 7220 7665 6374 6f72 2073 746f 7261 6765  r vector storage
+00001bb0: 2c20 796f 7520 7368 6f75 6c64 2070 6572  , you should per
+00001bc0: 666f 726d 2074 6865 2066 6f6c 6c6f 7769  form the followi
+00001bd0: 6e67 2073 7465 7073 3a0d 0a0d 0a31 2e20  ng steps:....1. 
+00001be0: 2a2a 496e 7374 616c 6c20 7067 7665 6374  **Install pgvect
+00001bf0: 6f72 2a2a 3a20 546f 2069 6e73 7461 6c6c  or**: To install
+00001c00: 2060 7067 7665 6374 6f72 6020 6f6e 2079   `pgvector` on y
+00001c10: 6f75 7220 506f 7374 6772 6553 514c 2073  our PostgreSQL s
+00001c20: 6572 7665 722c 2066 6f6c 6c6f 7720 7468  erver, follow th
+00001c30: 6520 6465 7461 696c 6564 2069 6e73 7461  e detailed insta
+00001c40: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
+00001c50: 696f 6e73 0d0a 2020 2061 7661 696c 6162  ions..   availab
+00001c60: 6c65 206f 6e20 7468 6520 6f66 6669 6369  le on the offici
+00001c70: 616c 2070 6776 6563 746f 7220 4769 7448  al pgvector GitH
+00001c80: 7562 2072 6570 6f73 6974 6f72 793a 0d0a  ub repository:..
+00001c90: 2020 205b 7067 7665 6374 6f72 2049 6e73     [pgvector Ins
+00001ca0: 7461 6c6c 6174 696f 6e20 496e 7374 7275  tallation Instru
+00001cb0: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
+00001cc0: 6769 7468 7562 2e63 6f6d 2f70 6776 6563  github.com/pgvec
+00001cd0: 746f 722f 7067 7665 6374 6f72 290d 0a0d  tor/pgvector)...
+00001ce0: 0a32 2e20 2a2a 4164 6420 5665 6374 6f72  .2. **Add Vector
+00001cf0: 2045 7874 656e 7369 6f6e 2a2a 3a0d 0a20   Extension**:.. 
+00001d00: 2020 436f 6e6e 6563 7420 746f 2079 6f75    Connect to you
+00001d10: 7220 506f 7374 6772 6553 514c 2064 6174  r PostgreSQL dat
+00001d20: 6162 6173 6520 616e 6420 6578 6563 7574  abase and execut
+00001d30: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001d40: 5351 4c20 636f 6d6d 616e 6420 746f 2063  SQL command to c
+00001d50: 7265 6174 6520 7468 6520 6070 6776 6563  reate the `pgvec
+00001d60: 746f 7260 2065 7874 656e 7369 6f6e 3a0d  tor` extension:.
+00001d70: 0a0d 0a20 2020 6060 6073 716c 0d0a 2020  ...   ```sql..  
+00001d80: 202d 2d20 436f 6e6e 6563 7420 746f 2079   -- Connect to y
+00001d90: 6f75 7220 6461 7461 6261 7365 0d0a 2020  our database..  
+00001da0: 2070 7371 6c20 2d55 2075 7365 726e 616d   psql -U usernam
+00001db0: 6520 2d64 2064 6174 6162 6173 655f 6e61  e -d database_na
+00001dc0: 6d65 0d0a 0d0a 2020 202d 2d20 5275 6e20  me....   -- Run 
+00001dd0: 696e 7369 6465 2079 6f75 7220 7073 716c  inside your psql
+00001de0: 2074 6572 6d69 6e61 6c0d 0a20 2020 4352   terminal..   CR
+00001df0: 4541 5445 2045 5854 454e 5349 4f4e 2076  EATE EXTENSION v
+00001e00: 6563 746f 723b 0d0a 2020 2023 2052 6570  ector;..   # Rep
+00001e10: 6c61 6365 2074 6865 2070 6c61 6365 686f  lace the placeho
+00001e20: 6c64 6572 7320 7769 7468 2079 6f75 7220  lders with your 
+00001e30: 6163 7475 616c 2050 6f73 7467 7265 5351  actual PostgreSQ
+00001e40: 4c20 6372 6564 656e 7469 616c 7320 616e  L credentials an
+00001e50: 6420 6465 7461 696c 730d 0a0d 0a41 6464  d details....Add
+00001e60: 6974 696f 6e61 6c6c 792c 2066 6f72 2074  itionally, for t
+00001e70: 686f 7365 2069 6e74 6572 6573 7465 6420  hose interested 
+00001e80: 696e 2065 7870 6c6f 7269 6e67 206f 7468  in exploring oth
+00001e90: 6572 2076 6563 746f 7220 6461 7461 6261  er vector databa
+00001ea0: 7365 206f 7074 696f 6e73 2c20 796f 7520  se options, you 
+00001eb0: 6361 6e20 636f 6e73 6964 6572 2075 7369  can consider usi
+00001ec0: 6e67 202a 2a43 6872 6f6d 612a 2a20 6f72  ng **Chroma** or
+00001ed0: 202a 0d0a 2a46 6169 7373 2a2a 2e20 5468   *..*Faiss**. Th
+00001ee0: 6573 6520 7072 6f76 6964 6520 616c 7465  ese provide alte
+00001ef0: 726e 6174 6976 6520 6170 7072 6f61 6368  rnative approach
+00001f00: 6573 2074 6f20 7665 6374 6f72 2073 746f  es to vector sto
+00001f10: 7261 6765 2061 6e64 2072 6574 7269 6576  rage and retriev
+00001f20: 616c 2074 6861 7420 6d61 7920 6265 7474  al that may bett
+00001f30: 6572 2073 7569 7420 7370 6563 6966 6963  er suit specific
+00001f40: 2075 7365 2063 6173 6573 0d0a 6f72 2070   use cases..or p
+00001f50: 6572 666f 726d 616e 6365 2072 6571 7569  erformance requi
+00001f60: 7265 6d65 6e74 732e 0d0a 0d0a 2323 2320  rements.....### 
+00001f70: 496d 706f 7274 696e 6720 5141 2061 6e64  Importing QA and
+00001f80: 2045 6d62 6564 6469 6e67 204d 6f64 656c   Embedding Model
+00001f90: 730d 0a0d 0a60 6060 2070 7974 686f 6e0d  s....``` python.
+00001fa0: 0a66 726f 6d20 496e 646f 782e 5161 4d6f  .from Indox.QaMo
+00001fb0: 6465 6c73 2069 6d70 6f72 7420 4f70 656e  dels import Open
+00001fc0: 4169 5141 0d0a 6060 600d 0a0d 0a60 6060  AiQA..```....```
+00001fd0: 2070 7974 686f 6e0d 0a66 726f 6d20 496e   python..from In
+00001fe0: 646f 782e 456d 6265 6464 696e 6773 2069  dox.Embeddings i
+00001ff0: 6d70 6f72 7420 4f70 656e 4169 456d 6265  mport OpenAiEmbe
+00002000: 6464 696e 670d 0a60 6060 0d0a 0d0a 0d0a  dding..```......
+00002010: 6060 6020 7079 7468 6f6e 0d0a 6f70 656e  ``` python..open
+00002020: 6169 5f71 6120 3d20 4f70 656e 4169 5141  ai_qa = OpenAiQA
+00002030: 2861 7069 5f6b 6579 3d4f 5045 4e41 495f  (api_key=OPENAI_
+00002040: 4150 495f 4b45 592c 6d6f 6465 6c3d 2267  API_KEY,model="g
+00002050: 7074 2d33 2e35 2d74 7572 626f 2d30 3132  pt-3.5-turbo-012
+00002060: 3522 290d 0a6f 7065 6e61 695f 656d 6265  5")..openai_embe
+00002070: 6464 696e 6773 203d 204f 7065 6e41 6945  ddings = OpenAiE
+00002080: 6d62 6564 6469 6e67 286d 6f64 656c 3d22  mbedding(model="
+00002090: 7465 7874 2d65 6d62 6564 6469 6e67 2d33  text-embedding-3
+000020a0: 2d73 6d61 6c6c 222c 6f70 656e 6169 5f61  -small",openai_a
+000020b0: 7069 5f6b 6579 3d4f 5045 4e41 495f 4150  pi_key=OPENAI_AP
+000020c0: 495f 4b45 5929 0d0a 6060 600d 0a0d 0a23  I_KEY)..```....#
+000020d0: 2320 4d6f 6469 6679 696e 6720 436f 6e66  # Modifying Conf
+000020e0: 6967 7572 6174 696f 6e20 5365 7474 696e  iguration Settin
+000020f0: 6773 0d0a 0d0a 546f 2063 6861 6e67 6520  gs....To change 
+00002100: 6120 636f 6e66 6967 7572 6174 696f 6e20  a configuration 
+00002110: 7365 7474 696e 672c 2079 6f75 2063 616e  setting, you can
+00002120: 2064 6972 6563 746c 7920 6d6f 6469 6679   directly modify
+00002130: 2074 6865 0d0a 6049 6e64 6f78 2e63 6f6e   the..`Indox.con
+00002140: 6669 6760 2064 6963 7469 6f6e 6172 792e  fig` dictionary.
+00002150: 2048 6572 6520 6973 2061 6e20 6578 616d   Here is an exam
+00002160: 706c 6520 6f66 2068 6f77 2079 6f75 2063  ple of how you c
+00002170: 616e 2075 7064 6174 6520 610d 0a63 6f6e  an update a..con
+00002180: 6669 6775 7261 7469 6f6e 2073 6574 7469  figuration setti
+00002190: 6e67 3a0d 0a0d 0a60 6060 2070 7974 686f  ng:....``` pytho
+000021a0: 6e0d 0a23 2045 7861 6d70 6c65 206f 6620  n..# Example of 
+000021b0: 6d6f 6469 6679 696e 6720 6120 636f 6e66  modifying a conf
+000021c0: 6967 7572 6174 696f 6e20 7365 7474 696e  iguration settin
+000021d0: 670d 0a49 6e64 6f78 2e63 6f6e 6669 675b  g..Indox.config[
+000021e0: 226f 6c64 5f63 6f6e 6669 6722 5d20 3d20  "old_config"] = 
+000021f0: 226e 6577 5f63 6f6e 6669 6722 0d0a 0d0a  "new_config"....
+00002200: 2320 4170 706c 7969 6e67 2074 6865 2075  # Applying the u
+00002210: 7064 6174 6564 2063 6f6e 6669 6775 7261  pdated configura
+00002220: 7469 6f6e 0d0a 496e 646f 782e 7570 6461  tion..Indox.upda
+00002230: 7465 5f63 6f6e 6669 6728 290d 0a60 6060  te_config()..```
+00002240: 0d0a 0d0a 0d0a 5765 2074 616b 6520 6164  ......We take ad
+00002250: 7661 6e74 6167 6520 6f66 2074 6865 2060  vantage of the `
+00002260: 756e 7374 7275 6374 7572 6564 6020 6c69  unstructured` li
+00002270: 6272 6172 7920 746f 206c 6f61 640d 0a64  brary to load..d
+00002280: 6f63 756d 656e 7473 2061 6e64 2073 706c  ocuments and spl
+00002290: 6974 2074 6865 6d20 696e 746f 2063 6875  it them into chu
+000022a0: 6e6b 7320 6279 2074 6974 6c65 2e20 5468  nks by title. Th
+000022b0: 6973 206d 6574 686f 6420 6865 6c70 7320  is method helps 
+000022c0: 696e 0d0a 6f72 6761 6e69 7a69 6e67 2074  in..organizing t
+000022d0: 686d 6520 646f 6375 6d65 6e74 2069 6e74  hme document int
+000022e0: 6f20 6d61 6e61 6765 6162 6c65 2073 6563  o manageable sec
+000022f0: 7469 6f6e 7320 666f 7220 6675 7274 6865  tions for furthe
+00002300: 720d 0a70 726f 6365 7373 696e 672e 0d0a  r..processing...
+00002310: 0d0a 6060 6020 7079 7468 6f6e 0d0a 6672  ..``` python..fr
+00002320: 6f6d 2049 6e64 6f78 2e44 6174 614c 6f61  om Indox.DataLoa
+00002330: 6465 7253 706c 6974 7465 7220 696d 706f  derSplitter impo
+00002340: 7274 2055 6e73 7472 7563 7475 7265 644c  rt UnstructuredL
+00002350: 6f61 6441 6e64 5370 6c69 740d 0a60 6060  oadAndSplit..```
+00002360: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
+00002370: 646f 6373 5f75 6e73 7472 7563 7475 7265  docs_unstructure
+00002380: 6420 3d20 556e 7374 7275 6374 7572 6564  d = Unstructured
+00002390: 4c6f 6164 416e 6453 706c 6974 2866 696c  LoadAndSplit(fil
+000023a0: 655f 7061 7468 3d66 696c 655f 7061 7468  e_path=file_path
+000023b0: 290d 0a60 6060 0d0a 0d0a 2020 2020 5374  )..```....    St
+000023c0: 6172 7469 6e67 2070 726f 6365 7373 696e  arting processin
+000023d0: 672e 2e2e 0d0a 2020 2020 456e 6420 4368  g.....    End Ch
+000023e0: 756e 6b69 6e67 2070 726f 6365 7373 2e0d  unking process..
+000023f0: 0a0d 0a53 746f 7269 6e67 2064 6f63 756d  ...Storing docum
+00002400: 656e 7420 6368 756e 6b73 2069 6e20 6120  ent chunks in a 
+00002410: 7665 6374 6f72 2073 746f 7265 2069 7320  vector store is 
+00002420: 6372 7563 6961 6c20 666f 7220 656e 6162  crucial for enab
+00002430: 6c69 6e67 0d0a 6566 6669 6369 656e 7420  ling..efficient 
+00002440: 7265 7472 6965 7661 6c20 616e 6420 7365  retrieval and se
+00002450: 6172 6368 206f 7065 7261 7469 6f6e 732e  arch operations.
+00002460: 2042 7920 636f 6e76 6572 7469 6e67 2074   By converting t
+00002470: 6578 7420 6461 7461 2069 6e74 6f0d 0a76  ext data into..v
+00002480: 6563 746f 7220 7265 7072 6573 656e 7461  ector representa
+00002490: 7469 6f6e 7320 616e 6420 7374 6f72 696e  tions and storin
+000024a0: 6720 7468 656d 2069 6e20 6120 7665 6374  g them in a vect
+000024b0: 6f72 2073 746f 7265 2c20 796f 7520 6361  or store, you ca
+000024c0: 6e0d 0a70 6572 666f 726d 2072 6170 6964  n..perform rapid
+000024d0: 2073 696d 696c 6172 6974 7920 7365 6172   similarity sear
+000024e0: 6368 6573 2061 6e64 206f 7468 6572 2076  ches and other v
+000024f0: 6563 746f 722d 6261 7365 6420 6f70 6572  ector-based oper
+00002500: 6174 696f 6e73 2e0d 0a0d 0a60 6060 2070  ations.....``` p
+00002510: 7974 686f 6e0d 0a49 6e64 6f78 2e63 6f6e  ython..Indox.con
+00002520: 6e65 6374 5f74 6f5f 7665 6374 6f72 7374  nect_to_vectorst
+00002530: 6f72 6528 636f 6c6c 6563 7469 6f6e 5f6e  ore(collection_n
+00002540: 616d 653d 2273 616d 706c 6522 2c65 6d62  ame="sample",emb
+00002550: 6564 6469 6e67 733d 6f70 656e 6169 5f65  eddings=openai_e
+00002560: 6d62 6564 6469 6e67 7329 0d0a 496e 646f  mbeddings)..Indo
+00002570: 782e 7374 6f72 655f 696e 5f76 6563 746f  x.store_in_vecto
+00002580: 7273 746f 7265 2863 6875 6e6b 733d 646f  rstore(chunks=do
+00002590: 6373 5f75 6e73 7472 7563 7475 7265 6429  cs_unstructured)
+000025a0: 0d0a 6060 600d 0a0d 0a23 2320 5175 6572  ..```....## Quer
+000025b0: 696e 670d 0a0d 0a60 6060 2070 7974 686f  ing....``` pytho
+000025c0: 6e0d 0a71 7565 7279 203d 2022 796f 7572  n..query = "your
+000025d0: 2071 7565 7279 2121 3f3f 220d 0a60 6060   query!!??"..```
+000025e0: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
+000025f0: 7265 7370 6f6e 7365 5f6f 7065 6e61 6920  response_openai 
+00002600: 3d20 496e 646f 782e 616e 7377 6572 5f71  = Indox.answer_q
+00002610: 7565 7374 696f 6e28 7175 6572 793d 7175  uestion(query=qu
+00002620: 6572 792c 7161 5f6d 6f64 656c 3d6f 7065  ery,qa_model=ope
+00002630: 6e61 695f 7161 290d 0a60 6060 0d0a 0d0a  nai_qa)..```....
+00002640: 6060 6020 7079 7468 6f6e 0d0a 616e 7377  ``` python..answ
+00002650: 6572 203d 2072 6573 706f 6e73 655f 6f70  er = response_op
+00002660: 656e 6169 5b30 5d0d 0a60 6060 0d0a 0d0a  enai[0]..```....
+00002670: 6060 6020 7079 7468 6f6e 0d0a 636f 6e74  ``` python..cont
+00002680: 6578 742c 2073 636f 7265 203d 2072 6573  ext, score = res
+00002690: 706f 6e73 655f 6f70 656e 6169 5b31 5d0d  ponse_openai[1].
+000026a0: 0a60 6060 0d0a 0d0a                      .```....
```

### Comparing `indox-0.1.4/README.md` & `Indox-0.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,433 +1,535 @@
-00000000: 2320 696e 446f 783a 2041 6476 616e 6365  # inDox: Advance
-00000010: 6420 5365 6172 6368 2061 6e64 2052 6574  d Search and Ret
-00000020: 7269 6576 616c 2041 7567 6d65 6e74 6174  rieval Augmentat
-00000030: 696f 6e20 4765 6e65 7261 7469 7665 0d0a  ion Generative..
-00000040: 0d0a 2a2a 496e 646f 7820 5265 7472 6965  ..**Indox Retrie
-00000050: 7661 6c20 4175 676d 656e 7461 7469 6f6e  val Augmentation
-00000060: 2a2a 2069 7320 616e 2069 6e6e 6f76 6174  ** is an innovat
-00000070: 6976 6520 6170 706c 6963 6174 696f 6e20  ive application 
-00000080: 6465 7369 676e 6564 2074 6f20 7374 7265  designed to stre
-00000090: 616d 6c69 6e65 2069 6e66 6f72 6d61 7469  amline informati
-000000a0: 6f6e 2065 7874 7261 6374 696f 6e20 6672  on extraction fr
-000000b0: 6f6d 2061 2077 6964 650d 0a72 616e 6765  om a wide..range
-000000c0: 206f 6620 646f 6375 6d65 6e74 2074 7970   of document typ
-000000d0: 6573 2c20 696e 636c 7564 696e 6720 7465  es, including te
-000000e0: 7874 2066 696c 6573 2c20 5044 462c 2048  xt files, PDF, H
-000000f0: 544d 4c2c 204d 6172 6b64 6f77 6e2c 2061  TML, Markdown, a
-00000100: 6e64 204c 6154 6558 2e20 5768 6574 6865  nd LaTeX. Whethe
-00000110: 7220 7374 7275 6374 7572 6564 206f 7220  r structured or 
-00000120: 756e 7374 7275 6374 7572 6564 2c20 496e  unstructured, In
-00000130: 646f 780d 0a70 726f 7669 6465 7320 7573  dox..provides us
-00000140: 6572 7320 7769 7468 2061 2070 6f77 6572  ers with a power
-00000150: 6675 6c20 746f 6f6c 7365 7420 746f 2065  ful toolset to e
-00000160: 6666 6963 6965 6e74 6c79 2065 7874 7261  fficiently extra
-00000170: 6374 2072 656c 6576 616e 7420 6461 7461  ct relevant data
-00000180: 2e0d 0a0d 0a49 6e64 6f78 2052 6574 7269  .....Indox Retri
-00000190: 6576 616c 2041 7567 6d65 6e74 6174 696f  eval Augmentatio
-000001a0: 6e20 6973 2061 6e20 696e 6e6f 7661 7469  n is an innovati
-000001b0: 7665 2061 7070 6c69 6361 7469 6f6e 2064  ve application d
-000001c0: 6573 6967 6e65 6420 746f 2073 7472 6561  esigned to strea
-000001d0: 6d6c 696e 6520 696e 666f 726d 6174 696f  mline informatio
-000001e0: 6e20 6578 7472 6163 7469 6f6e 2066 726f  n extraction fro
-000001f0: 6d20 6120 7769 6465 0d0a 7261 6e67 6520  m a wide..range 
-00000200: 6f66 2064 6f63 756d 656e 7420 7479 7065  of document type
-00000210: 732c 2069 6e63 6c75 6469 6e67 2074 6578  s, including tex
-00000220: 7420 6669 6c65 732c 2050 4446 2c20 4854  t files, PDF, HT
-00000230: 4d4c 2c20 4d61 726b 646f 776e 2c20 616e  ML, Markdown, an
-00000240: 6420 4c61 5465 582e 2057 6865 7468 6572  d LaTeX. Whether
-00000250: 2073 7472 7563 7475 7265 6420 6f72 2075   structured or u
-00000260: 6e73 7472 7563 7475 7265 642c 2049 6e64  nstructured, Ind
-00000270: 6f78 0d0a 7072 6f76 6964 6573 2075 7365  ox..provides use
-00000280: 7273 2077 6974 6820 6120 706f 7765 7266  rs with a powerf
-00000290: 756c 2074 6f6f 6c73 6574 2074 6f20 6566  ul toolset to ef
-000002a0: 6669 6369 656e 746c 7920 6578 7472 6163  ficiently extrac
-000002b0: 7420 7265 6c65 7661 6e74 2064 6174 612e  t relevant data.
-000002c0: 204f 6e65 206f 6620 6974 7320 6b65 7920   One of its key 
-000002d0: 6665 6174 7572 6573 2069 7320 7468 6520  features is the 
-000002e0: 6162 696c 6974 7920 746f 0d0a 696e 7465  ability to..inte
-000002f0: 6c6c 6967 656e 746c 7920 636c 7573 7465  lligently cluste
-00000300: 7220 7072 696d 6172 7920 6368 756e 6b73  r primary chunks
-00000310: 2074 6f20 666f 726d 206d 6f72 6520 726f   to form more ro
-00000320: 6275 7374 2067 726f 7570 696e 6773 2c20  bust groupings, 
-00000330: 656e 6861 6e63 696e 6720 7468 6520 7175  enhancing the qu
-00000340: 616c 6974 7920 616e 6420 7265 6c65 7661  ality and releva
-00000350: 6e63 6520 6f66 2074 6865 2065 7874 7261  nce of the extra
-00000360: 6374 6564 0d0a 696e 666f 726d 6174 696f  cted..informatio
-00000370: 6e2e 0d0a 5769 7468 2061 2066 6f63 7573  n...With a focus
-00000380: 206f 6e20 6164 6170 7461 6269 6c69 7479   on adaptability
-00000390: 2061 6e64 2075 7365 722d 6365 6e74 7269   and user-centri
-000003a0: 6320 6465 7369 676e 2c20 496e 646f 7820  c design, Indox 
-000003b0: 6169 6d73 2074 6f20 6465 6c69 7665 7220  aims to deliver 
-000003c0: 6675 7475 7265 2d72 6561 6479 2066 756e  future-ready fun
-000003d0: 6374 696f 6e61 6c69 7479 2077 6974 6820  ctionality with 
-000003e0: 6d6f 7265 0d0a 6665 6174 7572 6573 2070  more..features p
-000003f0: 6c61 6e6e 6564 2066 6f72 2075 7063 6f6d  lanned for upcom
-00000400: 696e 6720 7265 6c65 6173 6573 2e20 4a6f  ing releases. Jo
-00000410: 696e 2075 7320 696e 2065 7870 6c6f 7269  in us in explori
-00000420: 6e67 2068 6f77 2049 6e64 6f78 2063 616e  ng how Indox can
-00000430: 2072 6576 6f6c 7574 696f 6e69 7a65 2079   revolutionize y
-00000440: 6f75 7220 646f 6375 6d65 6e74 2070 726f  our document pro
-00000450: 6365 7373 696e 670d 0a77 6f72 6b66 6c6f  cessing..workflo
-00000460: 772c 2062 7269 6e67 696e 6720 636c 6172  w, bringing clar
-00000470: 6974 7920 616e 6420 6f72 6761 6e69 7a61  ity and organiza
-00000480: 7469 6f6e 2074 6f20 796f 7572 2064 6174  tion to your dat
-00000490: 6120 7265 7472 6965 7661 6c20 6e65 6564  a retrieval need
-000004a0: 732e 0d0a 0d0a 2323 2050 7265 7265 7175  s.....## Prerequ
-000004b0: 6973 6974 6573 0d0a 0d0a 4265 666f 7265  isites....Before
-000004c0: 2072 756e 6e69 6e67 2074 6869 7320 7072   running this pr
-000004d0: 6f6a 6563 742c 2065 6e73 7572 6520 7468  oject, ensure th
-000004e0: 6174 2079 6f75 2068 6176 6520 7468 6520  at you have the 
-000004f0: 666f 6c6c 6f77 696e 6720 696e 7374 616c  following instal
-00000500: 6c65 643a 0d0a 0d0a 2d20 2a2a 5079 7468  led:....- **Pyth
-00000510: 6f6e 2033 2e38 2b2a 2a3a 2052 6571 7569  on 3.8+**: Requi
-00000520: 7265 6420 666f 7220 7275 6e6e 696e 6720  red for running 
-00000530: 7468 6520 5079 7468 6f6e 2062 6163 6b65  the Python backe
-00000540: 6e64 2e0d 0a2d 202a 2a50 6f73 7467 7265  nd...- **Postgre
-00000550: 5351 4c2a 2a3a 204e 6565 6465 6420 6966  SQL**: Needed if
-00000560: 2079 6f75 2077 6973 6820 746f 2073 746f   you wish to sto
-00000570: 7265 2079 6f75 7220 6461 7461 2069 6e20  re your data in 
-00000580: 6120 506f 7374 6772 6553 514c 2064 6174  a PostgreSQL dat
-00000590: 6162 6173 652e 0d0a 2d20 2a2a 4f70 656e  abase...- **Open
-000005a0: 4149 2041 5049 204b 6579 2a2a 3a20 4e65  AI API Key**: Ne
-000005b0: 6365 7373 6172 7920 6966 2079 6f75 2061  cessary if you a
-000005c0: 7265 2075 7369 6e67 2074 6865 204f 7065  re using the Ope
-000005d0: 6e41 4920 656d 6265 6464 696e 6720 6d6f  nAI embedding mo
-000005e0: 6465 6c2e 0d0a 2d20 2a2a 4875 6767 696e  del...- **Huggin
-000005f0: 6746 6163 6520 4150 4920 4b65 792a 2a3a  gFace API Key**:
-00000600: 204e 6563 6573 7361 7279 2069 6620 796f   Necessary if yo
-00000610: 7520 6172 6520 7573 696e 6720 7468 6520  u are using the 
-00000620: 4875 6767 696e 6746 6163 6520 6c6c 6d73  HuggingFace llms
-00000630: 2e0d 0a0d 0a45 6e73 7572 6520 796f 7572  .....Ensure your
-00000640: 2073 7973 7465 6d20 616c 736f 206d 6565   system also mee
-00000650: 7473 2074 6865 7365 2072 6571 7569 7265  ts these require
-00000660: 6d65 6e74 733a 0d0a 0d0a 2d20 4163 6365  ments:....- Acce
-00000670: 7373 2074 6f20 656e 7669 726f 6e6d 656e  ss to environmen
-00000680: 7461 6c20 7661 7269 6162 6c65 7320 666f  tal variables fo
-00000690: 7220 6861 6e64 6c69 6e67 2073 656e 7369  r handling sensi
-000006a0: 7469 7665 2069 6e66 6f72 6d61 7469 6f6e  tive information
-000006b0: 206c 696b 6520 4150 4920 6b65 7973 2e0d   like API keys..
-000006c0: 0a2d 2053 7569 7461 626c 6520 6861 7264  .- Suitable hard
-000006d0: 7761 7265 2063 6170 6162 6c65 206f 6620  ware capable of 
-000006e0: 7375 7070 6f72 7469 6e67 2069 6e74 656e  supporting inten
-000006f0: 7369 7665 2063 6f6d 7075 7461 7469 6f6e  sive computation
-00000700: 616c 2074 6173 6b73 2e0d 0a0d 0a23 2320  al tasks.....## 
-00000710: 496e 7374 616c 6c61 7469 6f6e 0d0a 0d0a  Installation....
-00000720: 436c 6f6e 6520 7468 6520 7265 706f 7369  Clone the reposi
-00000730: 746f 7279 2061 6e64 206e 6176 6967 6174  tory and navigat
-00000740: 6520 746f 2074 6865 2064 6972 6563 746f  e to the directo
-00000750: 7279 3a0d 0a0d 0a60 6060 6261 7368 0d0a  ry:....```bash..
-00000760: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-00000770: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
-00000780: 6c6d 6169 2f69 6e44 6f78 2e67 6974 0d0a  lmai/inDox.git..
-00000790: 6364 2069 6e44 6f78 0d0a 6060 600d 0a0d  cd inDox..```...
-000007a0: 0a49 6e73 7461 6c6c 2074 6865 2072 6571  .Install the req
-000007b0: 7569 7265 6420 5079 7468 6f6e 2070 6163  uired Python pac
-000007c0: 6b61 6765 733a 0d0a 0d0a 6060 6062 6173  kages:....```bas
-000007d0: 680d 0a70 6970 2069 6e73 7461 6c6c 202d  h..pip install -
-000007e0: 7220 7265 7175 6972 656d 656e 7473 2e74  r requirements.t
-000007f0: 7874 0d0a 6060 600d 0a0d 0a23 2320 436f  xt..```....## Co
-00000800: 6e66 6967 7572 6174 696f 6e0d 0a0d 0a23  nfiguration....#
-00000810: 2323 2045 6e76 6972 6f6e 6d65 6e74 2056  ## Environment V
-00000820: 6172 6961 626c 6573 0d0a 0d0a 5365 7420  ariables....Set 
-00000830: 796f 7572 2060 4f50 454e 4149 5f41 5049  your `OPENAI_API
-00000840: 5f4b 4559 6020 6f72 2060 4846 5f41 5049  _KEY` or `HF_API
-00000850: 5f4b 4559 6020 696e 2079 6f75 7220 656e  _KEY` in your en
-00000860: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00000870: 6c65 7320 666f 7220 7365 6375 7265 2061  les for secure a
-00000880: 6363 6573 732e 0d0a 0d0a 2323 2320 4461  ccess.....### Da
-00000890: 7461 6261 7365 2053 6574 7570 0d0a 0d0a  tabase Setup....
-000008a0: 456e 7375 7265 2079 6f75 7220 506f 7374  Ensure your Post
-000008b0: 6772 6553 514c 2064 6174 6162 6173 6520  greSQL database 
-000008c0: 6973 2075 7020 616e 6420 7275 6e6e 696e  is up and runnin
-000008d0: 672c 2061 6e64 2061 6363 6573 7369 626c  g, and accessibl
-000008e0: 6520 6672 6f6d 2079 6f75 7220 6170 706c  e from your appl
-000008f0: 6963 6174 696f 6e2e 2054 6869 7320 6973  ication. This is
-00000900: 206e 6563 6573 7361 7279 2069 6620 796f   necessary if yo
-00000910: 7520 706c 616e 2074 6f20 7573 6520 7067  u plan to use pg
-00000920: 7665 6374 6f72 2061 7320 796f 7572 2076  vector as your v
-00000930: 6563 746f 7220 7374 6f72 652e 0d0a 0d0a  ector store.....
-00000940: 416c 7465 726e 6174 6976 656c 792c 2079  Alternatively, y
-00000950: 6f75 2063 616e 2075 7365 2043 6872 6f6d  ou can use Chrom
-00000960: 6120 6f72 2046 6169 7373 2061 7320 796f  a or Faiss as yo
-00000970: 7572 2076 6563 746f 7220 7374 6f72 652e  ur vector store.
-00000980: 204d 616b 6520 7375 7265 2074 6f20 7370   Make sure to sp
-00000990: 6563 6966 7920 796f 7572 2063 686f 6963  ecify your choic
-000009a0: 6520 616e 6420 7468 6520 6e65 6365 7373  e and the necess
-000009b0: 6172 7920 636f 6e66 6967 7572 6174 696f  ary configuratio
-000009c0: 6e73 2069 6e20 7468 6520 636f 6e66 6967  ns in the config
-000009d0: 2e79 616d 6c20 6669 6c65 2e0d 0a0d 0a23  .yaml file.....#
-000009e0: 2320 5573 6167 650d 0a0d 0a23 2323 2050  # Usage....### P
-000009f0: 7265 7061 7269 6e67 2059 6f75 7220 4461  reparing Your Da
-00000a00: 7461 0d0a 0d0a 312e 202a 2a44 6566 696e  ta....1. **Defin
-00000a10: 6520 7468 6520 4669 6c65 2050 6174 682a  e the File Path*
-00000a20: 2a3a 2053 7065 6369 6679 2074 6865 2070  *: Specify the p
-00000a30: 6174 6820 746f 2079 6f75 7220 7465 7874  ath to your text
-00000a40: 206f 7220 5044 4620 6669 6c65 2e0d 0a32   or PDF file...2
-00000a50: 2e20 2a2a 4c6f 6164 2045 6d62 6564 6469  . **Load Embeddi
-00000a60: 6e67 204d 6f64 656c 732a 2a3a 2049 6e69  ng Models**: Ini
-00000a70: 7469 616c 697a 6520 796f 7572 2065 6d62  tialize your emb
-00000a80: 6564 6469 6e67 206d 6f64 656c 2066 726f  edding model fro
-00000a90: 6d20 4f70 656e 4149 2773 2073 656c 6563  m OpenAI's selec
-00000aa0: 7469 6f6e 206f 6620 7072 652d 7472 6169  tion of pre-trai
-00000ab0: 6e65 6420 6d6f 6465 6c73 2e0d 0a0d 0a23  ned models.....#
-00000ac0: 2051 7569 636b 2053 7461 7274 200d 0a0d   Quick Start ...
-00000ad0: 0a23 2320 496d 706f 7274 2049 6e64 6f78  .## Import Indox
-00000ae0: 2050 6163 6b61 6765 0d0a 0d0a 496d 706f   Package....Impo
-00000af0: 7274 2074 6865 206e 6563 6573 7361 7279  rt the necessary
-00000b00: 2063 6c61 7373 6573 2066 726f 6d20 7468   classes from th
-00000b10: 6520 496e 646f 7820 7061 636b 6167 652e  e Indox package.
-00000b20: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
-00000b30: 6672 6f6d 2049 6e64 6f78 2069 6d70 6f72  from Indox impor
-00000b40: 7420 496e 646f 7852 6574 7269 6576 616c  t IndoxRetrieval
-00000b50: 4175 676d 656e 7461 7469 6f6e 0d0a 6060  Augmentation..``
-00000b60: 600d 0a0d 0a23 2323 2049 6e69 7469 616c  `....### Initial
-00000b70: 697a 6520 496e 646f 780d 0a0d 0a43 7265  ize Indox....Cre
-00000b80: 6174 6520 616e 2069 6e73 7461 6e63 6520  ate an instance 
-00000b90: 6f66 2049 6e64 6f78 5265 7472 6965 7661  of IndoxRetrieva
-00000ba0: 6c41 7567 6d65 6e74 6174 696f 6e2e 0d0a  lAugmentation...
-00000bb0: 0d0a 6060 6020 7079 7468 6f6e 0d0a 496e  ..``` python..In
-00000bc0: 646f 7820 3d20 496e 646f 7852 6574 7269  dox = IndoxRetri
-00000bd0: 6576 616c 4175 676d 656e 7461 7469 6f6e  evalAugmentation
-00000be0: 2829 0d0a 6060 600d 0a23 2320 496e 6974  ()..```..## Init
-00000bf0: 6961 6c20 436f 6e66 6967 7572 6174 696f  ial Configuratio
-00000c00: 6e0d 0a0d 0a2d 202a 2a43 6f6e 6669 6775  n....- **Configu
-00000c10: 7261 7469 6f6e 2046 696c 652a 2a3a 2045  ration File**: E
-00000c20: 6e73 7572 6520 796f 7520 6c6f 6361 7465  nsure you locate
-00000c30: 2061 6e64 206d 6f64 6966 7920 7468 6520   and modify the 
-00000c40: 6049 6e64 6f78 2e63 6f6e 6669 6760 2059  `Indox.config` Y
-00000c50: 414d 4c20 6669 6c65 2061 6363 6f72 6469  AML file accordi
-00000c60: 6e67 2074 6f20 796f 7572 206e 6565 6473  ng to your needs
-00000c70: 2062 6566 6f72 650d 0a20 2073 7461 7274   before..  start
-00000c80: 696e 6720 7468 6520 6170 706c 6963 6174  ing the applicat
-00000c90: 696f 6e2e 0d0a 0d0a 2323 2044 796e 616d  ion.....## Dynam
-00000ca0: 6963 2043 6f6e 6669 6775 7261 7469 6f6e  ic Configuration
-00000cb0: 2043 6861 6e67 6573 0d0a 0d0a 466f 7220   Changes....For 
-00000cc0: 6368 616e 6765 7320 7468 6174 206e 6565  changes that nee
-00000cd0: 6420 746f 2062 6520 6170 706c 6965 6420  d to be applied 
-00000ce0: 6166 7465 7220 7468 6520 696e 6974 6961  after the initia
-00000cf0: 6c20 7365 7475 7020 6f72 2064 7572 696e  l setup or durin
-00000d00: 6720 7275 6e74 696d 653a 0d0a 0d0a 2d20  g runtime:....- 
-00000d10: 2a2a 4d6f 6469 6679 696e 6720 436f 6e66  **Modifying Conf
-00000d20: 6967 7572 6174 696f 6e73 2a2a 3a20 5573  igurations**: Us
-00000d30: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-00000d40: 5079 7468 6f6e 2073 6e69 7070 6574 2074  Python snippet t
-00000d50: 6f20 7570 6461 7465 2079 6f75 7220 7365  o update your se
-00000d60: 7474 696e 6773 2064 796e 616d 6963 616c  ttings dynamical
-00000d70: 6c79 3a0d 0a20 2060 6060 7079 7468 6f6e  ly:..  ```python
-00000d80: 0d0a 2020 496e 646f 782e 636f 6e66 6967  ..  Indox.config
-00000d90: 5b22 796f 7572 5f73 6574 7469 6e67 5f74  ["your_setting_t
-00000da0: 6861 745f 6e65 6564 5f74 6f5f 6368 616e  hat_need_to_chan
-00000db0: 6765 225d 203d 2022 6e65 775f 7365 7474  ge"] = "new_sett
-00000dc0: 696e 6722 0d0a 2020 496e 646f 782e 7570  ing"..  Indox.up
-00000dd0: 6461 7465 5f63 6f6e 6669 6728 290d 0a0d  date_config()...
-00000de0: 0a23 2320 436f 6e66 6967 7572 6174 696f  .## Configuratio
-00000df0: 6e20 4465 7461 696c 730d 0a0d 0a48 6572  n Details....Her
-00000e00: 6527 7320 6120 6272 6561 6b64 6f77 6e20  e's a breakdown 
-00000e10: 6f66 2074 6865 2063 6f6e 6669 6720 6469  of the config di
-00000e20: 6374 696f 6e61 7279 2061 6e64 2069 7473  ctionary and its
-00000e30: 2070 726f 7065 7274 6965 733a 0d0a 0d0a   properties:....
-00000e40: 2323 2320 506f 7374 6772 6553 514c 0d0a  ### PostgreSQL..
-00000e50: 0d0a 2d20 6063 6f6e 6e5f 7374 7269 6e67  ..- `conn_string
-00000e60: 603a 2059 6f75 7220 506f 7374 6772 6553  `: Your PostgreS
-00000e70: 514c 2064 6174 6162 6173 6520 6372 6564  QL database cred
-00000e80: 656e 7469 616c 732e 0d0a 0d0a 2323 2320  entials.....### 
-00000e90: 5375 6d6d 6172 7920 4d6f 6465 6c0d 0a0d  Summary Model...
-00000ea0: 0a2d 2060 6d61 785f 746f 6b65 6e73 603a  .- `max_tokens`:
-00000eb0: 204d 6178 696d 756d 2074 6f6b 656e 2063   Maximum token c
-00000ec0: 6f75 6e74 2074 6865 2073 756d 6d61 7279  ount the summary
-00000ed0: 206d 6f64 656c 2063 616e 2067 656e 6572   model can gener
-00000ee0: 6174 652e 0d0a 2d20 606d 696e 5f6c 656e  ate...- `min_len
-00000ef0: 603a 204d 696e 696d 756d 2074 6f6b 656e  `: Minimum token
-00000f00: 2063 6f75 6e74 2074 6865 2073 756d 6d61   count the summa
-00000f10: 7279 206d 6f64 656c 2067 656e 6572 6174  ry model generat
-00000f20: 6573 2e0d 0a2d 2060 6d6f 6465 6c5f 6e61  es...- `model_na
-00000f30: 6d65 603a 2044 6566 6175 6c74 2069 7320  me`: Default is 
-00000f40: 6067 7074 2d33 2e35 2d74 7572 626f 2d30  `gpt-3.5-turbo-0
-00000f50: 3132 3560 2c20 6275 7420 6974 2063 616e  125`, but it can
-00000f60: 2062 6520 7265 706c 6163 6564 2077 6974   be replaced wit
-00000f70: 6820 616e 7920 4875 6767 696e 6720 4661  h any Hugging Fa
-00000f80: 6365 206d 6f64 656c 2073 7570 706f 7274  ce model support
-00000f90: 696e 6720 7468 650d 0a20 2073 756d 6d61  ing the..  summa
-00000fa0: 7269 7a61 7469 6f6e 2070 6970 656c 696e  rization pipelin
-00000fb0: 652e 0d0a 0d0a 2323 2320 506f 7374 6772  e.....### Postgr
-00000fc0: 6553 514c 2053 6574 7570 2077 6974 6820  eSQL Setup with 
-00000fd0: 7067 7665 6374 6f72 0d0a 0d0a 4966 2079  pgvector....If y
-00000fe0: 6f75 2077 616e 7420 746f 2075 7365 2050  ou want to use P
-00000ff0: 6f73 7467 7265 5351 4c20 666f 7220 7665  ostgreSQL for ve
-00001000: 6374 6f72 2073 746f 7261 6765 2c20 796f  ctor storage, yo
-00001010: 7520 7368 6f75 6c64 2070 6572 666f 726d  u should perform
-00001020: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
-00001030: 7465 7073 3a0d 0a0d 0a31 2e20 2a2a 496e  teps:....1. **In
-00001040: 7374 616c 6c20 7067 7665 6374 6f72 2a2a  stall pgvector**
-00001050: 3a20 546f 2069 6e73 7461 6c6c 2060 7067  : To install `pg
-00001060: 7665 6374 6f72 6020 6f6e 2079 6f75 7220  vector` on your 
-00001070: 506f 7374 6772 6553 514c 2073 6572 7665  PostgreSQL serve
-00001080: 722c 2066 6f6c 6c6f 7720 7468 6520 6465  r, follow the de
-00001090: 7461 696c 6564 2069 6e73 7461 6c6c 6174  tailed installat
-000010a0: 696f 6e20 696e 7374 7275 6374 696f 6e73  ion instructions
-000010b0: 0d0a 2020 2061 7661 696c 6162 6c65 206f  ..   available o
-000010c0: 6e20 7468 6520 6f66 6669 6369 616c 2070  n the official p
-000010d0: 6776 6563 746f 7220 4769 7448 7562 2072  gvector GitHub r
-000010e0: 6570 6f73 6974 6f72 793a 0d0a 2020 205b  epository:..   [
-000010f0: 7067 7665 6374 6f72 2049 6e73 7461 6c6c  pgvector Install
-00001100: 6174 696f 6e20 496e 7374 7275 6374 696f  ation Instructio
-00001110: 6e73 5d28 6874 7470 733a 2f2f 6769 7468  ns](https://gith
-00001120: 7562 2e63 6f6d 2f70 6776 6563 746f 722f  ub.com/pgvector/
-00001130: 7067 7665 6374 6f72 290d 0a0d 0a32 2e20  pgvector)....2. 
-00001140: 2a2a 4164 6420 5665 6374 6f72 2045 7874  **Add Vector Ext
-00001150: 656e 7369 6f6e 2a2a 3a0d 0a20 2020 436f  ension**:..   Co
-00001160: 6e6e 6563 7420 746f 2079 6f75 7220 506f  nnect to your Po
-00001170: 7374 6772 6553 514c 2064 6174 6162 6173  stgreSQL databas
-00001180: 6520 616e 6420 6578 6563 7574 6520 7468  e and execute th
-00001190: 6520 666f 6c6c 6f77 696e 6720 5351 4c20  e following SQL 
-000011a0: 636f 6d6d 616e 6420 746f 2063 7265 6174  command to creat
-000011b0: 6520 7468 6520 6070 6776 6563 746f 7260  e the `pgvector`
-000011c0: 2065 7874 656e 7369 6f6e 3a0d 0a0d 0a20   extension:.... 
-000011d0: 2020 6060 6073 716c 0d0a 2020 202d 2d20    ```sql..   -- 
-000011e0: 436f 6e6e 6563 7420 746f 2079 6f75 7220  Connect to your 
-000011f0: 6461 7461 6261 7365 0d0a 2020 2070 7371  database..   psq
-00001200: 6c20 2d55 2075 7365 726e 616d 6520 2d64  l -U username -d
-00001210: 2064 6174 6162 6173 655f 6e61 6d65 0d0a   database_name..
-00001220: 0d0a 2020 202d 2d20 5275 6e20 696e 7369  ..   -- Run insi
-00001230: 6465 2079 6f75 7220 7073 716c 2074 6572  de your psql ter
-00001240: 6d69 6e61 6c0d 0a20 2020 4352 4541 5445  minal..   CREATE
-00001250: 2045 5854 454e 5349 4f4e 2076 6563 746f   EXTENSION vecto
-00001260: 723b 0d0a 2020 2023 2052 6570 6c61 6365  r;..   # Replace
-00001270: 2074 6865 2070 6c61 6365 686f 6c64 6572   the placeholder
-00001280: 7320 7769 7468 2079 6f75 7220 6163 7475  s with your actu
-00001290: 616c 2050 6f73 7467 7265 5351 4c20 6372  al PostgreSQL cr
-000012a0: 6564 656e 7469 616c 7320 616e 6420 6465  edentials and de
-000012b0: 7461 696c 730d 0a0d 0a41 6464 6974 696f  tails....Additio
-000012c0: 6e61 6c6c 792c 2066 6f72 2074 686f 7365  nally, for those
-000012d0: 2069 6e74 6572 6573 7465 6420 696e 2065   interested in e
-000012e0: 7870 6c6f 7269 6e67 206f 7468 6572 2076  xploring other v
-000012f0: 6563 746f 7220 6461 7461 6261 7365 206f  ector database o
-00001300: 7074 696f 6e73 2c20 796f 7520 6361 6e20  ptions, you can 
-00001310: 636f 6e73 6964 6572 2075 7369 6e67 202a  consider using *
-00001320: 2a43 6872 6f6d 612a 2a20 6f72 202a 0d0a  *Chroma** or *..
-00001330: 2a46 6169 7373 2a2a 2e20 5468 6573 6520  *Faiss**. These 
-00001340: 7072 6f76 6964 6520 616c 7465 726e 6174  provide alternat
-00001350: 6976 6520 6170 7072 6f61 6368 6573 2074  ive approaches t
-00001360: 6f20 7665 6374 6f72 2073 746f 7261 6765  o vector storage
-00001370: 2061 6e64 2072 6574 7269 6576 616c 2074   and retrieval t
-00001380: 6861 7420 6d61 7920 6265 7474 6572 2073  hat may better s
-00001390: 7569 7420 7370 6563 6966 6963 2075 7365  uit specific use
-000013a0: 2063 6173 6573 0d0a 6f72 2070 6572 666f   cases..or perfo
-000013b0: 726d 616e 6365 2072 6571 7569 7265 6d65  rmance requireme
-000013c0: 6e74 732e 0d0a 0d0a 2323 2320 496d 706f  nts.....### Impo
-000013d0: 7274 696e 6720 5141 2061 6e64 2045 6d62  rting QA and Emb
-000013e0: 6564 6469 6e67 204d 6f64 656c 730d 0a0d  edding Models...
-000013f0: 0a60 6060 2070 7974 686f 6e0d 0a66 726f  .``` python..fro
-00001400: 6d20 496e 646f 782e 5161 4d6f 6465 6c73  m Indox.QaModels
-00001410: 2069 6d70 6f72 7420 4f70 656e 4169 5141   import OpenAiQA
-00001420: 0d0a 6060 600d 0a0d 0a60 6060 2070 7974  ..```....``` pyt
-00001430: 686f 6e0d 0a66 726f 6d20 496e 646f 782e  hon..from Indox.
-00001440: 456d 6265 6464 696e 6773 2069 6d70 6f72  Embeddings impor
-00001450: 7420 4f70 656e 4169 456d 6265 6464 696e  t OpenAiEmbeddin
-00001460: 670d 0a60 6060 0d0a 0d0a 0d0a 6060 6020  g..```......``` 
-00001470: 7079 7468 6f6e 0d0a 6f70 656e 6169 5f71  python..openai_q
-00001480: 6120 3d20 4f70 656e 4169 5141 2861 7069  a = OpenAiQA(api
-00001490: 5f6b 6579 3d4f 5045 4e41 495f 4150 495f  _key=OPENAI_API_
-000014a0: 4b45 592c 6d6f 6465 6c3d 2267 7074 2d33  KEY,model="gpt-3
-000014b0: 2e35 2d74 7572 626f 2d30 3132 3522 290d  .5-turbo-0125").
-000014c0: 0a6f 7065 6e61 695f 656d 6265 6464 696e  .openai_embeddin
-000014d0: 6773 203d 204f 7065 6e41 6945 6d62 6564  gs = OpenAiEmbed
-000014e0: 6469 6e67 286d 6f64 656c 3d22 7465 7874  ding(model="text
-000014f0: 2d65 6d62 6564 6469 6e67 2d33 2d73 6d61  -embedding-3-sma
-00001500: 6c6c 222c 6f70 656e 6169 5f61 7069 5f6b  ll",openai_api_k
-00001510: 6579 3d4f 5045 4e41 495f 4150 495f 4b45  ey=OPENAI_API_KE
-00001520: 5929 0d0a 6060 600d 0a0d 0a23 2320 4d6f  Y)..```....## Mo
-00001530: 6469 6679 696e 6720 436f 6e66 6967 7572  difying Configur
-00001540: 6174 696f 6e20 5365 7474 696e 6773 0d0a  ation Settings..
-00001550: 0d0a 546f 2063 6861 6e67 6520 6120 636f  ..To change a co
-00001560: 6e66 6967 7572 6174 696f 6e20 7365 7474  nfiguration sett
-00001570: 696e 672c 2079 6f75 2063 616e 2064 6972  ing, you can dir
-00001580: 6563 746c 7920 6d6f 6469 6679 2074 6865  ectly modify the
-00001590: 0d0a 6049 6e64 6f78 2e63 6f6e 6669 6760  ..`Indox.config`
-000015a0: 2064 6963 7469 6f6e 6172 792e 2048 6572   dictionary. Her
-000015b0: 6520 6973 2061 6e20 6578 616d 706c 6520  e is an example 
-000015c0: 6f66 2068 6f77 2079 6f75 2063 616e 2075  of how you can u
-000015d0: 7064 6174 6520 610d 0a63 6f6e 6669 6775  pdate a..configu
-000015e0: 7261 7469 6f6e 2073 6574 7469 6e67 3a0d  ration setting:.
-000015f0: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a23  ...``` python..#
-00001600: 2045 7861 6d70 6c65 206f 6620 6d6f 6469   Example of modi
-00001610: 6679 696e 6720 6120 636f 6e66 6967 7572  fying a configur
-00001620: 6174 696f 6e20 7365 7474 696e 670d 0a49  ation setting..I
-00001630: 6e64 6f78 2e63 6f6e 6669 675b 226f 6c64  ndox.config["old
-00001640: 5f63 6f6e 6669 6722 5d20 3d20 226e 6577  _config"] = "new
-00001650: 5f63 6f6e 6669 6722 0d0a 0d0a 2320 4170  _config"....# Ap
-00001660: 706c 7969 6e67 2074 6865 2075 7064 6174  plying the updat
-00001670: 6564 2063 6f6e 6669 6775 7261 7469 6f6e  ed configuration
-00001680: 0d0a 496e 646f 782e 7570 6461 7465 5f63  ..Indox.update_c
-00001690: 6f6e 6669 6728 290d 0a60 6060 0d0a 0d0a  onfig()..```....
-000016a0: 0d0a 5765 2074 616b 6520 6164 7661 6e74  ..We take advant
-000016b0: 6167 6520 6f66 2074 6865 2060 756e 7374  age of the `unst
-000016c0: 7275 6374 7572 6564 6020 6c69 6272 6172  ructured` librar
-000016d0: 7920 746f 206c 6f61 640d 0a64 6f63 756d  y to load..docum
-000016e0: 656e 7473 2061 6e64 2073 706c 6974 2074  ents and split t
-000016f0: 6865 6d20 696e 746f 2063 6875 6e6b 7320  hem into chunks 
-00001700: 6279 2074 6974 6c65 2e20 5468 6973 206d  by title. This m
-00001710: 6574 686f 6420 6865 6c70 7320 696e 0d0a  ethod helps in..
-00001720: 6f72 6761 6e69 7a69 6e67 2074 686d 6520  organizing thme 
-00001730: 646f 6375 6d65 6e74 2069 6e74 6f20 6d61  document into ma
-00001740: 6e61 6765 6162 6c65 2073 6563 7469 6f6e  nageable section
-00001750: 7320 666f 7220 6675 7274 6865 720d 0a70  s for further..p
-00001760: 726f 6365 7373 696e 672e 0d0a 0d0a 6060  rocessing.....``
-00001770: 6020 7079 7468 6f6e 0d0a 6672 6f6d 2049  ` python..from I
-00001780: 6e64 6f78 2e44 6174 614c 6f61 6465 7253  ndox.DataLoaderS
-00001790: 706c 6974 7465 7220 696d 706f 7274 2055  plitter import U
-000017a0: 6e73 7472 7563 7475 7265 644c 6f61 6441  nstructuredLoadA
-000017b0: 6e64 5370 6c69 740d 0a60 6060 0d0a 0d0a  ndSplit..```....
-000017c0: 6060 6020 7079 7468 6f6e 0d0a 646f 6373  ``` python..docs
-000017d0: 5f75 6e73 7472 7563 7475 7265 6420 3d20  _unstructured = 
-000017e0: 556e 7374 7275 6374 7572 6564 4c6f 6164  UnstructuredLoad
-000017f0: 416e 6453 706c 6974 2866 696c 655f 7061  AndSplit(file_pa
-00001800: 7468 3d66 696c 655f 7061 7468 290d 0a60  th=file_path)..`
-00001810: 6060 0d0a 0d0a 2020 2020 5374 6172 7469  ``....    Starti
-00001820: 6e67 2070 726f 6365 7373 696e 672e 2e2e  ng processing...
-00001830: 0d0a 2020 2020 456e 6420 4368 756e 6b69  ..    End Chunki
-00001840: 6e67 2070 726f 6365 7373 2e0d 0a0d 0a53  ng process.....S
-00001850: 746f 7269 6e67 2064 6f63 756d 656e 7420  toring document 
-00001860: 6368 756e 6b73 2069 6e20 6120 7665 6374  chunks in a vect
-00001870: 6f72 2073 746f 7265 2069 7320 6372 7563  or store is cruc
-00001880: 6961 6c20 666f 7220 656e 6162 6c69 6e67  ial for enabling
-00001890: 0d0a 6566 6669 6369 656e 7420 7265 7472  ..efficient retr
-000018a0: 6965 7661 6c20 616e 6420 7365 6172 6368  ieval and search
-000018b0: 206f 7065 7261 7469 6f6e 732e 2042 7920   operations. By 
-000018c0: 636f 6e76 6572 7469 6e67 2074 6578 7420  converting text 
-000018d0: 6461 7461 2069 6e74 6f0d 0a76 6563 746f  data into..vecto
-000018e0: 7220 7265 7072 6573 656e 7461 7469 6f6e  r representation
-000018f0: 7320 616e 6420 7374 6f72 696e 6720 7468  s and storing th
-00001900: 656d 2069 6e20 6120 7665 6374 6f72 2073  em in a vector s
-00001910: 746f 7265 2c20 796f 7520 6361 6e0d 0a70  tore, you can..p
-00001920: 6572 666f 726d 2072 6170 6964 2073 696d  erform rapid sim
-00001930: 696c 6172 6974 7920 7365 6172 6368 6573  ilarity searches
-00001940: 2061 6e64 206f 7468 6572 2076 6563 746f   and other vecto
-00001950: 722d 6261 7365 6420 6f70 6572 6174 696f  r-based operatio
-00001960: 6e73 2e0d 0a0d 0a60 6060 2070 7974 686f  ns.....``` pytho
-00001970: 6e0d 0a49 6e64 6f78 2e63 6f6e 6e65 6374  n..Indox.connect
-00001980: 5f74 6f5f 7665 6374 6f72 7374 6f72 6528  _to_vectorstore(
-00001990: 636f 6c6c 6563 7469 6f6e 5f6e 616d 653d  collection_name=
-000019a0: 2273 616d 706c 6522 2c65 6d62 6564 6469  "sample",embeddi
-000019b0: 6e67 733d 6f70 656e 6169 5f65 6d62 6564  ngs=openai_embed
-000019c0: 6469 6e67 7329 0d0a 496e 646f 782e 7374  dings)..Indox.st
-000019d0: 6f72 655f 696e 5f76 6563 746f 7273 746f  ore_in_vectorsto
-000019e0: 7265 2863 6875 6e6b 733d 646f 6373 5f75  re(chunks=docs_u
-000019f0: 6e73 7472 7563 7475 7265 6429 0d0a 6060  nstructured)..``
-00001a00: 600d 0a0d 0a23 2320 5175 6572 696e 670d  `....## Quering.
-00001a10: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a71  ...``` python..q
-00001a20: 7565 7279 203d 2022 796f 7572 2071 7565  uery = "your que
-00001a30: 7279 2121 3f3f 220d 0a60 6060 0d0a 0d0a  ry!!??"..```....
-00001a40: 6060 6020 7079 7468 6f6e 0d0a 7265 7370  ``` python..resp
-00001a50: 6f6e 7365 5f6f 7065 6e61 6920 3d20 496e  onse_openai = In
-00001a60: 646f 782e 616e 7377 6572 5f71 7565 7374  dox.answer_quest
-00001a70: 696f 6e28 7175 6572 793d 7175 6572 792c  ion(query=query,
-00001a80: 7161 5f6d 6f64 656c 3d6f 7065 6e61 695f  qa_model=openai_
-00001a90: 7161 290d 0a60 6060 0d0a 0d0a 6060 6020  qa)..```....``` 
-00001aa0: 7079 7468 6f6e 0d0a 616e 7377 6572 203d  python..answer =
-00001ab0: 2072 6573 706f 6e73 655f 6f70 656e 6169   response_openai
-00001ac0: 5b30 5d0d 0a60 6060 0d0a 0d0a 6060 6020  [0]..```....``` 
-00001ad0: 7079 7468 6f6e 0d0a 636f 6e74 6578 742c  python..context,
-00001ae0: 2073 636f 7265 203d 2072 6573 706f 6e73   score = respons
-00001af0: 655f 6f70 656e 6169 5b31 5d0d 0a60 6060  e_openai[1]..```
-00001b00: 0d0a 0d0a                                ....
+00000000: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000010: 6572 223e 0d0a 0d0a 0d0a 3c68 3320 616c  er">......<h3 al
+00000020: 6967 6e3d 2263 656e 7465 7222 3e0d 0a20  ign="center">.. 
+00000030: 2020 203c 696d 6720 7372 633d 2264 6f63     <img src="doc
+00000040: 732f 6c69 7465 2d6c 6f67 6f20 312e 706e  s/lite-logo 1.pn
+00000050: 6722 2061 6c74 3d22 4c6f 676f 2220 7374  g" alt="Logo" st
+00000060: 796c 653d 2277 6964 7468 3a20 3830 253b  yle="width: 80%;
+00000070: 206f 7061 6369 7479 3a20 302e 373b 222f   opacity: 0.7;"/
+00000080: 3e0d 0a0d 0a3c 2f68 333e 0d0a 0d0a 0d0a  >....</h3>......
+00000090: 3c64 6976 2073 7479 6c65 3d22 706f 7369  <div style="posi
+000000a0: 7469 6f6e 3a20 7265 6c61 7469 7665 3b20  tion: relative; 
+000000b0: 7769 6474 683a 2031 3030 253b 2074 6578  width: 100%; tex
+000000c0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000000d0: 223e 0d0a 3c68 313e 0d0a 696e 446f 7820  ">..<h1>..inDox 
+000000e0: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+000000f0: 6572 223e 4164 7661 6e63 6564 2053 6561  er">Advanced Sea
+00000100: 7263 6820 616e 6420 5265 7472 6965 7661  rch and Retrieva
+00000110: 6c20 4175 676d 656e 7461 7469 6f6e 2047  l Augmentation G
+00000120: 656e 6572 6174 6976 650d 0a3c 2f70 3e0d  enerative..</p>.
+00000130: 0a0d 0a3c 2f68 313e 0d0a 0d0a 5b21 5b4c  ...</h1>....[![L
+00000140: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00000150: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000160: 6974 6875 622f 6c69 6365 6e73 652f 6f73  ithub/license/os
+00000170: 6c6c 6d61 692f 696e 446f 7829 5d28 6874  llmai/inDox)](ht
+00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000190: 2f6f 736c 6c6d 6169 2f69 6e44 6f78 2f62  /osllmai/inDox/b
+000001a0: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
+000001b0: 290d 0a5b 215b 5079 5049 5d28 6874 7470  )..[![PyPI](http
+000001c0: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
+000001d0: 6f2f 7079 2f49 6e64 6f78 2e73 7667 295d  o/py/Indox.svg)]
+000001e0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000001f0: 672f 7072 6f6a 6563 742f 496e 646f 782f  g/project/Indox/
+00000200: 302e 312e 342f 290d 0a5b 215b 5079 7468  0.1.4/)..[![Pyth
+00000210: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+00000220: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000230: 7079 7665 7273 696f 6e73 2f49 6e64 6f78  pyversions/Indox
+00000240: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
+00000250: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000260: 496e 646f 782f 302e 312e 342f 290d 0a5b  Indox/0.1.4/)..[
+00000270: 215b 446f 776e 6c6f 6164 735d 2868 7474  ![Downloads](htt
+00000280: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000290: 2e74 6563 682f 6261 6467 652f 696e 646f  .tech/badge/indo
+000002a0: 7829 5d28 6874 7470 733a 2f2f 7065 7079  x)](https://pepy
+000002b0: 2e74 6563 682f 7072 6f6a 6563 742f 696e  .tech/project/in
+000002c0: 646f 7829 0d0a 0d0a 5b21 5b44 6973 636f  dox)....[![Disco
+000002d0: 7264 5d28 6874 7470 733a 2f2f 696d 672e  rd](https://img.
+000002e0: 7368 6965 6c64 732e 696f 2f64 6973 636f  shields.io/disco
+000002f0: 7264 2f31 3232 3338 3637 3338 3234 3630  rd/1223867382460
+00000300: 3537 3939 3631 3f6c 6162 656c 3d44 6973  579961?label=Dis
+00000310: 636f 7264 266c 6f67 6f3d 4469 7363 6f72  cord&logo=Discor
+00000320: 6426 7374 796c 653d 736f 6369 616c 295d  d&style=social)]
+00000330: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00000340: 2e63 6f6d 2f69 6e76 6974 652f 6f73 736c  .com/invite/ossl
+00000350: 6c6d 6169 290d 0a5b 215b 4769 7448 7562  lmai)..[![GitHub
+00000360: 2073 7461 7273 5d28 6874 7470 733a 2f2f   stars](https://
+00000370: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000380: 6974 6875 622f 7374 6172 732f 6f73 6c6c  ithub/stars/osll
+00000390: 6d61 692f 696e 446f 783f 7374 796c 653d  mai/inDox?style=
+000003a0: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
+000003b0: 2f67 6974 6875 622e 636f 6d2f 6f73 6c6c  /github.com/osll
+000003c0: 6d61 692f 696e 446f 7829 0d0a 0d0a 0d0a  mai/inDox)......
+000003d0: 0d0a 0d0a 3c70 2061 6c69 676e 3d22 6365  ....<p align="ce
+000003e0: 6e74 6572 223e 0d0a 2020 3c61 2068 7265  nter">..  <a hre
+000003f0: 663d 2268 7474 7073 3a2f 2f6f 736c 6c6d  f="https://osllm
+00000400: 2e61 6922 3e4f 6666 6963 6961 6c20 5765  .ai">Official We
+00000410: 6273 6974 653c 2f61 3e20 2662 756c 6c3b  bsite</a> &bull;
+00000420: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000430: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 736c  //github.com/osl
+00000440: 6c6d 6169 2f69 6e44 6f78 2f77 696b 6922  lmai/inDox/wiki"
+00000450: 3e44 6f63 756d 656e 7461 7469 6f6e 3c2f  >Documentation</
+00000460: 613e 2026 6275 6c6c 3b20 3c61 2068 7265  a> &bull; <a hre
+00000470: 663d 2268 7474 7073 3a2f 2f64 6973 636f  f="https://disco
+00000480: 7264 2e67 672f 7172 4363 3536 5a52 223e  rd.gg/qrCc56ZR">
+00000490: 4469 7363 6f72 643c 2f61 3e0d 0a3c 2f70  Discord</a>..</p
+000004a0: 3e0d 0a0d 0a0d 0a3c 7020 616c 6967 6e3d  >......<p align=
+000004b0: 2263 656e 7465 7222 3e0d 0a20 203c 623e  "center">..  <b>
+000004c0: 4e45 573a 3c2f 623e 203c 6120 6872 6566  NEW:</b> <a href
+000004d0: 3d22 6874 7470 733a 2f2f 646f 6373 2e67  ="https://docs.g
+000004e0: 6f6f 676c 652e 636f 6d2f 666f 726d 732f  oogle.com/forms/
+000004f0: 642f 3143 5158 4a76 784c 5571 4c42 5358  d/1CQXJvxLUqLBSX
+00000500: 6e6a 7151 6d52 704f 795a 7144 366e 724b  njqQmRpOyZqD6nrK
+00000510: 7562 4c7a 3257 5463 494a 3337 6655 2f70  ubLz2WTcIJ37fU/p
+00000520: 7265 6669 6c6c 223e 5375 6273 6372 6962  refill">Subscrib
+00000530: 6520 746f 206f 7572 206d 6169 6c69 6e67  e to our mailing
+00000540: 206c 6973 743c 2f61 3e20 666f 7220 7570   list</a> for up
+00000550: 6461 7465 7320 616e 6420 6e65 7773 210d  dates and news!.
+00000560: 0a3c 2f70 3e0d 0a0d 0a0d 0a0d 0a2a 2a49  .</p>........**I
+00000570: 6e64 6f78 2052 6574 7269 6576 616c 2041  ndox Retrieval A
+00000580: 7567 6d65 6e74 6174 696f 6e2a 2a20 6973  ugmentation** is
+00000590: 2061 6e20 696e 6e6f 7661 7469 7665 2061   an innovative a
+000005a0: 7070 6c69 6361 7469 6f6e 2064 6573 6967  pplication desig
+000005b0: 6e65 6420 746f 2073 7472 6561 6d6c 696e  ned to streamlin
+000005c0: 6520 696e 666f 726d 6174 696f 6e20 6578  e information ex
+000005d0: 7472 6163 7469 6f6e 2066 726f 6d20 6120  traction from a 
+000005e0: 7769 6465 0d0a 7261 6e67 6520 6f66 2064  wide..range of d
+000005f0: 6f63 756d 656e 7420 7479 7065 732c 2069  ocument types, i
+00000600: 6e63 6c75 6469 6e67 2074 6578 7420 6669  ncluding text fi
+00000610: 6c65 732c 2050 4446 2c20 4854 4d4c 2c20  les, PDF, HTML, 
+00000620: 4d61 726b 646f 776e 2c20 616e 6420 4c61  Markdown, and La
+00000630: 5465 582e 2057 6865 7468 6572 2073 7472  TeX. Whether str
+00000640: 7563 7475 7265 6420 6f72 2075 6e73 7472  uctured or unstr
+00000650: 7563 7475 7265 642c 2049 6e64 6f78 0d0a  uctured, Indox..
+00000660: 7072 6f76 6964 6573 2075 7365 7273 2077  provides users w
+00000670: 6974 6820 6120 706f 7765 7266 756c 2074  ith a powerful t
+00000680: 6f6f 6c73 6574 2074 6f20 6566 6669 6369  oolset to effici
+00000690: 656e 746c 7920 6578 7472 6163 7420 7265  ently extract re
+000006a0: 6c65 7661 6e74 2064 6174 612e 0d0a 0d0a  levant data.....
+000006b0: 496e 646f 7820 5265 7472 6965 7661 6c20  Indox Retrieval 
+000006c0: 4175 676d 656e 7461 7469 6f6e 2069 7320  Augmentation is 
+000006d0: 616e 2069 6e6e 6f76 6174 6976 6520 6170  an innovative ap
+000006e0: 706c 6963 6174 696f 6e20 6465 7369 676e  plication design
+000006f0: 6564 2074 6f20 7374 7265 616d 6c69 6e65  ed to streamline
+00000700: 2069 6e66 6f72 6d61 7469 6f6e 2065 7874   information ext
+00000710: 7261 6374 696f 6e20 6672 6f6d 2061 2077  raction from a w
+00000720: 6964 650d 0a72 616e 6765 206f 6620 646f  ide..range of do
+00000730: 6375 6d65 6e74 2074 7970 6573 2c20 696e  cument types, in
+00000740: 636c 7564 696e 6720 7465 7874 2066 696c  cluding text fil
+00000750: 6573 2c20 5044 462c 2048 544d 4c2c 204d  es, PDF, HTML, M
+00000760: 6172 6b64 6f77 6e2c 2061 6e64 204c 6154  arkdown, and LaT
+00000770: 6558 2e20 5768 6574 6865 7220 7374 7275  eX. Whether stru
+00000780: 6374 7572 6564 206f 7220 756e 7374 7275  ctured or unstru
+00000790: 6374 7572 6564 2c20 496e 646f 780d 0a70  ctured, Indox..p
+000007a0: 726f 7669 6465 7320 7573 6572 7320 7769  rovides users wi
+000007b0: 7468 2061 2070 6f77 6572 6675 6c20 746f  th a powerful to
+000007c0: 6f6c 7365 7420 746f 2065 6666 6963 6965  olset to efficie
+000007d0: 6e74 6c79 2065 7874 7261 6374 2072 656c  ntly extract rel
+000007e0: 6576 616e 7420 6461 7461 2e20 4f6e 6520  evant data. One 
+000007f0: 6f66 2069 7473 206b 6579 2066 6561 7475  of its key featu
+00000800: 7265 7320 6973 2074 6865 2061 6269 6c69  res is the abili
+00000810: 7479 2074 6f0d 0a69 6e74 656c 6c69 6765  ty to..intellige
+00000820: 6e74 6c79 2063 6c75 7374 6572 2070 7269  ntly cluster pri
+00000830: 6d61 7279 2063 6875 6e6b 7320 746f 2066  mary chunks to f
+00000840: 6f72 6d20 6d6f 7265 2072 6f62 7573 7420  orm more robust 
+00000850: 6772 6f75 7069 6e67 732c 2065 6e68 616e  groupings, enhan
+00000860: 6369 6e67 2074 6865 2071 7561 6c69 7479  cing the quality
+00000870: 2061 6e64 2072 656c 6576 616e 6365 206f   and relevance o
+00000880: 6620 7468 6520 6578 7472 6163 7465 640d  f the extracted.
+00000890: 0a69 6e66 6f72 6d61 7469 6f6e 2e0d 0a57  .information...W
+000008a0: 6974 6820 6120 666f 6375 7320 6f6e 2061  ith a focus on a
+000008b0: 6461 7074 6162 696c 6974 7920 616e 6420  daptability and 
+000008c0: 7573 6572 2d63 656e 7472 6963 2064 6573  user-centric des
+000008d0: 6967 6e2c 2049 6e64 6f78 2061 696d 7320  ign, Indox aims 
+000008e0: 746f 2064 656c 6976 6572 2066 7574 7572  to deliver futur
+000008f0: 652d 7265 6164 7920 6675 6e63 7469 6f6e  e-ready function
+00000900: 616c 6974 7920 7769 7468 206d 6f72 650d  ality with more.
+00000910: 0a66 6561 7475 7265 7320 706c 616e 6e65  .features planne
+00000920: 6420 666f 7220 7570 636f 6d69 6e67 2072  d for upcoming r
+00000930: 656c 6561 7365 732e 204a 6f69 6e20 7573  eleases. Join us
+00000940: 2069 6e20 6578 706c 6f72 696e 6720 686f   in exploring ho
+00000950: 7720 496e 646f 7820 6361 6e20 7265 766f  w Indox can revo
+00000960: 6c75 7469 6f6e 697a 6520 796f 7572 2064  lutionize your d
+00000970: 6f63 756d 656e 7420 7072 6f63 6573 7369  ocument processi
+00000980: 6e67 0d0a 776f 726b 666c 6f77 2c20 6272  ng..workflow, br
+00000990: 696e 6769 6e67 2063 6c61 7269 7479 2061  inging clarity a
+000009a0: 6e64 206f 7267 616e 697a 6174 696f 6e20  nd organization 
+000009b0: 746f 2079 6f75 7220 6461 7461 2072 6574  to your data ret
+000009c0: 7269 6576 616c 206e 6565 6473 2e0d 0a0d  rieval needs....
+000009d0: 0a23 2320 4465 7065 6e64 656e 6379 2052  .## Dependency R
+000009e0: 6571 7569 7265 6d65 6e74 730d 0a0d 0a42  equirements....B
+000009f0: 6566 6f72 6520 7275 6e6e 696e 6720 7468  efore running th
+00000a00: 6973 2070 726f 6a65 6374 2c20 656e 7375  is project, ensu
+00000a10: 7265 2074 6861 7420 796f 7520 6861 7665  re that you have
+00000a20: 2074 6865 2066 6f6c 6c6f 7769 6e67 2069   the following i
+00000a30: 6e73 7461 6c6c 6564 3a0d 0a0d 0a2d 202a  nstalled:....- *
+00000a40: 2a50 7974 686f 6e20 332e 382b 2a2a 3a20  *Python 3.8+**: 
+00000a50: 5265 7175 6972 6564 2066 6f72 2072 756e  Required for run
+00000a60: 6e69 6e67 2074 6865 2050 7974 686f 6e20  ning the Python 
+00000a70: 6261 636b 656e 642e 0d0a 2d20 2a2a 506f  backend...- **Po
+00000a80: 7374 6772 6553 514c 2a2a 3a20 4e65 6564  stgreSQL**: Need
+00000a90: 6564 2069 6620 796f 7520 7769 7368 2074  ed if you wish t
+00000aa0: 6f20 7374 6f72 6520 796f 7572 2064 6174  o store your dat
+00000ab0: 6120 696e 2061 2050 6f73 7467 7265 5351  a in a PostgreSQ
+00000ac0: 4c20 6461 7461 6261 7365 2e0d 0a2d 202a  L database...- *
+00000ad0: 2a4f 7065 6e41 4920 4150 4920 4b65 792a  *OpenAI API Key*
+00000ae0: 2a3a 204e 6563 6573 7361 7279 2069 6620  *: Necessary if 
+00000af0: 796f 7520 6172 6520 7573 696e 6720 7468  you are using th
+00000b00: 6520 4f70 656e 4149 2065 6d62 6564 6469  e OpenAI embeddi
+00000b10: 6e67 206d 6f64 656c 2e0d 0a2d 202a 2a48  ng model...- **H
+00000b20: 7567 6769 6e67 4661 6365 2041 5049 204b  uggingFace API K
+00000b30: 6579 2a2a 3a20 4e65 6365 7373 6172 7920  ey**: Necessary 
+00000b40: 6966 2079 6f75 2061 7265 2075 7369 6e67  if you are using
+00000b50: 2074 6865 2048 7567 6769 6e67 4661 6365   the HuggingFace
+00000b60: 206c 6c6d 732e 0d0a 0d0a 456e 7375 7265   llms.....Ensure
+00000b70: 2079 6f75 7220 7379 7374 656d 2061 6c73   your system als
+00000b80: 6f20 6d65 6574 7320 7468 6573 6520 7265  o meets these re
+00000b90: 7175 6972 656d 656e 7473 3a0d 0a0d 0a2d  quirements:....-
+00000ba0: 2041 6363 6573 7320 746f 2065 6e76 6972   Access to envir
+00000bb0: 6f6e 6d65 6e74 616c 2076 6172 6961 626c  onmental variabl
+00000bc0: 6573 2066 6f72 2068 616e 646c 696e 6720  es for handling 
+00000bd0: 7365 6e73 6974 6976 6520 696e 666f 726d  sensitive inform
+00000be0: 6174 696f 6e20 6c69 6b65 2041 5049 206b  ation like API k
+00000bf0: 6579 732e 0d0a 2d20 5375 6974 6162 6c65  eys...- Suitable
+00000c00: 2068 6172 6477 6172 6520 6361 7061 626c   hardware capabl
+00000c10: 6520 6f66 2073 7570 706f 7274 696e 6720  e of supporting 
+00000c20: 696e 7465 6e73 6976 6520 636f 6d70 7574  intensive comput
+00000c30: 6174 696f 6e61 6c20 7461 736b 732e 0d0a  ational tasks...
+00000c40: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000c50: 6e0d 0a0d 0a0d 0a23 2320 4765 7474 696e  n......## Gettin
+00000c60: 6720 5374 6172 7465 640d 0a0d 0a54 6865  g Started....The
+00000c70: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00000c80: 6e64 2077 696c 6c20 696e 7374 616c 6c20  nd will install 
+00000c90: 7468 6520 6c61 7465 7374 2073 7461 626c  the latest stabl
+00000ca0: 6520 696e 446f 780d 0a0d 0a60 6060 0d0a  e inDox....```..
+00000cb0: 7069 7020 696e 7374 616c 6c20 496e 646f  pip install Indo
+00000cc0: 780d 0a60 6060 0d0a 0d0a 546f 2069 6e73  x..```....To ins
+00000cd0: 7461 6c6c 2074 6865 206c 6174 6573 7420  tall the latest 
+00000ce0: 6465 7665 6c6f 706d 656e 7420 7665 7273  development vers
+00000cf0: 696f 6e2c 2079 6f75 206d 6179 2072 756e  ion, you may run
+00000d00: 0d0a 0d0a 6060 600d 0a70 6970 2069 6e73  ....```..pip ins
+00000d10: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
+00000d20: 2f67 6974 6875 622e 636f 6d2f 6f73 6c6c  /github.com/osll
+00000d30: 6d61 692f 696e 446f 7840 6d61 696e 0d0a  mai/inDox@main..
+00000d40: 6060 600d 0a0d 0a54 6f20 636f 6e66 6967  ```....To config
+00000d50: 7572 6520 7468 6520 434c 492c 2072 756e  ure the CLI, run
+00000d60: 0d0a 0d0a 6060 600d 0a69 6e64 6f78 2063  ....```..indox c
+00000d70: 6f6e 6669 6775 7265 0d0a 6060 600d 0a0d  onfigure..```...
+00000d80: 0a0d 0a43 6c6f 6e65 2074 6865 2072 6570  ...Clone the rep
+00000d90: 6f73 6974 6f72 7920 616e 6420 6e61 7669  ository and navi
+00000da0: 6761 7465 2074 6f20 7468 6520 6469 7265  gate to the dire
+00000db0: 6374 6f72 793a 0d0a 0d0a 6060 6062 6173  ctory:....```bas
+00000dc0: 680d 0a67 6974 2063 6c6f 6e65 2068 7474  h..git clone htt
+00000dd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000de0: 6f73 6c6c 6d61 692f 696e 446f 782e 6769  osllmai/inDox.gi
+00000df0: 740d 0a63 6420 696e 446f 780d 0a60 6060  t..cd inDox..```
+00000e00: 0d0a 0d0a 496e 7374 616c 6c20 7468 6520  ....Install the 
+00000e10: 7265 7175 6972 6564 2050 7974 686f 6e20  required Python 
+00000e20: 7061 636b 6167 6573 3a0d 0a0d 0a60 6060  packages:....```
+00000e30: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+00000e40: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+00000e50: 732e 7478 740d 0a60 6060 0d0a 0d0a 2323  s.txt..```....##
+00000e60: 2043 6f6e 6669 6775 7261 7469 6f6e 0d0a   Configuration..
+00000e70: 0d0a 2323 2320 456e 7669 726f 6e6d 656e  ..### Environmen
+00000e80: 7420 5661 7269 6162 6c65 730d 0a0d 0a53  t Variables....S
+00000e90: 6574 2079 6f75 7220 604f 5045 4e41 495f  et your `OPENAI_
+00000ea0: 4150 495f 4b45 5960 206f 7220 6048 465f  API_KEY` or `HF_
+00000eb0: 4150 495f 4b45 5960 2069 6e20 796f 7572  API_KEY` in your
+00000ec0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00000ed0: 6961 626c 6573 2066 6f72 2073 6563 7572  iables for secur
+00000ee0: 6520 6163 6365 7373 2e0d 0a0d 0a23 2323  e access.....###
+00000ef0: 2044 6174 6162 6173 6520 5365 7475 700d   Database Setup.
+00000f00: 0a0d 0a45 6e73 7572 6520 796f 7572 2050  ...Ensure your P
+00000f10: 6f73 7467 7265 5351 4c20 6461 7461 6261  ostgreSQL databa
+00000f20: 7365 2069 7320 7570 2061 6e64 2072 756e  se is up and run
+00000f30: 6e69 6e67 2c20 616e 6420 6163 6365 7373  ning, and access
+00000f40: 6962 6c65 2066 726f 6d20 796f 7572 2061  ible from your a
+00000f50: 7070 6c69 6361 7469 6f6e 2e20 5468 6973  pplication. This
+00000f60: 2069 7320 6e65 6365 7373 6172 7920 6966   is necessary if
+00000f70: 2079 6f75 2070 6c61 6e20 746f 2075 7365   you plan to use
+00000f80: 2070 6776 6563 746f 7220 6173 2079 6f75   pgvector as you
+00000f90: 7220 7665 6374 6f72 2073 746f 7265 2e0d  r vector store..
+00000fa0: 0a0d 0a41 6c74 6572 6e61 7469 7665 6c79  ...Alternatively
+00000fb0: 2c20 796f 7520 6361 6e20 7573 6520 4368  , you can use Ch
+00000fc0: 726f 6d61 206f 7220 4661 6973 7320 6173  roma or Faiss as
+00000fd0: 2079 6f75 7220 7665 6374 6f72 2073 746f   your vector sto
+00000fe0: 7265 2e20 4d61 6b65 2073 7572 6520 746f  re. Make sure to
+00000ff0: 2073 7065 6369 6679 2079 6f75 7220 6368   specify your ch
+00001000: 6f69 6365 2061 6e64 2074 6865 206e 6563  oice and the nec
+00001010: 6573 7361 7279 2063 6f6e 6669 6775 7261  essary configura
+00001020: 7469 6f6e 7320 696e 2074 6865 2063 6f6e  tions in the con
+00001030: 6669 672e 7961 6d6c 2066 696c 652e 0d0a  fig.yaml file...
+00001040: 0d0a 2323 2055 7361 6765 0d0a 0d0a 2323  ..## Usage....##
+00001050: 2320 5072 6570 6172 696e 6720 596f 7572  # Preparing Your
+00001060: 2044 6174 610d 0a0d 0a31 2e20 2a2a 4465   Data....1. **De
+00001070: 6669 6e65 2074 6865 2046 696c 6520 5061  fine the File Pa
+00001080: 7468 2a2a 3a20 5370 6563 6966 7920 7468  th**: Specify th
+00001090: 6520 7061 7468 2074 6f20 796f 7572 2074  e path to your t
+000010a0: 6578 7420 6f72 2050 4446 2066 696c 652e  ext or PDF file.
+000010b0: 0d0a 322e 202a 2a4c 6f61 6420 456d 6265  ..2. **Load Embe
+000010c0: 6464 696e 6720 4d6f 6465 6c73 2a2a 3a20  dding Models**: 
+000010d0: 496e 6974 6961 6c69 7a65 2079 6f75 7220  Initialize your 
+000010e0: 656d 6265 6464 696e 6720 6d6f 6465 6c20  embedding model 
+000010f0: 6672 6f6d 204f 7065 6e41 4927 7320 7365  from OpenAI's se
+00001100: 6c65 6374 696f 6e20 6f66 2070 7265 2d74  lection of pre-t
+00001110: 7261 696e 6564 206d 6f64 656c 732e 0d0a  rained models...
+00001120: 0d0a 2320 5175 6963 6b20 5374 6172 7420  ..# Quick Start 
+00001130: 0d0a 0d0a 2323 2049 6d70 6f72 7420 496e  ....## Import In
+00001140: 646f 7820 5061 636b 6167 650d 0a0d 0a49  dox Package....I
+00001150: 6d70 6f72 7420 7468 6520 6e65 6365 7373  mport the necess
+00001160: 6172 7920 636c 6173 7365 7320 6672 6f6d  ary classes from
+00001170: 2074 6865 2049 6e64 6f78 2070 6163 6b61   the Indox packa
+00001180: 6765 2e0d 0a0d 0a60 6060 2070 7974 686f  ge.....``` pytho
+00001190: 6e0d 0a66 726f 6d20 496e 646f 7820 696d  n..from Indox im
+000011a0: 706f 7274 2049 6e64 6f78 5265 7472 6965  port IndoxRetrie
+000011b0: 7661 6c41 7567 6d65 6e74 6174 696f 6e0d  valAugmentation.
+000011c0: 0a60 6060 0d0a 0d0a 2323 2320 496e 6974  .```....### Init
+000011d0: 6961 6c69 7a65 2049 6e64 6f78 0d0a 0d0a  ialize Indox....
+000011e0: 4372 6561 7465 2061 6e20 696e 7374 616e  Create an instan
+000011f0: 6365 206f 6620 496e 646f 7852 6574 7269  ce of IndoxRetri
+00001200: 6576 616c 4175 676d 656e 7461 7469 6f6e  evalAugmentation
+00001210: 2e0d 0a0d 0a60 6060 2070 7974 686f 6e0d  .....``` python.
+00001220: 0a49 6e64 6f78 203d 2049 6e64 6f78 5265  .Indox = IndoxRe
+00001230: 7472 6965 7661 6c41 7567 6d65 6e74 6174  trievalAugmentat
+00001240: 696f 6e28 290d 0a60 6060 0d0a 2323 2049  ion()..```..## I
+00001250: 6e69 7469 616c 2043 6f6e 6669 6775 7261  nitial Configura
+00001260: 7469 6f6e 0d0a 0d0a 2d20 2a2a 436f 6e66  tion....- **Conf
+00001270: 6967 7572 6174 696f 6e20 4669 6c65 2a2a  iguration File**
+00001280: 3a20 456e 7375 7265 2079 6f75 206c 6f63  : Ensure you loc
+00001290: 6174 6520 616e 6420 6d6f 6469 6679 2074  ate and modify t
+000012a0: 6865 2060 496e 646f 782e 636f 6e66 6967  he `Indox.config
+000012b0: 6020 5941 4d4c 2066 696c 6520 6163 636f  ` YAML file acco
+000012c0: 7264 696e 6720 746f 2079 6f75 7220 6e65  rding to your ne
+000012d0: 6564 7320 6265 666f 7265 0d0a 2020 7374  eds before..  st
+000012e0: 6172 7469 6e67 2074 6865 2061 7070 6c69  arting the appli
+000012f0: 6361 7469 6f6e 2e0d 0a0d 0a23 2320 4479  cation.....## Dy
+00001300: 6e61 6d69 6320 436f 6e66 6967 7572 6174  namic Configurat
+00001310: 696f 6e20 4368 616e 6765 730d 0a0d 0a46  ion Changes....F
+00001320: 6f72 2063 6861 6e67 6573 2074 6861 7420  or changes that 
+00001330: 6e65 6564 2074 6f20 6265 2061 7070 6c69  need to be appli
+00001340: 6564 2061 6674 6572 2074 6865 2069 6e69  ed after the ini
+00001350: 7469 616c 2073 6574 7570 206f 7220 6475  tial setup or du
+00001360: 7269 6e67 2072 756e 7469 6d65 3a0d 0a0d  ring runtime:...
+00001370: 0a2d 202a 2a4d 6f64 6966 7969 6e67 2043  .- **Modifying C
+00001380: 6f6e 6669 6775 7261 7469 6f6e 732a 2a3a  onfigurations**:
+00001390: 2055 7365 2074 6865 2066 6f6c 6c6f 7769   Use the followi
+000013a0: 6e67 2050 7974 686f 6e20 736e 6970 7065  ng Python snippe
+000013b0: 7420 746f 2075 7064 6174 6520 796f 7572  t to update your
+000013c0: 2073 6574 7469 6e67 7320 6479 6e61 6d69   settings dynami
+000013d0: 6361 6c6c 793a 0d0a 2020 6060 6070 7974  cally:..  ```pyt
+000013e0: 686f 6e0d 0a20 2049 6e64 6f78 2e63 6f6e  hon..  Indox.con
+000013f0: 6669 675b 2279 6f75 725f 7365 7474 696e  fig["your_settin
+00001400: 675f 7468 6174 5f6e 6565 645f 746f 5f63  g_that_need_to_c
+00001410: 6861 6e67 6522 5d20 3d20 226e 6577 5f73  hange"] = "new_s
+00001420: 6574 7469 6e67 220d 0a20 2049 6e64 6f78  etting"..  Indox
+00001430: 2e75 7064 6174 655f 636f 6e66 6967 2829  .update_config()
+00001440: 0d0a 0d0a 2323 2043 6f6e 6669 6775 7261  ....## Configura
+00001450: 7469 6f6e 2044 6574 6169 6c73 0d0a 0d0a  tion Details....
+00001460: 4865 7265 2773 2061 2062 7265 616b 646f  Here's a breakdo
+00001470: 776e 206f 6620 7468 6520 636f 6e66 6967  wn of the config
+00001480: 2064 6963 7469 6f6e 6172 7920 616e 6420   dictionary and 
+00001490: 6974 7320 7072 6f70 6572 7469 6573 3a0d  its properties:.
+000014a0: 0a0d 0a23 2323 2050 6f73 7467 7265 5351  ...### PostgreSQ
+000014b0: 4c0d 0a0d 0a2d 2060 636f 6e6e 5f73 7472  L....- `conn_str
+000014c0: 696e 6760 3a20 596f 7572 2050 6f73 7467  ing`: Your Postg
+000014d0: 7265 5351 4c20 6461 7461 6261 7365 2063  reSQL database c
+000014e0: 7265 6465 6e74 6961 6c73 2e0d 0a0d 0a23  redentials.....#
+000014f0: 2323 2053 756d 6d61 7279 204d 6f64 656c  ## Summary Model
+00001500: 0d0a 0d0a 2d20 606d 6178 5f74 6f6b 656e  ....- `max_token
+00001510: 7360 3a20 4d61 7869 6d75 6d20 746f 6b65  s`: Maximum toke
+00001520: 6e20 636f 756e 7420 7468 6520 7375 6d6d  n count the summ
+00001530: 6172 7920 6d6f 6465 6c20 6361 6e20 6765  ary model can ge
+00001540: 6e65 7261 7465 2e0d 0a2d 2060 6d69 6e5f  nerate...- `min_
+00001550: 6c65 6e60 3a20 4d69 6e69 6d75 6d20 746f  len`: Minimum to
+00001560: 6b65 6e20 636f 756e 7420 7468 6520 7375  ken count the su
+00001570: 6d6d 6172 7920 6d6f 6465 6c20 6765 6e65  mmary model gene
+00001580: 7261 7465 732e 0d0a 2d20 606d 6f64 656c  rates...- `model
+00001590: 5f6e 616d 6560 3a20 4465 6661 756c 7420  _name`: Default 
+000015a0: 6973 2060 6770 742d 332e 352d 7475 7262  is `gpt-3.5-turb
+000015b0: 6f2d 3031 3235 602c 2062 7574 2069 7420  o-0125`, but it 
+000015c0: 6361 6e20 6265 2072 6570 6c61 6365 6420  can be replaced 
+000015d0: 7769 7468 2061 6e79 2048 7567 6769 6e67  with any Hugging
+000015e0: 2046 6163 6520 6d6f 6465 6c20 7375 7070   Face model supp
+000015f0: 6f72 7469 6e67 2074 6865 0d0a 2020 7375  orting the..  su
+00001600: 6d6d 6172 697a 6174 696f 6e20 7069 7065  mmarization pipe
+00001610: 6c69 6e65 2e0d 0a0d 0a23 2323 2050 6f73  line.....### Pos
+00001620: 7467 7265 5351 4c20 5365 7475 7020 7769  tgreSQL Setup wi
+00001630: 7468 2070 6776 6563 746f 720d 0a0d 0a49  th pgvector....I
+00001640: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00001650: 6520 506f 7374 6772 6553 514c 2066 6f72  e PostgreSQL for
+00001660: 2076 6563 746f 7220 7374 6f72 6167 652c   vector storage,
+00001670: 2079 6f75 2073 686f 756c 6420 7065 7266   you should perf
+00001680: 6f72 6d20 7468 6520 666f 6c6c 6f77 696e  orm the followin
+00001690: 6720 7374 6570 733a 0d0a 0d0a 312e 202a  g steps:....1. *
+000016a0: 2a49 6e73 7461 6c6c 2070 6776 6563 746f  *Install pgvecto
+000016b0: 722a 2a3a 2054 6f20 696e 7374 616c 6c20  r**: To install 
+000016c0: 6070 6776 6563 746f 7260 206f 6e20 796f  `pgvector` on yo
+000016d0: 7572 2050 6f73 7467 7265 5351 4c20 7365  ur PostgreSQL se
+000016e0: 7276 6572 2c20 666f 6c6c 6f77 2074 6865  rver, follow the
+000016f0: 2064 6574 6169 6c65 6420 696e 7374 616c   detailed instal
+00001700: 6c61 7469 6f6e 2069 6e73 7472 7563 7469  lation instructi
+00001710: 6f6e 730d 0a20 2020 6176 6169 6c61 626c  ons..   availabl
+00001720: 6520 6f6e 2074 6865 206f 6666 6963 6961  e on the officia
+00001730: 6c20 7067 7665 6374 6f72 2047 6974 4875  l pgvector GitHu
+00001740: 6220 7265 706f 7369 746f 7279 3a0d 0a20  b repository:.. 
+00001750: 2020 5b70 6776 6563 746f 7220 496e 7374    [pgvector Inst
+00001760: 616c 6c61 7469 6f6e 2049 6e73 7472 7563  allation Instruc
+00001770: 7469 6f6e 735d 2868 7474 7073 3a2f 2f67  tions](https://g
+00001780: 6974 6875 622e 636f 6d2f 7067 7665 6374  ithub.com/pgvect
+00001790: 6f72 2f70 6776 6563 746f 7229 0d0a 0d0a  or/pgvector)....
+000017a0: 322e 202a 2a41 6464 2056 6563 746f 7220  2. **Add Vector 
+000017b0: 4578 7465 6e73 696f 6e2a 2a3a 0d0a 2020  Extension**:..  
+000017c0: 2043 6f6e 6e65 6374 2074 6f20 796f 7572   Connect to your
+000017d0: 2050 6f73 7467 7265 5351 4c20 6461 7461   PostgreSQL data
+000017e0: 6261 7365 2061 6e64 2065 7865 6375 7465  base and execute
+000017f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2053   the following S
+00001800: 514c 2063 6f6d 6d61 6e64 2074 6f20 6372  QL command to cr
+00001810: 6561 7465 2074 6865 2060 7067 7665 6374  eate the `pgvect
+00001820: 6f72 6020 6578 7465 6e73 696f 6e3a 0d0a  or` extension:..
+00001830: 0d0a 2020 2060 6060 7371 6c0d 0a20 2020  ..   ```sql..   
+00001840: 2d2d 2043 6f6e 6e65 6374 2074 6f20 796f  -- Connect to yo
+00001850: 7572 2064 6174 6162 6173 650d 0a20 2020  ur database..   
+00001860: 7073 716c 202d 5520 7573 6572 6e61 6d65  psql -U username
+00001870: 202d 6420 6461 7461 6261 7365 5f6e 616d   -d database_nam
+00001880: 650d 0a0d 0a20 2020 2d2d 2052 756e 2069  e....   -- Run i
+00001890: 6e73 6964 6520 796f 7572 2070 7371 6c20  nside your psql 
+000018a0: 7465 726d 696e 616c 0d0a 2020 2043 5245  terminal..   CRE
+000018b0: 4154 4520 4558 5445 4e53 494f 4e20 7665  ATE EXTENSION ve
+000018c0: 6374 6f72 3b0d 0a20 2020 2320 5265 706c  ctor;..   # Repl
+000018d0: 6163 6520 7468 6520 706c 6163 6568 6f6c  ace the placehol
+000018e0: 6465 7273 2077 6974 6820 796f 7572 2061  ders with your a
+000018f0: 6374 7561 6c20 506f 7374 6772 6553 514c  ctual PostgreSQL
+00001900: 2063 7265 6465 6e74 6961 6c73 2061 6e64   credentials and
+00001910: 2064 6574 6169 6c73 0d0a 0d0a 4164 6469   details....Addi
+00001920: 7469 6f6e 616c 6c79 2c20 666f 7220 7468  tionally, for th
+00001930: 6f73 6520 696e 7465 7265 7374 6564 2069  ose interested i
+00001940: 6e20 6578 706c 6f72 696e 6720 6f74 6865  n exploring othe
+00001950: 7220 7665 6374 6f72 2064 6174 6162 6173  r vector databas
+00001960: 6520 6f70 7469 6f6e 732c 2079 6f75 2063  e options, you c
+00001970: 616e 2063 6f6e 7369 6465 7220 7573 696e  an consider usin
+00001980: 6720 2a2a 4368 726f 6d61 2a2a 206f 7220  g **Chroma** or 
+00001990: 2a0d 0a2a 4661 6973 732a 2a2e 2054 6865  *..*Faiss**. The
+000019a0: 7365 2070 726f 7669 6465 2061 6c74 6572  se provide alter
+000019b0: 6e61 7469 7665 2061 7070 726f 6163 6865  native approache
+000019c0: 7320 746f 2076 6563 746f 7220 7374 6f72  s to vector stor
+000019d0: 6167 6520 616e 6420 7265 7472 6965 7661  age and retrieva
+000019e0: 6c20 7468 6174 206d 6179 2062 6574 7465  l that may bette
+000019f0: 7220 7375 6974 2073 7065 6369 6669 6320  r suit specific 
+00001a00: 7573 6520 6361 7365 730d 0a6f 7220 7065  use cases..or pe
+00001a10: 7266 6f72 6d61 6e63 6520 7265 7175 6972  rformance requir
+00001a20: 656d 656e 7473 2e0d 0a0d 0a23 2323 2049  ements.....### I
+00001a30: 6d70 6f72 7469 6e67 2051 4120 616e 6420  mporting QA and 
+00001a40: 456d 6265 6464 696e 6720 4d6f 6465 6c73  Embedding Models
+00001a50: 0d0a 0d0a 6060 6020 7079 7468 6f6e 0d0a  ....``` python..
+00001a60: 6672 6f6d 2049 6e64 6f78 2e51 614d 6f64  from Indox.QaMod
+00001a70: 656c 7320 696d 706f 7274 204f 7065 6e41  els import OpenA
+00001a80: 6951 410d 0a60 6060 0d0a 0d0a 6060 6020  iQA..```....``` 
+00001a90: 7079 7468 6f6e 0d0a 6672 6f6d 2049 6e64  python..from Ind
+00001aa0: 6f78 2e45 6d62 6564 6469 6e67 7320 696d  ox.Embeddings im
+00001ab0: 706f 7274 204f 7065 6e41 6945 6d62 6564  port OpenAiEmbed
+00001ac0: 6469 6e67 0d0a 6060 600d 0a0d 0a0d 0a60  ding..```......`
+00001ad0: 6060 2070 7974 686f 6e0d 0a6f 7065 6e61  `` python..opena
+00001ae0: 695f 7161 203d 204f 7065 6e41 6951 4128  i_qa = OpenAiQA(
+00001af0: 6170 695f 6b65 793d 4f50 454e 4149 5f41  api_key=OPENAI_A
+00001b00: 5049 5f4b 4559 2c6d 6f64 656c 3d22 6770  PI_KEY,model="gp
+00001b10: 742d 332e 352d 7475 7262 6f2d 3031 3235  t-3.5-turbo-0125
+00001b20: 2229 0d0a 6f70 656e 6169 5f65 6d62 6564  ")..openai_embed
+00001b30: 6469 6e67 7320 3d20 4f70 656e 4169 456d  dings = OpenAiEm
+00001b40: 6265 6464 696e 6728 6d6f 6465 6c3d 2274  bedding(model="t
+00001b50: 6578 742d 656d 6265 6464 696e 672d 332d  ext-embedding-3-
+00001b60: 736d 616c 6c22 2c6f 7065 6e61 695f 6170  small",openai_ap
+00001b70: 695f 6b65 793d 4f50 454e 4149 5f41 5049  i_key=OPENAI_API
+00001b80: 5f4b 4559 290d 0a60 6060 0d0a 0d0a 2323  _KEY)..```....##
+00001b90: 204d 6f64 6966 7969 6e67 2043 6f6e 6669   Modifying Confi
+00001ba0: 6775 7261 7469 6f6e 2053 6574 7469 6e67  guration Setting
+00001bb0: 730d 0a0d 0a54 6f20 6368 616e 6765 2061  s....To change a
+00001bc0: 2063 6f6e 6669 6775 7261 7469 6f6e 2073   configuration s
+00001bd0: 6574 7469 6e67 2c20 796f 7520 6361 6e20  etting, you can 
+00001be0: 6469 7265 6374 6c79 206d 6f64 6966 7920  directly modify 
+00001bf0: 7468 650d 0a60 496e 646f 782e 636f 6e66  the..`Indox.conf
+00001c00: 6967 6020 6469 6374 696f 6e61 7279 2e20  ig` dictionary. 
+00001c10: 4865 7265 2069 7320 616e 2065 7861 6d70  Here is an examp
+00001c20: 6c65 206f 6620 686f 7720 796f 7520 6361  le of how you ca
+00001c30: 6e20 7570 6461 7465 2061 0d0a 636f 6e66  n update a..conf
+00001c40: 6967 7572 6174 696f 6e20 7365 7474 696e  iguration settin
+00001c50: 673a 0d0a 0d0a 6060 6020 7079 7468 6f6e  g:....``` python
+00001c60: 0d0a 2320 4578 616d 706c 6520 6f66 206d  ..# Example of m
+00001c70: 6f64 6966 7969 6e67 2061 2063 6f6e 6669  odifying a confi
+00001c80: 6775 7261 7469 6f6e 2073 6574 7469 6e67  guration setting
+00001c90: 0d0a 496e 646f 782e 636f 6e66 6967 5b22  ..Indox.config["
+00001ca0: 6f6c 645f 636f 6e66 6967 225d 203d 2022  old_config"] = "
+00001cb0: 6e65 775f 636f 6e66 6967 220d 0a0d 0a23  new_config"....#
+00001cc0: 2041 7070 6c79 696e 6720 7468 6520 7570   Applying the up
+00001cd0: 6461 7465 6420 636f 6e66 6967 7572 6174  dated configurat
+00001ce0: 696f 6e0d 0a49 6e64 6f78 2e75 7064 6174  ion..Indox.updat
+00001cf0: 655f 636f 6e66 6967 2829 0d0a 6060 600d  e_config()..```.
+00001d00: 0a0d 0a0d 0a57 6520 7461 6b65 2061 6476  .....We take adv
+00001d10: 616e 7461 6765 206f 6620 7468 6520 6075  antage of the `u
+00001d20: 6e73 7472 7563 7475 7265 6460 206c 6962  nstructured` lib
+00001d30: 7261 7279 2074 6f20 6c6f 6164 0d0a 646f  rary to load..do
+00001d40: 6375 6d65 6e74 7320 616e 6420 7370 6c69  cuments and spli
+00001d50: 7420 7468 656d 2069 6e74 6f20 6368 756e  t them into chun
+00001d60: 6b73 2062 7920 7469 746c 652e 2054 6869  ks by title. Thi
+00001d70: 7320 6d65 7468 6f64 2068 656c 7073 2069  s method helps i
+00001d80: 6e0d 0a6f 7267 616e 697a 696e 6720 7468  n..organizing th
+00001d90: 6d65 2064 6f63 756d 656e 7420 696e 746f  me document into
+00001da0: 206d 616e 6167 6561 626c 6520 7365 6374   manageable sect
+00001db0: 696f 6e73 2066 6f72 2066 7572 7468 6572  ions for further
+00001dc0: 0d0a 7072 6f63 6573 7369 6e67 2e0d 0a0d  ..processing....
+00001dd0: 0a60 6060 2070 7974 686f 6e0d 0a66 726f  .``` python..fro
+00001de0: 6d20 496e 646f 782e 4461 7461 4c6f 6164  m Indox.DataLoad
+00001df0: 6572 5370 6c69 7474 6572 2069 6d70 6f72  erSplitter impor
+00001e00: 7420 556e 7374 7275 6374 7572 6564 4c6f  t UnstructuredLo
+00001e10: 6164 416e 6453 706c 6974 0d0a 6060 600d  adAndSplit..```.
+00001e20: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a64  ...``` python..d
+00001e30: 6f63 735f 756e 7374 7275 6374 7572 6564  ocs_unstructured
+00001e40: 203d 2055 6e73 7472 7563 7475 7265 644c   = UnstructuredL
+00001e50: 6f61 6441 6e64 5370 6c69 7428 6669 6c65  oadAndSplit(file
+00001e60: 5f70 6174 683d 6669 6c65 5f70 6174 6829  _path=file_path)
+00001e70: 0d0a 6060 600d 0a0d 0a20 2020 2053 7461  ..```....    Sta
+00001e80: 7274 696e 6720 7072 6f63 6573 7369 6e67  rting processing
+00001e90: 2e2e 2e0d 0a20 2020 2045 6e64 2043 6875  .....    End Chu
+00001ea0: 6e6b 696e 6720 7072 6f63 6573 732e 0d0a  nking process...
+00001eb0: 0d0a 5374 6f72 696e 6720 646f 6375 6d65  ..Storing docume
+00001ec0: 6e74 2063 6875 6e6b 7320 696e 2061 2076  nt chunks in a v
+00001ed0: 6563 746f 7220 7374 6f72 6520 6973 2063  ector store is c
+00001ee0: 7275 6369 616c 2066 6f72 2065 6e61 626c  rucial for enabl
+00001ef0: 696e 670d 0a65 6666 6963 6965 6e74 2072  ing..efficient r
+00001f00: 6574 7269 6576 616c 2061 6e64 2073 6561  etrieval and sea
+00001f10: 7263 6820 6f70 6572 6174 696f 6e73 2e20  rch operations. 
+00001f20: 4279 2063 6f6e 7665 7274 696e 6720 7465  By converting te
+00001f30: 7874 2064 6174 6120 696e 746f 0d0a 7665  xt data into..ve
+00001f40: 6374 6f72 2072 6570 7265 7365 6e74 6174  ctor representat
+00001f50: 696f 6e73 2061 6e64 2073 746f 7269 6e67  ions and storing
+00001f60: 2074 6865 6d20 696e 2061 2076 6563 746f   them in a vecto
+00001f70: 7220 7374 6f72 652c 2079 6f75 2063 616e  r store, you can
+00001f80: 0d0a 7065 7266 6f72 6d20 7261 7069 6420  ..perform rapid 
+00001f90: 7369 6d69 6c61 7269 7479 2073 6561 7263  similarity searc
+00001fa0: 6865 7320 616e 6420 6f74 6865 7220 7665  hes and other ve
+00001fb0: 6374 6f72 2d62 6173 6564 206f 7065 7261  ctor-based opera
+00001fc0: 7469 6f6e 732e 0d0a 0d0a 6060 6020 7079  tions.....``` py
+00001fd0: 7468 6f6e 0d0a 496e 646f 782e 636f 6e6e  thon..Indox.conn
+00001fe0: 6563 745f 746f 5f76 6563 746f 7273 746f  ect_to_vectorsto
+00001ff0: 7265 2863 6f6c 6c65 6374 696f 6e5f 6e61  re(collection_na
+00002000: 6d65 3d22 7361 6d70 6c65 222c 656d 6265  me="sample",embe
+00002010: 6464 696e 6773 3d6f 7065 6e61 695f 656d  ddings=openai_em
+00002020: 6265 6464 696e 6773 290d 0a49 6e64 6f78  beddings)..Indox
+00002030: 2e73 746f 7265 5f69 6e5f 7665 6374 6f72  .store_in_vector
+00002040: 7374 6f72 6528 6368 756e 6b73 3d64 6f63  store(chunks=doc
+00002050: 735f 756e 7374 7275 6374 7572 6564 290d  s_unstructured).
+00002060: 0a60 6060 0d0a 0d0a 2323 2051 7565 7269  .```....## Queri
+00002070: 6e67 0d0a 0d0a 6060 6020 7079 7468 6f6e  ng....``` python
+00002080: 0d0a 7175 6572 7920 3d20 2279 6f75 7220  ..query = "your 
+00002090: 7175 6572 7921 213f 3f22 0d0a 6060 600d  query!!??"..```.
+000020a0: 0a0d 0a60 6060 2070 7974 686f 6e0d 0a72  ...``` python..r
+000020b0: 6573 706f 6e73 655f 6f70 656e 6169 203d  esponse_openai =
+000020c0: 2049 6e64 6f78 2e61 6e73 7765 725f 7175   Indox.answer_qu
+000020d0: 6573 7469 6f6e 2871 7565 7279 3d71 7565  estion(query=que
+000020e0: 7279 2c71 615f 6d6f 6465 6c3d 6f70 656e  ry,qa_model=open
+000020f0: 6169 5f71 6129 0d0a 6060 600d 0a0d 0a60  ai_qa)..```....`
+00002100: 6060 2070 7974 686f 6e0d 0a61 6e73 7765  `` python..answe
+00002110: 7220 3d20 7265 7370 6f6e 7365 5f6f 7065  r = response_ope
+00002120: 6e61 695b 305d 0d0a 6060 600d 0a0d 0a60  nai[0]..```....`
+00002130: 6060 2070 7974 686f 6e0d 0a63 6f6e 7465  `` python..conte
+00002140: 7874 2c20 7363 6f72 6520 3d20 7265 7370  xt, score = resp
+00002150: 6f6e 7365 5f6f 7065 6e61 695b 315d 0d0a  onse_openai[1]..
+00002160: 6060 600d 0a0d 0a                        ```....
```

### Comparing `indox-0.1.4/setup.py` & `Indox-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Read the README file for the long description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='Indox',
-    version='0.1.4',
+    version='0.1.5',
     license='MIT',
     packages=find_packages(),
     package_data={'Indox': ['config.yaml']},
     include_package_data=True,
     description='Indox Retrieval Augmentation',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

