# Comparing `tmp/interlinked-0.3.2.zip` & `tmp/interlinked-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,14 @@
-Zip file size: 11813 bytes, number of entries: 24
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 17:02 interlinked-0.3.2/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 17:02 interlinked-0.3.2/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 17:02 interlinked-0.3.2/interlinked/
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-18 17:02 interlinked-0.3.2/PKG-INFO
--rw-r--r--  2.0 unx      278 b- defN 24-Apr-18 17:00 interlinked-0.3.2/pyproject.toml
--rw-r--r--  2.0 unx     2551 b- defN 23-Jun-19 17:12 interlinked-0.3.2/README.md
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-19 17:12 interlinked-0.3.2/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 17:02 interlinked-0.3.2/setup.cfg
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      433 b- defN 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 17:02 interlinked-0.3.2/interlinked.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      447 b- defN 24-Apr-18 16:50 interlinked-0.3.2/tests/test_mutate.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-19 17:12 interlinked-0.3.2/tests/test_loop.py
--rw-r--r--  2.0 unx     1124 b- defN 24-Apr-18 16:50 interlinked-0.3.2/tests/test_workflow.py
--rw-r--r--  2.0 unx      981 b- defN 24-Apr-18 16:50 interlinked-0.3.2/tests/test_route.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 17:12 interlinked-0.3.2/interlinked/__init__.py
--rw-r--r--  2.0 unx     3854 b- defN 24-Apr-18 17:00 interlinked-0.3.2/interlinked/cli.py
--rw-r--r--  2.0 unx      213 b- defN 23-Jun-19 17:12 interlinked-0.3.2/interlinked/exceptions.py
--rw-r--r--  2.0 unx     8050 b- defN 24-Apr-18 16:50 interlinked-0.3.2/interlinked/workflow.py
--rw-r--r--  2.0 unx     2242 b- defN 24-Apr-18 16:50 interlinked-0.3.2/interlinked/router.py
--rw-r--r--  2.0 unx       71 b- defN 24-Apr-11 16:44 interlinked-0.3.2/interlinked/__main__.py
-24 files, 21900 bytes uncompressed, 8159 bytes compressed:  62.7%
+Zip file size: 9785 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 15:12 interlinked/__init__.py
+-rw-r--r--  2.0 unx       71 b- defN 24-Apr-18 15:50 interlinked/__main__.py
+-rw-r--r--  2.0 unx     3876 b- defN 24-Apr-22 13:33 interlinked/cli.py
+-rw-r--r--  2.0 unx      268 b- defN 24-May-28 12:32 interlinked/exceptions.py
+-rw-r--r--  2.0 unx     1677 b- defN 24-May-16 12:23 interlinked/provider.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-May-28 12:46 interlinked/router.py
+-rw-r--r--  2.0 unx    11737 b- defN 24-May-28 12:41 interlinked/workflow.py
+-rw-r--r--  2.0 unx      132 b- defN 24-May-28 12:55 interlinked-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 12:55 interlinked-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-28 12:55 interlinked-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-28 12:55 interlinked-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      964 b- defN 24-May-28 12:55 interlinked-0.4.0.dist-info/RECORD
+12 files, 22746 bytes uncompressed, 8163 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,73 +1,37 @@
-Filename: interlinked-0.3.2/
+Filename: interlinked/__init__.py
 Comment: 
 
-Filename: interlinked-0.3.2/interlinked.egg-info/
+Filename: interlinked/__main__.py
 Comment: 
 
-Filename: interlinked-0.3.2/tests/
+Filename: interlinked/cli.py
 Comment: 
 
-Filename: interlinked-0.3.2/interlinked/
+Filename: interlinked/exceptions.py
 Comment: 
 
-Filename: interlinked-0.3.2/PKG-INFO
+Filename: interlinked/provider.py
 Comment: 
 
-Filename: interlinked-0.3.2/pyproject.toml
+Filename: interlinked/router.py
 Comment: 
 
