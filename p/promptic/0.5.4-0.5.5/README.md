# Comparing `tmp/promptic-0.5.4.tar.gz` & `tmp/promptic-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.5.4.tar` & `promptic-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      487 2024-05-27 23:37:25.901406 promptic-0.5.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-27 23:37:25.901406 promptic-0.5.4/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-27 23:37:25.901406 promptic-0.5.4/LICENSE
--rw-r--r--   0        0        0     3840 2024-05-27 23:37:25.901406 promptic-0.5.4/README.md
--rw-r--r--   0        0        0     4198 2024-05-27 23:37:25.901406 promptic-0.5.4/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 23:37:25.901406 promptic-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 promptic-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-27 23:40:42.234890 promptic-0.5.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 23:40:42.234890 promptic-0.5.5/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-27 23:40:42.234890 promptic-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3507 2024-05-27 23:40:42.234890 promptic-0.5.5/README.md
+-rw-r--r--   0        0        0     4198 2024-05-27 23:40:42.234890 promptic-0.5.5/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 23:40:42.234890 promptic-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 promptic-0.5.5/PKG-INFO
```

### Comparing `promptic-0.5.4/.gitignore` & `promptic-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.5.4/LICENSE` & `promptic-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.5.4/README.md` & `promptic-0.5.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # promptic
 
-<div style="display: flex; align-items: center; flex-direction: column">
-    <img src="https://github.com/knowsuchagency/promptic/assets/11974795/f268c049-5f33-4ee6-81d0-a976e855dc43" alt="Promptic Python logo" width="200" height="200">
-    <div>
-        <code>promptic</code> is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using <a href="https://github.com/litellm/litellm">litellm</a>. With <code>promptic</code>, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
-    </div>
-</div>
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

### Comparing `promptic-0.5.4/promptic.py` & `promptic-0.5.5/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.5.4/pyproject.toml` & `promptic-0.5.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.5.4"
+version = "0.5.5"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.5.4/PKG-INFO` & `promptic-0.5.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.5.4
+Version: 0.5.5
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
-<div style="display: flex; align-items: center; flex-direction: column">
-    <img src="https://github.com/knowsuchagency/promptic/assets/11974795/f268c049-5f33-4ee6-81d0-a976e855dc43" alt="Promptic Python logo" width="200" height="200">
-    <div>
-        <code>promptic</code> is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using <a href="https://github.com/litellm/litellm">litellm</a>. With <code>promptic</code>, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
-    </div>
-</div>
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

