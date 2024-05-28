# Comparing `tmp/semantic_chunkers-0.0.5.tar.gz` & `tmp/semantic_chunkers-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_chunkers-0.0.5.tar", max compression
+gzip compressed data, was "semantic_chunkers-0.0.6.tar", max compression
```

## Comparing `semantic_chunkers-0.0.5.tar` & `semantic_chunkers-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-22 07:54:59.900323 semantic_chunkers-0.0.5/LICENSE
--rw-r--r--   0        0        0     1397 2024-05-22 07:54:59.900323 semantic_chunkers-0.0.5/README.md
--rw-r--r--   0        0        0     1066 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/__init__.py
--rw-r--r--   0        0        0      375 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/__init__.py
--rw-r--r--   0        0        0     1521 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/base.py
--rw-r--r--   0        0        0     2734 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/consecutive.py
--rw-r--r--   0        0        0     3582 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/cumulative.py
--rw-r--r--   0        0        0    18475 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/statistical.py
--rw-r--r--   0        0        0      353 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/schema.py
--rw-r--r--   0        0        0        0 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/splitters/__init__.py
--rw-r--r--   0        0        0     2003 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/splitters/sentence.py
--rw-r--r--   0        0        0        0 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/logger.py
--rw-r--r--   0        0        0      192 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/text.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-28 05:55:12.784777 semantic_chunkers-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1397 2024-05-28 05:55:12.784777 semantic_chunkers-0.0.6/README.md
+-rw-r--r--   0        0        0     1066 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      374 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/chunkers/__init__.py
+-rw-r--r--   0        0        0     1541 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/chunkers/base.py
+-rw-r--r--   0        0        0     2924 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/chunkers/consecutive.py
+-rw-r--r--   0        0        0     3772 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/chunkers/cumulative.py
+-rw-r--r--   0        0        0    20812 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/chunkers/statistical.py
+-rw-r--r--   0        0        0      353 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/schema.py
+-rw-r--r--   0        0        0      178 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/splitters/__init__.py
+-rw-r--r--   0        0        0      268 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/splitters/base.py
+-rw-r--r--   0        0        0     2004 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/splitters/sentence.py
+-rw-r--r--   0        0        0        0 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/utils/logger.py
+-rw-r--r--   0        0        0      192 2024-05-28 05:55:12.840776 semantic_chunkers-0.0.6/semantic_chunkers/utils/text.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.6/PKG-INFO
```

### Comparing `semantic_chunkers-0.0.5/LICENSE` & `semantic_chunkers-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.5/README.md` & `semantic_chunkers-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.5/pyproject.toml` & `semantic_chunkers-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-chunkers"
-version = "0.0.5"
+version = "0.0.6"
 description = "Super advanced chunking methods for AI"
 authors = ["Aurelio AI <hello@aurelio.ai>"]
 readme = "README.md"
 packages = [{include = "semantic_chunkers"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/base.py` & `semantic_chunkers-0.0.6/semantic_chunkers/chunkers/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Any, List
 
 from colorama import Fore, Style
 from pydantic.v1 import BaseModel, Extra
 
 from semantic_router.encoders.base import BaseEncoder
 from semantic_chunkers.schema import Chunk
-from semantic_chunkers.splitters.sentence import regex_splitter
+from semantic_chunkers.splitters.base import BaseSplitter
 
 
 class BaseChunker(BaseModel):
     name: str
     encoder: BaseEncoder
+    splitter: BaseSplitter
 
     class Config:
         extra = Extra.allow
 
     def __call__(self, docs: List[str]) -> List[List[Chunk]]:
         raise NotImplementedError("Subclasses must implement this method")
 
     def _split(self, doc: str) -> List[str]:
-        return regex_splitter(doc)
+        return self.splitter(doc)
 
     def _chunk(self, splits: List[Any]) -> List[Chunk]:
         raise NotImplementedError("Subclasses must implement this method")
 
     def print(self, document_splits: List[Chunk]) -> None:
         colors = [Fore.RED, Fore.GREEN, Fore.BLUE, Fore.MAGENTA]
         for i, split in enumerate(document_splits):
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/consecutive.py` & `semantic_chunkers-0.0.6/semantic_chunkers/chunkers/consecutive.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from tqdm.auto import tqdm
 
 import numpy as np
 
 from semantic_router.encoders.base import BaseEncoder
 from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
+from semantic_chunkers.splitters.base import BaseSplitter
+from semantic_chunkers.splitters.sentence import RegexSplitter
 
 
 class ConsecutiveChunker(BaseChunker):
     """
     Called "consecutive sim chunker" because we check the similarities of consecutive document embeddings (compare ith to i+1th document embedding).
     """
 
     def __init__(
         self,
         encoder: BaseEncoder,
+        splitter: BaseSplitter = RegexSplitter(),
         name: str = "consecutive_chunker",
         score_threshold: float = 0.45,
     ):
-        super().__init__(name=name, encoder=encoder)
+        super().__init__(name=name, encoder=encoder, splitter=splitter)
         encoder.score_threshold = score_threshold
         self.score_threshold = score_threshold
 
     def _chunk(self, splits: List[Any], batch_size: int = 64) -> List[Chunk]:
         """Merge splits into chunks using semantic similarity.
 
         :param splits: splits to be merged into chunks.
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/cumulative.py` & `semantic_chunkers-0.0.6/semantic_chunkers/chunkers/cumulative.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 from tqdm.auto import tqdm
 
 import numpy as np
 
 from semantic_router.encoders import BaseEncoder
 from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
+from semantic_chunkers.splitters.base import BaseSplitter
+from semantic_chunkers.splitters.sentence import RegexSplitter
 
 
 class CumulativeChunker(BaseChunker):
     """
     Called "cumulative sim" because we check the similarities of the
     embeddings of cumulative concatenated documents with the next document.
     """
 
     def __init__(
         self,
         encoder: BaseEncoder,
+        splitter: BaseSplitter = RegexSplitter(),
         name: str = "cumulative_chunker",
         score_threshold: float = 0.45,
     ):
-        super().__init__(name=name, encoder=encoder)
+        super().__init__(name=name, encoder=encoder, splitter=splitter)
         encoder.score_threshold = score_threshold
         self.score_threshold = score_threshold
 
     def _chunk(self, splits: List[Any], batch_size: int = 64) -> List[Chunk]:
         """Merge splits into chunks using semantic similarity.
 
         :param splits: splits to be merged into chunks.
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/statistical.py` & `semantic_chunkers-0.0.6/semantic_chunkers/chunkers/statistical.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from dataclasses import dataclass
-from typing import List
+from typing import Any, List
 
 import numpy as np
 
 from semantic_router.encoders.base import BaseEncoder
 from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
+from semantic_chunkers.splitters.base import BaseSplitter
+from semantic_chunkers.splitters.sentence import RegexSplitter
 from semantic_chunkers.utils.text import tiktoken_length
 from semantic_chunkers.utils.logger import logger
 
+from tqdm.auto import tqdm
+
 
 @dataclass
 class ChunkStatistics:
     total_documents: int
     total_chunks: int
     chunks_by_threshold: int
     chunks_by_max_chunk_size: int
@@ -35,75 +39,128 @@
         )
 
 
 class StatisticalChunker(BaseChunker):
     def __init__(
         self,
         encoder: BaseEncoder,
+        splitter: BaseSplitter = RegexSplitter(),
         name="statistical_chunker",
         threshold_adjustment=0.01,
         dynamic_threshold: bool = True,
         window_size=5,
         min_split_tokens=100,
         max_split_tokens=300,
         split_tokens_tolerance=10,
         plot_chunks=False,
         enable_statistics=False,
     ):
-        super().__init__(name=name, encoder=encoder)
+        super().__init__(name=name, encoder=encoder, splitter=splitter)
         self.calculated_threshold: float
         self.encoder = encoder
         self.threshold_adjustment = threshold_adjustment
         self.dynamic_threshold = dynamic_threshold
         self.window_size = window_size
         self.plot_chunks = plot_chunks
         self.min_split_tokens = min_split_tokens
         self.max_split_tokens = max_split_tokens
         self.split_tokens_tolerance = split_tokens_tolerance
         self.enable_statistics = enable_statistics
         self.statistics: ChunkStatistics
 
-    def __call__(self, docs: List[str]) -> List[List[Chunk]]:
-        """Chunk documents into smaller chunks based on semantic similarity.
+    def _chunk(
+        self, splits: List[Any], batch_size: int = 64, enforce_max_tokens: bool = False
+    ) -> List[Chunk]:
+        """Merge splits into chunks using semantic similarity, with optional enforcement of maximum token limits per chunk.
+
+        :param splits: Splits to be merged into chunks.
+        :param batch_size: Number of splits to process in one batch.
+        :param enforce_max_tokens: If True, further split chunks that exceed the maximum token limit.
+
+        :return: List of chunks.
+        """
+        # Split the docs that already exceed max_split_tokens to smaller chunks
+        if enforce_max_tokens:
+            new_splits = []
+            for split in splits:
+                token_count = tiktoken_length(split)
+                if token_count > self.max_split_tokens:
+                    logger.info(
+                        f"Single document exceeds the maximum token limit "
+                        f"of {self.max_split_tokens}. "
+                        "Splitting to sentences before semantically merging."
+                    )
+                    _splits = self._split(split)
+                    new_splits.extend(_splits)
+                else:
+                    new_splits.append(split)
+
+            splits = [split for split in new_splits if split and split.strip()]
+
+        chunks = []
+        last_split = None
+        for i in tqdm(range(0, len(splits), batch_size)):
+            batch_splits = splits[i : i + batch_size]
+            if last_split is not None:
+                batch_splits = last_split.splits + batch_splits
+
+            encoded_splits = self._encode_documents(batch_splits)
+            similarities = self._calculate_similarity_scores(encoded_splits)
+            if self.dynamic_threshold:
+                self._find_optimal_threshold(batch_splits, similarities)
+            else:
+                self.calculated_threshold = self.encoder.score_threshold
+            split_indices = self._find_split_indices(similarities=similarities)
+            doc_chunks = self._split_documents(
+                batch_splits, split_indices, similarities
+            )
+
+            if len(doc_chunks) > 1:
+                chunks.extend(doc_chunks[:-1])
+                last_split = doc_chunks[-1]
+            else:
+                last_split = doc_chunks[0]
+
+            if self.plot_chunks:
+                self.plot_similarity_scores(similarities, split_indices, doc_chunks)
+
+            if self.enable_statistics:
+                print(self.statistics)
+
+        if last_split:
+            chunks.append(last_split)
+
+        return chunks
+
+    def __call__(self, docs: List[str], batch_size: int = 64) -> List[List[Chunk]]:
+        """Split documents into smaller chunks based on semantic similarity.
 
         :param docs: list of text documents to be split, if only wanted to
             split a single document, pass it as a list with a single element.
 
-        :return: list of DocumentChunk objects containing the split documents.
+        :return: list of Chunk objects containing the split documents.
         """
         if not docs:
             raise ValueError("At least one document is required for splitting.")
 
         all_chunks = []
-
         for doc in docs:
             token_count = tiktoken_length(doc)
             if token_count > self.max_split_tokens:
                 logger.info(
                     f"Single document exceeds the maximum token limit "
                     f"of {self.max_split_tokens}. "
                     "Splitting to sentences before semantically merging."
                 )
-            splits = self._split(doc)
-            encoded_splits = self._encode_documents(splits)
-            similarities = self._calculate_similarity_scores(encoded_splits)
-            if self.dynamic_threshold:
-                self._find_optimal_threshold(splits, similarities)
+            if isinstance(doc, str):
+                splits = self._split(doc)
+                doc_chunks = self._chunk(splits, batch_size=batch_size)
+                all_chunks.append(doc_chunks)
             else:
-                self.calculated_threshold = self.encoder.score_threshold
-            split_indices = self._find_split_indices(similarities=similarities)
-            doc_chunks = self._split_documents(splits, split_indices, similarities)
-
-            if self.plot_chunks:
-                self.plot_similarity_scores(similarities, split_indices, doc_chunks)
-
-            if self.enable_statistics:
-                print(self.statistics)
-            all_chunks.append(doc_chunks)
-
+                raise ValueError("The document must be a string.")
         return all_chunks
 
     def _encode_documents(self, docs: List[str]) -> np.ndarray:
         """
         Encodes a list of documents into embeddings. If the number of documents exceeds 2000,
         the documents are split into batches to avoid overloading the encoder. OpenAI has a
         limit of len(array) < 2048.
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/splitters/sentence.py` & `semantic_chunkers-0.0.6/semantic_chunkers/splitters/sentence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import regex
+from typing import List
 
+from semantic_chunkers.splitters.base import BaseSplitter
 
-def regex_splitter(text: str) -> list[str]:
+
+class RegexSplitter(BaseSplitter):
     """
     Enhanced regex pattern to split a given text into sentences more accurately.
 
     The enhanced regex pattern includes handling for:
     - Direct speech and quotations.
     - Abbreviations, initials, and acronyms.
     - Decimal numbers and dates.
     - Ellipses and other punctuation marks used in informal text.
     - Removing control characters and format characters.
-
-    Args:
-        text (str): The text to split into sentences.
-
-    Returns:
-        list: A list of sentences extracted from the text.
     """
+
     regex_pattern = r"""
         # Negative lookbehind for word boundary, word char, dot, word char
         (?<!\b\w\.\w.)
         # Negative lookbehind for single uppercase initials like "A."
         (?<!\b[A-Z][a-z]\.)
         # Negative lookbehind for abbreviations like "U.S."
         (?<!\b[A-Z]\.)
@@ -47,10 +45,12 @@
         # Handles splitting after ellipses
         (?<=\.\.\.)\s+(?=[A-Z])
         # OR
         |
         # Matches and removes control characters and format characters
         [\p{Cc}\p{Cf}]+
     """
-    sentences = regex.split(regex_pattern, text, flags=regex.VERBOSE)
-    sentences = [sentence.strip() for sentence in sentences if sentence.strip()]
-    return sentences
+
+    def __call__(self, doc: str) -> List[str]:
+        sentences = regex.split(self.regex_pattern, doc, flags=regex.VERBOSE)
+        sentences = [sentence.strip() for sentence in sentences if sentence.strip()]
+        return sentences
```

### Comparing `semantic_chunkers-0.0.5/semantic_chunkers/utils/logger.py` & `semantic_chunkers-0.0.6/semantic_chunkers/utils/logger.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.5/PKG-INFO` & `semantic_chunkers-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-chunkers
-Version: 0.0.5
+Version: 0.0.6
 Summary: Super advanced chunking methods for AI
 Author: Aurelio AI
 Author-email: hello@aurelio.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

