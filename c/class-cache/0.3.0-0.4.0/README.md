# Comparing `tmp/class_cache-0.3.0.tar.gz` & `tmp/class_cache-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.3.0.tar` & `class_cache-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       77 2024-05-27 18:03:27.717955 class_cache-0.3.0/.markdownlint.json
--rw-r--r--   0        0        0      569 2024-05-27 18:03:27.717955 class_cache-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       61 2024-05-27 18:03:27.717955 class_cache-0.3.0/.taplo.toml
--rw-r--r--   0        0        0     2496 2024-05-27 18:03:27.717955 class_cache-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-27 18:03:27.717955 class_cache-0.3.0/LICENSE
--rw-r--r--   0        0        0     3331 2024-05-27 18:03:27.717955 class_cache-0.3.0/README.md
--rw-r--r--   0        0        0      141 2024-05-27 18:03:27.717955 class_cache-0.3.0/class_cache/__init__.py
--rw-r--r--   0        0        0     6519 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/backends.py
--rw-r--r--   0        0        0     3586 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/core.py
--rw-r--r--   0        0        0      229 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/types.py
--rw-r--r--   0        0        0      310 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/utils.py
--rw-r--r--   0        0        0     2141 2024-05-27 18:03:27.721955 class_cache-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 class_cache-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-27 21:59:36.127565 class_cache-0.4.0/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-05-27 21:59:36.127565 class_cache-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-05-27 21:59:36.127565 class_cache-0.4.0/.taplo.toml
+-rw-r--r--   0        0        0     2829 2024-05-27 21:59:36.127565 class_cache-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-27 21:59:36.127565 class_cache-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3331 2024-05-27 21:59:36.127565 class_cache-0.4.0/README.md
+-rw-r--r--   0        0        0      141 2024-05-27 21:59:36.127565 class_cache-0.4.0/class_cache/__init__.py
+-rw-r--r--   0        0        0     9438 2024-05-27 21:59:36.127565 class_cache-0.4.0/class_cache/backends.py
+-rw-r--r--   0        0        0     3596 2024-05-27 21:59:36.127565 class_cache-0.4.0/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-05-27 21:59:36.127565 class_cache-0.4.0/class_cache/types.py
+-rw-r--r--   0        0        0      310 2024-05-27 21:59:36.127565 class_cache-0.4.0/class_cache/utils.py
+-rw-r--r--   0        0        0     2141 2024-05-27 21:59:36.127565 class_cache-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 class_cache-0.4.0/PKG-INFO
```

### Comparing `class_cache-0.3.0/.pre-commit-config.yaml` & `class_cache-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `class_cache-0.3.0/CHANGELOG.md` & `class_cache-0.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.4.0 (2024-05-27)
+
+### Feature
+
+* feat(backend): add SQLiteBackend ([`f5640ce`](https://github.com/Rizhiy/class-cache/commit/f5640cec799a81e15eb65ef53950f59f6d5decc0))
+
+### Test
+
+* test(backend): add test for block splitting ([`7b6aa1d`](https://github.com/Rizhiy/class-cache/commit/7b6aa1dd127f5ab9f6ef9623f240e054aa83f366))
+
+
 ## v0.3.0 (2024-05-27)
 
 ### Chore
 
 * chore(pyproject): add benchmark to exclude ([`26d4219`](https://github.com/Rizhiy/class-cache/commit/26d421977a14d7e0519b86284a1d334064c24b27))
 
 ### Feature
```

### Comparing `class_cache-0.3.0/LICENSE` & `class_cache-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.3.0/README.md` & `class_cache-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `class_cache-0.3.0/class_cache/backends.py` & `class_cache-0.4.0/class_cache/backends.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+# ruff: noqa: S608
+import codecs
 import json
 import pickle  # noqa: S403
+import sqlite3
 from abc import ABC
 from collections import defaultdict
 from pathlib import Path
