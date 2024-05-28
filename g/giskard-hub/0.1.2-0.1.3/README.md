# Comparing `tmp/giskard_hub-0.1.2.tar.gz` & `tmp/giskard_hub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard_hub-0.1.2.tar", max compression
+gzip compressed data, was "giskard_hub-0.1.3.tar", max compression
```

## Comparing `giskard_hub-0.1.2.tar` & `giskard_hub-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/LICENSE
--rw-r--r--   0        0        0     5237 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/README.md
--rw-r--r--   0        0        0     1282 2024-05-27 16:18:02.256055 giskard_hub-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/src/giskard_hub/__init__.py
--rw-r--r--   0        0        0     5663 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/src/giskard_hub/cli.py
--rw-r--r--   0        0        0     9904 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/src/giskard_hub/client.py
--rw-r--r--   0        0        0     3900 2024-05-27 16:17:46.396068 giskard_hub-0.1.2/src/giskard_hub/data.py
--rw-r--r--   0        0        0     6258 1970-01-01 00:00:00.000000 giskard_hub-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 16:27:50.767679 giskard_hub-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5350 2024-05-28 16:27:50.767679 giskard_hub-0.1.3/README.md
+-rw-r--r--   0        0        0     1282 2024-05-28 16:28:08.343843 giskard_hub-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 16:27:50.771679 giskard_hub-0.1.3/src/giskard_hub/__init__.py
+-rw-r--r--   0        0        0     5663 2024-05-28 16:27:50.771679 giskard_hub-0.1.3/src/giskard_hub/cli.py
+-rw-r--r--   0        0        0     9904 2024-05-28 16:27:50.771679 giskard_hub-0.1.3/src/giskard_hub/client.py
+-rw-r--r--   0        0        0     5387 2024-05-28 16:27:50.771679 giskard_hub-0.1.3/src/giskard_hub/data.py
+-rw-r--r--   0        0        0     6371 1970-01-01 00:00:00.000000 giskard_hub-0.1.3/PKG-INFO
```

### Comparing `giskard_hub-0.1.2/LICENSE` & `giskard_hub-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.2/README.md` & `giskard_hub-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Quick Start
 
+## Install the library
+
+The library is compatible with Python 3.9 - 3.12.
+
+```bash
+pip install giskard-hub
+```
+
 ## Evaluating from your Jupyter notebook
 
 Start by initializing a client.
 
 ```python
 from giskard_hub.client import HubClient
 
@@ -158,8 +166,8 @@
                 "Agent must be polite",
             ],
             expected_output="Orange.",
         )
     )
     print("Got results")
     print(results)
-```
+```
```

### Comparing `giskard_hub-0.1.2/pyproject.toml` & `giskard_hub-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giskard-hub"
-version = "0.1.2"
+version = "0.1.3"
 description = "The giskard_hub library allows you to interact with the Giskard Hub, a platform that centralizes the validation process of LLM applications, empowering product teams to ensure all functional, business & legal requirements are met, and keeping them in close contact with the development team to avoid delayed deployment timelines."
 authors = ["Bazire <bazire@giskard.ai>"]
 readme = "README.md"
 packages = [{ include = "giskard_hub", from = "src" }]
 repository = "https://github.com/Giskard-AI/giskard-hub"
 homepage = "https://github.com/Giskard-AI/giskard-hub"
 documentation = "https://docs-hub.giskard.ai/"
```

### Comparing `giskard_hub-0.1.2/src/giskard_hub/cli.py` & `giskard_hub-0.1.3/src/giskard_hub/cli.py`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.2/src/giskard_hub/client.py` & `giskard_hub-0.1.3/src/giskard_hub/client.py`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.2/src/giskard_hub/data.py` & `giskard_hub-0.1.3/src/giskard_hub/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
 
 
 @dataclass
-class Entity:
-    """Base class containing audit fields and id."""
-
-    id: str
-    created_at: datetime
-    updated_at: datetime
+class BaseDataclass:
+    """Base dataclass containing utility function."""
 
     @classmethod
     def from_dict(
         cls, data: Dict[str, Any], filter: Optional[List[str]] = None
     ) -> "Entity":
         """Class method factory, allowing to filter from a dict.
 
@@ -25,14 +21,23 @@
         """
         if filter is None:
             filter = []
         return cls(**{k: v for k, v in data.items() if k not in filter})
 
 
 @dataclass
+class Entity(BaseDataclass):
+    """Base class containing audit fields and id."""
+
+    id: str
+    created_at: datetime
+    updated_at: datetime
+
+
+@dataclass
 class Project(Entity):
     """Project object (container with name and description)."""
 
     name: str
     description: str
 
 
@@ -55,49 +60,75 @@
     project_id: str
     name: str
     description: str
     tags: List[str]
 
 
 @dataclass
-class Metric:
+class Metric(BaseDataclass):
     """Metric object, with number of passed, failed and errored evaluations."""
 
     name: str
     passed: int
     failed: int
     errored: int
     total: int
 
 
 @dataclass
