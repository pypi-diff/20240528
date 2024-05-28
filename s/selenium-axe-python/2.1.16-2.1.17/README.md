# Comparing `tmp/selenium_axe_python-2.1.16.tar.gz` & `tmp/selenium_axe_python-2.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_axe_python-2.1.16.tar", max compression
+gzip compressed data, was "selenium_axe_python-2.1.17.tar", max compression
```

## Comparing `selenium_axe_python-2.1.16.tar` & `selenium_axe_python-2.1.17.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    16725 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/LICENSE.txt
--rwxr-xr-x   0        0        0     7126 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/README.md
--rw-r--r--   0        0        0     6024 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/pyproject.toml
--rw-r--r--   0        0        0      247 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/selenium_axe_python/__init__.py
--rw-r--r--   0        0        0   540010 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/selenium_axe_python/axe-core/axe.min.js
--rwxr-xr-x   0        0        0     3871 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/selenium_axe_python/axe.py
--rw-r--r--   0        0        0      199 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/selenium_axe_python/tests/__init__.py
--rw-r--r--   0        0        0     1124 2024-01-16 23:23:33.126203 selenium_axe_python-2.1.16/selenium_axe_python/tests/conftest.py
--rw-r--r--   0        0        0     2318 2024-01-16 23:23:33.130203 selenium_axe_python-2.1.16/selenium_axe_python/tests/pytest.ini
--rwxr-xr-x   0        0        0    11699 2024-01-16 23:23:33.130203 selenium_axe_python-2.1.16/selenium_axe_python/tests/test_axe.py
--rw-r--r--   0        0        0      379 2024-01-16 23:23:33.130203 selenium_axe_python-2.1.16/selenium_axe_python/tests/test_page.html
--rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.16/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-28 21:30:18.539058 selenium_axe_python-2.1.17/LICENSE.txt
+-rwxr-xr-x   0        0        0     7126 2024-05-28 21:30:18.539058 selenium_axe_python-2.1.17/README.md
+-rw-r--r--   0        0        0     5862 2024-05-28 21:30:18.539058 selenium_axe_python-2.1.17/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-05-28 21:30:18.539058 selenium_axe_python-2.1.17/selenium_axe_python/__init__.py
+-rw-r--r--   0        0        0   540010 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/axe-core/axe.min.js
+-rwxr-xr-x   0        0        0     3871 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/axe.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/py.typed
+-rw-r--r--   0        0        0      199 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/tests/__init__.py
+-rw-r--r--   0        0        0     1124 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/tests/conftest.py
+-rw-r--r--   0        0        0     2318 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/tests/pytest.ini
+-rwxr-xr-x   0        0        0    11699 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/tests/test_axe.py
+-rw-r--r--   0        0        0      379 2024-05-28 21:30:18.543058 selenium_axe_python-2.1.17/selenium_axe_python/tests/test_page.html
+-rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.17/PKG-INFO
```

### Comparing `selenium_axe_python-2.1.16/LICENSE.txt` & `selenium_axe_python-2.1.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/README.md` & `selenium_axe_python-2.1.17/README.md`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/pyproject.toml` & `selenium_axe_python-2.1.17/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Poetry:
 #   poetry install --extras dev
 # PIP:
 #   pip install -e .[dev]
 
 [tool.poetry]
 name = "selenium-axe-python"
-version = "2.1.16"
+version = "2.1.17"
 description = "Python library to integrate axe and selenium for web accessibility testing."
 authors = ["Marcel Wilson"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 repository = "https://github.com/bandophahita/selenium-axe-python"
 #documentation = ""
 readme = "README.md"
 classifiers = [
@@ -83,17 +83,45 @@
 include_trailing_comma = "True"
 use_parentheses = "True"
 combine_as_imports = "True"
 src_paths = "selenium-axe-python"
 
 
 [tool.ruff]
-# Enable the pycodestyle (`E`) and Pyflakes (`F`) rules by default.
-# Unlike Flake8, Ruff doesn't enable pycodestyle warnings (`W`) or
-# McCabe complexity (`C901`) by default.
+target-version = "py311"
+line-length = 88
+
+extend-exclude = [
+    ".github",
+    ".pytest_cache",
+    ".venv",
+    "venv",
+    "dockerfiles",
+    "docs",
+    ".coverage",
+    ".coveragerc",
+    ".env",
+    ".env.example",
+    ".flake8",
+    ".gitignore",
+    "alembic.ini",
+    "bandit.yaml",
+    "docker-compose-dev.yaml",
+    "docker-compose-pro.yaml",
+    "Makefile",
+    "mkdocks.yml",
+    "mypy.ini",
+    "poetry.lock",
+    "pyproject.toml",
+    "pytest.ini",
+    "README.md",
+    ".idea",
+]
+
+[tool.ruff.lint]
 select = [
     "A",  # flake8-builtins
     "ANN",  # flake8-annotations  # coming back to this one later to compare against mypy
     "ARG",  # flake8-unused-arguments
     "B",  # flake8-bugbear
     "BLE",  # flake8-blind-except
     "C4",  # flake8-comprehensions
@@ -135,79 +163,46 @@
     #    "ANN401",  # any-type
     # 3.8 & 3.9 support
     "UP006",  # Use `dict` instead of `Dict` for type annotation
     "UP007",  # Use `X | Y` for type annotations
     "UP035",  # 3.8 still needs Dict for typealias
 ]
 
-# Same as Black.
-line-length = 88
-
-exclude = [
-    ".github",
-    ".pytest_cache",
-    ".venv",
-    "venv",
-    "dockerfiles",
-    "docs",
-    ".coverage",
-    ".coveragerc",
-    ".env",
-    ".env.example",
-    ".flake8",
-    ".gitignore",
-    "alembic.ini",
-    "bandit.yaml",
-    "docker-compose-dev.yaml",
-    "docker-compose-pro.yaml",
-    "Makefile",
-    "mkdocks.yml",
-    "mypy.ini",
-    "poetry.lock",
-    "pyproject.toml",
-    "pytest.ini",
-    "README.md",
-    ".idea",
-]
-
-target-version = "py311"
-
-[tool.ruff.lint]
 extend-safe-fixes = [
     "EM101",
     "EM102",
     "TCH001", "TCH002", "TCH003", "TCH004",
     #    "SIM108"
     # maybe?
     #    "F841",
     "C419",
     "D200", "D205", "D415",
     "PT003", "PT006", "PT018",
     "RET504",
     "UP007",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "test_axe.py" = ["E501", "PLR"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 split-on-trailing-comma = true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 mark-parentheses = false
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 ignore-overlong-task-comments = true
 
 #[tool.ruff.flake8-annotations]
 #mypy-init-return = true
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 # ignore returns types for functions that implicity or explicitly only return None
 suppress-none-returning = true
 allow-star-arg-any = true
 
 [tool.black]
 line-length = 88
 target-version = ['py311']
```

### Comparing `selenium_axe_python-2.1.16/selenium_axe_python/axe-core/axe.min.js` & `selenium_axe_python-2.1.17/selenium_axe_python/axe-core/axe.min.js`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/selenium_axe_python/axe.py` & `selenium_axe_python-2.1.17/selenium_axe_python/axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/selenium_axe_python/tests/conftest.py` & `selenium_axe_python-2.1.17/selenium_axe_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/selenium_axe_python/tests/pytest.ini` & `selenium_axe_python-2.1.17/selenium_axe_python/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/selenium_axe_python/tests/test_axe.py` & `selenium_axe_python-2.1.17/selenium_axe_python/tests/test_axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.16/PKG-INFO` & `selenium_axe_python-2.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-axe-python
-Version: 2.1.16
+Version: 2.1.17
 Summary: Python library to integrate axe and selenium for web accessibility testing.
 Home-page: https://github.com/bandophahita/selenium-axe-python
 License: Mozilla Public License 2.0 (MPL 2.0)
 Author: Marcel Wilson
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
```

