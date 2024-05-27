# Comparing `tmp/promptic-0.5.0.tar.gz` & `tmp/promptic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.5.0.tar` & `promptic-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      487 2024-05-27 23:09:52.547532 promptic-0.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-27 23:09:52.547532 promptic-0.5.0/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-27 23:09:52.547532 promptic-0.5.0/LICENSE
--rw-r--r--   0        0        0     3525 2024-05-27 23:09:52.547532 promptic-0.5.0/README.md
--rw-r--r--   0        0        0     4109 2024-05-27 23:09:52.547532 promptic-0.5.0/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 23:09:52.547532 promptic-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 promptic-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-27 23:13:11.523017 promptic-0.5.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 23:13:11.523017 promptic-0.5.1/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-27 23:13:11.523017 promptic-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3507 2024-05-27 23:13:11.523017 promptic-0.5.1/README.md
+-rw-r--r--   0        0        0     4109 2024-05-27 23:13:11.523017 promptic-0.5.1/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 23:13:11.523017 promptic-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 promptic-0.5.1/PKG-INFO
```

### Comparing `promptic-0.5.0/.gitignore` & `promptic-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.5.0/LICENSE` & `promptic-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.5.0/README.md` & `promptic-0.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -42,20 +42,18 @@
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import llm
 
-@llm(
-    # most arguments are passed directly to litellm.completion
-    # see https://docs.litellm.ai/docs/completion
-    stream=True,
-    model="claude-3-haiku-20240307",
-)
+# most arguments are passed directly to litellm.completion
+# see https://docs.litellm.ai/docs/completion
+
+@llm(stream=True, model="claude-3-haiku-20240307")
 def haiku(subject, adjective, verb="delights"):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
 print("".join(haiku("programming", adjective="witty")))
 # Bits and bytes abound,
 # Bugs and features intertwine,
 # Code, the poet's rhyme.
```

### Comparing `promptic-0.5.0/promptic.py` & `promptic-0.5.1/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.5.0/pyproject.toml` & `promptic-0.5.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.5.0"
+version = "0.5.1"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.5.0/PKG-INFO` & `promptic-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
@@ -51,20 +51,18 @@
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import llm
 
-@llm(
-    # most arguments are passed directly to litellm.completion
-    # see https://docs.litellm.ai/docs/completion
-    stream=True,
-    model="claude-3-haiku-20240307",
-)
+# most arguments are passed directly to litellm.completion
+# see https://docs.litellm.ai/docs/completion
+
+@llm(stream=True, model="claude-3-haiku-20240307")
 def haiku(subject, adjective, verb="delights"):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
 print("".join(haiku("programming", adjective="witty")))
 # Bits and bytes abound,
 # Bugs and features intertwine,
 # Code, the poet's rhyme.
```

