# Comparing `tmp/puyuan_modelhub-1.1.7.tar.gz` & `tmp/puyuan_modelhub-1.1.8.tar.gz`

## Comparing `puyuan_modelhub-1.1.7.tar` & `puyuan_modelhub-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/client/__init__.py
--rw-r--r--   0        0        0    15782 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/client/client.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/client/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/constants.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/audio.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/base.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/chat.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/encoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/errors.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/generation.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/modelhub/common/types/message.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/LICENSE.txt
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/_version.py
+-rw-r--r--   0        0        0    13294 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/client.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/constants.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/errors.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/utils.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/audio.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/base.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/chat.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/encoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/errors.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/generation.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/message.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/LICENSE.txt
+-rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/PKG-INFO
```

### Comparing `puyuan_modelhub-1.1.7/modelhub/client/client.py` & `puyuan_modelhub-1.1.8/modelhub/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-import pydantic
-
-if pydantic.VERSION < "2.0.0":
-    from pydantic import BaseModel
-else:
-    from pydantic.v1 import BaseModel
-
+from modelhub.utils import BaseModel
 import json
 import os
 from io import TextIOWrapper
 from typing import Any, Dict, Generator, List, Literal, Optional, Union, AsyncGenerator
 
-import anyio
 import httpx
 import retrying
 from httpx import Response
 
