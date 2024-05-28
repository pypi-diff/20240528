# Comparing `tmp/opthub_runner-1.0.4.tar.gz` & `tmp/opthub_runner-1.0.6.dev20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opthub_runner-1.0.4.tar", max compression
+gzip compressed data, was "opthub_runner-1.0.6.dev20.tar", max compression
```

## Comparing `opthub_runner-1.0.4.tar` & `opthub_runner-1.0.6.dev20.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/converter.py
--rw-r--r--   0        0        0     1899 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/docker_executor.py
--rw-r--r--   0        0        0     2317 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/evaluator.py
--rw-r--r--   0        0        0     2249 2024-05-28 10:15:03.466853 opthub_runner-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 opthub_runner-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/converter.py
+-rw-r--r--   0        0        0     1899 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/docker_executor.py
+-rw-r--r--   0        0        0     2317 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/evaluator.py
+-rw-r--r--   0        0        0     2481 2024-05-28 14:08:27.090590 opthub_runner-1.0.6.dev20/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 opthub_runner-1.0.6.dev20/PKG-INFO
```

### Comparing `opthub_runner-1.0.4/opthub_runner/converter.py` & `opthub_runner-1.0.6.dev20/opthub_runner/converter.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.4/opthub_runner/docker_executor.py` & `opthub_runner-1.0.6.dev20/opthub_runner/docker_executor.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.4/opthub_runner/evaluator.py` & `opthub_runner-1.0.6.dev20/opthub_runner/evaluator.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.4/pyproject.toml` & `opthub_runner-1.0.6.dev20/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "1.0.4"
+version = "1.0.6"
 name = "opthub_runner"
 description = "Library for running OptHub problems locally."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 keywords = ["opthub", "runner", "evaluator"]
 authors = [
@@ -22,46 +22,48 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "python >= 3.8",
     "docker >= 7.1.0",
 ]
 
-
 [project.urls]
 Homepage = "https://github.com/opthub-org/opthub-runner-python"
 Documentation = "https://github.com/opthub-org/opthub-runner-python"
 Repository = "https://github.com/opthub-org/opthub-runner-python"
 
 
 [tool.poetry]
-version = "1.0.4"
+version = "1.0.6.dev20" # using poetry-dynamic-versioning
 name = "opthub_runner"
 description = "Library for running OptHub problems locally."
 authors = ["Opthub Inc. <dev@opthub.ai>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/opthub-org/opthub-runner-python"
 repository = "https://github.com/opthub-org/opthub-runner-python"
 documentation = "https://github.com/opthub-org/opthub-runner-python"
 keywords = ["opthub", "runner", "evaluator"]
 
+[tool.poetry-dynamic-versioning]
+enable = false
+format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}.dev{{ distance }}{% endif %}"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 docker = "^7.1.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 
-
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 target-version = "py312"
 line-length = 120
 select = ["ALL"]
 ignore = [
     "ANN101",   # Don't require type hints for self.
```

### Comparing `opthub_runner-1.0.4/PKG-INFO` & `opthub_runner-1.0.6.dev20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opthub_runner
-Version: 1.0.4
+Version: 1.0.6.dev20
 Summary: Library for running OptHub problems locally.
 Home-page: https://github.com/opthub-org/opthub-runner-python
 License: MIT
 Keywords: opthub,runner,evaluator
 Author: Opthub Inc.
 Author-email: dev@opthub.ai
 Requires-Python: >=3.8,<4.0
```

