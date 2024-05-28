# Comparing `tmp/llama_index_embeddings_bedrock-0.1.5.tar.gz` & `tmp/llama_index_embeddings_bedrock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_bedrock-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_embeddings_bedrock-0.2.0.tar", max compression
```

## Comparing `llama_index_embeddings_bedrock-0.1.5.tar` & `llama_index_embeddings_bedrock-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/README.md
--rw-r--r--   0        0        0      115 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/__init__.py
--rw-r--r--   0        0        0    15391 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/base.py
--rw-r--r--   0        0        0     1471 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_embeddings_bedrock-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-28 18:50:16.353497 llama_index_embeddings_bedrock-0.2.0/README.md
+-rw-r--r--   0        0        0      115 2024-05-28 18:50:16.353497 llama_index_embeddings_bedrock-0.2.0/llama_index/embeddings/bedrock/__init__.py
+-rw-r--r--   0        0        0    16460 2024-05-28 18:50:16.353497 llama_index_embeddings_bedrock-0.2.0/llama_index/embeddings/bedrock/base.py
+-rw-r--r--   0        0        0     1471 2024-05-28 18:50:16.353497 llama_index_embeddings_bedrock-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_embeddings_bedrock-0.2.0/PKG-INFO
```

### Comparing `llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/base.py` & `llama_index_embeddings_bedrock-0.2.0/llama_index/embeddings/bedrock/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class PROVIDERS(str, Enum):
     AMAZON = "amazon"
     COHERE = "cohere"
 
 
 class Models(str, Enum):
     TITAN_EMBEDDING = "amazon.titan-embed-text-v1"
+    TITAN_EMBEDDING_V2_0 = "amazon.titan-embed-text-v2:0"
     TITAN_EMBEDDING_G1_TEXT_02 = "amazon.titan-embed-g1-text-02"
     COHERE_EMBED_ENGLISH_V3 = "cohere.embed-english-v3"
     COHERE_EMBED_MULTILINGUAL_V3 = "cohere.embed-multilingual-v3"
 
 
 PROVIDER_SPECIFIC_IDENTIFIERS = {
     PROVIDERS.AMAZON.value: {
@@ -34,15 +35,15 @@
             r.get("embeddings") if isbatch else r.get("embeddings")[0]
         ),
     },
 }
 
 
 class BedrockEmbedding(BaseEmbedding):
-    model: str = Field(description="The modelId of the Bedrock model to use.")
+    model_name: str = Field(description="The modelId of the Bedrock model to use.")
     profile_name: Optional[str] = Field(
         description="The name of aws profile to use. If not given, then the default profile is used.",
         exclude=True,
     )
     aws_access_key_id: Optional[str] = Field(
         description="AWS Access Key ID to use", exclude=True
     )
@@ -74,15 +75,15 @@
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the bedrock client."
     )
     _client: Any = PrivateAttr()
 
     def __init__(
         self,
-        model: str = Models.TITAN_EMBEDDING,
+        model_name: str = Models.TITAN_EMBEDDING,
         profile_name: Optional[str] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         region_name: Optional[str] = None,
         client: Optional[Any] = None,
         botocore_session: Optional[Any] = None,
@@ -105,15 +106,15 @@
             "profile_name": profile_name,
             "region_name": region_name,
             "aws_access_key_id": aws_access_key_id,
             "aws_secret_access_key": aws_secret_access_key,
             "aws_session_token": aws_session_token,
             "botocore_session": botocore_session,
         }
