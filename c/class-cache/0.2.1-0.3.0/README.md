# Comparing `tmp/class_cache-0.2.1.tar.gz` & `tmp/class_cache-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.2.1.tar` & `class_cache-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       77 2024-05-27 14:14:06.306109 class_cache-0.2.1/.markdownlint.json
--rw-r--r--   0        0        0      569 2024-05-27 14:14:06.306109 class_cache-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       61 2024-05-27 14:14:06.306109 class_cache-0.2.1/.taplo.toml
--rw-r--r--   0        0        0     2144 2024-05-27 14:14:06.310109 class_cache-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-27 14:14:06.310109 class_cache-0.2.1/LICENSE
--rw-r--r--   0        0        0     3277 2024-05-27 14:14:06.310109 class_cache-0.2.1/README.md
--rw-r--r--   0        0        0      141 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/__init__.py
--rw-r--r--   0        0        0     3941 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/backends.py
--rw-r--r--   0        0        0     3424 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/core.py
--rw-r--r--   0        0        0      229 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/types.py
--rw-r--r--   0        0        0      225 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/utils.py
--rw-r--r--   0        0        0     2087 2024-05-27 14:14:06.310109 class_cache-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 class_cache-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-27 18:03:27.717955 class_cache-0.3.0/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-05-27 18:03:27.717955 class_cache-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-05-27 18:03:27.717955 class_cache-0.3.0/.taplo.toml
+-rw-r--r--   0        0        0     2496 2024-05-27 18:03:27.717955 class_cache-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-27 18:03:27.717955 class_cache-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3331 2024-05-27 18:03:27.717955 class_cache-0.3.0/README.md
+-rw-r--r--   0        0        0      141 2024-05-27 18:03:27.717955 class_cache-0.3.0/class_cache/__init__.py
+-rw-r--r--   0        0        0     6519 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/backends.py
+-rw-r--r--   0        0        0     3586 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/types.py
+-rw-r--r--   0        0        0      310 2024-05-27 18:03:27.721955 class_cache-0.3.0/class_cache/utils.py
+-rw-r--r--   0        0        0     2141 2024-05-27 18:03:27.721955 class_cache-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 class_cache-0.3.0/PKG-INFO
```

### Comparing `class_cache-0.2.1/.pre-commit-config.yaml` & `class_cache-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `class_cache-0.2.1/CHANGELOG.md` & `class_cache-0.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.3.0 (2024-05-27)
+
+### Chore
+
+* chore(pyproject): add benchmark to exclude ([`26d4219`](https://github.com/Rizhiy/class-cache/commit/26d421977a14d7e0519b86284a1d334064c24b27))
+
+### Feature
+
+* feat(backend): add block splitting to PickleBackend ([`a8fcb94`](https://github.com/Rizhiy/class-cache/commit/a8fcb94d28b8eb5c6bf8264e5d263b9b6a756e89))
+
+
 ## v0.2.1 (2024-05-27)
 
 ### Chore
 
 * chore: add pre-commit ([`f7050eb`](https://github.com/Rizhiy/class-cache/commit/f7050eb57345a667a681e6d93233c0c49c389f3b))
 
 ### Documentation
```

### Comparing `class_cache-0.2.1/LICENSE` & `class_cache-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.2.1/README.md` & `class_cache-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
   ```python
   from class_cache import CacheWithDefault
 
   class MyCache(CacheWithDefault[str, str]):
       NON_HASH_ATTRIBUTES = frozenset({*CacheWithDefault.NON_HASH_ATTRIBUTES, "_misc"})
       def __init__(self, name: str):
           # Attributes which affect default value generation should come before super().__init__()
+          # They will be used to generate a unique id
           self._name = name
           super().__init__()
           # Other attributes should not affect how default value is generated, add them to NON_HASH_ATTRIBUTES
           self._misc = "foo"
 
       # Define logic for defaults in _get_data
       def _get_data(self, key: str) -> str:
```

### Comparing `class_cache-0.2.1/class_cache/core.py` & `class_cache-0.3.0/class_cache/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 from class_cache.backends import BaseBackend, PickleBackend
 from class_cache.types import KeyType, ValueType
 
 DEFAULT_BACKEND_TYPE = PickleBackend
 
 
 class Cache(ABC, MutableMapping[KeyType, ValueType]):
