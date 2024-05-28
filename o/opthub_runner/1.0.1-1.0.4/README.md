# Comparing `tmp/opthub_runner-1.0.1.tar.gz` & `tmp/opthub_runner-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opthub_runner-1.0.1.tar", max compression
+gzip compressed data, was "opthub_runner-1.0.4.tar", max compression
```

## Comparing `opthub_runner-1.0.1.tar` & `opthub_runner-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/opthub_runner/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/opthub_runner/converter.py
--rw-r--r--   0        0        0     1899 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/opthub_runner/docker_executor.py
--rw-r--r--   0        0        0     1925 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/opthub_runner/evaluator.py
--rw-r--r--   0        0        0     2282 2024-05-27 15:27:26.232538 opthub_runner-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 opthub_runner-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/converter.py
+-rw-r--r--   0        0        0     1899 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/docker_executor.py
+-rw-r--r--   0        0        0     2317 2024-05-28 10:14:57.382817 opthub_runner-1.0.4/opthub_runner/evaluator.py
+-rw-r--r--   0        0        0     2249 2024-05-28 10:15:03.466853 opthub_runner-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 opthub_runner-1.0.4/PKG-INFO
```

### Comparing `opthub_runner-1.0.1/opthub_runner/converter.py` & `opthub_runner-1.0.4/opthub_runner/converter.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.1/opthub_runner/docker_executor.py` & `opthub_runner-1.0.4/opthub_runner/docker_executor.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.1/pyproject.toml` & `opthub_runner-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
+version = "1.0.4"
 name = "opthub_runner"
-version = "1.0.1"
 description = "Library for running OptHub problems locally."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "MIT License"}
+license = {text = "MIT"}
 keywords = ["opthub", "runner", "evaluator"]
 authors = [
   {email = "dev@opthub.ai", name = "Opthub Inc."}
 ]
 maintainers = [
   {email = "dev@opthub.ai", name = "Opthub Inc."}
 ]
@@ -30,25 +30,38 @@
 [project.urls]
 Homepage = "https://github.com/opthub-org/opthub-runner-python"
 Documentation = "https://github.com/opthub-org/opthub-runner-python"
 Repository = "https://github.com/opthub-org/opthub-runner-python"
 
 
 [tool.poetry]
+version = "1.0.4"
 name = "opthub_runner"
-version = "1.0.1"
 description = "Library for running OptHub problems locally."
 authors = ["Opthub Inc. <dev@opthub.ai>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/opthub-org/opthub-runner-python"
 repository = "https://github.com/opthub-org/opthub-runner-python"
 documentation = "https://github.com/opthub-org/opthub-runner-python"
 keywords = ["opthub", "runner", "evaluator"]
 
+[tool.poetry.dependencies]
+python = ">=3.8,<4.0"
+docker = "^7.1.0"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.3.3"
+mypy = "^1.9.0"
+pytest = "^8.1.1"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py312"
 line-length = 120
 select = ["ALL"]
 ignore = [
     "ANN101",   # Don't require type hints for self.
@@ -60,24 +73,7 @@
     "TRY301",   # Allow abstract `raise` to an inner function
     "DTZ005",   # Allow timezone naive datetime
     "BLE001",   # Allow builtin exceptions
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
-
-[tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-docker = "^7.1.0"
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.3.3"
-mypy = "^1.9.0"
-pytest = "^8.1.1"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-
```

### Comparing `opthub_runner-1.0.1/PKG-INFO` & `opthub_runner-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opthub_runner
-Version: 1.0.1
+Version: 1.0.4
 Summary: Library for running OptHub problems locally.
 Home-page: https://github.com/opthub-org/opthub-runner-python
 License: MIT
 Keywords: opthub,runner,evaluator
 Author: Opthub Inc.
 Author-email: dev@opthub.ai
 Requires-Python: >=3.8,<4.0
```

