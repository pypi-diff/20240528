# Comparing `tmp/chatgpt-klient-0.5.2.tar.gz` & `tmp/chatgpt_klient-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.5.2.tar", last modified: Tue Jan 30 13:56:52 2024, max compression
+gzip compressed data, was "chatgpt_klient-0.6.1.tar", last modified: Tue May 28 08:25:19 2024, max compression
```

## Comparing `chatgpt-klient-0.5.2.tar` & `chatgpt_klient-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-01-30 13:56:52.526853 chatgpt-klient-0.5.2/
--rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-01-30 13:56:52.522853 chatgpt-klient-0.5.2/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      508 2023-11-07 16:15:45.000000 chatgpt-klient-0.5.2/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      274 2024-01-30 13:55:50.000000 chatgpt-klient-0.5.2/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2024-01-30 13:56:52.526853 chatgpt-klient-0.5.2/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-01-30 13:56:52.518854 chatgpt-klient-0.5.2/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-01-30 13:56:52.518854 chatgpt-klient-0.5.2/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2024-01-30 13:09:15.000000 chatgpt-klient-0.5.2/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)    16897 2024-01-30 12:58:29.000000 chatgpt-klient-0.5.2/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1773 2024-01-30 11:37:07.000000 chatgpt-klient-0.5.2/src/chatgpt_klient/consts.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt-klient-0.5.2/src/chatgpt_klient/exceptions.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-01-30 13:56:52.522853 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/
--rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-01-30 13:56:52.000000 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      376 2024-01-30 13:56:52.000000 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2024-01-30 13:56:52.000000 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       86 2024-01-30 13:56:52.000000 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2024-01-30 13:56:52.000000 chatgpt-klient-0.5.2/src/chatgpt_klient.egg-info/top_level.txt
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-01-30 13:56:52.522853 chatgpt-klient-0.5.2/tests/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1736 2023-12-12 09:23:40.000000 chatgpt-klient-0.5.2/tests/test_client.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/
+-rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      508 2023-11-07 16:15:45.000000 chatgpt_klient-0.6.1/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      274 2024-05-28 08:24:20.000000 chatgpt_klient-0.6.1/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.561268 chatgpt_klient-0.6.1/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.569268 chatgpt_klient-0.6.1/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2024-05-28 08:24:26.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)    17830 2024-05-28 07:45:57.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     2306 2024-05-28 07:45:31.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/consts.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/exceptions.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/
+-rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      376 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       86 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.569268 chatgpt_klient-0.6.1/tests/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     2015 2024-05-28 08:10:24.000000 chatgpt_klient-0.6.1/tests/test_client.py
```

### Comparing `chatgpt-klient-0.5.2/src/chatgpt_klient/client.py` & `chatgpt_klient-0.6.1/src/chatgpt_klient/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,34 @@
 
 class ChatGPTPrompt:
     def __init__(
         self,
         api_key,
         engine="gpt3.5-default",
         cap_tokens=math.inf,
-        service: Literal["openai", "azure"] = "openai",
+        service: Literal["openai", "azure", "openai-compatible"] = "openai",
         azure_api_version: str = DEFAULT_AZURE_API_VERSION,
         azure_endpoint: str = DEFAULT_AZURE_ENDPOINT,
         azure_instance: str | None = None,
+        openai_endpoint: str | None = None,
     ):
         self.api_key = api_key
         self.service = service
         if self.service == "openai":
             logger.info(f"Initializing an OpenAI {engine} engine")
             self.openai = OpenAI(api_key=self.api_key, timeout=CLIENT_TIMEOUT)
+        elif self.service == "openai-compatible":
+            logger.info(
+                f"Initializing an OpenAI-compatible {engine} engine with endpoint {openai_endpoint}"
+            )
+            self.openai = OpenAI(
+                api_key=self.api_key,
+                base_url=openai_endpoint,
+                timeout=CLIENT_TIMEOUT,
+            )
         elif self.service == "azure":
             if azure_instance is None:
                 raise NoAzureInstanceError
             logger.info(
                 f"Initializing an Azure connection to the {azure_instance} instance (model {engine})"
             )
             self.openai = AzureOpenAI(
@@ -74,14 +84,21 @@
             elif self.service == "azure":
                 r = self.openai.chat.completions.create(
                     model=self.engine,
                     messages=[{"role": "user", "content": "Hola!"}],
                     max_tokens=5,
                     stream=False,
                 ).model_dump()
+            elif self.service == "openai-compatible":
+                r = self.openai.chat.completions.create(
+                    model="poligpt-light",
+                    messages=[{"role": "user", "content": "Hola!"}],
+                    max_tokens=5,
+                    stream=False,
+                ).model_dump()
             r = self.check_response_validity(r)
         except Exception:
             logger.exception("Invalid API key.")
             raise InvalidAPIKeyError(
                 "Your API key does not seem to be valid. Please check it."
             )
         else:
@@ -112,17 +129,17 @@
                     max_tokens=5,
                 ).model_dump()
                 r = self.check_response_validity(r)
                 logger.debug(
                     f'Model validity test: {r["choices"][0]["message"]["content"]}'
                 )
             else:
-                raise InvalidModelError(f"Engine {self.engine} not supported")
+                raise InvalidModelError(f"Engine {self.real_engine} not supported")
         except Exception:
-            logger.info(f"Invalid model ({self.engine}) for your API key")
+            logger.exception(f"Invalid model ({self.engine}) for your API key")
             raise InvalidModelError(f"Engine {self.engine} not supported")
         else:
             logger.info(f"Model ({self.engine}) seems to be valid.")
 
     def check_response_validity(self, r) -> dict:
         try:
             match r:
@@ -139,24 +156,27 @@
             return r
 
     def set_engine(self, engine: str, azure_instance: str | None = None):
         if engine in DEFAULT_ENGINES.keys():
             self.real_engine = DEFAULT_ENGINES[engine]
         else:
             self.real_engine = engine
-        if self.service == "openai":
+        if self.service in ("openai", "openai-compatible"):
             self.engine = self.real_engine
             self.azure_instance = None
         elif self.service == "azure":
             if azure_instance is None:
                 raise NoAzureInstanceError("Azure API requires passing an instance")
             self.engine = azure_instance
             self.azure_instance = azure_instance
         self.check_model_validity()
-        self.encoding = tiktoken.encoding_for_model(self.real_engine)
+        if self.service in ("openai", "azure"):
+            self.encoding = tiktoken.encoding_for_model(self.real_engine)
+        else:
+            self.encoding = tiktoken.get_encoding(ENGINES[self.real_engine]["encoding"])
         eng_attrs = ENGINES[self.real_engine]
         if "max_output_tokens" in eng_attrs:
             self.max_tokens = eng_attrs["max_tokens"] - eng_attrs["max_output_tokens"]
         else:
             self.max_tokens = int(eng_attrs["max_tokens"] / 2)
 
     def set_system_directive(self, directive: str):
```

### Comparing `chatgpt-klient-0.5.2/src/chatgpt_klient/consts.py` & `chatgpt_klient-0.6.1/src/chatgpt_klient/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,35 @@
 INVALID_JSON_MSG = """
 The config file should be in a valid JSON format like the following:
 {
     "api_key": "dk39??!meerLq"
 }
 """
 
+OLLAMA_ENGINES = {
+    # Ollama
+    "poligpt:latest": {
+        "type": "chat",
+        "max_tokens": 8192,
+        "base_model": "llama3-70b",
+        "encoding": "cl100k_base",
+    },
+    "poligpt-light:latest": {
+        "type": "chat",
+        "max_tokens": 8192,
+        "base_model": "llama3-8b",
+        "encoding": "cl100k_base",
+    },
+    "poligpt-asistente:latest": {
+        "type": "chat",
+        "max_tokens": 8192,
+        "base_model": "llama3-70b",
+        "encoding": "cl100k_base",
+    },
+}
 
 ENGINES = {
     "babbage-002": {
         "type": "legacy",
         "max_tokens": 16384,
     },
     "davinci-002": {
@@ -50,14 +71,15 @@
         "max_output_tokens": 4096,
     },
     "gpt-3.5-turbo-1106": {
         "type": "chat",
         "max_tokens": 16384,
         "max_output_tokens": 4096,
     },
+    **OLLAMA_ENGINES,
 }
 
 DEFAULT_ENGINES = {
     "gpt3.5-default": "gpt-3.5-turbo-1106",
     "gpt4-default": "gpt-4-1106-preview",
 }
```

### Comparing `chatgpt-klient-0.5.2/tests/test_client.py` & `chatgpt_klient-0.6.1/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import pytest
 import json
 from pathlib import Path
-from chatgpt_klient.consts import ROOT_DIR, ENGINES, DEFAULT_ENGINES
+from chatgpt_klient.consts import ROOT_DIR, ENGINES, DEFAULT_ENGINES, OLLAMA_ENGINES
 from chatgpt_klient.client import ChatGPTPrompt
 
 
 @pytest.fixture
 def config():
     config_f = ROOT_DIR.joinpath("config.json")
     return json.loads(config_f.read_text())
 
 
 @pytest.mark.parametrize("model", ENGINES.keys())
 def test_ChatGPTPrompt_init_all_models_OK(model, config):
-    ChatGPTPrompt(api_key=config["openai_key"], engine=model)
+    if model in OLLAMA_ENGINES:
+        ChatGPTPrompt(
+            service="openai-compatible",
+            api_key=config["poligpt_key"],
+            openai_endpoint=config["poligpt_endpoint"],
+            engine=model,
+        )
+    else:
+        ChatGPTPrompt(service="openai", api_key=config["openai_key"], engine=model)
 
 
 @pytest.mark.parametrize("model", DEFAULT_ENGINES.keys())
 def test_ChatGPTPrompt_init_default_models_OK(model, config):
     ChatGPTPrompt(api_key=config["openai_key"], engine=model)
```

