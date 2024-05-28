# Comparing `tmp/valsai-0.0.34.tar.gz` & `tmp/valsai-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valsai-0.0.34.tar", last modified: Sat May  4 17:49:08 2024, max compression
+gzip compressed data, was "valsai-0.0.35.tar", last modified: Tue May 28 16:30:48 2024, max compression
```

## Comparing `valsai-0.0.34.tar` & `valsai-0.0.35.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.142785 valsai-0.0.34/
--rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-04 17:49:08.142349 valsai-0.0.34/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)     2829 2024-05-04 01:58:49.000000 valsai-0.0.34/README.md
--rw-r--r--   0 langston   (501) staff       (20)       38 2024-05-04 17:49:08.142852 valsai-0.0.34/setup.cfg
--rw-r--r--   0 langston   (501) staff       (20)      615 2024-05-04 17:48:41.000000 valsai-0.0.34/setup.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.133226 valsai-0.0.34/vals/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/__init__.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.136130 valsai-0.0.34/vals/cli/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/cli/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     1424 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/auth.py
--rw-r--r--   0 langston   (501) staff       (20)      284 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/cli/main.py
--rw-r--r--   0 langston   (501) staff       (20)     5048 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/rag.py
--rw-r--r--   0 langston   (501) staff       (20)     4350 2024-05-04 16:17:59.000000 valsai-0.0.34/vals/cli/run.py
--rw-r--r--   0 langston   (501) staff       (20)     4768 2024-05-04 16:17:59.000000 valsai-0.0.34/vals/cli/suite.py
--rw-r--r--   0 langston   (501) staff       (20)     1061 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/util.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.138788 valsai-0.0.34/vals/sdk/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     3415 2024-05-04 16:20:15.000000 valsai-0.0.34/vals/sdk/auth.py
--rw-r--r--   0 langston   (501) staff       (20)      134 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/exceptions.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.139730 valsai-0.0.34/vals/sdk/jsonschemas/
--rw-r--r--   0 langston   (501) staff       (20)      550 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/jsonschemas/run_params_schema.json
--rw-r--r--   0 langston   (501) staff       (20)     2482 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/jsonschemas/suiteschema.json
--rw-r--r--   0 langston   (501) staff       (20)     6526 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/run.py
--rw-r--r--   0 langston   (501) staff       (20)     2421 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/sdk.py
--rw-r--r--   0 langston   (501) staff       (20)    11362 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/suite.py
--rw-r--r--   0 langston   (501) staff       (20)     1685 2024-05-04 16:20:15.000000 valsai-0.0.34/vals/sdk/util.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.141862 valsai-0.0.34/valsai.egg-info/
--rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      549 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/SOURCES.txt
--rw-r--r--   0 langston   (501) staff       (20)        1 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/dependency_links.txt
--rw-r--r--   0 langston   (501) staff       (20)       43 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/entry_points.txt
--rw-r--r--   0 langston   (501) staff       (20)       80 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/requires.txt
--rw-r--r--   0 langston   (501) staff       (20)        5 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.724544 valsai-0.0.35/
+-rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-28 16:30:48.724177 valsai-0.0.35/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)     2822 2024-05-27 22:53:44.000000 valsai-0.0.35/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2024-05-28 16:30:48.724615 valsai-0.0.35/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      615 2024-05-28 16:28:22.000000 valsai-0.0.35/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.716945 valsai-0.0.35/vals/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/__init__.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.718770 valsai-0.0.35/vals/cli/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     1416 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/auth.py
+-rw-r--r--   0 langston   (501) staff       (20)      284 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/main.py
+-rw-r--r--   0 langston   (501) staff       (20)     5048 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/rag.py
+-rw-r--r--   0 langston   (501) staff       (20)     4350 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/run.py
+-rw-r--r--   0 langston   (501) staff       (20)     4768 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/suite.py
+-rw-r--r--   0 langston   (501) staff       (20)     1061 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/cli/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.721083 valsai-0.0.35/vals/sdk/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     3415 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/auth.py
+-rw-r--r--   0 langston   (501) staff       (20)      134 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/exceptions.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.721799 valsai-0.0.35/vals/sdk/jsonschemas/
+-rw-r--r--   0 langston   (501) staff       (20)      550 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/jsonschemas/run_params_schema.json
+-rw-r--r--   0 langston   (501) staff       (20)     2482 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/jsonschemas/suiteschema.json
+-rw-r--r--   0 langston   (501) staff       (20)     6526 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/run.py
+-rw-r--r--   0 langston   (501) staff       (20)     2421 2024-05-27 23:45:04.000000 valsai-0.0.35/vals/sdk/sdk.py
+-rw-r--r--   0 langston   (501) staff       (20)    11458 2024-05-28 05:44:55.000000 valsai-0.0.35/vals/sdk/suite.py
+-rw-r--r--   0 langston   (501) staff       (20)     1685 2024-05-27 22:53:45.000000 valsai-0.0.35/vals/sdk/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-28 16:30:48.723772 valsai-0.0.35/valsai.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      549 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       43 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/entry_points.txt
+-rw-r--r--   0 langston   (501) staff       (20)       80 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)        5 2024-05-28 16:30:48.000000 valsai-0.0.35/valsai.egg-info/top_level.txt
```

### Comparing `valsai-0.0.34/README.md` & `valsai-0.0.35/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# PlaygroundRL CLI Tool
+# Vals AI CLI Tool
 
 ## Install
 
 ```
-pip install vals-cli
+pip install valsai
 ```
 
 ### _Internal: Install during development_
 
 ```
 cd legal-evaluator/cli
 pip install -e .
```