-Filename: interlinked-0.3.2/README.md
+Filename: interlinked/workflow.py
 Comment: 
 
-Filename: interlinked-0.3.2/setup.py
+Filename: interlinked-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: interlinked-0.3.2/setup.cfg
+Filename: interlinked-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: interlinked-0.3.2/interlinked.egg-info/PKG-INFO
+Filename: interlinked-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: interlinked-0.3.2/interlinked.egg-info/SOURCES.txt
+Filename: interlinked-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: interlinked-0.3.2/interlinked.egg-info/entry_points.txt
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked.egg-info/top_level.txt
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked.egg-info/dependency_links.txt
-Comment: 
-
-Filename: interlinked-0.3.2/tests/test_mutate.py
-Comment: 
-
-Filename: interlinked-0.3.2/tests/test_loop.py
-Comment: 
-
-Filename: interlinked-0.3.2/tests/test_workflow.py
-Comment: 
-
-Filename: interlinked-0.3.2/tests/test_route.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/__init__.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/cli.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/exceptions.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/workflow.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/router.py
-Comment: 
-
-Filename: interlinked-0.3.2/interlinked/__main__.py
+Filename: interlinked-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `interlinked-0.3.2/interlinked/cli.py` & `interlinked/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,20 @@
     for target in args.targets:
         res = wkf.config(config).run(target)
         if args.show:
             print(res)
 
 
 def load_conf(path):
+    if path is None:
+        return None
+
     if path.endswith(".toml"):
         import toml
+
         return toml.load(path)
     elif path.endswith(".json"):
         return json.load(open(path))
     else:
         raise ValueError("File type not supported (should be json or toml)")
 
 
@@ -93,51 +97,46 @@
 
 def main():
     parser = argparse.ArgumentParser(
         prog="interlinked",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
-        "source", help="ressource to load in the form of file_name (without the .py) "
-        "or file_name:workflow_name",
+        "source",
+        help="ressource to load in the form of 'file_name' (without the .py), 'folder.file'  "
+        "or 'file_name:workflow_variable'",
     )
     parser.add_argument(
         "-v", "--verbose", action="count", default=0, help="Increase verbosity"
     )
     subparsers = parser.add_subparsers(dest="command")
 
-    parser_deps = subparsers.add_parser(
-        "deps", description="Show dependencies")
+    parser_deps = subparsers.add_parser("deps", description="Show dependencies")
     parser_deps.set_defaults(func=deps)
 
-    parser_version = subparsers.add_parser(
-        "version", description="Print version")
+    parser_version = subparsers.add_parser("version", description="Print version")
     parser_version.set_defaults(func=lambda a: print(__version__))
 
-    parser_validate = subparsers.add_parser(
-        "validate", description="Validate Workflow")
+    parser_validate = subparsers.add_parser("validate", description="Validate Workflow")
     parser_validate.add_argument(
-        "-n", "--name", default="default_workflow", help="Workflow name",
+        "-n",
+        "--name",
+        default="default_workflow",
+        help="Workflow name",
     )
     parser_validate.set_defaults(func=validate)
 
-    parser_run = subparsers.add_parser(
-        "run", description="Print run")
-    parser_run.add_argument(
-        "-s", "--show", action="store_true", help="Show output"
-    )
-    parser_run.add_argument(
-        "-c", "--config", help="Load parameters from config"
-    )
-    parser_run.add_argument(
-        "targets", nargs="*", help="Run given targets"
-    )
+    parser_run = subparsers.add_parser("run", description="Print run")
+    parser_run.add_argument("-s", "--show", action="store_true", help="Show output")
+    parser_run.add_argument("-c", "--config", help="Load parameters from config")
+    parser_run.add_argument("targets", nargs="*", help="Run given targets")
     parser_run.set_defaults(func=run_cmd)
 
     args = parser.parse_args()
+
     if args.verbose == 1:
         logger.setLevel("INFO")
     elif args.verbose > 1:
         logger.setLevel("DEBUG")
 
     if not args.command:
         parser.print_help()
```