-import modelhub.common.constants as constants
-from modelhub.common.types import (
+import modelhub.constants as constants
+from modelhub.types import (
     BaseMessage,
     ChatParameters,
     CrossEncoderOutput,
     CrossEncoderParams,
     EmbeddingOutput,
     ModelInfo,
     ModelInfoOutput,
@@ -123,16 +116,14 @@
         """
         Get the number of tokens in a prompt
         params:
             prompt: the prompt
             model: the model name
         """
         model = model or self.model
-        if model not in self.supported_models:
-            raise ValueError(f"Model {model} not supported")
         response = self._post(
             self.host + "/tokens",
             json={
                 "prompt": prompt,
                 "model": model,
                 "params": params,
             },
@@ -146,19 +137,14 @@
         history: List[Union[BaseMessage, Dict[str, Any]]] = [],
         return_type: Literal["text", "json", "regex"] = "text",
         return_schema: Union[Dict[str, Any], str, None] = None,
         parameters: ChatParameters = {},
         **kwargs,
     ) -> TextGenerationOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         parameters["history"] = [
             m.dict() if isinstance(m, BaseMessage) else m for m in history
         ]
         parameters["return_type"] = return_type
         parameters["schema"] = return_schema
         response = self._post(
             self.host + "/chat",
@@ -174,19 +160,14 @@
     def batch_chat(
         self,
         batch_prompts: List[str],
         model: str = "",
         batch_parameters: List[ChatParameters] = [],
     ):
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         response = self._post(
             self.host + "/batch_chat",
             json={
                 "batch_prompts": batch_prompts,
                 "model": model,
                 "batch_parameters": batch_parameters,
             },
@@ -197,19 +178,14 @@
     async def abatch_chat(
         self,
         batch_prompts: List[str],
         model: str = "",
         batch_parameters: List[ChatParameters] = [],
     ):
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         response = await self._apost(
             self.host + "/batch_chat",
             json={
                 "batch_prompts": batch_prompts,
                 "model": model,
                 "batch_parameters": batch_parameters,
             },
@@ -223,19 +199,14 @@
         model: str = "",
         history: List[BaseMessage] = [],
         return_type: Literal["text", "json", "regex"] = "text",
         return_schema: Union[Dict[str, Any], str, None] = None,
         parameters: ChatParameters = {},
     ) -> TextGenerationOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         parameters["history"] = [
             m.dict() if isinstance(m, BaseMessage) else m for m in history
         ]
         parameters["return_type"] = return_type
         parameters["schema"] = return_schema
         response = await self._apost(
             self.host + "/chat",
@@ -253,19 +224,14 @@
         self,
         prompt: str,
         model: str = "",
         history: List[BaseMessage] = [],
         parameters: Dict[str, Any] = {},
     ) -> Generator[TextGenerationStreamOutput, None, None]:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         parameters["history"] = [
             m.dict() if isinstance(m, BaseMessage) else m for m in history
         ]
         with httpx.Client() as client:
             with client.stream(
                 "post",
                 url=self.host + "/chat",
@@ -289,19 +255,14 @@
         self,
         prompt: str,
         model: str = "",
         history: List[BaseMessage] = [],
         parameters: Dict[str, Any] = {},
     ) -> AsyncGenerator[TextGenerationStreamOutput, None]:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "chat" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         parameters["history"] = [
             m.dict() if isinstance(m, BaseMessage) else m for m in history
         ]
         async with httpx.AsyncClient() as client:
             async with client.stream(
                 "post",
                 url=self.host + "/chat",
@@ -320,38 +281,28 @@
                         self.raise_for_status(r, out.code, out.msg)
                         yield out
 
     def get_embeddings(
         self, prompt: str, model: str = "", parameters: Dict[str, Any] = {}
     ) -> EmbeddingOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "embedding" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         response = self._post(
             self.host + "/embedding",
             json={
                 "prompt": prompt,
                 "model": model,
                 "parameters": parameters,
             },
         )
         return EmbeddingOutput(**response.json())
 
     async def aget_embeddings(
         self, prompt: str, model: str = "", parameters: Dict[str, Any] = {}
     ) -> EmbeddingOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "embedding" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         response = await self._apost(
             self.host + "/embedding",
             json={
                 "prompt": prompt,
                 "model": model,
                 "parameters": parameters,
             },
@@ -361,18 +312,14 @@
     def cross_embedding(
         self,
         sentences: List[List[str]],
         model: str = "",
         parameters: CrossEncoderParams = {},
     ) -> CrossEncoderOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "reranker" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
         res = self._post(
             self.host + "/cross_embedding",
             json={
                 "sentences": sentences,
                 "model": model,
                 "parameters": parameters,
             },
@@ -382,18 +329,14 @@
     async def across_embedding(
         self,
         sentences: List[List[str]],
         model: str = "",
         parameters: CrossEncoderParams = {},
     ) -> CrossEncoderOutput:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "reranker" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
         res = await self._apost(
             self.host + "/cross_embedding",
             json={
                 "sentences": sentences,
                 "model": model,
                 "parameters": parameters,
             },
@@ -404,19 +347,14 @@
         self,
         file: Union[str, TextIOWrapper],
         model: str = "",
         language: str = "",
         temperature: float = 0.0,
     ) -> Transcription:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "audio" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         if isinstance(file, str):
             file = open(file, "rb")
 
         r = self._post(
             url=self.host + "/audio/transcriptions",
             files={"file": file},
             data={
@@ -432,19 +370,14 @@
         self,
         file: Union[str, TextIOWrapper],
         model: str = "",
         language: str = "",
         temperature: float = 0.0,
     ) -> Transcription:
         model = model or self.model
-        if (model not in self.supported_models) or (
-            "audio" not in self.supported_models[model].types
-        ):
-            raise ValueError(f"Model {model} not supported")
-
         if isinstance(file, str):
             file = open(file, "rb")
 
         r = await self._apost(
             url=self.host + "/audio/transcriptions",
             files={"file": file},
             data={
```

### Comparing `puyuan_modelhub-1.1.7/modelhub/client/errors.py` & `puyuan_modelhub-1.1.8/modelhub/errors.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.7/modelhub/common/types/__init__.py` & `puyuan_modelhub-1.1.8/modelhub/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,8 +54,11 @@
     "ChatParameters",
     "BaichuanParameters",
     "OpenAIParameters",
     "StreamErrorOutput",
     "Transcription",
     "CrossEncoderParams",
     "CrossEncoderOutput",
+    "ChatGLM2Parameters",
+    "ChatGLM3Parameters",
+    "GeminiParameters",
 ]
```

### Comparing `puyuan_modelhub-1.1.7/modelhub/common/types/chat.py` & `puyuan_modelhub-1.1.8/modelhub/types/chat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional, Union, Literal
+from typing import Dict, List, Optional, Union, Literal
 
 from openai.types.chat import (
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionToolParam,
     completion_create_params,
 )
 from typing_extensions import NotRequired, TypedDict
@@ -66,16 +66,8 @@
     temperature: NotRequired[float]
 
 
 class ChatGLM3Parameters(ChatGLM2Parameters):
     role: NotRequired[str]
 
 
-ChatParameters = Union[
-    OpenAIParameters,
-    BaichuanParameters,
-    ChatGLMParameters,
-    GeminiParameters,
-    ChatGLM2Parameters,
-    ChatGLM3Parameters,
-    Dict[str, Any],
-]
+ChatParameters = dict
```

### Comparing `puyuan_modelhub-1.1.7/modelhub/common/types/encoder.py` & `puyuan_modelhub-1.1.8/modelhub/types/encoder.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.7/modelhub/common/types/generation.py` & `puyuan_modelhub-1.1.8/modelhub/types/generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,17 @@
     success: bool = False
     msg: str = "failed"
 
 
 class ModelInfo(BaseModel):
     types: List[Literal["chat", "embedding", "audio", "reranker"]]
 
+    class Config:
+        extra = "allow"
+
 
 class ModelInfoOutput(BaseOutput):
     models: Dict[str, ModelInfo]
 
 
 class ModelParamsOutput(BaseOutput):
     param_schema: Dict[str, Any]
```

### Comparing `puyuan_modelhub-1.1.7/modelhub/common/types/message.py` & `puyuan_modelhub-1.1.8/modelhub/types/message.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.7/LICENSE.txt` & `puyuan_modelhub-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.7/pyproject.toml` & `puyuan_modelhub-1.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "modelhub/_version.py"
 
 [tool.hatch.build]
 include = ["/modelhub"]
-exclude = ["/modelhub/server"]
 
 
 [tool.hatch.build.targets.wheel]
 packages = ["modelhub"]
 # only-include = ['nuitka_output/*']
 
 # [tool.hatch.build.hooks.nuitka]
```