-    def __init__(self, id_: str | int = None, backend: type[BaseBackend] = DEFAULT_BACKEND_TYPE) -> None:
+    def __init__(self, id_: str | int | None = None, backend: type[BaseBackend] = DEFAULT_BACKEND_TYPE) -> None:
         self._backend = backend(id_)
         self._data: dict[KeyType, ValueType] = {}
         self._to_write = set()
         self._to_delete = set()
 
+    @property
+    def backend(self) -> BaseBackend:
+        return self._backend
+
     def __contains__(self, key: KeyType) -> bool:
         if key in self._data:
             return True
         return key not in self._to_delete and key in self._backend
 
     def __setitem__(self, key: KeyType, value: ValueType) -> None:
         self._data[key] = value
@@ -27,17 +31,19 @@
 
     def __getitem__(self, key: KeyType) -> ValueType:
         if key not in self._data:
             self._data[key] = self._backend[key]
         return self._data[key]
 
     def __iter__(self) -> Iterable[KeyType]:
+        self.write()
         return iter(self._backend)
 
     def __len__(self) -> int:
+        self.write()
         return len(self._backend)
 
     def __delitem__(self, key: KeyType) -> None:
         # Check that key is present. Can't check self._data, since it can be unloaded
         if key not in self:
             raise KeyError(key)
         self._data.pop(key, None)
@@ -92,9 +98,11 @@
 
     def __setattr__(self, key: str, value: Any) -> None:
         if (
             not isinstance(getattr(self.__class__, key, None), property)
             and getattr(self, "_backend_set", None)
             and key not in self.NON_HASH_ATTRIBUTES
         ):
-            raise TypeError(f"Trying to update hash inclusive attribute after hash has been decided: {key}")
+            raise TypeError(
+                f"Trying to update hash inclusive attribute after hash has been decided: {key}",
+            )
         object.__setattr__(self, key, value)
```

### Comparing `class_cache-0.2.1/pyproject.toml` & `class_cache-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 [project]
 name = "class-cache"
 maintainers = [{ name = "Artem Vasenin", email = "vasart169@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["description", "version"]
-dependencies = ["Pympler", "marisa-trie", "replete"]
+dependencies = ["Pympler", "fasteners", "marisa-trie", "replete"]
 
 [project.urls]
 Home = "https://github.com/Rizhiy/class-cache"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "replete[testing]"]
-dev = ["black", "class-cache[test]", "pre-commit", "ruff"]
+dev = ["black", "class-cache[test]", "numpy", "pre-commit", "ruff"]
 
 [tool.flit.sdist]
 include = ["README.md"]
-exclude = [".github", ".gitignore", "tests/*"]
+exclude = [".github", ".gitignore", "benchmark", "tests/*"]
 
 [tool.semantic_release]
 version_variables = ["class_cache/__init__.py:__version__"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--doctest-modules"
+addopts = "--doctest-modules --ignore=benchmark"
 
 [tool.black]
 line-length = 120
 # skip-magic-trailing-comma = true
 
 [tool.yamlfix]
 line_length = 120
```

### Comparing `class_cache-0.2.1/PKG-INFO` & `class_cache-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: class-cache
-Version: 0.2.1
+Version: 0.3.0
 Summary: Caching for class based generators
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: Pympler
+Requires-Dist: fasteners
 Requires-Dist: marisa-trie
 Requires-Dist: replete
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: class-cache[test] ; extra == "dev"
+Requires-Dist: numpy ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: replete[testing] ; extra == "test"
 Project-URL: Home, https://github.com/Rizhiy/class-cache
 Provides-Extra: dev
@@ -74,14 +76,15 @@
   ```python
   from class_cache import CacheWithDefault
 
   class MyCache(CacheWithDefault[str, str]):
       NON_HASH_ATTRIBUTES = frozenset({*CacheWithDefault.NON_HASH_ATTRIBUTES, "_misc"})
       def __init__(self, name: str):
           # Attributes which affect default value generation should come before super().__init__()
+          # They will be used to generate a unique id
           self._name = name
           super().__init__()
           # Other attributes should not affect how default value is generated, add them to NON_HASH_ATTRIBUTES
           self._misc = "foo"
 
       # Define logic for defaults in _get_data
       def _get_data(self, key: str) -> str:
```

