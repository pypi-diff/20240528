# Comparing `tmp/vrocky_gitignore_parser-0.1.11.tar.gz` & `tmp/vrocky_gitignore_parser-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrocky_gitignore_parser-0.1.11.tar", last modified: Mon May 27 04:38:06 2024, max compression
+gzip compressed data, was "vrocky_gitignore_parser-0.1.12.tar", last modified: Tue May 28 18:05:02 2024, max compression
```

## Comparing `vrocky_gitignore_parser-0.1.11.tar` & `vrocky_gitignore_parser-0.1.12.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 04:38:06.594343 vrocky_gitignore_parser-0.1.11/
--rw-rw-rw-   0        0        0     1125 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.11/LICENSE
--rw-rw-rw-   0        0        0     1347 2024-05-27 04:38:06.593337 vrocky_gitignore_parser-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.11/README.md
--rw-rw-rw-   0        0        0     6901 2024-05-27 04:31:44.000000 vrocky_gitignore_parser-0.1.11/gitignore_parser.py
--rw-rw-rw-   0        0        0       84 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.11/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-27 04:38:06.598842 vrocky_gitignore_parser-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0     1562 2024-05-27 04:34:50.000000 vrocky_gitignore_parser-0.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:38:06.593337 vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/
--rw-rw-rw-   0        0        0     1347 2024-05-27 04:38:06.000000 vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-27 04:38:06.000000 vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 04:38:06.000000 vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 04:38:06.000000 vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 18:05:02.631911 vrocky_gitignore_parser-0.1.12/
+-rw-rw-rw-   0        0        0     1125 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.12/LICENSE
+-rw-rw-rw-   0        0        0     1347 2024-05-28 18:05:02.631390 vrocky_gitignore_parser-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1404 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.12/README.md
+-rw-rw-rw-   0        0        0     8085 2024-05-27 11:49:37.000000 vrocky_gitignore_parser-0.1.12/gitignore_parser.py
+-rw-rw-rw-   0        0        0       84 2024-05-27 04:16:55.000000 vrocky_gitignore_parser-0.1.12/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-28 18:05:02.632914 vrocky_gitignore_parser-0.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1562 2024-05-28 18:03:28.000000 vrocky_gitignore_parser-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:05:02.630387 vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/
+-rw-rw-rw-   0        0        0     1347 2024-05-28 18:05:02.000000 vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-28 18:05:02.000000 vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 18:05:02.000000 vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 18:05:02.000000 vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/top_level.txt
```

### Comparing `vrocky_gitignore_parser-0.1.11/LICENSE` & `vrocky_gitignore_parser-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `vrocky_gitignore_parser-0.1.11/PKG-INFO` & `vrocky_gitignore_parser-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrocky_gitignore_parser
-Version: 0.1.11
+Version: 0.1.12
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
 Keywords: gitignore
 Platform: MacOS
```

### Comparing `vrocky_gitignore_parser-0.1.11/README.md` & `vrocky_gitignore_parser-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `vrocky_gitignore_parser-0.1.11/gitignore_parser.py` & `vrocky_gitignore_parser-0.1.12/gitignore_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import collections
+import logging
 import os
 import re
 
 from os.path import abspath, dirname
 from pathlib import Path
 from typing import Reversible, Union
 
+
 def handle_negation(file_path, rules: Reversible["IgnoreRule"]):
     for rule in reversed(rules):
         if rule.match(file_path):
             return not rule.negation
     return False
 
+
 def parse_gitignore(full_path, base_dir=None):
     if base_dir is None:
         base_dir = dirname(full_path)
     rules = []
     with open(full_path) as ignore_file:
         counter = 0
         for line in ignore_file:
@@ -28,14 +31,15 @@
     if not any(r.negation for r in rules):
         return lambda file_path: any(r.match(file_path) for r in rules)
     else:
         # We have negation rules. We can't use a simple "any" to evaluate them.
         # Later rules override earlier rules.
         return lambda file_path: handle_negation(file_path, rules)
 
