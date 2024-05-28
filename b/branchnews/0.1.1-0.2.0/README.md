# Comparing `tmp/branchnews-0.1.1.tar.gz` & `tmp/branchnews-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branchnews-0.1.1.tar", last modified: Thu Jan 25 11:20:46 2024, max compression
+gzip compressed data, was "branchnews-0.2.0.tar", last modified: Tue May 28 14:57:05 2024, max compression
```

## Comparing `branchnews-0.1.1.tar` & `branchnews-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-01-25 11:20:46.590757 branchnews-0.1.1/
--rw-r--r--   0 skieffer   (501) staff       (20)     1070 2024-01-18 19:39:07.000000 branchnews-0.1.1/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)     6498 2024-01-25 11:20:46.590683 branchnews-0.1.1/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)     5938 2024-01-25 11:19:30.000000 branchnews-0.1.1/README.md
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-01-25 11:20:46.588954 branchnews-0.1.1/branchnews/
--rw-r--r--   0 skieffer   (501) staff       (20)      210 2024-01-25 11:19:52.000000 branchnews-0.1.1/branchnews/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1607 2024-01-18 18:53:34.000000 branchnews-0.1.1/branchnews/create.py
--rw-r--r--   0 skieffer   (501) staff       (20)     2608 2024-01-18 18:53:34.000000 branchnews-0.1.1/branchnews/rename.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1222 2024-01-18 19:09:20.000000 branchnews-0.1.1/branchnews/util.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-01-25 11:20:46.590205 branchnews-0.1.1/branchnews.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)     6498 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      332 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       46 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/entry_points.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       58 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/requires.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       11 2024-01-25 11:20:46.000000 branchnews-0.1.1/branchnews.egg-info/top_level.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       81 2024-01-18 14:20:57.000000 branchnews-0.1.1/pyproject.toml
--rw-r--r--   0 skieffer   (501) staff       (20)      651 2024-01-25 11:20:46.591039 branchnews-0.1.1/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-05-28 14:57:05.228987 branchnews-0.2.0/
+-rw-r--r--   0 skieffer   (501) staff       (20)     1070 2024-01-18 19:39:07.000000 branchnews-0.2.0/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)     6498 2024-05-28 14:57:05.228916 branchnews-0.2.0/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)     5938 2024-05-28 14:29:50.000000 branchnews-0.2.0/README.md
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-05-28 14:57:05.227196 branchnews-0.2.0/branchnews/
+-rw-r--r--   0 skieffer   (501) staff       (20)      210 2024-05-28 14:45:42.000000 branchnews-0.2.0/branchnews/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2404 2024-05-28 14:29:50.000000 branchnews-0.2.0/branchnews/create.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2608 2024-01-18 18:53:34.000000 branchnews-0.2.0/branchnews/rename.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1222 2024-01-18 19:09:20.000000 branchnews-0.2.0/branchnews/util.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-05-28 14:57:05.228355 branchnews-0.2.0/branchnews.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)     6498 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      332 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       46 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/entry_points.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       58 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       11 2024-05-28 14:57:05.000000 branchnews-0.2.0/branchnews.egg-info/top_level.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2024-01-18 14:20:57.000000 branchnews-0.2.0/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      651 2024-05-28 14:57:05.229252 branchnews-0.2.0/setup.cfg
```

### Comparing `branchnews-0.1.1/LICENSE` & `branchnews-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `branchnews-0.1.1/PKG-INFO` & `branchnews-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchnews
-Version: 0.1.1
+Version: 0.2.0
 Summary: Branch-based fragment file names for towncrier
 Home-page: https://github.com/skieffer/branchnews
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,20 +120,20 @@
 
 A session for which there *is* an associated issue number might look like this:
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 1234
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 3
 Created 1234.added.txt
 Please edit the file to provide a release note.
 ```
 
 (The menu of alternatives for the news *type* is generated directly from your
 `towncrier` config.)
@@ -142,20 +142,20 @@
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 
 GitHub username: example
 Branch name is fix-that-pesky-bug
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 5
 Created example.fix-that-pesky-bug.branchnews.fixed.txt
 Please edit the file to provide a release note.
 ```
 
 After generating the file, the contributor should edit it, recording the desired
 news entry, and then `git commit` the file, before opening a PR.
```

### Comparing `branchnews-0.1.1/README.md` & `branchnews-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,20 @@
 
 A session for which there *is* an associated issue number might look like this:
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 1234
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 3
 Created 1234.added.txt
 Please edit the file to provide a release note.
 ```
 
 (The menu of alternatives for the news *type* is generated directly from your
 `towncrier` config.)
@@ -124,20 +124,20 @@
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 
 GitHub username: example
 Branch name is fix-that-pesky-bug
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 5
 Created example.fix-that-pesky-bug.branchnews.fixed.txt
 Please edit the file to provide a release note.
 ```
 
 After generating the file, the contributor should edit it, recording the desired
 news entry, and then `git commit` the file, before opening a PR.
