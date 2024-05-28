# Comparing `tmp/flytekitplugins_openai-1.12.1b3.tar.gz` & `tmp/flytekitplugins_openai-1.12.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_openai-1.12.1b3.tar", last modified: Wed May 22 18:21:14 2024, max compression
+gzip compressed data, was "flytekitplugins_openai-1.12.1b4.tar", last modified: Tue May 28 15:50:28 2024, max compression
```

## Comparing `flytekitplugins_openai-1.12.1b3.tar` & `flytekitplugins_openai-1.12.1b4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.994888 flytekitplugins_openai-1.12.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 18:21:13.994888 flytekitplugins_openai-1.12.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.990888 flytekitplugins_openai-1.12.1b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.990888 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.990888 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.990888 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-22 18:20:42.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:13.994888 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:13.000000 flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:13.994888 flytekitplugins_openai-1.12.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 18:21:06.000000 flytekitplugins_openai-1.12.1b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.635393 flytekitplugins_openai-1.12.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-28 15:50:28.635393 flytekitplugins_openai-1.12.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.631393 flytekitplugins_openai-1.12.1b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.631393 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.631393 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.631393 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-28 15:49:57.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:28.631393 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:28.000000 flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:28.635393 flytekitplugins_openai-1.12.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-28 15:50:20.000000 flytekitplugins_openai-1.12.1b4/setup.py
```

### Comparing `flytekitplugins_openai-1.12.1b3/PKG-INFO` & `flytekitplugins_openai-1.12.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_openai-1.12.1b3/README.md` & `flytekitplugins_openai-1.12.1b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/__init__.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/agent.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,22 +98,20 @@
 
         message = None
         if current_state in State.Failed.value and retrieved_result.errors:
             data = retrieved_result.errors.data
             if data and data[0].message:
                 message = data[0].message
 
-        outputs = {"result": {"result": None}}
-        if current_state in State.Success.value:
-            result = retrieved_result.to_dict()
+        result = retrieved_result.to_dict()
 
-            ctx = FlyteContextManager.current_context()
-            outputs = LiteralMap(
-                literals={"result": TypeEngine.to_literal(ctx, result, Dict, TypeEngine.to_literal_type(Dict))}
-            )
+        ctx = FlyteContextManager.current_context()
+        outputs = LiteralMap(
+            literals={"result": TypeEngine.to_literal(ctx, result, Dict, TypeEngine.to_literal_type(Dict))}
+        )
 
         return Resource(phase=flyte_phase, outputs=outputs, message=message)
 
     async def delete(
         self,
         resource_meta: BatchEndpointMetadata,
         **kwargs,
```

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/task.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/batch/workflow.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/batch/workflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Iterator
 
-from flytekit import Workflow
+from flytekit import Resources, Workflow
 from flytekit.models.security import Secret
 from flytekit.types.file import JSONLFile
 from flytekit.types.iterator import JSON
 
 from .task import (
     BatchEndpointTask,
     BatchResult,
@@ -16,23 +16,27 @@
 
 def create_batch(
     name: str,
     openai_organization: str,
     secret: Secret,
     config: Dict[str, Any] = {},
     is_json_iterator: bool = True,
+    file_upload_mem: str = "700Mi",
+    file_download_mem: str = "700Mi",
 ) -> Workflow:
     """
     Uploads JSON data to a JSONL file, creates a batch, waits for it to complete, and downloads the output/error JSON files.
 
     :param name: The suffix to be added to workflow and task names.
     :param openai_organization: Name of the OpenAI organization.
     :param secret: Secret comprising the OpenAI API key.
     :param config: Additional config for batch creation.
     :param is_json_iterator: Set to True if you're sending an iterator/generator; if a JSONL file, set to False.
+    :param file_upload_mem: Memory to allocate to the upload file task.
+    :param file_download_mem: Memory to allocate to the download file task.
     """
     wf = Workflow(name=f"openai-batch-{name.replace('.', '')}")
 
     if is_json_iterator:
         wf.add_workflow_input("jsonl_in", Iterator[JSON])
     else:
         wf.add_workflow_input("jsonl_in", JSONLFile)
@@ -60,10 +64,13 @@
         input_file_id=node_1.outputs["result"],
     )
     node_3 = wf.add_entity(
         download_json_files_task_obj,
         batch_endpoint_result=node_2.outputs["result"],
     )
 
+    node_1.with_overrides(requests=Resources(mem=file_upload_mem), limits=Resources(mem=file_upload_mem))
+    node_3.with_overrides(requests=Resources(mem=file_download_mem), limits=Resources(mem=file_download_mem))
+
     wf.add_workflow_output("batch_output", node_3.outputs["result"], BatchResult)
 
     return wf
```

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/agent.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins/openai/chatgpt/task.py` & `flytekitplugins_openai-1.12.1b4/flytekitplugins/openai/chatgpt/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/PKG-INFO` & `flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_openai-1.12.1b3/flytekitplugins_openai.egg-info/SOURCES.txt` & `flytekitplugins_openai-1.12.1b4/flytekitplugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b3/setup.py` & `flytekitplugins_openai-1.12.1b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "openai"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>1.10.7", "openai>=1.12.0", "flyteidl>=1.11.0"]
 
-__version__ = "1.12.1b3"
+__version__ = "1.12.1b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the openai plugins for flytekit",
```