-class LLMMessage:
+class LLMMessage(BaseDataclass):
     """Message from an agent/llm, with role & content."""
 
     role: Literal["system", "assistant", "user"]
     content: str
 
 
 @dataclass
 class Conversation(Entity):
     """Dataset item, containing full conversation (ie messages), policies for compliance, expected_output for correctness and tags for filtering"""
 
     messages: List[LLMMessage]
     policies: List[str]
     tags: List[str]
     expected_output: Optional[str]
+    demo_output: Optional[LLMMessage]
+
+    @classmethod
+    def from_dict(
+        cls, data: Dict[str, Any], filter: Optional[List[str]] = None
+    ) -> "Conversation":
+        if filter is None:
+            filter = ["dataset_id", "notes"]
+        data: Conversation = super().from_dict(data, filter=filter)
+        data.messages = (
+            []
+            if data.messages is None
+            else [LLMMessage.from_dict(msg) for msg in data.messages]
+        )
+        data.demo_output = (
+            None if data.demo_output is None else LLMMessage.from_dict(data.demo_output)
+        )
+        return data
 
 
 @dataclass
-class ModelOutput:
+class ModelOutput(BaseDataclass):
     """Expected format for an answer from an agent/model"""
 
     response: LLMMessage
     metadata: dict[str, Any] = field(default_factory=dict)
 
+    @classmethod
+    def from_dict(
+        cls, data: Dict[str, Any], filter: Optional[List[str]] = None
+    ) -> "ModelOutput":
+        data: ModelOutput = super().from_dict(data, filter=filter)
+        data.response = LLMMessage.from_dict(data.response)
+        return data
+
 
 @dataclass
 class Evaluation(Entity):
     """Single item evaluation, containing both the conversation, output of the agent and results of the evaluation."""
 
     execution_id: str
     conversation: Conversation
@@ -108,41 +139,55 @@
         """Convenience method to create a ModelOutput from a string.
 
         Args:
             output (str): the simple output from the model/agent
         """
         self.output = ModelOutput(response=LLMMessage(role="assistant", content=output))
 
+    @classmethod
+    def from_dict(
+        cls, data: Dict[str, Any], filter: Optional[List[str]] = None
+    ) -> "Evaluation":
+        data: Evaluation = super().from_dict(data, filter=filter)
+        data.conversation = Conversation.from_dict(data.conversation)
+        data.output = (
+            None if data.output is None else ModelOutput.from_dict(data.output)
+        )
+        return data
+
 
 @dataclass
-class TransientEvaluation:
+class TransientEvaluation(BaseDataclass):
     """Object to run a single evaluation without saving anything"""
+
     model_output: ModelOutput
     model_description: str
     messages: List[LLMMessage]
     policies: Optional[List[str]] = field(default_factory=list)
     expected_output: Optional[str] = field(default=None)
 
+    @classmethod
+    def from_dict(
+        cls, data: Dict[str, Any], filter: Optional[List[str]] = None
+    ) -> "TransientEvaluation":
+        data: TransientEvaluation = super().from_dict(data, filter=filter)
+        data.messages = (
+            []
+            if data.messages is None
+            else [LLMMessage.from_dict(msg) for msg in data.messages]
+        )
+        data.model_output = (
+            None
+            if data.model_output is None
+            else ModelOutput.from_dict(data.model_output)
+        )
+        return data
+
 
 @dataclass
-class TestResult:
+class TestResult(BaseDataclass):
     """Object containing the metric for a transient evaluation"""
+
     name: str
     passed: Optional[bool] = field(default=None)
     error: Optional[str] = field(default=None)
     reason: Optional[str] = field(default=None)
-
-    @classmethod
-    def from_dict(
-        cls, data: Dict[str, Any], filter: Optional[List[str]] = None
-    ) -> "Entity":
-        """Class method factory, allowing to filter from a dict.
-
-        Args:
-            data (Dict[str, Any]): the data to use to initialise the dataclass
-            filter (Optional[List[str]], optional): list of fields to ignore. Defaults to None.
-
-        Returns:
-        """
-        if filter is None:
-            filter = []
-        return cls(**{k: v for k, v in data.items() if k not in filter})
```

### Comparing `giskard_hub-0.1.2/PKG-INFO` & `giskard_hub-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard-hub
-Version: 0.1.2
+Version: 0.1.3
 Summary: The giskard_hub library allows you to interact with the Giskard Hub, a platform that centralizes the validation process of LLM applications, empowering product teams to ensure all functional, business & legal requirements are met, and keeping them in close contact with the development team to avoid delayed deployment timelines.
 Home-page: https://github.com/Giskard-AI/giskard-hub
 Author: Bazire
 Author-email: bazire@giskard.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,22 @@
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://docs-hub.giskard.ai/
 Project-URL: Repository, https://github.com/Giskard-AI/giskard-hub
 Description-Content-Type: text/markdown
 
 # Quick Start
 
+## Install the library
+
+The library is compatible with Python 3.9 - 3.12.
+
+```bash
+pip install giskard-hub
+```
+
 ## Evaluating from your Jupyter notebook
 
 Start by initializing a client.
 
 ```python
 from giskard_hub.client import HubClient
 
@@ -178,7 +186,8 @@
             ],
             expected_output="Orange.",
         )
     )
     print("Got results")
     print(results)
 ```
+
```