```

### Comparing `branchnews-0.1.1/branchnews/create.py` & `branchnews-0.2.0/branchnews/create.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+import pathlib
 import subprocess
 
 import click
 
 from .util import get_frag_dir_and_config, percent_encode
 
 
+TEMPLATE = """\
+# Please replace this comment with a release note.
+# - Your note may span multiple lines.
+# - You do NOT need to put a bullet symbol at the start.
+"""
+
 @click.command(name='create')
 def main():
     """
     Create a news fragment.
 
     Enter an issue number, or let the filename be based on your GitHub username and
     the current branch name.
@@ -20,37 +27,55 @@
     issue_num = input("Issue number (leave blank to use branch name instead): ")
 
     if issue_num:
         filename_parts.append(issue_num)
     else:
         username = input("GitHub username: ")
         branch = subprocess.check_output(["git", "branch", "--show-current"]).decode().strip()
+
+        if branch in ['main', 'master']:
+            print(f'\n*** Branch name "{branch}" does not sound like a topic branch! ***')
+            click.confirm(f'Are you sure you want to proceed?', abort=True)
+
         print("Branch name is", branch)
         pct_enc_branch = percent_encode(branch)
         filename_parts.extend([username, pct_enc_branch, 'branchnews'])
 
-    types_lookup = {i: t for i, t in enumerate(config.types)}
+    news_types = [(k, d['name']) for k, d in config.types.items()]
     print('What type of news is it?')
-    for i, t in types_lookup.items():
-        print(f'({i}): {t}')
+    for i, t in enumerate(news_types):
+        print(f'({i}): {t[1]}')
     type_index = input("Type: ")
     try:
         i = int(type_index)
-        news_type = types_lookup[i]
+        news_type = news_types[i][0]
     except (ValueError, KeyError):
         raise click.UsageError('Invalid choice!')
 
     filename_parts.append(news_type)
     filename_parts.append('txt')
 
     filename = '.'.join(filename_parts)
     filepath = fragments_directory / filename
-    template = "# Please replace this line with a release note."
+    if not fragments_directory.exists():
+        fragments_directory.mkdir(parents=True)
     with open(filepath, "w") as f:
-        f.write(template)
+        f.write(TEMPLATE)
 
-    print("Created", filename)
+    try:
+        cwd = pathlib.Path('.').absolute()
+        home = fragments_directory.relative_to(cwd)
+    except ValueError:
+        home = fragments_directory
+
+    print()
+    print(f"Created file:\n  {filename}")
+    print(f"in directory:\n  {home}")
+    print()
     print("Please edit the file to provide a release note.")
+    print("  - Your note may span multiple lines.")
+    print("  - You do NOT need to put a bullet symbol at the start.")
+    print()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `branchnews-0.1.1/branchnews/rename.py` & `branchnews-0.2.0/branchnews/rename.py`

 * *Files identical despite different names*

### Comparing `branchnews-0.1.1/branchnews/util.py` & `branchnews-0.2.0/branchnews/util.py`

 * *Files identical despite different names*

### Comparing `branchnews-0.1.1/branchnews.egg-info/PKG-INFO` & `branchnews-0.2.0/branchnews.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchnews
-Version: 0.1.1
+Version: 0.2.0
 Summary: Branch-based fragment file names for towncrier
 Home-page: https://github.com/skieffer/branchnews
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,20 +120,20 @@
 
 A session for which there *is* an associated issue number might look like this:
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 1234
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 3
 Created 1234.added.txt
 Please edit the file to provide a release note.
 ```
 
 (The menu of alternatives for the news *type* is generated directly from your
 `towncrier` config.)
@@ -142,20 +142,20 @@
 
 ```
 $ branchnews create
 Issue number (leave blank to use branch name instead): 
 GitHub username: example
 Branch name is fix-that-pesky-bug
 What type of news is it?
-(0): security
-(1): removed
-(2): deprecated
-(3): added
-(4): changed
-(5): fixed
+(0): Security
+(1): Removed
+(2): Deprecated
+(3): Added
+(4): Changed
+(5): Fixed
 Type: 5
 Created example.fix-that-pesky-bug.branchnews.fixed.txt
 Please edit the file to provide a release note.
 ```
 
 After generating the file, the contributor should edit it, recording the desired
 news entry, and then `git commit` the file, before opening a PR.
```

### Comparing `branchnews-0.1.1/setup.cfg` & `branchnews-0.2.0/setup.cfg`

 * *Files identical despite different names*