-        config = None
+
         try:
             import boto3
             from botocore.config import Config
 
             config = (
                 Config(
                     retries={"max_attempts": max_retries, "mode": "standard"},
@@ -137,15 +138,15 @@
             self._client = client
         elif "bedrock-runtime" in session.get_available_services():
             self._client = session.client("bedrock-runtime", config=config)
         else:
             self._client = session.client("bedrock", config=config)
 
         super().__init__(
-            model=model,
+            model_name=model_name,
             max_retries=max_retries,
             timeout=timeout,
             botocore_config=config,
             profile_name=profile_name,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
@@ -161,15 +162,17 @@
             **kwargs,
         )
 
     @staticmethod
     def list_supported_models() -> Dict[str, List[str]]:
         list_models = {}
         for provider in PROVIDERS:
-            list_models[provider.value] = [m.value for m in Models]
+            list_models[provider.value] = [
+                m.value for m in Models if provider.value in m.value
+            ]
         return list_models
 
     @classmethod
     def class_name(self) -> str:
         return "BedrockEmbedding"
 
     @deprecated(
@@ -333,20 +336,20 @@
         """
         if self._client is None:
             self.set_credentials()
 
         if self._client is None:
             raise ValueError("Client not set")
 
-        provider = self.model.split(".")[0]
+        provider = self.model_name.split(".")[0]
         request_body = self._get_request_body(provider, payload, type)
 
         response = self._client.invoke_model(
             body=request_body,
-            modelId=self.model,
+            modelId=self.model_name,
             accept="application/json",
             contentType="application/json",
         )
 
         resp = json.loads(response.get("body").read().decode("utf-8"))
         identifiers = PROVIDER_SPECIFIC_IDENTIFIERS.get(provider, None)
         if identifiers is None:
@@ -356,15 +359,15 @@
     def _get_query_embedding(self, query: str) -> Embedding:
         return self._get_embedding(query, "query")
 
     def _get_text_embedding(self, text: str) -> Embedding:
         return self._get_embedding(text, "text")
 
     def _get_text_embeddings(self, texts: List[str]) -> List[Embedding]:
-        provider = self.model.split(".")[0]
+        provider = self.model_name.split(".")[0]
         if provider == PROVIDERS.COHERE:
             return self._get_embedding(texts, "text")
         return super()._get_text_embeddings(texts)
 
     def _get_request_body(
         self,
         provider: str,
@@ -378,35 +381,57 @@
             Sample Payload of type str
             "Hello World!"
 
         cohere:
             Sample Payload of type dict of following format
             {
                 'texts': ["This is a test document", "This is another document"],
-                'input_type': 'search_document',
-                'truncate': 'NONE'
+                'input_type': 'search_document'
             }
 
         """
         if provider == PROVIDERS.AMAZON:
             if isinstance(payload, list):
                 raise ValueError("Amazon provider does not support list of texts")
-            request_body = json.dumps({"inputText": payload})
+
+            titan_body_request = {"inputText": payload}
+
+            # Titan Embedding V2.0 has additional body parameters to check.
+            if "dimensions" in self.additional_kwargs:
+                if self.model_name == Models.TITAN_EMBEDDING_V2_0:
+                    titan_body_request["dimensions"] = self.additional_kwargs[
+                        "dimensions"
+                    ]
+                else:
+                    raise ValueError(
+                        "'dimensions' param not supported outside of 'titan-embed-text-v2:0' model."
+                    )
+            if "normalize" in self.additional_kwargs:
+                if self.model_name == Models.TITAN_EMBEDDING_V2_0:
+                    titan_body_request["normalize"] = self.additional_kwargs[
+                        "normalize"
+                    ]
+                else:
+                    raise ValueError(
+                        "'normalize' param not supported outside of 'titan-embed-text-v2:0' model."
+                    )
+
+            request_body = json.dumps(titan_body_request)
+
         elif provider == PROVIDERS.COHERE:
             input_types = {
                 "text": "search_document",
                 "query": "search_query",
             }
             payload = [payload] if isinstance(payload, str) else payload
             payload = [p[:2048] if len(p) > 2048 else p for p in payload]
             request_body = json.dumps(
                 {
                     "texts": payload,
                     "input_type": input_types[input_type],
-                    "truncate": "NONE",
                 }
             )
         else:
             raise ValueError("Provider not supported")
         return request_body
 
     async def _aget_query_embedding(self, query: str) -> Embedding:
```

### Comparing `llama_index_embeddings_bedrock-0.1.5/pyproject.toml` & `llama_index_embeddings_bedrock-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings bedrock integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-bedrock"
 readme = "README.md"
-version = "0.1.5"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 boto3 = "^1.34.23"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_embeddings_bedrock-0.1.5/PKG-INFO` & `llama_index_embeddings_bedrock-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-bedrock
-Version: 0.1.5
+Version: 0.2.0
 Summary: llama-index embeddings bedrock integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

