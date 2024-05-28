# Comparing `tmp/melting_schemas-1.0.8.tar.gz` & `tmp/melting_schemas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melting_schemas-1.0.8.tar", last modified: Mon Apr 29 18:26:10 2024, max compression
+gzip compressed data, was "melting_schemas-1.0.9.tar", last modified: Tue May 28 16:20:29 2024, max compression
```

## Comparing `melting_schemas-1.0.8.tar` & `melting_schemas-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.552070 melting_schemas-1.0.8/melting_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/completion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/fcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/tcall.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/completion/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/encoding/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/encoding/text_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/historian/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/chat_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/historian/text_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas/templating/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/templating/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/melting_schemas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/melting_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 18:26:10.000000 melting_schemas-1.0.8/melting_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:26:10.556069 melting_schemas-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-29 18:26:02.000000 melting_schemas-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/completion/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/completion/fcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/completion/tcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/completion/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas/encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/encoding/text_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas/historian/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/historian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/historian/chat_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/historian/text_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/templating/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/melting_schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/melting_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 16:20:29.000000 melting_schemas-1.0.9/melting_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-28 16:20:29.000000 melting_schemas-1.0.9/melting_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:20:29.000000 melting_schemas-1.0.9/melting_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 16:20:29.000000 melting_schemas-1.0.9/melting_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 16:20:29.000000 melting_schemas-1.0.9/melting_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:20:29.544018 melting_schemas-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-28 16:20:20.000000 melting_schemas-1.0.9/setup.py
```

### Comparing `melting_schemas-1.0.8/melting_schemas/completion/chat.py` & `melting_schemas-1.0.9/melting_schemas/completion/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class ChatModelSettings(TypedDict, total=False):
     """
     Change these settings to tweak the model's behavior.
 
     Heavily inspired by https://platform.openai.com/docs/api-reference/chat/create
     """
+
     model: Required[str]
     max_tokens: int  # defaults to inf
     temperature: float  # ValueRange(0, 2)
     top_p: float  # ValueRange(0, 1)
     frequency_penalty: float  # ValueRange(-2, 2) defaults to 0
     presence_penalty: float  # ValueRange(-2, 2) defaults to 0
     logit_bias: dict[int, int]  # valmap(ValueRange(-100, 100))
@@ -35,15 +36,15 @@
     completion_tokens: int
     total_tokens: int
 
 
 class TemplateInputs(TypedDict):
     inputs: dict[str, str]
     name: NotRequired[str]
-    role: Literal["user", "system"]
+    role: Literal["user", "system", "assistant"]
     # advanced usage: select sub-templates
     template_name: NotRequired[str]
 
 
 class Templating(TypedDict):
     prompt_inputs: list[TemplateInputs | dict]
     prompt_id: str
```

### Comparing `melting_schemas-1.0.8/melting_schemas/completion/fcall.py` & `melting_schemas-1.0.9/melting_schemas/completion/fcall.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/melting_schemas/completion/tcall.py` & `melting_schemas-1.0.9/melting_schemas/completion/tcall.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import datetime
+from datetime import datetime
 from typing import Literal, Optional, Required, TypedDict
-from pydantic import BaseModel
-
-from melting_schemas.meta import Creator
-
-from ..completion.chat import ChatMLMessage, Templating
 
-from ..json_schema import FunctionJSONSchema
-from datetime import datetime
 from pydantic import BaseModel, Field
-from melting_schemas.utils import Timings, StreamTimings
 
-from ..completion.chat import ChatModelSettings
+from melting_schemas.meta import Creator
+from melting_schemas.utils import StreamTimings, Timings
+
+from ..completion.chat import ChatMLMessage, ChatModelSettings, Templating
 from ..json_schema import FunctionJSONSchema
 from ..meta import Creator
 
 
 class TCallModelSettings(TypedDict, total=False):
     """
     Change these settings to tweak the model's behavior.
@@ -55,14 +51,15 @@
     function: FunctionJSONSchema
 
 
 class RawTCallRequest(BaseModel):
     tools: list[ToolJSONSchema]
     messages: list[ChatMLMessage | ToolCallMLMessage | ToolMLMessage]
     settings: TCallModelSettings
+    tool_choice: Optional[Literal["auto", "required"] | dict] = "auto"
 
     class Config:
         smart_unions = True
         examples = {
             "Tool calling": {
                 "tools": [
                     {
@@ -93,14 +90,15 @@
                         "function_call": {
                             "name": "my_function",
                             "arguments": '{"my_param": "my_value"}',
                         },
                         "role": "assistant",
                     },
                 ],
+                "tool_choice": "auto",
             }
         }
 
 
 class TokenUsage(TypedDict):
     prompt_tokens: int
     completion_tokens: int
```

### Comparing `melting_schemas-1.0.8/melting_schemas/completion/text.py` & `melting_schemas-1.0.9/melting_schemas/completion/text.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/melting_schemas/encoding/text_encoding.py` & `melting_schemas-1.0.9/melting_schemas/encoding/text_encoding.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/melting_schemas/historian/text_completions.py` & `melting_schemas-1.0.9/melting_schemas/historian/text_completions.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/melting_schemas/templating/prompt.py` & `melting_schemas-1.0.9/melting_schemas/templating/prompt.py`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/melting_schemas.egg-info/SOURCES.txt` & `melting_schemas-1.0.9/melting_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melting_schemas-1.0.8/setup.py` & `melting_schemas-1.0.9/setup.py`

 * *Files identical despite different names*