-from typing import Any, Iterable, Iterator, MutableMapping
+from typing import Any, Iterable, Iterator, MutableMapping, TypeAlias, cast
 
 from fasteners import InterProcessReaderWriterLock
 from marisa_trie import Trie
 from replete.consistent_hash import consistent_hash
 
 from class_cache.types import KeyType, ValueType
 from class_cache.utils import get_class_cache_dir
 
+ID_TYPE: TypeAlias = str | int | None
+
 
 class BaseBackend(ABC, MutableMapping[KeyType, ValueType]):
-    def __init__(self, id_: str | int | None = None) -> None:
+    def __init__(self, id_: ID_TYPE = None) -> None:
         self._id = id_
 
     @property
-    def id(self) -> str | int | None:
+    def id(self) -> ID_TYPE:
         return self._id
 
     # Override these methods to allow getting results in a more optimal fashion
     def contains_many(self, keys: Iterable[KeyType]) -> Iterator[tuple[KeyType, bool]]:
         for key in keys:
             yield key, key in self
 
@@ -43,19 +48,19 @@
 
 
 class PickleBackend(BaseBackend[KeyType, ValueType]):
     ROOT_DIR = get_class_cache_dir() / "PickleBackend"
     BLOCK_SUFFIX = ".block.pkl"
     META_TYPE = dict[str, Any]
 
-    def __init__(self, id_: str | int, target_block_size=1024 * 1024) -> None:
+    def __init__(self, id_: ID_TYPE = None, max_block_size=1024 * 1024) -> None:
         super().__init__(id_)
-        self._dir = self.ROOT_DIR / str(self._id)
+        self._dir = self.ROOT_DIR / str(self.id)
         self._dir.mkdir(exist_ok=True, parents=True)
-        self._target_block_size = target_block_size
+        self._max_block_size = max_block_size
         self._meta_path = self._dir / "meta.json"
         self._lock = InterProcessReaderWriterLock(self._dir / "lock.file")
         self._check_meta()
 
     @property
     def dir(self) -> Path:
         return self._dir
@@ -142,15 +147,15 @@
             block_id = self._get_block_id_for_key(key, prefix_len=prefix_len)
             block = self._get_block(block_id)
             change = 0 if key in block else 1
             block[key] = value
             self._write_block(block_id, block)
             self._update_length(change)
 
-        if self.get_path_for_block_id(block_id).stat().st_size > self._target_block_size:
+        if self.get_path_for_block_id(block_id).stat().st_size > self._max_block_size:
             self._split_block(block_id)
 
     def _split_block(self, block_id: str) -> None:
         with self._lock.write_lock():
             block = self._get_block(block_id)
             self.get_path_for_block_id(block_id).unlink()
             new_prefix_len = len(block_id) + 1
@@ -170,7 +175,79 @@
 
     def clear(self) -> None:
         with self._lock.write_lock():
             for block_id in self.get_all_block_ids():
                 self.get_path_for_block_id(block_id).unlink()
             self._meta_path.unlink()
             self._write_clean_meta()