### Comparing `valsai-0.0.34/setup.py` & `valsai-0.0.35/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="valsai",
-    version="0.0.34",
+    version="0.0.35",
     author="Langston Nashold, Rayan Krishnan",
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["jsonschemas/*"]},
     install_requires=[
         "Click",
         "gql",
```

### Comparing `valsai-0.0.34/vals/cli/auth.py` & `valsai-0.0.35/vals/cli/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import click
 from vals.sdk.auth import CREDS_PATH, PRL_PATH, get_client_id
 
 
 @click.command(name="login")
 def login_command():
     """
-    Authenticate with PlaygroundRL CLI
+    Authenticate with Vals CLI
     """
     in_eu = click.confirm("Are you located in Europe?")
     region = "eu-north-1" if in_eu else "us-east-1"
     username = click.prompt("email")
     password = click.prompt("password", hide_input=True)
 
     client_id = get_client_id(in_eu, False)
```

### Comparing `valsai-0.0.34/vals/cli/rag.py` & `valsai-0.0.35/vals/cli/rag.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/cli/run.py` & `valsai-0.0.35/vals/cli/run.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/cli/suite.py` & `valsai-0.0.35/vals/cli/suite.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/cli/util.py` & `valsai-0.0.35/vals/cli/util.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/auth.py` & `valsai-0.0.35/vals/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/jsonschemas/run_params_schema.json` & `valsai-0.0.35/vals/sdk/jsonschemas/run_params_schema.json`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/jsonschemas/suiteschema.json` & `valsai-0.0.35/vals/sdk/jsonschemas/suiteschema.json`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/run.py` & `valsai-0.0.35/vals/sdk/run.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/sdk.py` & `valsai-0.0.35/vals/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/vals/sdk/suite.py` & `valsai-0.0.35/vals/sdk/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     "negative_answer",
     "matches_tone",
     "check_salesiness",
     "matches_format",
     "grammar",
     "equal_intent",
     "capitalized_correctly",
+    "is_polite",
+    "progresses_conversation",
 ]
 
 UNARY_OPERATORS = [
     "answers",
     "not_answers",
     "is_concise",
     "is_coherent",
@@ -60,14 +62,16 @@
     "valid_yaml",
     "list_format",
     "paragraph_format",
     "affirmative_answer",
     "negative_answer",
     "grammar",
     "capitalized_correctly",
+    "is_polite",
+    "progresses_conversation",
 ]
 
 
 def create_suite(suite_data: Dict[str, Any]) -> str:
     """
     Method to create a test suite. Suite_data
     should be a JSON-like python dict that contains the information outlined in our docs.
```

### Comparing `valsai-0.0.34/vals/sdk/util.py` & `valsai-0.0.35/vals/sdk/util.py`

 * *Files identical despite different names*

### Comparing `valsai-0.0.34/valsai.egg-info/SOURCES.txt` & `valsai-0.0.35/valsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

