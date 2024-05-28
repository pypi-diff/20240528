# Comparing `tmp/pdm_readiness-0.1.6.tar.gz` & `tmp/pdm_readiness-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_readiness-0.1.6.tar", last modified: Tue Dec  5 21:35:23 2023, max compression
+gzip compressed data, was "pdm_readiness-0.1.7.tar", last modified: Tue May 28 15:41:57 2024, max compression
```

## Comparing `pdm_readiness-0.1.6.tar` & `pdm_readiness-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/LICENSE
--rw-r--r--   0        0        0     1514 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/README.md
--rw-r--r--   0        0        0     1106 2023-12-05 21:35:23.264506 pdm_readiness-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6682 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/src/pdm_readiness/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/src/pdm_readiness/py.typed
--rw-r--r--   0        0        0        0 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     1697 2023-12-05 21:35:09.192446 pdm_readiness-0.1.6/tests/test_readiness.py
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pdm_readiness-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1512 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/README.md
+-rw-r--r--   0        0        0     1106 2024-05-28 15:41:57.844546 pdm_readiness-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6682 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/src/pdm_readiness/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/src/pdm_readiness/py.typed
+-rw-r--r--   0        0        0        0 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     1697 2024-05-28 15:41:41.704556 pdm_readiness-0.1.7/tests/test_readiness.py
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 pdm_readiness-0.1.7/PKG-INFO
```

### Comparing `pdm_readiness-0.1.6/LICENSE` & `pdm_readiness-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_readiness-0.1.6/README.md` & `pdm_readiness-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 ## Synopsis
 
 The readiness report is divided into 4 sections:
 
 - **Supported dependencies** - currently locked dependencies that support the target Python version.
 - **Update required** - currently locked dependencies that do not support the target Python version, but have newer versions that do.
-- **Unsupported** - dependencies: the most recent version of the dependency does not support the target Python version.
+- **Unsupported dependencies** - the most recent version of the dependency does not support the target Python version.
 - **Missing metadata** - the package does not provide metadata about the supported Python versions.
 
-Plugins uses [PyPI JSON API](https://warehouse.pypa.io/api-reference/json.html) to get the metadata.
+Plugin uses [PyPI JSON API](https://warehouse.pypa.io/api-reference/json.html) to get the metadata.
 It looks at classifiers like `Programming Language :: Python :: 3.12` to determine which versions are supported.
 
 ## Installation
 
 ```sh
 pdm self add pdm-readiness
 ```
```

### Comparing `pdm_readiness-0.1.6/pyproject.toml` & `pdm_readiness-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-readiness"
-version = "0.1.6"
+version = "0.1.7"
 description = "A pdm plugin to check if your project dependencies support specific Python version."
 authors = [
     { name = "Andrii Kohut", email = "kogut.andriy@gmail.com" },
 ]
 dependencies = [
     "pdm>=2.9.0",
     "requests",
```

### Comparing `pdm_readiness-0.1.6/src/pdm_readiness/__init__.py` & `pdm_readiness-0.1.7/src/pdm_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_readiness-0.1.6/tests/test_readiness.py` & `pdm_readiness-0.1.7/tests/test_readiness.py`

 * *Files identical despite different names*

### Comparing `pdm_readiness-0.1.6/PKG-INFO` & `pdm_readiness-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-readiness
-Version: 0.1.6
+Version: 0.1.7
 Summary: A pdm plugin to check if your project dependencies support specific Python version.
 Author-Email: Andrii Kohut <kogut.andriy@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,18 +28,18 @@
 
 ## Synopsis
 
 The readiness report is divided into 4 sections:
 
 - **Supported dependencies** - currently locked dependencies that support the target Python version.
 - **Update required** - currently locked dependencies that do not support the target Python version, but have newer versions that do.
-- **Unsupported** - dependencies: the most recent version of the dependency does not support the target Python version.
+- **Unsupported dependencies** - the most recent version of the dependency does not support the target Python version.
 - **Missing metadata** - the package does not provide metadata about the supported Python versions.
 
-Plugins uses [PyPI JSON API](https://warehouse.pypa.io/api-reference/json.html) to get the metadata.
+Plugin uses [PyPI JSON API](https://warehouse.pypa.io/api-reference/json.html) to get the metadata.
 It looks at classifiers like `Programming Language :: Python :: 3.12` to determine which versions are supported.
 
 ## Installation
 
 ```sh
 pdm self add pdm-readiness
 ```
```

