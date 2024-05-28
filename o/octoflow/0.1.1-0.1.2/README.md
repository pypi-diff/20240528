# Comparing `tmp/octoflow-0.1.1.tar.gz` & `tmp/octoflow-0.1.2.tar.gz`

## Comparing `octoflow-0.1.1.tar` & `octoflow-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/config.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/constants.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/core.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/exceptions.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/logging.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/plugin.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/typing.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/base.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/dataclass.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/dataset.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/expression.py
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/loaders.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/metadata.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/sampler.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/schema.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/data/types.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/tracking/__init__.py
--rw-r--r--   0        0        0    12459 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/tracking/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/tracking/artifact/__init__.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/tracking/artifact/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/cache.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/collections.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/config.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/func.py
--rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/hashing.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/objects.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/rsync.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.1/octoflow/utils/string.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.1/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.1/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.1/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.1/README.md
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/config.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/constants.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/core.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/exceptions.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/logging.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/plugin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/typing.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/base.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/dataclass.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/dataset.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/expression.py
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/loaders.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/metadata.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/sampler.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/schema.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/data/types.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/tracking/__init__.py
+-rw-r--r--   0        0        0    12459 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/tracking/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/tracking/artifact/__init__.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/tracking/artifact/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/cache.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/collections.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/config.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/func.py
+-rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/hashing.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/objects.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/rsync.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.2/octoflow/utils/string.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.2/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.2/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.2/README.md
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.2/PKG-INFO
```

### Comparing `octoflow-0.1.1/octoflow/__init__.py` & `octoflow-0.1.2/octoflow/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from octoflow import logging
 from octoflow.config import config
 from octoflow.utils.config import Config
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __all__ = [
     "Config",
     "config",
     "logger",
     "logging",
 ]
```

### Comparing `octoflow-0.1.1/octoflow/config.py` & `octoflow-0.1.2/octoflow/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/core.py` & `octoflow-0.1.2/octoflow/core.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/logging.py` & `octoflow-0.1.2/octoflow/logging.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/plugin.py` & `octoflow-0.1.2/octoflow/plugin.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/__init__.py` & `octoflow-0.1.2/octoflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/base.py` & `octoflow-0.1.2/octoflow/data/base.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/dataclass.py` & `octoflow-0.1.2/octoflow/data/dataclass.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/dataset.py` & `octoflow-0.1.2/octoflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/expression.py` & `octoflow-0.1.2/octoflow/data/expression.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/loaders.py` & `octoflow-0.1.2/octoflow/data/loaders.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/metadata.py` & `octoflow-0.1.2/octoflow/data/metadata.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/schema.py` & `octoflow-0.1.2/octoflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/data/types.py` & `octoflow-0.1.2/octoflow/data/types.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/tracking/models.py` & `octoflow-0.1.2/octoflow/tracking/models.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/tracking/artifact/handler.py` & `octoflow-0.1.2/octoflow/tracking/artifact/handler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/cache.py` & `octoflow-0.1.2/octoflow/utils/cache.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/collections.py` & `octoflow-0.1.2/octoflow/utils/collections.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/config.py` & `octoflow-0.1.2/octoflow/utils/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/func.py` & `octoflow-0.1.2/octoflow/utils/func.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/hashing.py` & `octoflow-0.1.2/octoflow/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/objects.py` & `octoflow-0.1.2/octoflow/utils/objects.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/rsync.py` & `octoflow-0.1.2/octoflow/utils/rsync.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/octoflow/utils/string.py` & `octoflow-0.1.2/octoflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/.gitignore` & `octoflow-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/LICENSE` & `octoflow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/README.md` & `octoflow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/pyproject.toml` & `octoflow-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.1/PKG-INFO` & `octoflow-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
```
