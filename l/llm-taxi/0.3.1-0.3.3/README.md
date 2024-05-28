# Comparing `tmp/llm_taxi-0.3.1.tar.gz` & `tmp/llm_taxi-0.3.3.tar.gz`

## Comparing `llm_taxi-0.3.1.tar` & `llm_taxi-0.3.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/.python-version
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/pyrightconfig.json
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/requirements-dev.lock
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/requirements.lock
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/cli.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/conversation.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/factory.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/anthropic.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/base.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/dashscope.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/deepinfra.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/deepseek.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/google.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/groq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/mistral.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/openai.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/openrouter.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/perplexity.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/together.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/__init__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/base.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/google.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/mistral.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/openai.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/anthropic.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/base.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/dashscope.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/deepinfra.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/deepseek.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/google.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/groq.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/mistral.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/openai.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/openrouter.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/perplexity.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/together.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/tests/test_llm.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/.gitignore
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/.python-version
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/pyrightconfig.json
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/requirements-dev.lock
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/requirements.lock
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/cli.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/conversation.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/factory.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/utils.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/anthropic.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/base.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/dashscope.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/deepinfra.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/deepseek.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/google.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/groq.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/mistral.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/openai.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/openrouter.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/perplexity.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/clients/together.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/__init__.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/base.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/google.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/mistral.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/openai.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/embeddings/utils.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/anthropic.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/base.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/dashscope.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/deepinfra.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/deepseek.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/google.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/groq.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/mistral.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/openai.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/openrouter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/perplexity.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/src/llm_taxi/llms/together.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/tests/test_llm.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 llm_taxi-0.3.3/PKG-INFO
```

### Comparing `llm_taxi-0.3.1/requirements-dev.lock` & `llm_taxi-0.3.3/requirements-dev.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
+#   generate-hashes: false
 
 -e file:.
 aiohttp==3.9.5
     # via together
 aiosignal==1.3.1
     # via aiohttp
 annotated-types==0.6.0
@@ -69,15 +70,15 @@
 google-auth-httplib2==0.2.0
     # via google-api-python-client
 google-generativeai==0.5.2
     # via llm-taxi
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
-groq==0.5.0
+groq==0.8.0
     # via llm-taxi
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
```

### Comparing `llm_taxi-0.3.1/requirements.lock` & `llm_taxi-0.3.3/requirements.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
+#   generate-hashes: false
 
 -e file:.
 aiohttp==3.9.5
     # via together
 aiosignal==1.3.1
     # via aiohttp
 annotated-types==0.6.0
@@ -69,15 +70,15 @@
 google-auth-httplib2==0.2.0
     # via google-api-python-client
 google-generativeai==0.5.2
     # via llm-taxi
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
-groq==0.5.0
+groq==0.8.0
     # via llm-taxi
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
```

### Comparing `llm_taxi-0.3.1/src/llm_taxi/cli.py` & `llm_taxi-0.3.3/src/llm_taxi/cli.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/factory.py` & `llm_taxi-0.3.3/src/llm_taxi/factory.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/clients/__init__.py` & `llm_taxi-0.3.3/src/llm_taxi/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/clients/google.py` & `llm_taxi-0.3.3/src/llm_taxi/clients/google.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from typing import Any, ClassVar
+from typing import ClassVar
+
+from google import generativeai as genai
+from google.generativeai import GenerativeModel
 
 from llm_taxi.clients.base import Client
 
 
-class Google(Client):
+class Google(Client[GenerativeModel]):
     env_vars: ClassVar[dict[str, str]] = {
         "api_key": "GOOGLE_API_KEY",
     }
 
     def __init__(
         self,
         *,
@@ -20,19 +23,15 @@
         super().__init__(
             model=model,
             api_key=api_key,
             base_url=base_url,
             call_kwargs=call_kwargs,
             **client_kwargs,
         )
-
-        from google import generativeai as genai
-
         genai.configure(api_key=api_key, **client_kwargs)
 
         self._call_kwargs.pop("model", None)
 
-    def _init_client(self, **kwargs) -> Any:
+    def _init_client(self, **kwargs) -> GenerativeModel:
         kwargs = {k: v for k, v in kwargs.items() if k not in {"api_key", "base_url"}}
-        from google import generativeai as genai
 
-        return genai.GenerativeModel(self.model, **kwargs)
+        return GenerativeModel(self.model, **kwargs)
```

### Comparing `llm_taxi-0.3.1/src/llm_taxi/embeddings/mistral.py` & `llm_taxi-0.3.3/src/llm_taxi/embeddings/mistral.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/embeddings/openai.py` & `llm_taxi-0.3.3/src/llm_taxi/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/llms/__init__.py` & `llm_taxi-0.3.3/src/llm_taxi/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/llms/anthropic.py` & `llm_taxi-0.3.3/src/llm_taxi/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/llms/google.py` & `llm_taxi-0.3.3/src/llm_taxi/llms/google.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/llms/mistral.py` & `llm_taxi-0.3.3/src/llm_taxi/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/src/llm_taxi/llms/openai.py` & `llm_taxi-0.3.3/src/llm_taxi/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.3.1/tests/test_llm.py` & `llm_taxi-0.3.3/tests/test_llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from llm_taxi.conversation import Message, Role
 from llm_taxi.factory import embedding, llm
 
 
 async def main():
     clients = [
-        llm(model="openai:gpt-3.5-turbo"),
-        llm(model="google:gemini-pro"),
-        llm(model="together:meta-llama/Llama-3-70b-chat-hf"),
         llm(model="groq:llama3-70b-8192"),
-        llm(model="anthropic:claude-2.1"),
-        llm(model="mistral:mistral-small"),
-        llm(model="perplexity:llama-3-8b-instruct"),
-        llm(model="deepinfra:meta-llama/Meta-Llama-3-8B-Instruct"),
-        llm(model="deepseek:deepseek-chat"),
-        llm(model="openrouter:rwkv/rwkv-5-world-3b"),
-        llm(model="dashscope:qwen-turbo"),
+        # llm(model="openai:gpt-3.5-turbo"),
+        # llm(model="google:gemini-pro"),
+        # llm(model="together:meta-llama/Llama-3-70b-chat-hf"),
+        # llm(model="anthropic:claude-2.1"),
+        # llm(model="mistral:mistral-small"),
+        # llm(model="perplexity:llama-3-8b-instruct"),
+        # llm(model="deepinfra:meta-llama/Meta-Llama-3-8B-Instruct"),
+        # llm(model="deepseek:deepseek-chat"),
+        # llm(model="openrouter:rwkv/rwkv-5-world-3b"),
+        # llm(model="dashscope:qwen-turbo"),
     ]
 
     for client in clients:
         print("========================================")
         print(client.model)
         messages = [
             Message(role=Role.User, content="What is the capital of France?"),
```

### Comparing `llm_taxi-0.3.1/pyproject.toml` & `llm_taxi-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "llm-taxi"
-version = "0.3.1"
+version = "0.3.3"
 description = "Call LLM as easily as calling a taxi."
 authors = [{ name = "Yevgnen Koh", email = "wherejoystarts@gmail.com" }]
 dependencies = [
     "openai>=1.28.1",
     "pydantic>=2.7.1",
     "google-generativeai>=0.5.2",
     "together>=1.1.5",
-    "groq>=0.5.0",
+    "groq>=0.8.0",
     "anthropic>=0.25.8",
     "mistralai>=0.1.8",
     "httpx[socks]<0.26.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

