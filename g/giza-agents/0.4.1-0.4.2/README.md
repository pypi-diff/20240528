# Comparing `tmp/giza_agents-0.4.1.tar.gz` & `tmp/giza_agents-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_agents-0.4.1.tar", max compression
+gzip compressed data, was "giza_agents-0.4.2.tar", max compression
```

## Comparing `giza_agents-0.4.1.tar` & `giza_agents-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2024-05-23 15:02:13.436045 giza_agents-0.4.1/LICENSE
--rw-r--r--   0        0        0     4609 2024-05-23 15:02:13.436045 giza_agents-0.4.1/README.md
--rw-r--r--   0        0        0      395 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/__init__.py
--rw-r--r--   0        0        0     5991 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/action.py
--rw-r--r--   0        0        0    17968 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/agent.py
--rw-r--r--   0        0        0      630 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/deployments.py
--rw-r--r--   0        0        0      252 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/logger.py
--rw-r--r--   0        0        0     3051 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/logging.yaml
--rw-r--r--   0        0        0    18146 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/model.py
--rw-r--r--   0        0        0      576 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/task.py
--rw-r--r--   0        0        0     1974 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/utils.py
--rw-r--r--   0        0        0     1206 2024-05-23 15:02:13.452045 giza_agents-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5659 1970-01-01 00:00:00.000000 giza_agents-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-28 08:36:23.612660 giza_agents-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4609 2024-05-28 08:36:23.612660 giza_agents-0.4.2/README.md
+-rw-r--r--   0        0        0      395 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/__init__.py
+-rw-r--r--   0        0        0     5991 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/action.py
+-rw-r--r--   0        0        0    17968 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/agent.py
+-rw-r--r--   0        0        0      630 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/deployments.py
+-rw-r--r--   0        0        0      252 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/logger.py
+-rw-r--r--   0        0        0     3051 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/logging.yaml
+-rw-r--r--   0        0        0    18187 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/model.py
+-rw-r--r--   0        0        0      576 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/task.py
+-rw-r--r--   0        0        0     1974 2024-05-28 08:36:23.624660 giza_agents-0.4.2/giza/agents/utils.py
+-rw-r--r--   0        0        0     1206 2024-05-28 08:36:23.624660 giza_agents-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5659 1970-01-01 00:00:00.000000 giza_agents-0.4.2/PKG-INFO
```

### Comparing `giza_agents-0.4.1/LICENSE` & `giza_agents-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/README.md` & `giza_agents-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/action.py` & `giza_agents-0.4.2/giza/agents/action.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/agent.py` & `giza_agents-0.4.2/giza/agents/agent.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/deployments.py` & `giza_agents-0.4.2/giza/agents/deployments.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/logging.yaml` & `giza_agents-0.4.2/giza/agents/logging.yaml`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/model.py` & `giza_agents-0.4.2/giza/agents/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,15 @@
         Returns:
             A tuple (predictions, request_id) where predictions is the result of the prediction and request_id
             is the identifier of the prediction request if verifiable computation is used, otherwise None.
 
         Raises:
             ValueError: If required parameters are not provided or the session is not initialized.
         """
+        output_dtype = "Tensor<FP16x16>"
         try:
             logger.info("Predicting")
             if verifiable:
                 if not self.uri:
                     raise ValueError("Model has not been deployed")
 
                 # Non common arguments should be named parameters
```

### Comparing `giza_agents-0.4.1/giza/agents/task.py` & `giza_agents-0.4.2/giza/agents/task.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/giza/agents/utils.py` & `giza_agents-0.4.2/giza/agents/utils.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.1/pyproject.toml` & `giza_agents-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-agents"
-version = "0.4.1"
+version = "0.4.2"
 
 description = "A Python SDK for Giza platform"
 authors = [
     "Francisco Algaba <fran@gizatech.xyz>",
     "Raphael Doukhan <raphael@gizatech.xyz>",
     "Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
```

### Comparing `giza_agents-0.4.1/PKG-INFO` & `giza_agents-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-agents
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python SDK for Giza platform
 License: MIT
 Author: Francisco Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