+
 def rule_from_pattern(pattern, base_path=None, source=None):
     """
     Take a .gitignore match pattern, such as "*.py[cod]" or "**/*.bak",
     and return an IgnoreRule suitable for matching against files and
     directories. Patterns which do not match files, such as comments
     and blank lines, will return None.
     Because git allows for nested .gitignore files, a base_path value
@@ -76,19 +80,19 @@
     if pattern[-1] == '/':
         pattern = pattern[:-1]
     # patterns with leading hashes or exclamation marks are escaped with a
     # backslash in front, unescape it
     if pattern[0] == '\\' and pattern[1] in ('#', '!'):
         pattern = pattern[1:]
     # trailing spaces are ignored unless they are escaped with a backslash
-    i = len(pattern)-1
+    i = len(pattern) - 1
     striptrailingspaces = True
     while i > 1 and pattern[i] == ' ':
-        if pattern[i-1] == '\\':
-            pattern = pattern[:i-1] + pattern[i:]
+        if pattern[i - 1] == '\\':
+            pattern = pattern[:i - 1] + pattern[i:]
             i = i - 1
             striptrailingspaces = False
         else:
             if striptrailingspaces:
                 pattern = pattern[:i]
         i = i - 1
     regex = fnmatch_pathname_to_regex(
@@ -110,87 +114,116 @@
     'negation', 'directory_only', 'anchored',  # Behavior flags
     'base_path',  # Meaningful for gitignore-style behavior
     'source'  # (file, line) tuple for reporting
 ]
 
 
 class IgnoreRule(collections.namedtuple('IgnoreRule_', IGNORE_RULE_FIELDS)):
-    def __str__(self):
-        return self.pattern
-
-    def __repr__(self):
-        return ''.join(['IgnoreRule(\'', self.pattern, '\')'])
-
     def match(self, abs_path: Union[str, Path]):
         matched = False
         if self.base_path:
-            rel_path = str(_normalize_path(abs_path).relative_to(self.base_path))
+            normalized_path = _normalize_path(abs_path)
+            # Check if the path is actually a subpath to avoid ValueError
+            if str(normalized_path).startswith(str(self.base_path)):
+                rel_path = str(normalized_path.relative_to(self.base_path))
+            else:
+                # Handle the case where it's not a subpath
+                # You might want to log this or handle it in another way
+                logging.debug(f"Path {normalized_path} is not a subpath of {self.base_path}.")
+                return False
         else:
             rel_path = str(_normalize_path(abs_path))
-        # Path() strips the trailing slash, so we need to preserve it
-        # in case of directory-only negation
+
+        # Further processing...
         if self.negation and type(abs_path) == str and abs_path[-1] == '/':
             rel_path += '/'
         if rel_path.startswith('./'):
             rel_path = rel_path[2:]
         if re.search(self.regex, rel_path):
             matched = True
         return matched
 
 
 # Frustratingly, python's fnmatch doesn't provide the FNM_PATHNAME
 # option that .gitignore's behavior depends on.
-def fnmatch_pathname_to_regex(pattern, directory_only: bool, negation: bool, anchored: bool = False):
-    # Handle both Unix and Windows file separators
-    sep_group = '[/\\\\]'  # Regex group for both '/' and '\'
-    non_sep = '[^/\\\\]'  # Match anything except '/' and '\'
+def fnmatch_pathname_to_regex(
+        pattern, directory_only: bool, negation: bool, anchored: bool = False
+):
+    """
+    Implements fnmatch style-behavior, as though with FNM_PATHNAME flagged;
+    the path separator will not match shell-style '*' and '.' wildcards.
+    """
+    i, n = 0, len(pattern)
+
+    seps = [re.escape(os.sep)]
+    if os.altsep is not None:
+        seps.append(re.escape(os.altsep))
+    seps_group = '[' + '|'.join(seps) + ']'
+    nonsep = r'[^{}]'.format('|'.join(seps))
 
     res = []
-    i, n = 0, len(pattern)
     while i < n:
         c = pattern[i]
         i += 1
         if c == '*':
-            if i < n and pattern[i] == '*':
-                i += 1
-                if i < n and pattern[i] in {'/', '\\'}:
+            try:
+                if pattern[i] == '*':
                     i += 1
-                    res.append(''.join(['(.*', sep_group, ')?']))
+                    if i < n and pattern[i] == '/':
+                        i += 1
+                        res.append(''.join(['(.*', seps_group, ')?']))
+                    else:
+                        res.append('.*')
                 else:
-                    res.append('.*')
-            else:
-                res.append(''.join([non_sep, '*']))
+                    res.append(''.join([nonsep, '*']))
+            except IndexError:
+                res.append(''.join([nonsep, '*']))
         elif c == '?':
-            res.append(non_sep)
-        elif c in {'/', '\\'}:
-            res.append(sep_group)
+            res.append(nonsep)
+        elif c == '/':
+            res.append(seps_group)
         elif c == '[':
-            # Handle character classes
-            ...
+            j = i
+            if j < n and pattern[j] == '!':
+                j += 1
+            if j < n and pattern[j] == ']':
+                j += 1
+            while j < n and pattern[j] != ']':
+                j += 1
+            if j >= n:
+                res.append('\\[')
+            else:
+                stuff = pattern[i:j].replace('\\', '\\\\').replace('/', '')
+                i = j + 1
+                if stuff[0] == '!':
+                    stuff = ''.join(['^', stuff[1:]])
+                elif stuff[0] == '^':
+                    stuff = ''.join('\\' + stuff)
+                res.append('[{}]'.format(stuff))
         else:
             res.append(re.escape(c))
-
-    # Apply anchors
     if anchored:
         res.insert(0, '^')
     else:
-        res.insert(0, f"(^|{sep_group})")
-
-    # Adjust end match based on directory_only and negation
+        res.insert(0, f"(^|{seps_group})")
     if not directory_only:
         res.append('$')
     elif directory_only and negation:
-        res.append(f'{sep_group}$')
+        res.append('/$')
     else:
-        res.append(f'($|{sep_group})')
-
+        res.append('($|\\/)')
     return ''.join(res)
 
 
+def to_unix_style(path):
+    return str(path).replace('\\', '/')
+
+
 def _normalize_path(path: Union[str, Path]) -> Path:
     """Normalize a path without resolving symlinks.
 
     This is equivalent to `Path.resolve()` except that it does not resolve symlinks.
     Note that this simplifies paths by removing double slashes, `..`, `.` etc. like
     `Path.resolve()` does.
     """
-    return Path(abspath(path))
+    path = Path(to_unix_style(path)).resolve(strict=False)
+    return path
```

### Comparing `vrocky_gitignore_parser-0.1.11/setup.py` & `vrocky_gitignore_parser-0.1.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from setuptools import setup
 
 description = 'A spec-compliant gitignore parser for Python 3.5+'
 setup(
     name='vrocky_gitignore_parser',
-    version='0.1.11',
+    version='0.1.12',
     description=description,
     long_description=
         description + '\n\nhttps://github.com/mherrmann/gitignore_parser',
     author='Michael Herrmann',
     author_email='michael+removethisifyouarehuman@herrmann.io',
     url='https://github.com/mherrmann/gitignore_parser',
     py_modules=['gitignore_parser'],
```

### Comparing `vrocky_gitignore_parser-0.1.11/vrocky_gitignore_parser.egg-info/PKG-INFO` & `vrocky_gitignore_parser-0.1.12/vrocky_gitignore_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrocky_gitignore_parser
-Version: 0.1.11
+Version: 0.1.12
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
 Keywords: gitignore
 Platform: MacOS
```