+
+
+class SQLiteBackend(BaseBackend[KeyType, ValueType]):
+    ROOT_DIR = get_class_cache_dir() / "SQLiteBackend"
+    ROOT_DIR.mkdir(parents=True, exist_ok=True)
+    DATA_TABLE_NAME = "data"
+
+    def __init__(self, id_: ID_TYPE = None) -> None:
+        super().__init__(id_)
+        self._db_path = self.ROOT_DIR / str(self.id)
+        self._con = sqlite3.connect(self._db_path)
+        self._cursor = self._con.cursor()
+        self._check_table()
+
+    @property
+    def db_path(self) -> Path:
+        return self._db_path
+
+    def _check_table(self):
+        tables = self._cursor.execute("SELECT name FROM sqlite_master LIMIT 1").fetchone()
+        if tables is None:
+            self._cursor.execute(f"CREATE TABLE {self.DATA_TABLE_NAME}(key TEXT, value TEXT)")
+            self._cursor.execute(f"CREATE UNIQUE INDEX key_index ON {self.DATA_TABLE_NAME}(key)")
+
+    # TODO: Can probably cache these
+    def _encode(self, obj: KeyType | ValueType) -> str:
+        return codecs.encode(pickle.dumps(obj), "base64").decode()
+
+    def _decode(self, stored: str) -> KeyType | ValueType:
+        return pickle.loads(codecs.decode(stored.encode(), "base64"))  # noqa: S301
+
+    def __contains__(self, key: KeyType) -> bool:
+        key_str = self._encode(key)
+        sql = f"SELECT EXISTS(SELECT 1 FROM {self.DATA_TABLE_NAME} WHERE key=? LIMIT 1)"
+        value = self._cursor.execute(sql, (key_str,)).fetchone()[0]
+        return value != 0
+
+    def __len__(self) -> int:
+        return self._cursor.execute(f"SELECT COUNT(key) FROM {self.DATA_TABLE_NAME}").fetchone()[0]
+
+    def __iter__(self) -> Iterator[KeyType]:
+        for key_str in self._cursor.execute(f"SELECT key FROM {self.DATA_TABLE_NAME}").fetchall():
+            yield cast(KeyType, self._decode(key_str[0]))
+
+    def __getitem__(self, key: KeyType) -> ValueType:
+        key_str = self._encode(key)
+        sql = f"SELECT value FROM {self.DATA_TABLE_NAME} WHERE key=? LIMIT 1"
+        res = self._cursor.execute(sql, (key_str,)).fetchone()
+        if res is None:
+            raise KeyError(key)
+        return cast(ValueType, self._decode(res[0]))
+
+    def __setitem__(self, key: KeyType, value: ValueType) -> None:
+        key_str = self._encode(key)
+        value_str = self._encode(value)
+        self._cursor.execute(f"INSERT INTO {self.DATA_TABLE_NAME} VALUES (?, ?)", (key_str, value_str))
+        self._con.commit()
+
+    def __delitem__(self, key: KeyType) -> None:
+        key_str = self._encode(key)
+        self._cursor.execute(f"DELETE FROM {self.DATA_TABLE_NAME} WHERE key=?", (key_str,))
+        self._con.commit()
+
+    def clear(self) -> None:
+        self._cursor.execute(f"DROP TABLE IF EXISTS {self.DATA_TABLE_NAME}")
+        self._check_table()
+
+    def __del__(self):
+        self._con.commit()
+        self._con.close()
+
+    # TODO: implement *_many methods
```

### Comparing `class_cache-0.3.0/class_cache/core.py` & `class_cache-0.4.0/class_cache/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from class_cache.backends import BaseBackend, PickleBackend
 from class_cache.types import KeyType, ValueType
 
 DEFAULT_BACKEND_TYPE = PickleBackend
 
 
 class Cache(ABC, MutableMapping[KeyType, ValueType]):
-    def __init__(self, id_: str | int | None = None, backend: type[BaseBackend] = DEFAULT_BACKEND_TYPE) -> None:
-        self._backend = backend(id_)
+    def __init__(self, id_: str | int | None = None, backend_type: type[BaseBackend] = DEFAULT_BACKEND_TYPE) -> None:
+        self._backend = backend_type(id_)
         self._data: dict[KeyType, ValueType] = {}
         self._to_write = set()
         self._to_delete = set()
 
     @property
     def backend(self) -> BaseBackend:
         return self._backend
```

### Comparing `class_cache-0.3.0/pyproject.toml` & `class_cache-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `class_cache-0.3.0/PKG-INFO` & `class_cache-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class-cache
-Version: 0.3.0
+Version: 0.4.0
 Summary: Caching for class based generators
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: Pympler
 Requires-Dist: fasteners
 Requires-Dist: marisa-trie
```

