# Comparing `tmp/docopt_sh-2.0.0a4.tar.gz` & `tmp/docopt_sh-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docopt_sh-2.0.0a4.tar", max compression
+gzip compressed data, was "docopt_sh-2.0.1.tar", max compression
```

## Comparing `docopt_sh-2.0.0a4.tar` & `docopt_sh-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/LICENSE
--rw-r--r--   0        0        0      602 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/__init__.py
--rw-r--r--   0        0        0     3590 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/__main__.py
--rw-r--r--   0        0        0     4011 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/bash.py
--rw-r--r--   0        0        0    17767 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/docopt.sh
--rw-r--r--   0        0        0    10651 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/parser.py
--rw-r--r--   0        0        0     9063 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/script.py
--rw-r--r--   0        0        0      221 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docs/README.pypi.md
--rw-r--r--   0        0        0     1219 2024-05-16 12:24:36.376777 docopt_sh-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/LICENSE
+-rw-r--r--   0        0        0      602 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/__main__.py
+-rw-r--r--   0        0        0     4199 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/bash.py
+-rw-r--r--   0        0        0    17767 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/docopt.sh
+-rw-r--r--   0        0        0    10665 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/parser.py
+-rw-r--r--   0        0        0     9183 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docopt_sh/script.py
+-rw-r--r--   0        0        0      221 2024-05-28 18:00:07.221991 docopt_sh-2.0.1/docs/README.pypi.md
+-rw-r--r--   0        0        0     1212 2024-05-28 18:00:17.670017 docopt_sh-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 docopt_sh-2.0.1/PKG-INFO
```

### Comparing `docopt_sh-2.0.0a4/LICENSE` & `docopt_sh-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a4/docopt_sh/__init__.py` & `docopt_sh-2.0.1/docopt_sh/__init__.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a4/docopt_sh/__main__.py` & `docopt_sh-2.0.1/docopt_sh/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import sys
 import os
 import docopt
 import logging
 import termcolor
