# Comparing `tmp/agentkit-llm-0.1.7.post1.tar.gz` & `tmp/agentkit-llm-0.1.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.7.post1.tar", last modified: Thu May  9 00:26:26 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.7.post2.tar", last modified: Tue May 28 17:41:38 2024, max compression
```

## Comparing `agentkit-llm-0.1.7.post1.tar` & `agentkit-llm-0.1.7.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.7.post1/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8505 2024-05-06 21:46:13.000000 agentkit-llm-0.1.7.post1/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1074 2024-05-09 00:26:10.000000 agentkit-llm-0.1.7.post1/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.307713 agentkit-llm-0.1.7.post1/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.307713 agentkit-llm-0.1.7.post1/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.7.post1/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.7.post1/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-05-06 21:44:02.000000 agentkit-llm-0.1.7.post1/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.7.post1/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.7.post1/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.7.post1/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-06 21:41:05.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1635 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4226 2024-05-06 21:20:24.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3783 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/ollama.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1681 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.7.post1/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.7.post1/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.7.post1/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      683 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      124 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-28 17:41:38.712548 agentkit-llm-0.1.7.post2/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.7.post2/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-28 17:41:38.708548 agentkit-llm-0.1.7.post2/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8505 2024-05-06 21:46:13.000000 agentkit-llm-0.1.7.post2/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-28 17:41:38.712548 agentkit-llm-0.1.7.post2/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1074 2024-05-28 17:41:34.000000 agentkit-llm-0.1.7.post2/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-28 17:41:38.708548 agentkit-llm-0.1.7.post2/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-28 17:41:38.708548 agentkit-llm-0.1.7.post2/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.7.post2/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.7.post2/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-05-06 21:44:02.000000 agentkit-llm-0.1.7.post2/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.7.post2/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.7.post2/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.7.post2/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-28 17:41:38.708548 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-06 21:41:05.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1635 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4226 2024-05-06 21:20:24.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3783 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/ollama.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1907 2024-05-28 17:40:31.000000 agentkit-llm-0.1.7.post2/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.7.post2/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.7.post2/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2231 2024-05-28 17:37:56.000000 agentkit-llm-0.1.7.post2/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-28 17:41:38.708548 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      683 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      124 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-28 17:41:38.000000 agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.7.post1/LICENSE` & `agentkit-llm-0.1.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/PKG-INFO` & `agentkit-llm-0.1.7.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.7.post1/README.md` & `agentkit-llm-0.1.7.post2/README.md`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/setup.py` & `agentkit-llm-0.1.7.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.7.post1"
+VERSION = "0.1.7.post2"
 EXTRAS = {
     "logging": ["wandb"],
     "proprietary": ["wandb", "openai", "anthropic", "tiktoken"],
     "all": ["wandb", "openai", "anthropic", "tiktoken", "llama"],
 }
 
 setuptools.setup(
```

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/after_query.py` & `agentkit-llm-0.1.7.post2/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/base_node.py` & `agentkit-llm-0.1.7.post2/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.7.post2/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/exceptions.py` & `agentkit-llm-0.1.7.post2/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/graph.py` & `agentkit-llm-0.1.7.post2/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/ollama.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/ollama.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.7.post2/src/agentkit/llm_api/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 except ImportError:
     raise ImportError("Please install tiktoken to use built-in LLM API.")
 import difflib
 
 
 enc_fns = {
     "gpt-4":tiktoken.encoding_for_model("gpt-4"),
+    "gpt-4-o":tiktoken.encoding_for_model("gpt-4"),
     "gpt-4-turbo":tiktoken.encoding_for_model("gpt-4"),
     "gpt-4-1106-preview":tiktoken.encoding_for_model("gpt-4"),
     "gpt-4-32k-0613":tiktoken.encoding_for_model("gpt-4"),
     "gpt-3.5-turbo":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "gpt-3.5-turbo-1106":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "gpt-3.5-turbo-0125":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "claude-3": None,
     "claude-2.1": None,
     "ollama": None,
 }
 model_maxes = {
     "gpt-4":8192,
+    "gpt-4-o":128000,
     "gpt-4-turbo":128000,
     "gpt-4-1106-preview":128000,
     "gpt-4-32k-0613":32768,
     "gpt-3.5-turbo":16385,
     "gpt-3.5-turbo-1106":16385,
     "gpt-3.5-turbo-0125":16385,
     "claude-3":50000,
@@ -32,17 +34,22 @@
 }
 
 def match_model(model_name):
 
     # match model name to the closest string in enc_fns.keys()
     model_name = model_name.lower()
     if model_name.startswith('ollama'):
-    	model_name = 'ollama'
-    matches = difflib.get_close_matches(model_name, enc_fns.keys())
+        model_name = 'ollama'
+    
+    matches = []
     matches += [model for model in model_maxes.keys() if model_name.startswith(model)]
+    # sort by length of match
+    matches = sorted(matches, key=lambda x: len(x), reverse=True)
+    if len(matches) == 0:
+        matches += difflib.get_close_matches(model_name, enc_fns.keys())
     if len(matches) == 0:
         raise ValueError("Model name {} not found!".format(model_name))
     else:
         model = matches[0]
     print("Matched model_name {} to: {}. If this match is not accurate, then the token counter will not function properly.".format(model_name, model))
 
     model_max = model_maxes[model]
```

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/node.py` & `agentkit-llm-0.1.7.post2/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit/utils.py` & `agentkit-llm-0.1.7.post2/src/agentkit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+import traceback
+
 def extract_json_objects(input_string):
     try:
         # Initialize variables
         json_objects = []
         stack = []
         start_index = -1
```

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.7.post1
+Version: 0.1.7.post2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.7.post2/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

