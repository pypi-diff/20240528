# Comparing `tmp/databouncer-0.1.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/databouncer-0.2.0rc1-cp39-cp39-macosx_10_12_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7404697 bytes, number of entries: 7
--rw-r--r--  4.6 unx     1840 b- defN 24-May-16 08:23 databouncer-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx      134 b- defN 24-May-16 08:23 databouncer-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx      127 b- defN 24-May-16 08:23 databouncer/__init__.py
--rw-r--r--  4.6 unx     9331 b- defN 24-May-16 08:23 databouncer/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-16 08:23 databouncer/py.typed
--rwxr-xr-x  4.6 unx 23548312 b- defN 24-May-16 08:23 databouncer/databouncer.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      569 b- defN 24-May-16 08:23 databouncer-0.1.1.dist-info/RECORD
-7 files, 23560313 bytes uncompressed, 7403693 bytes compressed:  68.6%
+Zip file size: 6713063 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     1926 b- defN 24-May-28 10:25 databouncer-0.2.0rc1.dist-info/METADATA
+-rw-r--r--  4.6 unx      104 b- defN 24-May-28 10:25 databouncer-0.2.0rc1.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 24-May-28 10:25 databouncer/__init__.py
+-rw-r--r--  4.6 unx    10593 b- defN 24-May-28 10:25 databouncer/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-28 10:25 databouncer/py.typed
+-rwxr-xr-x  4.6 unx 21372056 b- defN 24-May-28 10:25 databouncer/databouncer.cpython-39-darwin.so
+-rw-r--r--  4.6 unx      568 b- defN 24-May-28 10:25 databouncer-0.2.0rc1.dist-info/RECORD
+7 files, 21385374 bytes uncompressed, 6712063 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: databouncer-0.1.1.dist-info/METADATA
+Filename: databouncer-0.2.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: databouncer-0.1.1.dist-info/WHEEL
+Filename: databouncer-0.2.0rc1.dist-info/WHEEL
 Comment: 
 
 Filename: databouncer/__init__.py
 Comment: 
 
 Filename: databouncer/__init__.pyi
 Comment: 
 
 Filename: databouncer/py.typed
 Comment: 
 
-Filename: databouncer/databouncer.pypy39-pp73-x86_64-linux-gnu.so
+Filename: databouncer/databouncer.cpython-39-darwin.so
 Comment: 
 
-Filename: databouncer-0.1.1.dist-info/RECORD
+Filename: databouncer-0.2.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databouncer/__init__.pyi

```diff
@@ -1,7 +1,9 @@
+from collections.abc import Collection
+
 import PIL.Image.Image
 
 class DataBouncer(object):
     """Provides access to the main functionalities of the DataBouncer SDK.
 
     Offers methods to embed images and texts and make decisions about which frames to select.
     """
@@ -50,37 +52,69 @@
 
                 embeddings = databouncer.embed_texts(["cat", "dog"])
         """
         ...
 
     def embed_frame(self, frame: PIL.Image.Image) -> list[float]:
         """
-        Embeds an RGB image.
+        Embeds a PIL image.
 
         Args:
-           frame:
+            frame:
                 A PIL image to embed.
 
         Returns:
-           An embedding (list of floats). The dimension of the embedding is determined by the model.
+            An embedding (list of floats). The dimension of the embedding is determined by the model.
 
         Raises:
-           DataBouncerError:
+            DataBouncerError:
                 If an error occurs during the embedding process.
 
         Example:
             .. code-block:: python
 
                 from PIL.Image import Image
 
                 with Image.open("cat.jpg") as frame:
                     embedding = databouncer.embed_frame(frame=frame)
         """
         ...
 
+    # Note: We don't want to have numpy as a dependency in the SDK, but want to support
+    # numpy arrays. We use the Collection type hint to support both lists and numpy
+    # arrays. Note that this solution is not perfect, mypy won't check that the numpy
+    # array is three-dimensional.
+    def embed_rgb_array(self, rgb_array: Collection[Collection[Collection[int]]]) -> list[float]:
+        """
+        Embeds an RGB image.
+
+        Args:
+            rgb_array:
+                A 3D array of shape (height, width, channels). There must be three
+                channels encoding each pixel in the RGB order. Each value must be
+                an 8-bit integer between 0 and 255.
+
+        Returns:
+           An embedding (list of floats). The dimension of the embedding is determined by the model.
+
+        Raises:
+           DataBouncerError:
+                If an error occurs during the embedding process.
+
+        Example:
+            .. code-block:: python
+
+                rgb_array = [
+                    [[255, 0, 0], [0, 255, 0]],
+                    [[0, 0, 255], [255, 255, 255]],
+                ]
+                embedding = databouncer.embed_rgb_array(rgb_array=rgb_array)
+        """
+        ...
+
     def insert_into_embedding_database(self, embedding: list[float]) -> None:
         """
         Inserts an embedding into the embedding database.
 
         Embedding database is used by the diversity strategy.
         If an embedding is inserted into the database the strategy will not anymore select
         frames with embeddings similar to it. You should call ``insert_into_embedding_database``
@@ -149,15 +183,15 @@
                 # Add to the embedding database if the image is selected.
                 if select_info.diversity[0].should_select:
                     databouncer.insert_into_embedding_database(embedding)
         """
         ...
 
     def register_similarity_strategy(
-        self, embedding_query: list[float], max_distance: float
+        self, query_embedding: list[float], max_distance: float
     ) -> None:
         """
         Registers a similarity strategy.
 
         A similarity strategy selects frames that are similar to a query embedding.
         The ``max_distance`` parameter must be between 0 and 1 and controls how similar
         the embeddings must be for a frame to be selected: Only frames with a distance
```

## Comparing `databouncer-0.1.1.dist-info/METADATA` & `databouncer-0.2.0rc1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.3
 Name: databouncer
-Version: 0.1.1
+Version: 0.2.0rc1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: pillow
-Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
+Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: requests ; extra == 'dev'
+Requires-Dist: ruff ; extra == 'dev'
+Requires-Dist: types-pillow ; extra == 'dev'
 Requires-Dist: types-requests ; extra == 'dev'
 Requires-Dist: ruff-lsp ; extra == 'lsp'
 Requires-Dist: pylsp-mypy ; extra == 'lsp'
 Provides-Extra: dev
 Provides-Extra: lsp
 Summary: DataBouncer Python bindings
 Keywords: computer vision,data curation,data filtering,data selection,dataset analysis,image processing,similarity search
```