-from . import __doc__ as pkg_doc, __name__ as root_name, DocoptError, __version__
+from . import __doc__ as pkg_doc, __name__ as root_name, __version__
 from .parser import ParserParameters, Parser, Library
 from .script import Script
 
 log = logging.getLogger(root_name)
 
 __doc__ = pkg_doc + """
 Usage:
@@ -71,17 +71,17 @@
         else:
           with open(params['SCRIPT'], 'w') as h:
             h.write(str(patched_script))
           if patched_script == script:
             log.info('The parser in %s is already up-to-date.', params['SCRIPT'])
           else:
             log.info('%s has been updated.', params['SCRIPT'])
-    except DocoptError as e:
+    except Exception as e:
       log.error(str(e))
-      sys.exit(e.exit_code)
+      sys.exit(getattr(e, 'exit_code', 1))
 
 
 def setup_logging():
   level_colors = {
     logging.ERROR: 'red',
     logging.WARN: 'yellow',
   }
```

### Comparing `docopt_sh-2.0.0a4/docopt_sh/bash.py` & `docopt_sh-2.0.1/docopt_sh/bash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
 from shlex import quote
 from itertools import chain
 
+# WARNING: This code for transforming bash code is built very specifically for
+# the docopt.sh code. It is almost guaranteed to give wrong results when used in
+# any other context.
 
 class Code(object):
 
   def __init__(self, code):
     self.code = self._get_iter(code)
 
   def _get_iter(self, code):
@@ -111,15 +114,15 @@
     yield from re.sub(r"('[^']* [^']*')|( )", r'\1\2\\\n', line).split('\n')
 
 
 def split_sq_strings(lines):
   for line in lines:
     # Split every character in a single quoted string
     yield from re.sub(
-      r"'([^']+)'",
+      r"(?<!\")'([^']+)'",
       lambda sq: ''.join(map(lambda c: f"'{c}'\\\n", sq.group(1))),
       line,
     ).split('\n')
 
 
 def remove_newlines(lines, max_length):
   def get_seperator(line):
```

### Comparing `docopt_sh-2.0.0a4/docopt_sh/docopt.sh` & `docopt_sh-2.0.1/docopt_sh/docopt.sh`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a4/docopt_sh/parser.py` & `docopt_sh-2.0.1/docopt_sh/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     node_sort_order = [P.Option, P.Argument, P.Command, P.ArgumentSeparator]
     nodes = sorted(
       all_nodes,
       key=lambda p: node_sort_order.index(type(p)) if type(p) in node_sort_order else len(node_sort_order)
     )
 
     if self.parameters.library_path:
-      library = indent(f'''source {self.parameters.library_path} '{__version__}' || {{
+      library = indent(f'''local v='{__version__}'; source {self.parameters.library_path} "$v" || {{
   ret=$?
   printf -- "exit %d\\n" "$ret"
   exit "$ret"
 }}''', level=1)
     else:
       exclude = ['docopt', 'lib_version_check'] + list(set(helper_list) - set(map(helper_name, nodes)))
       library = indent(str(self.library.generate_code(exclude=exclude)), level=1)
```

### Comparing `docopt_sh-2.0.0a4/docopt_sh/script.py` & `docopt_sh-2.0.1/docopt_sh/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
       r'^(?:[^#\n]*)'
       r'DOC='
       r'(?P<quote_start>(?<![\\])[\'"])'
       r'(?P<raw_value>'
       r'(?P<trimmed_before>\s*)'
       r'(?P<trimmed_raw_value>(?:.(?!(?<![\\])\1))*?.?)'
       r'(?P<trimmed_after>\s*))'
-      r'(?P<quote_end>\1)(?:\n|;)',
+      r'(?P<quote_end>(?<![\\])\1)(?:\n|;)',
       script.contents,
       re.MULTILINE | re.DOTALL
     )
     super(Doc, self).__init__(script, matches, 0)
     if self.present:
       # Get bash to output what the docstring looks like when evaluated
       output_doc = 'DOC={quote}{trimmed_raw_value}{quote};printf "%s" "$DOC"'.format(
@@ -153,15 +153,18 @@
       process = subprocess.run(
         ['bash', '-c', 'eval "$(cat)"'],
         input=output_doc.encode('utf-8'),
         stdout=subprocess.PIPE, stderr=subprocess.PIPE
       )
       if process.returncode != 0:
         raise DocoptScriptValidationError(
-          self, 'Unable to evaluate DOC= with system bash: %s' % process.stderr.decode('utf-8')
+          self, (
+            f"Unable to evaluate DOC= with system bash: {process.stderr.decode('utf-8')}"
+            + f"The DOC region recognized was:\n{self.match.group(0)}"  # type: ignore
+          )
         )
       self.trimmed_value = process.stdout.decode('utf-8')
       self.trimmed_value_start = self.match.start('trimmed_raw_value') - self.match.end('quote_start')  # type: ignore
       self.untrimmed_value = (
         self.match.group('trimmed_before')  # type: ignore
         + self.trimmed_value
         + self.match.group('trimmed_after')  # type: ignore
```

### Comparing `docopt_sh-2.0.0a4/pyproject.toml` & `docopt_sh-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "docopt-sh"
 description = "Command-line argument parser for bash 3.2, 4+, and 5+."
-version = "v2.0.0-alpha4"
+version = "v2.0.1"
 authors = ["Anders Ingemann <anders@ingemann.de>"]
 license = "MIT"
 readme = "docs/README.pypi.md"
 homepage = "https://github.com/andsens/docopt.sh"
 repository = "https://github.com/andsens/docopt.sh"
 classifiers = [
   "Topic :: Utilities",
@@ -32,15 +32,15 @@
 docopt = "^0.6.2"
 termcolor = "^1.1.0"
 docopt-parser = ">=0.0.1"
 flake8-pyproject = "^1.1.0.post0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
-pytest = "^7.1.1"
+pytest = "^7.2.0"
 pytest-xdist = "^2.5.0"
 pytest-flake8 = "^1.1.1"
 
 [tool.poetry.scripts]
 "docopt.sh" = "docopt_sh.__main__:main"
 
 [build-system]
```

### Comparing `docopt_sh-2.0.0a4/PKG-INFO` & `docopt_sh-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docopt-sh
-Version: 2.0.0a4
+Version: 2.0.1
 Summary: Command-line argument parser for bash 3.2, 4+, and 5+.
 Home-page: https://github.com/andsens/docopt.sh
 License: MIT
 Author: Anders Ingemann
 Author-email: anders@ingemann.de
 Requires-Python: >=3.11.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

