# Comparing `tmp/opthub_runner-1.0.6.dev20.tar.gz` & `tmp/opthub_runner-1.0.6.post21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opthub_runner-1.0.6.dev20.tar", max compression
+gzip compressed data, was "opthub_runner-1.0.6.post21.tar", max compression
```

## Comparing `opthub_runner-1.0.6.dev20.tar` & `opthub_runner-1.0.6.post21.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/README.md
--rw-r--r--   0        0        0        0 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/converter.py
--rw-r--r--   0        0        0     1899 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/docker_executor.py
--rw-r--r--   0        0        0     2317 2024-05-28 14:08:06.326526 opthub_runner-1.0.6.dev20/opthub_runner/evaluator.py
--rw-r--r--   0        0        0     2481 2024-05-28 14:08:27.090590 opthub_runner-1.0.6.dev20/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 opthub_runner-1.0.6.dev20/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-28 14:09:08.014706 opthub_runner-1.0.6.post21/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 14:09:08.014706 opthub_runner-1.0.6.post21/opthub_runner/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-28 14:09:08.014706 opthub_runner-1.0.6.post21/opthub_runner/converter.py
+-rw-r--r--   0        0        0     1899 2024-05-28 14:09:08.014706 opthub_runner-1.0.6.post21/opthub_runner/docker_executor.py
+-rw-r--r--   0        0        0     2317 2024-05-28 14:09:08.014706 opthub_runner-1.0.6.post21/opthub_runner/evaluator.py
+-rw-r--r--   0        0        0     2483 2024-05-28 14:09:29.714696 opthub_runner-1.0.6.post21/pyproject.toml
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 opthub_runner-1.0.6.post21/PKG-INFO
```

### Comparing `opthub_runner-1.0.6.dev20/opthub_runner/converter.py` & `opthub_runner-1.0.6.post21/opthub_runner/converter.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.6.dev20/opthub_runner/docker_executor.py` & `opthub_runner-1.0.6.post21/opthub_runner/docker_executor.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.6.dev20/opthub_runner/evaluator.py` & `opthub_runner-1.0.6.post21/opthub_runner/evaluator.py`

 * *Files identical despite different names*

### Comparing `opthub_runner-1.0.6.dev20/pyproject.toml` & `opthub_runner-1.0.6.post21/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 [project.urls]
 Homepage = "https://github.com/opthub-org/opthub-runner-python"
 Documentation = "https://github.com/opthub-org/opthub-runner-python"
 Repository = "https://github.com/opthub-org/opthub-runner-python"
 
 
 [tool.poetry]
-version = "1.0.6.dev20" # using poetry-dynamic-versioning
+version = "1.0.6.post21" # using poetry-dynamic-versioning
 name = "opthub_runner"
 description = "Library for running OptHub problems locally."
 authors = ["Opthub Inc. <dev@opthub.ai>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/opthub-org/opthub-runner-python"
 repository = "https://github.com/opthub-org/opthub-runner-python"
 documentation = "https://github.com/opthub-org/opthub-runner-python"
 keywords = ["opthub", "runner", "evaluator"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
-format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}.dev{{ distance }}{% endif %}"
+format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}.post{{ distance }}{% endif %}"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 docker = "^7.1.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
```

### Comparing `opthub_runner-1.0.6.dev20/PKG-INFO` & `opthub_runner-1.0.6.post21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opthub_runner
-Version: 1.0.6.dev20
+Version: 1.0.6.post21
 Summary: Library for running OptHub problems locally.
 Home-page: https://github.com/opthub-org/opthub-runner-python
 License: MIT
 Keywords: opthub,runner,evaluator
 Author: Opthub Inc.
 Author-email: dev@opthub.ai
 Requires-Python: >=3.8,<4.0
```

