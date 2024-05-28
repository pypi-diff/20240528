# Comparing `tmp/processing_pypelines-0.0.58.tar.gz` & `tmp/processing_pypelines-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.58.tar", last modified: Tue May 14 18:43:45 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.59.tar", last modified: Tue May 28 16:22:55 2024, max compression
```

## Comparing `processing_pypelines-0.0.58.tar` & `processing_pypelines-0.0.59.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/LICENSE
--rw-r--r--   0        0        0      118 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/README.md
--rw-r--r--   0        0        0     1152 2024-05-14 18:43:45.204755 processing_pypelines-0.0.58/pyproject.toml
--rw-r--r--   0        0        0      367 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4633 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34226 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-05-14 18:43:35.128878 processing_pypelines-0.0.58/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17075 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6559 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     9444 2024-05-14 18:43:35.132878 processing_pypelines-0.0.58/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/sessions.py
--rw-r--r--   0        0        0    37032 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-05-14 18:43:35.208877 processing_pypelines-0.0.58/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-05-14 18:43:35.136878 processing_pypelines-0.0.58/tests/versions_example.json
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.58/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/README.md
+-rw-r--r--   0        0        0     1152 2024-05-28 16:22:55.231646 processing_pypelines-0.0.59/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4671 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34226 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17073 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6559 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9444 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    37032 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-05-28 16:22:45.879739 processing_pypelines-0.0.59/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.59/PKG-INFO
```

### Comparing `processing_pypelines-0.0.58/LICENSE` & `processing_pypelines-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/pyproject.toml` & `processing_pypelines-0.0.59/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.58"
+version = "0.0.59"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.58/src/pypelines/accessors.py` & `processing_pypelines-0.0.59/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/arguments.py` & `processing_pypelines-0.0.59/src/pypelines/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,17 @@
             is not found in the arguments file.
     """
     local_log = getLogger("autoload_arguments")
 
     try:
         config_args = read_session_arguments_file(session, step)["functions"][step.relative_name]
     except FileNotFoundError as e:
-        local_log.debug(f"{type(e).__name__} : {e}. Skipping")
+        local_log.debug(f"{type(e).__name__} : {e}. Skipping autoload_arguments")
         return {}
     except KeyError:
         local_log.debug(
             f"Could not find the `functions` key or the key `{step.relative_name}` in pipelines_arguments.json file at"
-            f" {session.path}. Skipping"
+            f" {session.path}. Skipping autoload_arguments"
         )
         return {}
 
     return config_args
```

### Comparing `processing_pypelines-0.0.58/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.59/src/pypelines/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/disk.py` & `processing_pypelines-0.0.59/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/examples.py` & `processing_pypelines-0.0.59/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.59/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/graphs.py` & `processing_pypelines-0.0.59/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/loggs.py` & `processing_pypelines-0.0.59/src/pypelines/loggs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     UserNameFilter,
     ProgramNameFilter,
     HostNameFilter,
 )
 from pathlib import Path
 
 NAMELENGTH = 33  # global variable for formatting the length of the padding dedicated to name part in a logging record
-LEVELLENGTH = 8  # global variable for formatting the length of the padding dedicated to levelname part in a record
+LEVELLENGTH = 9  # global variable for formatting the length of the padding dedicated to levelname part in a record
 
 
 def enable_logging(
     filename: str | None = None,
     terminal_level: str = "NOTE",
     file_level: str = "LOAD",
     programname: str = "",
@@ -242,19 +242,19 @@
             level_styles=self.LEVEL_STYLES,
             field_styles=self.FIELD_STYLES,
             dynamic_levels=self.DYNAMIC_LEVELS,
         )
 
 
 class TerminalFormatter(SugarColoredFormatter):
-    FORMAT = f"%(levelname)-{LEVELLENGTH}s : %(name)-{NAMELENGTH}s : %(message)s - %(asctime)s"
+    FORMAT = f"%(levelname)-{LEVELLENGTH}s: %(name)-{NAMELENGTH}s : %(message)s - %(asctime)s"
 
 
 class FileFormatter(SugarColoredFormatter):
-    FORMAT = f"[%(asctime)s] %(hostname)s %(levelname)-{LEVELLENGTH}s : %(name)-{NAMELENGTH}s : %(message)s"
+    FORMAT = f"[%(asctime)s] %(hostname)s %(levelname)-{LEVELLENGTH}s: %(name)-{NAMELENGTH}s : %(message)s"
 
 
 class ContextFilter(logging.Filter):
     """This is a filter which injects contextual information into the log."""
 
     def __init__(self, context_msg):
         """Initialization method.
```

### Comparing `processing_pypelines-0.0.58/src/pypelines/multisession.py` & `processing_pypelines-0.0.59/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.59/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/pipelines.py` & `processing_pypelines-0.0.59/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/pipes.py` & `processing_pypelines-0.0.59/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/sessions.py` & `processing_pypelines-0.0.59/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/steps.py` & `processing_pypelines-0.0.59/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/tasks.py` & `processing_pypelines-0.0.59/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/src/pypelines/versions.py` & `processing_pypelines-0.0.59/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/tests/tests.py` & `processing_pypelines-0.0.59/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/tests/versions_example.json` & `processing_pypelines-0.0.59/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.58/PKG-INFO` & `processing_pypelines-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.58
+Version: 0.0.59
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

