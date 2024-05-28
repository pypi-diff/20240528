# Comparing `tmp/jax_jynx-0.1.3.tar.gz` & `tmp/jax_jynx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_jynx-0.1.3.tar", max compression
+gzip compressed data, was "jax_jynx-0.1.4.tar", max compression
```

## Comparing `jax_jynx-0.1.3.tar` & `jax_jynx-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/LICENSE
--rw-r--r--   0        0        0     4048 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/README.md
--rw-r--r--   0        0        0      384 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/callbacks.py
--rw-r--r--   0        0        0     3603 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/fit.py
--rw-r--r--   0        0        0     1755 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/__init__.py
--rw-r--r--   0        0        0    21152 2024-04-18 13:25:50.893671 jax_jynx-0.1.3/jynx/layers/containers.py
--rw-r--r--   0        0        0     2059 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/factory.py
--rw-r--r--   0        0        0    12781 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/linear.py
--rw-r--r--   0        0        0     6896 2024-04-18 13:48:03.591997 jax_jynx-0.1.3/jynx/layers/misc.py
--rw-r--r--   0        0        0     2785 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/module.py
--rw-r--r--   0        0        0     4614 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/nets.py
--rw-r--r--   0        0        0     8084 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/rnn.py
--rw-r--r--   0        0        0     3922 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/static.py
--rw-r--r--   0        0        0    22219 2024-04-18 13:49:43.470562 jax_jynx-0.1.3/jynx/layers/transformer.py
--rw-r--r--   0        0        0     4849 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/pytree.py
--rw-r--r--   0        0        0     1138 2024-04-18 13:58:08.443083 jax_jynx-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4395 1970-01-01 00:00:00.000000 jax_jynx-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4048 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/README.md
+-rw-r--r--   0        0        0      384 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/__init__.py
+-rw-r--r--   0        0        0     5425 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/callbacks.py
+-rw-r--r--   0        0        0     3603 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/fit.py
+-rw-r--r--   0        0        0     1755 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/__init__.py
+-rw-r--r--   0        0        0    21152 2024-04-18 13:25:50.893671 jax_jynx-0.1.4/jynx/layers/containers.py
+-rw-r--r--   0        0        0     2059 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/factory.py
+-rw-r--r--   0        0        0    12781 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/linear.py
+-rw-r--r--   0        0        0     6896 2024-04-18 13:48:03.591997 jax_jynx-0.1.4/jynx/layers/misc.py
+-rw-r--r--   0        0        0     2785 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/module.py
+-rw-r--r--   0        0        0     4614 2024-05-28 13:37:39.495061 jax_jynx-0.1.4/jynx/layers/nets.py
+-rw-r--r--   0        0        0     8084 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/rnn.py
+-rw-r--r--   0        0        0     3922 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/layers/static.py
+-rw-r--r--   0        0        0    22219 2024-04-18 13:49:43.470562 jax_jynx-0.1.4/jynx/layers/transformer.py
+-rw-r--r--   0        0        0     4849 2024-04-18 13:22:10.769575 jax_jynx-0.1.4/jynx/pytree.py
+-rw-r--r--   0        0        0     1141 2024-05-28 13:35:33.484894 jax_jynx-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 jax_jynx-0.1.4/PKG-INFO
```

### Comparing `jax_jynx-0.1.3/LICENSE` & `jax_jynx-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/README.md` & `jax_jynx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/callbacks.py` & `jax_jynx-0.1.4/jynx/callbacks.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/fit.py` & `jax_jynx-0.1.4/jynx/fit.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/__init__.py` & `jax_jynx-0.1.4/jynx/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/containers.py` & `jax_jynx-0.1.4/jynx/layers/containers.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/factory.py` & `jax_jynx-0.1.4/jynx/layers/factory.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/linear.py` & `jax_jynx-0.1.4/jynx/layers/linear.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/misc.py` & `jax_jynx-0.1.4/jynx/layers/misc.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/module.py` & `jax_jynx-0.1.4/jynx/layers/module.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/nets.py` & `jax_jynx-0.1.4/jynx/layers/nets.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/rnn.py` & `jax_jynx-0.1.4/jynx/layers/rnn.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/static.py` & `jax_jynx-0.1.4/jynx/layers/static.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/layers/transformer.py` & `jax_jynx-0.1.4/jynx/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/jynx/pytree.py` & `jax_jynx-0.1.4/jynx/pytree.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.3/pyproject.toml` & `jax_jynx-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "jax-jynx"
-version = "0.1.3"
+version = "0.1.4"
 description = "A neural network library using jax"
 authors = ["Scott Cameron"]
 readme = "README.md"
 packages = [
   { include = "jynx" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.12"
-jax = "^0.4.24"
-jaxlib = "^0.4.24"
-optax = "^0.1.9"
+jax = ">=0.4.24"
+jaxlib = ">=0.4.24"
+optax = ">=0.1.9"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pre-commit = "^3.6.1"
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 hypothesis = "^6.98.3"
```

### Comparing `jax_jynx-0.1.3/PKG-INFO` & `jax_jynx-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jax-jynx
-Version: 0.1.3
+Version: 0.1.4
 Summary: A neural network library using jax
 Author: Scott Cameron
 Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: jax (>=0.4.24,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.24,<0.5.0)
-Requires-Dist: optax (>=0.1.9,<0.2.0)
+Requires-Dist: jax (>=0.4.24)
+Requires-Dist: jaxlib (>=0.4.24)
+Requires-Dist: optax (>=0.1.9)
 Description-Content-Type: text/markdown
 
 # Jynx
 
 A straight forward neural network library written in jax. No hidden mechanisms, no black
 magic. Requires only jax and optax.
```

