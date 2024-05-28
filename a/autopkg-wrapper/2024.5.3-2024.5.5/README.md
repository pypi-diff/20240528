# Comparing `tmp/autopkg_wrapper-2024.5.3.tar.gz` & `tmp/autopkg_wrapper-2024.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopkg_wrapper-2024.5.3.tar", max compression
+gzip compressed data, was "autopkg_wrapper-2024.5.5.tar", max compression
```

## Comparing `autopkg_wrapper-2024.5.3.tar` & `autopkg_wrapper-2024.5.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1602 2024-05-14 10:01:10.965797 autopkg_wrapper-2024.5.3/LICENSE
--rw-r--r--   0        0        0     1833 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/README.md
--rw-r--r--   0        0        0       25 2024-05-14 10:01:32.421535 autopkg_wrapper-2024.5.3/autopkg_wrapper/__init__.py
--rwxr-xr-x   0        0        0    10940 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/autopkg_wrapper.py
--rw-r--r--   0        0        0       22 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/notifier/__init__.py
--rw-r--r--   0        0        0     1982 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/notifier/slack.py
--rw-r--r--   0        0        0       22 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/__init__.py
--rw-r--r--   0        0        0     3934 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/args.py
--rw-r--r--   0        0        0     2975 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/git_functions.py
--rw-r--r--   0        0        0      324 2024-05-14 10:01:10.969797 autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/logging.py
--rw-r--r--   0        0        0     1038 2024-05-14 10:01:32.417535 autopkg_wrapper-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1602 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/LICENSE
+-rw-r--r--   0        0        0     1833 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/README.md
+-rw-r--r--   0        0        0       25 2024-05-28 02:43:49.930335 autopkg_wrapper-2024.5.5/autopkg_wrapper/__init__.py
+-rwxr-xr-x   0        0        0    10940 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/autopkg_wrapper.py
+-rw-r--r--   0        0        0       22 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/notifier/__init__.py
+-rw-r--r--   0        0        0     1982 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/notifier/slack.py
+-rw-r--r--   0        0        0       22 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/__init__.py
+-rw-r--r--   0        0        0     4212 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/args.py
+-rw-r--r--   0        0        0     2975 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/git_functions.py
+-rw-r--r--   0        0        0      324 2024-05-28 02:43:26.002437 autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/logging.py
+-rw-r--r--   0        0        0      964 2024-05-28 02:43:49.922335 autopkg_wrapper-2024.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.5.5/PKG-INFO
```

### Comparing `autopkg_wrapper-2024.5.3/LICENSE` & `autopkg_wrapper-2024.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.3/README.md` & `autopkg_wrapper-2024.5.5/README.md`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.3/autopkg_wrapper/autopkg_wrapper.py` & `autopkg_wrapper-2024.5.5/autopkg_wrapper/autopkg_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.3/autopkg_wrapper/notifier/slack.py` & `autopkg_wrapper-2024.5.5/autopkg_wrapper/notifier/slack.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/args.py` & `autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 
     if dir_exists:
         return dir_path
     else:
         message = f"Error! This is not valid directory: {arg}"
         raise argparse.ArgumentTypeError(message)
 
+def validate_bool(arg):
+    if isinstance(arg, bool):
+        return arg
+    elif isinstance(arg, str) and arg.lower() in ['0','false','no', 'f']:
+        return False
+    elif isinstance(arg, str) and arg.lower() in ['1','true','yes', 't']:
+        return True
+
 def setup_args():
     parser = argparse.ArgumentParser(description="Run autopkg recipes")
     recipe_arguments = parser.add_mutually_exclusive_group()
     recipe_arguments.add_argument(
         "--recipe-file",
         type=validate_file,
         default=os.getenv("AW_RECIPE_FILE", None),
@@ -46,15 +54,15 @@
                 `export AW_RECIPES="recipe_one.download recipe_two.download"`
                 `export AW_RECIPES="recipe_one.pkg,recipe_two.pkg"`
                 `autopkg-wrapper`
             """,
     )
     parser.add_argument(
         "--debug",
-        default=os.getenv("AW_DEBUG", False),
+        default=validate_bool(os.getenv("AW_DEBUG", False)),
         action="store_true",
         help="Enable debug logging when running script",
     )
     parser.add_argument(
         "--disable-recipe-trust-check",
         action="store_true",
         help="""
```

### Comparing `autopkg_wrapper-2024.5.3/autopkg_wrapper/utils/git_functions.py` & `autopkg_wrapper-2024.5.5/autopkg_wrapper/utils/git_functions.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.3/pyproject.toml` & `autopkg_wrapper-2024.5.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
     authors = ["James Smith <james@smithjw.me>"]
     description = "A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner."
     license = "BSD-3-Clause"
     name = "autopkg-wrapper"
     readme = "README.md"
     repository = "https://github.com/smithjw/autopkg-wrapper"
-    version = "2024.5.3"
+    version = "2024.5.5"
 
     [tool.poetry.scripts]
         # When built and installed by pip, the command autopkg_wrapper will be availble in to run within that environment
-        autopkg-wrapper = "autopkg_wrapper.autopkg_wrapper:main"
         autopkg_wrapper = "autopkg_wrapper.autopkg_wrapper:main"
 
     [tool.poetry.dependencies]
-        chardet = "5.2.0"
-        idna = "3.7"
-        pygithub = "2.3.0"
+        chardet = ">=5"
+        idna = ">=3"
+        pygithub = ">=2"
         python = "^3.12"
-        requests = "2.31.0"
-        ruamel-yaml = "0.18.6"
-        toml = "0.10.2"
-        urllib3 = "2.2.1"
+        requests = ">=2"
+        ruamel-yaml = ">=0.18"
+        toml = ">=0.10"
+        urllib3 = ">=2"
 
     [tool.poetry_bumpversion.file."autopkg_wrapper/__init__.py"]
 
 [build-system]
     build-backend = "poetry.core.masonry.api"
     requires = ["poetry-core"]
```

### Comparing `autopkg_wrapper-2024.5.3/PKG-INFO` & `autopkg_wrapper-2024.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: autopkg-wrapper
-Version: 2024.5.3
+Version: 2024.5.5
 Summary: A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner.
 Home-page: https://github.com/smithjw/autopkg-wrapper
 License: BSD-3-Clause
 Author: James Smith
 Author-email: james@smithjw.me
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: chardet (==5.2.0)
-Requires-Dist: idna (==3.7)
-Requires-Dist: pygithub (==2.3.0)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: ruamel-yaml (==0.18.6)
-Requires-Dist: toml (==0.10.2)
-Requires-Dist: urllib3 (==2.2.1)
+Requires-Dist: chardet (>=5)
+Requires-Dist: idna (>=3)
+Requires-Dist: pygithub (>=2)
+Requires-Dist: requests (>=2)
+Requires-Dist: ruamel-yaml (>=0.18)
+Requires-Dist: toml (>=0.10)
+Requires-Dist: urllib3 (>=2)
 Project-URL: Repository, https://github.com/smithjw/autopkg-wrapper
 Description-Content-Type: text/markdown
 
 # autopkg-wrapper
 
 `autopkg_wrapper` is a small package that can be used to run [`autopkg`](https://github.com/autopkg/autopkg) within CI/CD environments such as GitHub Actions.
```

