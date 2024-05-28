# Comparing `tmp/hardcoded-0.14.13.tar.gz` & `tmp/hardcoded-0.14.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardcoded-0.14.13.tar", max compression
+gzip compressed data, was "hardcoded-0.14.14.tar", max compression
```

## Comparing `hardcoded-0.14.13.tar` & `hardcoded-0.14.14.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1871 2024-04-20 08:58:50.133334 hardcoded-0.14.13/README.md
--rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.13/hardcoded/__init__.py
--rw-r--r--   0        0        0     2755 2024-05-22 07:07:15.294230 hardcoded-0.14.13/hardcoded/cli.py
--rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.13/hardcoded/git.py
--rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.13/hardcoded/logic.py
--rw-r--r--   0        0        0      687 2024-05-22 15:14:00.357138 hardcoded-0.14.13/pyproject.toml
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.14.13/PKG-INFO
+-rw-r--r--   0        0        0     1871 2024-04-20 08:58:50.133334 hardcoded-0.14.14/README.md
+-rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.14/hardcoded/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-28 17:51:08.224633 hardcoded-0.14.14/hardcoded/cli.py
+-rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.14/hardcoded/git.py
+-rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.14/hardcoded/logic.py
+-rw-r--r--   0        0        0      687 2024-05-24 09:57:22.621187 hardcoded-0.14.14/pyproject.toml
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.14.14/PKG-INFO
```

### Comparing `hardcoded-0.14.13/README.md` & `hardcoded-0.14.14/README.md`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.13/hardcoded/__init__.py` & `hardcoded-0.14.14/hardcoded/__init__.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.13/hardcoded/cli.py` & `hardcoded-0.14.14/hardcoded/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
-import yaml
+import re
 
 from hardcoded.logic import File, _debug
 
+import yaml
 import click
 
 
 @click.command()
 @click.option(
     "--encrypt",
     is_flag=True,
@@ -43,38 +44,46 @@
     # if import_file:
     #    click.echo('boo')
     #    exit()
 
     if key:
         click.echo(datafile.get(key), err=False, nl=False)
     else:
-        data = datafile._x._get_all_decrypted_data()
-        data_yaml = yaml.safe_dump(data)
-        edited_data_yaml = data_yaml
-        while True:
-            edited_data_yaml = click.edit(edited_data_yaml)
-            try:
-                if edited_data_yaml is None:
-                    click.echo("Data not changed.", err=True)
-                else:
-                    # Let's fail here if the user messed up the YAML.
-                    edited_data = yaml.safe_load(edited_data_yaml)
-                    datafile._x._set_all_data(edited_data)
-                    click.echo(f"{datafile._x.path} updated.", err=True)
-                break
-            except yaml.YAMLError as ex:
-                if hasattr(ex, "problem_mark"):
-                    mark = ex.problem_mark
-                    click.echo(
-                        f"Error in {datafile._x.path} YAML at {mark.line+1}:{mark.column+1}: {ex}",
-                        err=True,
-                    )
-                else:
-                    click.echo(f"Error in {datafile._x.path} YAML: {ex}", err=True)
-                if not click.confirm(
-                    "Do you want to try again?", default=True, err=True
-                ):
+        stdin_text = click.get_text_stream('stdin')
+        if stdin_text.isatty():
+            # Interactive session: open datafile in an editor.
+            data = datafile._x._get_all_decrypted_data()
+            data_yaml = yaml.safe_dump(data)
+            edited_data_yaml = data_yaml
+            while True:
+                edited_data_yaml = click.edit(edited_data_yaml)
+                try:
+                    if edited_data_yaml is None:
+                        click.echo("Data not changed.", err=True)
+                    else:
+                        # Let's fail here if the user messed up the YAML.
+                        edited_data = yaml.safe_load(edited_data_yaml)
+                        datafile._x._set_all_data(edited_data)
+                        click.echo(f"{datafile._x.path} updated.", err=True)
                     break
+                except yaml.YAMLError as ex:
+                    if hasattr(ex, "problem_mark"):
+                        mark = ex.problem_mark
+                        click.echo(
+                            f"Error in {datafile._x.path} YAML at {mark.line+1}:{mark.column+1}: {ex}",
+                            err=True,
+                        )
+                    else:
+                        click.echo(f"Error in {datafile._x.path} YAML: {ex}", err=True)
+                    if not click.confirm(
+                        "Do you want to try again?", default=True, err=True
+                    ):
+                        break
+        else:
+            # Non-interactive session: replace hardcoded patterns in stdin, send to stdout.
+            text = stdin_text.read()
+            text = re.sub(r'hardcoded[\.\(\'"]+([\w\d]+)[\'"]?\)?', lambda match: datafile.get(match.group(1)), text)
+            click.echo(text, err=False, nl=False)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `hardcoded-0.14.13/hardcoded/git.py` & `hardcoded-0.14.14/hardcoded/git.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.13/hardcoded/logic.py` & `hardcoded-0.14.14/hardcoded/logic.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.13/pyproject.toml` & `hardcoded-0.14.14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardcoded"
-version = "0.14.13"
+version = "0.14.14"
 description = "For everything that you really should not be hardcoding."
 license = "LGPL-3.0-or-later"
 authors = ["moizuo <no_spam@example.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/hardcoded"
 
 [tool.poetry.dependencies]
```

### Comparing `hardcoded-0.14.13/PKG-INFO` & `hardcoded-0.14.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardcoded
-Version: 0.14.13
+Version: 0.14.14
 Summary: For everything that you really should not be hardcoding.
 Home-page: https://pypi.org/project/hardcoded
 License: LGPL-3.0-or-later
 Author: moizuo
 Author-email: no_spam@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

