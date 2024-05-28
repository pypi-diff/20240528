# Comparing `tmp/hscitorchutil-0.1.64.tar.gz` & `tmp/hscitorchutil-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscitorchutil-0.1.64.tar", max compression
+gzip compressed data, was "hscitorchutil-0.1.65.tar", max compression
```

## Comparing `hscitorchutil-0.1.64.tar` & `hscitorchutil-0.1.65.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.64/README.md
--rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.64/hscitorchutil/callbacks.py
--rw-r--r--   0        0        0     8694 2024-04-17 14:29:04.250160 hscitorchutil-0.1.64/hscitorchutil/dataset.py
--rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.64/hscitorchutil/fsspec.py
--rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.64/hscitorchutil/processlocal.py
--rw-r--r--   0        0        0     8676 2024-04-18 13:19:14.770983 hscitorchutil-0.1.64/hscitorchutil/sqlite.py
--rw-r--r--   0        0        0      908 2024-04-18 13:19:22.804466 hscitorchutil-0.1.64/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.64/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.65/README.md
+-rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.65/hscitorchutil/callbacks.py
+-rw-r--r--   0        0        0     9043 2024-05-27 04:59:35.199538 hscitorchutil-0.1.65/hscitorchutil/dataset.py
+-rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.65/hscitorchutil/fsspec.py
+-rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.65/hscitorchutil/processlocal.py
+-rw-r--r--   0        0        0     8676 2024-04-18 13:19:14.770983 hscitorchutil-0.1.65/hscitorchutil/sqlite.py
+-rw-r--r--   0        0        0      908 2024-05-27 05:05:57.824030 hscitorchutil-0.1.65/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.65/PKG-INFO
```

### Comparing `hscitorchutil-0.1.64/hscitorchutil/callbacks.py` & `hscitorchutil-0.1.65/hscitorchutil/callbacks.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.64/hscitorchutil/dataset.py` & `hscitorchutil-0.1.65/hscitorchutil/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,39 +40,46 @@
         else:
             return [self.dataset[self.start + idx] for idx in indices]
 
     def __len__(self):
         return self.end - self.start
 
 
+K_co = TypeVar('K_co', covariant=True)
+K2_co = TypeVar('K2_co', covariant=True)
 T2_co = TypeVar('T2_co', covariant=True)
 
 
-class TransformedMapDataset(Dataset[T2_co], Generic[T2_co, T_co]):
+def identity(i: T_co) -> T_co:
+    return i
+
+
+class TransformedMapDataset(Dataset[T2_co], Generic[K_co, K2_co, T_co, T2_co]):
     r"""Create a transformed map dataset by applying a transform function to all samples.
 
     Args:
         dataset (Dataset[T_co]): The underlying map dataset
         transform (Callable[T:co,T2_co]): The transformation function to be applied to each sample
     """
 
-    def __init__(self, dataset: Dataset[T_co], transform: Callable[[Sequence[T_co]], Sequence[T2_co]]) -> None:
+    def __init__(self, dataset: Dataset[T_co], item_transform: Callable[[Sequence[T_co]], Sequence[T2_co]], key_transform: Callable[[Sequence[K_co]], Sequence[K2_co]] = identity) -> None:
         self.dataset = dataset
-        self.transform = transform
+        self.key_transform = key_transform
+        self.item_transform = item_transform
 
     def __getitem__(self, idx):
-        return self.transform([self.dataset[idx]])[0]
+        return self.item_transform([self.dataset[self.key_transform([idx])[0]]])[0]
 
-    def __getitems__(self, indices: Sequence[int]) -> Sequence[T2_co]:
+    def __getitems__(self, indices: Sequence[K_co]) -> Sequence[T2_co]:
         # add batched sampling support when parent dataset supports it.
         # see torch.utils.data._utils.fetch._MapDatasetFetcher
         if callable(getattr(self.dataset, "__getitems__", None)):
-            return self.transform(self.dataset.__getitems__(indices))  # type: ignore[attr-defined] # noqa
+            return self.item_transform(self.dataset.__getitems__(self.key_transform(indices)))  # type: ignore[attr-defined] # noqa
         else:
-            return self.transform([self.dataset[idx] for idx in indices])
+            return self.item_transform([self.dataset[idx] for idx in self.key_transform(indices)])
 
     def __len__(self):
         return len(self.dataset)  # type: ignore
 
 
 class ShuffledMapDataset(Dataset[T_co], Generic[T_co]):
     r"""
```

### Comparing `hscitorchutil-0.1.64/hscitorchutil/fsspec.py` & `hscitorchutil-0.1.65/hscitorchutil/fsspec.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.64/hscitorchutil/processlocal.py` & `hscitorchutil-0.1.65/hscitorchutil/processlocal.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.64/hscitorchutil/sqlite.py` & `hscitorchutil-0.1.65/hscitorchutil/sqlite.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.64/pyproject.toml` & `hscitorchutil-0.1.65/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hscitorchutil"
-version = "0.1.64"
+version = "0.1.65"
 description = "HSCI research group utilities for pytorch (lightning)"
 authors = ["Eetu Mäkelä <eetu.makela@helsinki.fi>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hsci-r/hscitorchutil"
 keywords = [
     "pytorch",
```

### Comparing `hscitorchutil-0.1.64/PKG-INFO` & `hscitorchutil-0.1.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscitorchutil
-Version: 0.1.64
+Version: 0.1.65
 Summary: HSCI research group utilities for pytorch (lightning)
 Home-page: https://github.com/hsci-r/hscitorchutil
 License: MIT
 Keywords: pytorch,dataset
 Author: Eetu Mäkelä
 Author-email: eetu.makela@helsinki.fi
 Requires-Python: >=3.10,<3.12
```

