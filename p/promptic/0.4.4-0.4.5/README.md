# Comparing `tmp/promptic-0.4.4.tar.gz` & `tmp/promptic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.4.4.tar` & `promptic-0.4.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3156 2024-05-27 19:31:43.907511 promptic-0.4.4/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.4.4/LICENSE
--rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.4.4/README.md
--rw-r--r--   0        0        0     3767 2024-05-27 19:39:51.368363 promptic-0.4.4/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 19:43:06.768444 promptic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      555 2024-05-27 22:30:42.716118 promptic-0.4.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 22:30:42.716118 promptic-0.4.5/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-27 22:30:42.716118 promptic-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3017 2024-05-27 22:30:42.716118 promptic-0.4.5/README.md
+-rw-r--r--   0        0        0     3767 2024-05-27 22:30:42.716118 promptic-0.4.5/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 22:30:42.716118 promptic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.5/PKG-INFO
```

### Comparing `promptic-0.4.4/.gitignore` & `promptic-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.4.4/LICENSE` & `promptic-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.4.4/README.md` & `promptic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.4.4/promptic.py` & `promptic-0.4.5/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.4.4/pyproject.toml` & `promptic-0.4.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.4.4"
+version = "0.4.5"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.4.4/PKG-INFO` & `promptic-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.4.4
+Version: 0.4.5
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

