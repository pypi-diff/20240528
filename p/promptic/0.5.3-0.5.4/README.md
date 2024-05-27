# Comparing `tmp/promptic-0.5.3.tar.gz` & `tmp/promptic-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.5.3.tar` & `promptic-0.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      487 2024-05-27 23:35:36.979170 promptic-0.5.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-27 23:35:36.979170 promptic-0.5.3/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-27 23:35:36.979170 promptic-0.5.3/LICENSE
--rw-r--r--   0        0        0     3844 2024-05-27 23:35:36.979170 promptic-0.5.3/README.md
--rw-r--r--   0        0        0     4198 2024-05-27 23:35:36.979170 promptic-0.5.3/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 23:35:36.979170 promptic-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 promptic-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-27 23:37:25.901406 promptic-0.5.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 23:37:25.901406 promptic-0.5.4/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-27 23:37:25.901406 promptic-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3840 2024-05-27 23:37:25.901406 promptic-0.5.4/README.md
+-rw-r--r--   0        0        0     4198 2024-05-27 23:37:25.901406 promptic-0.5.4/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 23:37:25.901406 promptic-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 promptic-0.5.4/PKG-INFO
```

### Comparing `promptic-0.5.3/.gitignore` & `promptic-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.5.3/LICENSE` & `promptic-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.5.3/README.md` & `promptic-0.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # promptic
 
-<div style="display: flex; align-items: center;">
+<div style="display: flex; align-items: center; flex-direction: column">
     <img src="https://github.com/knowsuchagency/promptic/assets/11974795/f268c049-5f33-4ee6-81d0-a976e855dc43" alt="Promptic Python logo" width="200" height="200">
-    <div style="margin-left: 20px;">
+    <div>
         <code>promptic</code> is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using <a href="https://github.com/litellm/litellm">litellm</a>. With <code>promptic</code>, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
     </div>
 </div>
 
 ## Installation
 
 ```bash
```

### Comparing `promptic-0.5.3/promptic.py` & `promptic-0.5.4/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.5.3/pyproject.toml` & `promptic-0.5.4/pyproject.toml`

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
-version = "0.5.3"
+version = "0.5.4"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.5.3/PKG-INFO` & `promptic-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.5.3
+Version: 0.5.4
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
-<div style="display: flex; align-items: center;">
+<div style="display: flex; align-items: center; flex-direction: column">
     <img src="https://github.com/knowsuchagency/promptic/assets/11974795/f268c049-5f33-4ee6-81d0-a976e855dc43" alt="Promptic Python logo" width="200" height="200">
-    <div style="margin-left: 20px;">
+    <div>
         <code>promptic</code> is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using <a href="https://github.com/litellm/litellm">litellm</a>. With <code>promptic</code>, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
     </div>
 </div>
 
 ## Installation
 
 ```bash
```

