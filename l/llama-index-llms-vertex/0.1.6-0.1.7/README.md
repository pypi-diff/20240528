# Comparing `tmp/llama_index_llms_vertex-0.1.6.tar.gz` & `tmp/llama_index_llms_vertex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_vertex-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_llms_vertex-0.1.7.tar", max compression
```

## Comparing `llama_index_llms_vertex-0.1.6.tar` & `llama_index_llms_vertex-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       38 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/README.md
--rw-r--r--   0        0        0       70 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/__init__.py
--rw-r--r--   0        0        0    13895 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/base.py
--rw-r--r--   0        0        0     1925 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/gemini_utils.py
--rw-r--r--   0        0        0     7793 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/utils.py
--rw-r--r--   0        0        0     1477 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/README.md
+-rw-r--r--   0        0        0       70 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/__init__.py
+-rw-r--r--   0        0        0    14285 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/base.py
+-rw-r--r--   0        0        0     2098 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/gemini_utils.py
+-rw-r--r--   0        0        0     7793 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/utils.py
+-rw-r--r--   0        0        0     1477 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.7/PKG-INFO
```

### Comparing `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/base.py` & `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     _parse_chat_history,
     _parse_examples,
     _parse_message,
     acompletion_with_retry,
     completion_with_retry,
     init_vertexai,
 )
+from vertexai.generative_models._generative_models import SafetySettingsType
 
 
 class Vertex(LLM):
     """Vertext LLM.
 
     Examples:
         `pip install llama-index-llms-vertex`
@@ -63,15 +64,17 @@
     model: str = Field(description="The vertex model to use.")
     temperature: float = Field(description="The temperature to use for sampling.")
     max_tokens: int = Field(description="The maximum number of tokens to generate.")
     examples: Optional[Sequence[ChatMessage]] = Field(
         description="Example messages for the chat model."
     )
     max_retries: int = Field(default=10, description="The maximum number of retries.")
-
+    safety_settings: Optional[SafetySettingsType] = Field(
+        default=None, description="Safety settings for the Vertex AI model."
+    )
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the Vertex."
     )
     iscode: bool = Field(
         default=False, description="Flag to determine if current model is a Code Model"
     )
     _is_gemini: bool = PrivateAttr()
@@ -86,24 +89,26 @@
         location: Optional[str] = None,
         credentials: Optional[Any] = None,
         examples: Optional[Sequence[ChatMessage]] = None,
         temperature: float = 0.1,
         max_tokens: int = 512,
         max_retries: int = 10,
         iscode: bool = False,
+        safety_settings: Optional[SafetySettingsType] = None,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
         pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
         output_parser: Optional[BaseOutputParser] = None,
     ) -> None:
         init_vertexai(project=project, location=location, credentials=credentials)
 
+        safety_settings = safety_settings or {}
         additional_kwargs = additional_kwargs or {}
         callback_manager = callback_manager or CallbackManager([])
 
         self._is_gemini = False
         self._is_chat_model = False
         if model in CHAT_MODELS:
             from vertexai.language_models import ChatModel
@@ -122,29 +127,30 @@
             self._client = CodeGenerationModel.from_pretrained(model)
             iscode = True
         elif model in TEXT_MODELS:
             from vertexai.language_models import TextGenerationModel
 
             self._client = TextGenerationModel.from_pretrained(model)
         elif is_gemini_model(model):
-            self._client = create_gemini_client(model)
+            self._client = create_gemini_client(model, safety_settings)
             self._chat_client = self._client
             self._is_gemini = True
             self._is_chat_model = True
         else:
             raise (ValueError(f"Model {model} not found, please verify the model name"))
 
         super().__init__(
             temperature=temperature,
             max_tokens=max_tokens,
             additional_kwargs=additional_kwargs,
             max_retries=max_retries,
             model=model,
             examples=examples,
             iscode=iscode,
+            safety_settings=safety_settings,
             callback_manager=callback_manager,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
             pydantic_program_mode=pydantic_program_mode,
             output_parser=output_parser,
         )
```

### Comparing `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/gemini_utils.py` & `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/gemini_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import base64
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, Optional
+from vertexai.generative_models._generative_models import SafetySettingsType
 
 from llama_index.core.llms import ChatMessage, MessageRole
 
 
 def is_gemini_model(model: str) -> bool:
     return model.startswith("gemini")
 
 
-def create_gemini_client(model: str) -> Any:
+def create_gemini_client(
+    model: str, safety_settings: Optional[SafetySettingsType]
+) -> Any:
     from vertexai.preview.generative_models import GenerativeModel
 
-    return GenerativeModel(model_name=model)
+    return GenerativeModel(model_name=model, safety_settings=safety_settings)
 
 
 def convert_chat_message_to_gemini_content(
     message: ChatMessage, is_history: bool = True
 ) -> Any:
     from vertexai.preview.generative_models import Content, Part
```

### Comparing `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/utils.py` & `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_vertex-0.1.6/pyproject.toml` & `llama_index_llms_vertex-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms vertex integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-vertex"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 google-cloud-aiplatform = "^1.39.0"
 pyarrow = "^15.0.2"
```

### Comparing `llama_index_llms_vertex-0.1.6/PKG-INFO` & `llama_index_llms_vertex-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-vertex
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index llms vertex integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

