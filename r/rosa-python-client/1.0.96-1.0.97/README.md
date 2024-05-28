# Comparing `tmp/rosa_python_client-1.0.96.tar.gz` & `tmp/rosa_python_client-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.96.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.97.tar", max compression
```

## Comparing `rosa_python_client-1.0.96.tar` & `rosa_python_client-1.0.97.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      865 2024-05-27 07:17:03.804429 rosa_python_client-1.0.96/README.md
--rw-r--r--   0        0        0     1412 2024-05-27 07:17:11.201408 rosa_python_client-1.0.96/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 07:17:03.806429 rosa_python_client-1.0.96/rosa/__init__.py
--rw-r--r--   0        0        0    11119 2024-05-27 07:17:03.806429 rosa_python_client-1.0.96/rosa/cli.py
--rw-r--r--   0        0        0        0 2024-05-27 07:17:03.807429 rosa_python_client-1.0.96/rosa/tests/__init__.py
--rw-r--r--   0        0        0      843 2024-05-27 07:17:03.807429 rosa_python_client-1.0.96/rosa/tests/conftest.py
--rw-r--r--   0        0        0       30 2024-05-27 07:17:03.807429 rosa_python_client-1.0.96/rosa/tests/const.py
--rw-r--r--   0        0        0     1031 2024-05-27 07:17:03.807429 rosa_python_client-1.0.96/rosa/tests/test_parse_command.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.96/PKG-INFO
+-rw-r--r--   0        0        0      865 2024-05-28 07:42:06.740632 rosa_python_client-1.0.97/README.md
+-rw-r--r--   0        0        0     1412 2024-05-28 07:42:11.250620 rosa_python_client-1.0.97/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 07:42:06.741632 rosa_python_client-1.0.97/rosa/__init__.py
+-rw-r--r--   0        0        0    11119 2024-05-28 07:42:06.741632 rosa_python_client-1.0.97/rosa/cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:42:06.741632 rosa_python_client-1.0.97/rosa/tests/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-28 07:42:06.742632 rosa_python_client-1.0.97/rosa/tests/conftest.py
+-rw-r--r--   0        0        0       30 2024-05-28 07:42:06.742632 rosa_python_client-1.0.97/rosa/tests/const.py
+-rw-r--r--   0        0        0     1031 2024-05-28 07:42:06.742632 rosa_python_client-1.0.97/rosa/tests/test_parse_command.py
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.97/PKG-INFO
```

### Comparing `rosa_python_client-1.0.96/README.md` & `rosa_python_client-1.0.97/README.md`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.96/pyproject.toml` & `rosa_python_client-1.0.97/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "rosa-python-client"
-version = "1.0.96"
+version = "1.0.97"
 description = "Wrapper for rosa cli"
 authors = ["Meni Yakove <myakove@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "rosa" }]
 license = "Apache-2.0"
 homepage = "https://github.com/RedHatQE/rosa-python-client"
 documentation = "https://github.com/RedHatQE/rosa-python-client/blob/main/README.md"
```

### Comparing `rosa_python_client-1.0.96/rosa/cli.py` & `rosa_python_client-1.0.97/rosa/cli.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.96/rosa/tests/conftest.py` & `rosa_python_client-1.0.97/rosa/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.96/rosa/tests/test_parse_command.py` & `rosa_python_client-1.0.97/rosa/tests/test_parse_command.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.96/PKG-INFO` & `rosa_python_client-1.0.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.96
+Version: 1.0.97
 Summary: Wrapper for rosa cli
 Home-page: https://github.com/RedHatQE/rosa-python-client
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

