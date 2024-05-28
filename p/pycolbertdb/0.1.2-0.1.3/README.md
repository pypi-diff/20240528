# Comparing `tmp/pycolbertdb-0.1.2.tar.gz` & `tmp/pycolbertdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolbertdb-0.1.2.tar", max compression
+gzip compressed data, was "pycolbertdb-0.1.3.tar", max compression
```

## Comparing `pycolbertdb-0.1.2.tar` & `pycolbertdb-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1092 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/pycolbertdb/__init__.py
--rw-r--r--   0        0        0     9622 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/pycolbertdb/client.py
--rw-r--r--   0        0        0     2229 2024-05-23 12:52:20.525684 pycolbertdb-0.1.2/pycolbertdb/models.py
--rw-r--r--   0        0        0      518 2024-05-23 12:52:20.525684 pycolbertdb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 pycolbertdb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1092 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/pycolbertdb/__init__.py
+-rw-r--r--   0        0        0     9797 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/pycolbertdb/client.py
+-rw-r--r--   0        0        0     2229 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/pycolbertdb/models.py
+-rw-r--r--   0        0        0      518 2024-05-28 18:37:31.564728 pycolbertdb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 pycolbertdb-0.1.3/PKG-INFO
```

### Comparing `pycolbertdb-0.1.2/README.md` & `pycolbertdb-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.1.2/pycolbertdb/client.py` & `pycolbertdb-0.1.3/pycolbertdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
             Dict[str, Any]: The JSON response from the server.
         """
         response = requests.post(
             f"{self.url}/client/connect",
             json={"api_key": self.api_key},
             timeout=TIMEOUT,
         )
+        if response.status_code != 200:
+            raise ValueError(
+                f"Failed to connect to the Colbertdb server - {response.json()['detail']}"
+            )
         self.access_token = response.json()["access_token"]
 
     def _get(self, path: str, data: Dict[str, Any]) -> Dict[str, Any]:
         """
         Sends a GET request to the Colbertdb server.
 
         Args:
```

### Comparing `pycolbertdb-0.1.2/pycolbertdb/models.py` & `pycolbertdb-0.1.3/pycolbertdb/models.py`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.1.2/pyproject.toml` & `pycolbertdb-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycolbertdb"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for colbertdb"
 authors = ["Ryan Sloan <rysloan4@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `pycolbertdb-0.1.2/PKG-INFO` & `pycolbertdb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolbertdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for colbertdb
 License: MIT
 Author: Ryan Sloan
 Author-email: rysloan4@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

