# Comparing `tmp/hardcoded-0.14.14.tar.gz` & `tmp/hardcoded-0.14.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardcoded-0.14.14.tar", max compression
+gzip compressed data, was "hardcoded-0.14.16.tar", max compression
```

## Comparing `hardcoded-0.14.14.tar` & `hardcoded-0.14.16.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1871 2024-04-20 08:58:50.133334 hardcoded-0.14.14/README.md
--rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.14/hardcoded/__init__.py
--rw-r--r--   0        0        0     3331 2024-05-28 17:51:08.224633 hardcoded-0.14.14/hardcoded/cli.py
--rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.14/hardcoded/git.py
--rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.14/hardcoded/logic.py
--rw-r--r--   0        0        0      687 2024-05-24 09:57:22.621187 hardcoded-0.14.14/pyproject.toml
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.14.14/PKG-INFO
+-rw-r--r--   0        0        0     1871 2024-05-28 19:57:09.065958 hardcoded-0.14.16/README.md
+-rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.16/hardcoded/__init__.py
+-rw-r--r--   0        0        0     3394 2024-05-28 19:37:43.326688 hardcoded-0.14.16/hardcoded/cli.py
+-rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.16/hardcoded/git.py
+-rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.16/hardcoded/logic.py
+-rw-r--r--   0        0        0      692 2024-05-28 20:01:23.865062 hardcoded-0.14.16/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 hardcoded-0.14.16/PKG-INFO
```

### Comparing `hardcoded-0.14.14/README.md` & `hardcoded-0.14.16/README.md`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.14/hardcoded/__init__.py` & `hardcoded-0.14.16/hardcoded/__init__.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.14/hardcoded/cli.py` & `hardcoded-0.14.16/hardcoded/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # if import_file:
     #    click.echo('boo')
     #    exit()
 
     if key:
         click.echo(datafile.get(key), err=False, nl=False)
     else:
-        stdin_text = click.get_text_stream('stdin')
+        stdin_text = click.get_text_stream("stdin")
         if stdin_text.isatty():
             # Interactive session: open datafile in an editor.
             data = datafile._x._get_all_decrypted_data()
             data_yaml = yaml.safe_dump(data)
             edited_data_yaml = data_yaml
             while True:
                 edited_data_yaml = click.edit(edited_data_yaml)
@@ -77,13 +77,17 @@
                     if not click.confirm(
                         "Do you want to try again?", default=True, err=True
                     ):
                         break
         else:
             # Non-interactive session: replace hardcoded patterns in stdin, send to stdout.
             text = stdin_text.read()
-            text = re.sub(r'hardcoded[\.\(\'"]+([\w\d]+)[\'"]?\)?', lambda match: datafile.get(match.group(1)), text)
+            text = re.sub(
+                r'hardcoded[\.\(\'"]+([\w\d]+)[\'"]?\)?',
+                lambda match: datafile.get(match.group(1)),
+                text,
+            )
             click.echo(text, err=False, nl=False)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `hardcoded-0.14.14/hardcoded/git.py` & `hardcoded-0.14.16/hardcoded/git.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.14/hardcoded/logic.py` & `hardcoded-0.14.16/hardcoded/logic.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.14/pyproject.toml` & `hardcoded-0.14.16/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "hardcoded"
-version = "0.14.14"
+version = "0.14.16"
 description = "For everything that you really should not be hardcoding."
 license = "LGPL-3.0-or-later"
 authors = ["moizuo <no_spam@example.com>"]
 readme = "README.md"
-homepage = "https://pypi.org/project/hardcoded"
+homepage = "https://gitlab.com/zeroconfig/hardcoded"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.8"
 Click = "^8.0.1"
 pyyaml = "*"
 python-gnupg = "*"
```

### Comparing `hardcoded-0.14.14/PKG-INFO` & `hardcoded-0.14.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hardcoded
-Version: 0.14.14
+Version: 0.14.16
 Summary: For everything that you really should not be hardcoding.
-Home-page: https://pypi.org/project/hardcoded
+Home-page: https://gitlab.com/zeroconfig/hardcoded
 License: LGPL-3.0-or-later
 Author: moizuo
 Author-email: no_spam@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

