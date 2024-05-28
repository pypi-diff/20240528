# Comparing `tmp/nlp_service-2.0.0b1.tar.gz` & `tmp/nlp_service-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-2.0.0b1.tar", max compression
+gzip compressed data, was "nlp_service-2.0.0b2.tar", max compression
```

## Comparing `nlp_service-2.0.0b1.tar` & `nlp_service-2.0.0b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-12-04 11:51:38.615823 nlp_service-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     7887 2023-12-04 11:51:38.615823 nlp_service-2.0.0b1/README.md
--rw-r--r--   0        0        0      526 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/__init__.py
--rw-r--r--   0        0        0       39 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/__main__.py
--rw-r--r--   0        0        0     3236 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/cli.py
--rw-r--r--   0        0        0     2092 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/client.py
--rw-r--r--   0        0        0    16461 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/lib.py
--rw-r--r--   0        0        0    15492 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/nlp_pb.py
--rw-r--r--   0        0        0        0 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/py.typed
--rw-r--r--   0        0        0     3493 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/server.py
--rw-r--r--   0        0        0     8946 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/sim_funcs.py
--rw-r--r--   0        0        0      317 2023-12-04 11:51:38.619823 nlp_service-2.0.0b1/nlp_service/typing.py
--rw-r--r--   0        0        0     1150 2023-12-04 11:52:29.528240 nlp_service-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     9303 1970-01-01 00:00:00.000000 nlp_service-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0     7887 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/README.md
+-rw-r--r--   0        0        0      526 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/__main__.py
+-rw-r--r--   0        0        0     3236 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/cli.py
+-rw-r--r--   0        0        0     2092 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/client.py
+-rw-r--r--   0        0        0    16411 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/lib.py
+-rw-r--r--   0        0        0    15492 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/nlp_pb.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/py.typed
+-rw-r--r--   0        0        0     3493 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/server.py
+-rw-r--r--   0        0        0     8946 2024-05-28 19:59:35.431357 nlp_service-2.0.0b2/nlp_service/sim_funcs.py
+-rw-r--r--   0        0        0      317 2024-05-28 19:59:35.435357 nlp_service-2.0.0b2/nlp_service/typing.py
+-rw-r--r--   0        0        0     1150 2024-05-28 20:00:40.831300 nlp_service-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     9303 1970-01-01 00:00:00.000000 nlp_service-2.0.0b2/PKG-INFO
```

### Comparing `nlp_service-2.0.0b1/LICENSE` & `nlp_service-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/README.md` & `nlp_service-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/__init__.py` & `nlp_service-2.0.0b2/nlp_service/__init__.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/cli.py` & `nlp_service-2.0.0b2/nlp_service/cli.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/client.py` & `nlp_service-2.0.0b2/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/lib.py` & `nlp_service-2.0.0b2/nlp_service/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     # tok2vec, transformer
 )
 custom_components: tuple[str, ...] = ("embeddings_factory", "similarity_factory")
 
 
 @dataclass(frozen=True, eq=True)
 class SerializableEmbeddingModel(DataClassDictMixin):
-    model_type: nlp_pb.EmbeddingType
+    model_type: int
     model_name: str
-    pooling_type: nlp_pb.Pooling
+    pooling_type: int
     pmean: float
 
     @classmethod
     def from_protobuf(cls, pb: nlp_pb.EmbeddingModel) -> "SerializableEmbeddingModel":
         return cls(pb.model_type, pb.model_name, pb.pooling_type, pb.pmean)
 
 
@@ -185,17 +185,17 @@
         def vector(self, text: str) -> SpacyVector:
             embeddings = t.cast(
                 NumpyVector, self.model.encode([text], convert_to_numpy=True)
             )
 
             return embeddings[0]
 
-    embedding_map[
-        nlp_pb.EmbeddingType.SENTENCE_TRANSFORMERS
-    ] = SentenceTransformersModel
+    embedding_map[nlp_pb.EmbeddingType.SENTENCE_TRANSFORMERS] = (
+        SentenceTransformersModel
+    )
 
 except ModuleNotFoundError:
     log.info("'sentence-transformers' not installed.")
 
 
 try:
     import openai
@@ -415,34 +415,31 @@
 
 
 @t.overload
 def vectors(
     texts: abc.Iterable[str],
     config: nlp_pb.NlpConfig,
     embedding_level: EmbeddingLevelSingle,
-) -> list[SpacyVector]:
-    ...
+) -> list[SpacyVector]: ...
 
 
 @t.overload
 def vectors(
     texts: abc.Iterable[str],
     config: nlp_pb.NlpConfig,
     embedding_level: EmbeddingLevelMulti,
-) -> list[list[SpacyVector]]:
-    ...
+) -> list[list[SpacyVector]]: ...
 
 
 @t.overload
 def vectors(
     texts: abc.Iterable[str],
     config: nlp_pb.NlpConfig,
     embedding_level: nlp_pb.EmbeddingLevel,
-) -> list[SpacyVector] | list[list[SpacyVector]]:
-    ...
+) -> list[SpacyVector] | list[list[SpacyVector]]: ...
 
 
 def vectors(
     texts: abc.Iterable[str],
     config: nlp_pb.NlpConfig,
     embedding_level: nlp_pb.EmbeddingLevel = nlp_pb.EmbeddingLevel.UNSPECIFIED,
 ) -> list[SpacyVector] | list[list[SpacyVector]]:
@@ -481,30 +478,27 @@
 
         return span_vecs
 
 
 @t.overload
 def vector(
     text: str, config: nlp_pb.NlpConfig, embedding_level: EmbeddingLevelSingle
-) -> SpacyVector:
-    ...
+) -> SpacyVector: ...
 
 
 @t.overload
 def vector(
     text: str, config: nlp_pb.NlpConfig, embedding_level: EmbeddingLevelMulti
-) -> list[SpacyVector]:
-    ...
+) -> list[SpacyVector]: ...
 
 
 @t.overload
 def vector(
     text: str, config: nlp_pb.NlpConfig, embedding_level: nlp_pb.EmbeddingLevel
-) -> SpacyVector | list[SpacyVector]:
-    ...
+) -> SpacyVector | list[SpacyVector]: ...
 
 
 def vector(
     text: str,
     config: nlp_pb.NlpConfig,
     embedding_level: nlp_pb.EmbeddingLevel = nlp_pb.EmbeddingLevel.UNSPECIFIED,
 ) -> SpacyVector | list[SpacyVector]:
```

### Comparing `nlp_service-2.0.0b1/nlp_service/nlp_pb.py` & `nlp_service-2.0.0b2/nlp_service/nlp_pb.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/server.py` & `nlp_service-2.0.0b2/nlp_service/server.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/nlp_service/sim_funcs.py` & `nlp_service-2.0.0b2/nlp_service/sim_funcs.py`

 * *Files identical despite different names*

### Comparing `nlp_service-2.0.0b1/pyproject.toml` & `nlp_service-2.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "2.0.0b1"
+version = "2.0.0b2"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
```

### Comparing `nlp_service-2.0.0b1/PKG-INFO` & `nlp_service-2.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

