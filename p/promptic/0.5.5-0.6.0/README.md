# Comparing `tmp/promptic-0.5.5.tar.gz` & `tmp/promptic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.5.5.tar` & `promptic-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      487 2024-05-27 23:40:42.234890 promptic-0.5.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-27 23:40:42.234890 promptic-0.5.5/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-27 23:40:42.234890 promptic-0.5.5/LICENSE
--rw-r--r--   0        0        0     3507 2024-05-27 23:40:42.234890 promptic-0.5.5/README.md
--rw-r--r--   0        0        0     4198 2024-05-27 23:40:42.234890 promptic-0.5.5/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 23:40:42.234890 promptic-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 promptic-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-28 07:52:00.932528 promptic-0.6.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-28 07:52:00.932528 promptic-0.6.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-28 07:52:00.932528 promptic-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3507 2024-05-28 07:52:00.932528 promptic-0.6.0/README.md
+-rw-r--r--   0        0        0     4323 2024-05-28 07:52:00.932528 promptic-0.6.0/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-28 07:52:00.932528 promptic-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 promptic-0.6.0/PKG-INFO
```

### Comparing `promptic-0.5.5/.gitignore` & `promptic-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.5.5/LICENSE` & `promptic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.5.5/README.md` & `promptic-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.5.5/promptic.py` & `promptic-0.6.0/promptic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import inspect
 import json
 import logging
 import re
+import os
 from functools import wraps
 from typing import Callable
 
 import litellm
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
+if os.getenv("PROMPTIC_DEBUG"):
+    logger.setLevel(logging.DEBUG)
+    logger.addHandler(logging.StreamHandler())
+
 
 def promptic(fn=None, model="gpt-3.5-turbo", system: str = None, **litellm_kwargs):
     """
     Decorator to call the LLM with a prompt generated from the function's docstring and arguments.
 
     Args:
         fn: The function to decorate.
```

### Comparing `promptic-0.5.5/pyproject.toml` & `promptic-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.5.5"
+version = "0.6.0"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.5.5/PKG-INFO` & `promptic-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.5.5
+Version: 0.6.0
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

