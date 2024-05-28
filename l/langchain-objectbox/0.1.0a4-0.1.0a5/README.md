# Comparing `tmp/langchain_objectbox-0.1.0a4.tar.gz` & `tmp/langchain_objectbox-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_objectbox-0.1.0a4.tar", max compression
+gzip compressed data, was "langchain_objectbox-0.1.0a5.tar", max compression
```

## Comparing `langchain_objectbox-0.1.0a4.tar` & `langchain_objectbox-0.1.0a5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-14 14:12:32.626479 langchain_objectbox-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     3874 2024-05-14 14:12:32.638479 langchain_objectbox-0.1.0a4/README.md
--rw-r--r--   0        0        0       86 2024-05-14 14:12:32.606479 langchain_objectbox-0.1.0a4/langchain_objectbox/__init__.py
--rw-r--r--   0        0        0     9651 2024-05-14 14:12:32.674479 langchain_objectbox-0.1.0a4/langchain_objectbox/vectorstores.py
--rw-r--r--   0        0        0      662 2024-05-17 07:07:36.083644 langchain_objectbox-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 14:12:32.626479 langchain_objectbox-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     3874 2024-05-14 14:12:32.638479 langchain_objectbox-0.1.0a5/README.md
+-rw-r--r--   0        0        0       86 2024-05-14 14:12:32.606479 langchain_objectbox-0.1.0a5/langchain_objectbox/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-27 14:06:13.388740 langchain_objectbox-0.1.0a5/langchain_objectbox/objectbox-model.json
+-rw-r--r--   0        0        0     9074 2024-05-27 14:12:41.190039 langchain_objectbox-0.1.0a5/langchain_objectbox/vectorstores.py
+-rw-r--r--   0        0        0      722 2024-05-28 11:15:18.893999 langchain_objectbox-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a5/PKG-INFO
```

### Comparing `langchain_objectbox-0.1.0a4/LICENSE` & `langchain_objectbox-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a4/README.md` & `langchain_objectbox-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a4/langchain_objectbox/vectorstores.py` & `langchain_objectbox-0.1.0a5/langchain_objectbox/vectorstores.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from objectbox.model.model import IdUid
 from objectbox.model.properties import (
     VectorDistanceType,
     HnswIndex,
     Id,
     Property,
     PropertyType,
+    String,
+    Float32Vector
 )
 
 DIRECTORY = "objectbox"
 
 
 class ObjectBox(VectorStore):
     """
@@ -150,17 +152,15 @@
 
         Returns:
             List of Documents with score most similar to the query vector.
         """
         embedded_query = self._embedding.embed_query(query)
 
         start = time.perf_counter()
-        embeddings_prop = self._entity_model.get_property("embeddings")
-        qb = self._vector_box.query()
-        qb.nearest_neighbors_f32(embeddings_prop, embedded_query, k)
+        qb = self._vector_box.query( self._entity_model.embeddings.nearest_neighbor(embedded_query, k) )
         query = qb.build()
         results = query.find_with_scores()
 
         if self._do_log:
             end = time.perf_counter()
             print(f"ObjectBox retrieved {len(results)} vectors in { end - start} seconds")
 
@@ -179,17 +179,15 @@
             k (int): Number of Documents to return. Defaults to 4.
 
         Returns:
             List of Documents most similar to the query vector.
         """
         start = time.perf_counter()
 
-        embeddings_prop = self._entity_model.get_property("embeddings")
-        qb = self._vector_box.query()
-        qb.nearest_neighbors_f32(embeddings_prop, embedding, k)
+        qb = self._vector_box.query( self._entity_model.embeddings.nearest_neighbor(embedding, k) )
         query = qb.build()
         results = query.find_with_scores()
 
         if self._do_log:
             end = time.perf_counter()
             print(f"ObjectBox retrieved {len(results)} vectors in { end - start} seconds")
 
@@ -242,34 +240,21 @@
 
     def _create_objectbox_db(self) -> objectbox:
         """registering the VectorEntity model and setting up objectbox database"""
         db_path = DIRECTORY if self.db_directory is None else self.db_directory
         if self._clear_db and os.path.exists(db_path):
             shutil.rmtree(db_path)
         model = objectbox.Model()
-        model.entity(self._entity_model, last_property_id=IdUid(4, 1004))
-        model.last_entity_id = IdUid(1, 1)
-        model.last_index_id = IdUid(3, 10001)
+        model.entity(self._entity_model)
         return objectbox.Store(model=model,directory=db_path)
 
     def _create_entity_class(self) -> Entity:
         """Dynamically define an Entity class according to the parameters."""
 
-        @Entity(id=1, uid=1)
+        @Entity()
         class VectorEntity:
-            id = Id(id=1, uid=1001)
-            text = Property(str, type=PropertyType.string, id=2, uid=1002)
+            id = Id()
+            text = String()
             metadata = Property(dict, type=PropertyType.flex, id=3, uid=1003)
-            embeddings = Property(
-                np.ndarray,
-                type=PropertyType.floatVector,
-                id=4,
-                uid=1004,
-                index=HnswIndex(
-                    id=1,
-                    uid=10001,
-                    dimensions=self._embedding_dimensions,
-                    distance_type=self._distance_type,
-                ),
-            )
+            embeddings = Float32Vector(index=HnswIndex(dimensions=self._embedding_dimensions, distance_type=self._distance_type))
 
         return VectorEntity
```

### Comparing `langchain_objectbox-0.1.0a4/pyproject.toml` & `langchain_objectbox-0.1.0a5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "langchain-objectbox"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = "Integration package connecting ObjectBox and LangChain"
 authors = ["ObjectBox" ]
 license = "MIT" 
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License"
 ]
+include = [
+    "langchain_objectbox/objectbox-model.json" 
+]
 [tool.poetry.dependencies]
 python = "^3.8.1" 
 langchain-core = "^0.1.45"
-objectbox = "^4.0.0a0"
+objectbox = "^4.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 langchain = "^0.1.16"
 numpy = [ 
     { version = "^1.26", python = "^3.12" },
```

### Comparing `langchain_objectbox-0.1.0a4/PKG-INFO` & `langchain_objectbox-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-objectbox
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Integration package connecting ObjectBox and LangChain
 License: MIT
 Author: ObjectBox
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
-Requires-Dist: objectbox (>=4.0.0a0,<5.0.0)
+Requires-Dist: objectbox (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # langchain-objectbox
 
 ## About
 
 This package contains the [ObjectBox](https://objectbox.io) integrations for [LangChain](https://www.langchain.com).
```

