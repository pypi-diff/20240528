# Comparing `tmp/python_re3data-0.3.0.tar.gz` & `tmp/python_re3data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun May 26 17:18:13 2024, max compression
+gzip compressed data, last modified: Tue May 28 11:52:42 2024, max compression
```

## Comparing `python_re3data-0.3.0.tar` & `python_re3data-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      113 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__about__.py
--rw-r--r--   0        0        0      295 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__init__.py
--rw-r--r--   0        0        0      185 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__main__.py
--rw-r--r--   0        0        0     1639 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/_cli.py
--rw-r--r--   0        0        0     4992 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/_client.py
--rw-r--r--   0        0        0        0 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/py.typed
--rw-r--r--   0        0        0     1160 2024-05-26 17:18:13.000000 python_re3data-0.3.0/.gitignore
--rw-r--r--   0        0        0     1082 2024-05-26 17:18:13.000000 python_re3data-0.3.0/LICENSE
--rw-r--r--   0        0        0     7650 2024-05-26 17:18:13.000000 python_re3data-0.3.0/README.md
--rw-r--r--   0        0        0     7039 2024-05-26 17:18:13.000000 python_re3data-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9734 2024-05-26 17:18:13.000000 python_re3data-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/__about__.py
+-rw-r--r--   0        0        0      295 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/__main__.py
+-rw-r--r--   0        0        0     1639 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/_cli.py
+-rw-r--r--   0        0        0     5008 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/_client.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:52:42.000000 python_re3data-0.4.0/src/re3data/py.typed
+-rw-r--r--   0        0        0     1160 2024-05-28 11:52:42.000000 python_re3data-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1082 2024-05-28 11:52:42.000000 python_re3data-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7650 2024-05-28 11:52:42.000000 python_re3data-0.4.0/README.md
+-rw-r--r--   0        0        0     7048 2024-05-28 11:52:42.000000 python_re3data-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9734 2024-05-28 11:52:42.000000 python_re3data-0.4.0/PKG-INFO
```

### Comparing `python_re3data-0.3.0/src/re3data/_cli.py` & `python_re3data-0.4.0/src/re3data/_cli.py`

 * *Files identical despite different names*

### Comparing `python_re3data-0.3.0/src/re3data/_client.py` & `python_re3data-0.4.0/src/re3data/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 BASE_URL: str = "https://www.re3data.org/api/beta/"
 DEFAULT_HEADERS: dict[str, str] = {
     "Accept": "text/xml; charset=utf-8",
     "User-Agent": f"python-re3data/{__version__}",
 }
 DEFAULT_TIMEOUT = httpx.Timeout(timeout=10.0)  # timeout in seconds
+ALLOWED_RETURN_TYPES = {"xml", "response"}
 
 
 def log_response(response: httpx.Response) -> None:
     """Log the details of an HTTP response.
 
     This function logs the HTTP method, URL, and status code of the response for debugging purposes.
     It uses the 'debug' logging level to provide detailed diagnostic information.
@@ -132,23 +133,21 @@
         Returns:
             A string representation of the response (if `return_type` is "xml") or the full response object.
 
         Raises:
             httpx.RequestError: If the request fails or times out.
             ValueError: If an invalid `return_type` is provided.
         """
+        if return_type not in ALLOWED_RETURN_TYPES:
+            raise ValueError(f"Invalid `return_type`: {return_type}. Expected one of: {ALLOWED_RETURN_TYPES}")
         response = self._client.get(endpoint)
         response.raise_for_status()
-        match return_type:
-            case "xml":
-                return response.text
-            case "response":
-                return response
-            case _:
-                raise ValueError(f"Invalid `return_type`: {return_type}. Expected one of: `xml`, `response`.")
+        if return_type == "xml":
+            return response.text
+        return response
 
     @property
     def repositories(self) -> RepositoryManager:
         """Get the repository manager for this client.
 
         Returns:
             The repository manager.
```

### Comparing `python_re3data-0.3.0/.gitignore` & `python_re3data-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_re3data-0.3.0/LICENSE` & `python_re3data-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_re3data-0.3.0/README.md` & `python_re3data-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python_re3data-0.3.0/pyproject.toml` & `python_re3data-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 type = "pip-compile"
 pip-compile-hashes = true
 pip-compile-installer = "uv"
 pip-compile-resolver = "uv"
 lock-filename = "requirements/{env_name}.txt"
 
 [tool.hatch.envs.docs.scripts]
-cli = "typer src/re3data/_cli.py utils docs --name=re3data --title='CLI Reference' --output docs/src/cli.md"
+cli = "typer src/re3data/_cli.py utils docs --name=re3data --title='Command Line Interface' --output docs/src/cli.md"
 build = "mkdocs build --config-file=docs/mkdocs.yml"
 serve = "mkdocs serve --verbose --config-file=docs/mkdocs.yml"
 deploy = "mike deploy --push --update-aliases $(hatch version) latest --config-file=docs/mkdocs.yml"
 
 [tool.ruff] # Ref: https://docs.astral.sh/ruff/configuration/
 line-length = 120
 src = [
```

### Comparing `python_re3data-0.3.0/PKG-INFO` & `python_re3data-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-re3data
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Pythonic client for the re3data API.
 Project-URL: Changelog, https://github.com/afuetterer/python-re3data/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://afuetterer.github.io/python-re3data
 Project-URL: Issues, https://github.com/afuetterer/python-re3data/issues
 Project-URL: Repository, https://github.com/afuetterer/python-re3data.git
 Author: Heinz-Alexander Fütterer
 License: MIT
```

