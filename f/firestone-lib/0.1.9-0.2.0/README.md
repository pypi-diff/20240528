# Comparing `tmp/firestone_lib-0.1.9.tar.gz` & `tmp/firestone_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestone_lib-0.1.9.tar", max compression
+gzip compressed data, was "firestone_lib-0.2.0.tar", max compression
```

## Comparing `firestone_lib-0.1.9.tar` & `firestone_lib-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/LICENSE
--rw-r--r--   0        0        0      311 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/README.md
--rw-r--r--   0        0        0        0 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/__init__.py
--rw-r--r--   0        0        0     4771 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/cli.py
--rw-r--r--   0        0        0     2114 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/resource.py
--rw-r--r--   0        0        0        0 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/resources/logging/__init__.py
--rw-r--r--   0        0        0      396 2024-03-25 16:03:19.833142 firestone_lib-0.1.9/firestone_lib/resources/logging/cli.conf
--rw-r--r--   0        0        0      320 2024-03-25 16:03:19.837143 firestone_lib-0.1.9/firestone_lib/utils.py
--rw-r--r--   0        0        0      959 2024-03-25 16:03:19.837143 firestone_lib-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 firestone_lib-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      311 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/__init__.py
+-rw-r--r--   0        0        0     5231 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/cli.py
+-rw-r--r--   0        0        0     2114 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/resource.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/resources/logging/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/resources/logging/cli.conf
+-rw-r--r--   0        0        0      320 2024-05-28 13:27:41.212613 firestone_lib-0.2.0/firestone_lib/utils.py
+-rw-r--r--   0        0        0      959 2024-05-28 13:27:41.216613 firestone_lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 firestone_lib-0.2.0/PKG-INFO
```

### Comparing `firestone_lib-0.1.9/LICENSE` & `firestone_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.9/firestone_lib/cli.py` & `firestone_lib-0.2.0/firestone_lib/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 
         try:
             return [self.item_type.convert(item, param, ctx) for item in value.split(",")]
         except AttributeError:
             self.fail(f"{value} is not comma-delimited", param, ctx)
 
 
-class FromJsonOrYaml(click.ParamType):
-    """Converts a string from the CLI as a parameter to JSON or YAML object."""
+class SlurpStrOrFile(click.ParamType):
+    """Slurp a string or optionally via a file, using @file.json and run jinja2 templating"""
 
-    name = "String to JSON or YAML object, optionally via a file, using @file.json"
+    name = "Slurp a string or optionally via a file, using @file.json and run jinja2 templating"
 
     def convert(self, value, param, ctx):
         """Convert a string from the CLI as a parameter to JSON object."""
         if value == "-":
             return "-"
         if not isinstance(value, str):
             return value
@@ -82,14 +82,27 @@
             _LOGGER.debug(f"Reading data from file {filename}...")
             with io.open(filename, "r", encoding="utf-8") as fh:
                 raw_str = fh.read()
 
         template = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(raw_str)
         data = template.render(**os.environ)
 
+        return data
+
+
+class FromJsonOrYaml(SlurpStrOrFile):
+    """Converts a string of JSON or YAML from the CLI as a parameter to python struct."""
+
+    name = "Converts a string of JSON or YAML from the CLI as a parameter to python struct."
+
+    def convert(self, value, param, ctx):
+        """Converts a string of JSON or YAML from the CLI as a parameter to python struct."""
+
+        data = super().convert(value, param, ctx)
+
         try:
             _LOGGER.debug("Trying json.load")
             return json.loads(data)
         # pylint: disable=broad-exception-caught
         except Exception:
             pass
```

### Comparing `firestone_lib-0.1.9/firestone_lib/resource.py` & `firestone_lib-0.2.0/firestone_lib/resource.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.9/pyproject.toml` & `firestone_lib-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestone-lib"
-version = "0.1.9"
+version = "0.2.0"
 description = "Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "firestone_lib" }
 ]
```

### Comparing `firestone_lib-0.1.9/PKG-INFO` & `firestone_lib-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestone-lib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

