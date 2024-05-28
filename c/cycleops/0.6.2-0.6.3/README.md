# Comparing `tmp/cycleops-0.6.2.tar.gz` & `tmp/cycleops-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.6.2.tar", max compression
+gzip compressed data, was "cycleops-0.6.3.tar", max compression
```

## Comparing `cycleops-0.6.2.tar` & `cycleops-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-04-03 06:20:04.445339 cycleops-0.6.2/LICENSE
--rw-r--r--   0        0        0     5466 2024-04-03 06:20:04.445339 cycleops-0.6.2/README.md
--rw-r--r--   0        0        0     1512 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/__main__.py
--rw-r--r--   0        0        0      414 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/auth.py
--rw-r--r--   0        0        0     8708 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/client.py
--rw-r--r--   0        0        0     1155 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/environments.py
--rw-r--r--   0        0        0     1113 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/exceptions.py
--rw-r--r--   0        0        0     3762 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/hostgroups.py
--rw-r--r--   0        0        0     4349 2024-04-03 06:20:04.445339 cycleops-0.6.2/cycleops/hosts.py
--rw-r--r--   0        0        0    13019 2024-04-03 06:20:04.449339 cycleops-0.6.2/cycleops/services.py
--rw-r--r--   0        0        0     5988 2024-04-03 06:20:04.449339 cycleops-0.6.2/cycleops/setups.py
--rw-r--r--   0        0        0     3607 2024-04-03 06:20:04.449339 cycleops-0.6.2/cycleops/stacks.py
--rw-r--r--   0        0        0      869 2024-04-03 06:20:04.449339 cycleops-0.6.2/cycleops/units.py
--rw-r--r--   0        0        0      972 2024-04-03 06:20:04.449339 cycleops-0.6.2/cycleops/utils.py
--rw-r--r--   0        0        0      558 2024-04-03 06:20:04.449339 cycleops-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5991 1970-01-01 00:00:00.000000 cycleops-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 05:35:01.708167 cycleops-0.6.3/LICENSE
+-rw-r--r--   0        0        0     5466 2024-05-28 05:35:01.708167 cycleops-0.6.3/README.md
+-rw-r--r--   0        0        0     1512 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/auth.py
+-rw-r--r--   0        0        0     8708 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/client.py
+-rw-r--r--   0        0        0     1126 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/environments.py
+-rw-r--r--   0        0        0     1113 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/exceptions.py
+-rw-r--r--   0        0        0     3762 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/hostgroups.py
+-rw-r--r--   0        0        0     4349 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/hosts.py
+-rw-r--r--   0        0        0    13019 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/services.py
+-rw-r--r--   0        0        0     5988 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/setups.py
+-rw-r--r--   0        0        0     3607 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/stacks.py
+-rw-r--r--   0        0        0      943 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/units.py
+-rw-r--r--   0        0        0      972 2024-05-28 05:35:01.708167 cycleops-0.6.3/cycleops/utils.py
+-rw-r--r--   0        0        0      558 2024-05-28 05:35:01.708167 cycleops-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5991 1970-01-01 00:00:00.000000 cycleops-0.6.3/PKG-INFO
```

### Comparing `cycleops-0.6.2/LICENSE` & `cycleops-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/README.md` & `cycleops-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/__main__.py` & `cycleops-0.6.3/cycleops/__main__.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/client.py` & `cycleops-0.6.3/cycleops/client.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/environments.py` & `cycleops-0.6.3/cycleops/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import typer
 from rich import print
-from rich.table import Table
 
 from .client import EnvironmentClient, cycleops_client
 from .exceptions import NotFound
 from .utils import display_error_message
 
 app = typer.Typer()
```

### Comparing `cycleops-0.6.2/cycleops/exceptions.py` & `cycleops-0.6.3/cycleops/exceptions.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/hostgroups.py` & `cycleops-0.6.3/cycleops/hostgroups.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/hosts.py` & `cycleops-0.6.3/cycleops/hosts.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/services.py` & `cycleops-0.6.3/cycleops/services.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/setups.py` & `cycleops-0.6.3/cycleops/setups.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/stacks.py` & `cycleops-0.6.3/cycleops/stacks.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/cycleops/utils.py` & `cycleops-0.6.3/cycleops/utils.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.6.2/pyproject.toml` & `cycleops-0.6.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycleops"
-version = "0.6.2"
+version = "0.6.3"
 description = "The official command line interface for Cycleops"
 authors = ["George Margaritis <george@withlogic.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cycleops-0.6.2/PKG-INFO` & `cycleops-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycleops
-Version: 0.6.2
+Version: 0.6.3
 Summary: The official command line interface for Cycleops
 License: MIT
 Author: George Margaritis
 Author-email: george@withlogic.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

