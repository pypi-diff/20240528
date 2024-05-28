# Comparing `tmp/wizlib-3.1.0.tar.gz` & `tmp/wizlib-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-3.1.0.tar", max compression
+gzip compressed data, was "wizlib-3.1.1.tar", max compression
```

## Comparing `wizlib-3.1.0.tar` & `wizlib-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1094 2024-05-20 16:26:57.317283 wizlib-3.1.0/README.md
--rw-r--r--   0        0        0      698 2024-05-20 16:27:09.054272 wizlib-3.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 16:26:57.410283 wizlib-3.1.0/wizlib/__init__.py
--rw-r--r--   0        0        0     3350 2024-05-20 16:26:57.355283 wizlib-3.1.0/wizlib/app.py
--rw-r--r--   0        0        0     4506 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/class_family.py
--rw-r--r--   0        0        0     1708 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/command.py
--rw-r--r--   0        0        0     2588 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/config_handler.py
--rw-r--r--   0        0        0       46 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/error.py
--rw-r--r--   0        0        0      446 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/handler.py
--rw-r--r--   0        0        0     1505 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/parser.py
--rw-r--r--   0        0        0      663 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/stream_handler.py
--rw-r--r--   0        0        0      272 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/super_wrapper.py
--rw-r--r--   0        0        0     4241 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/__init__.py
--rw-r--r--   0        0        0      943 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell/__init__.py
--rw-r--r--   0        0        0     7419 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell/line_editor.py
--rw-r--r--   0        0        0     2029 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell_ui.py
--rw-r--r--   0        0        0      634 2024-05-20 16:26:57.357283 wizlib-3.1.0/wizlib/ui_handler.py
--rw-r--r--   0        0        0      156 2024-05-20 16:26:57.357283 wizlib-3.1.0/wizlib/util.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-28 01:48:35.641901 wizlib-3.1.1/README.md
+-rw-r--r--   0        0        0      698 2024-05-28 01:48:47.229882 wizlib-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 01:48:35.734901 wizlib-3.1.1/wizlib/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-28 01:48:35.679901 wizlib-3.1.1/wizlib/app.py
+-rw-r--r--   0        0        0     4506 2024-05-28 01:48:35.679901 wizlib-3.1.1/wizlib/class_family.py
+-rw-r--r--   0        0        0     1708 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/command.py
+-rw-r--r--   0        0        0     2588 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/config_handler.py
+-rw-r--r--   0        0        0       46 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/error.py
+-rw-r--r--   0        0        0      446 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/handler.py
+-rw-r--r--   0        0        0     1550 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/parser.py
+-rw-r--r--   0        0        0      663 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/stream_handler.py
+-rw-r--r--   0        0        0      272 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/super_wrapper.py
+-rw-r--r--   0        0        0     4241 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/ui/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/ui/shell/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/ui/shell/line_editor.py
+-rw-r--r--   0        0        0     2029 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/ui/shell_ui.py
+-rw-r--r--   0        0        0      634 2024-05-28 01:48:35.680901 wizlib-3.1.1/wizlib/ui_handler.py
+-rw-r--r--   0        0        0      156 2024-05-28 01:48:35.681901 wizlib-3.1.1/wizlib/util.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.1.1/PKG-INFO
```

### Comparing `wizlib-3.1.0/README.md` & `wizlib-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/pyproject.toml` & `wizlib-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizlib"
-version = "3.1.0"
+version = "3.1.1"
 description = "Framework for flexible and powerful command-line applications"
 authors = ["Steampunk Wizard <wizlib@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `wizlib-3.1.0/wizlib/app.py` & `wizlib-3.1.1/wizlib/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from argparse import ArgumentError
 import sys
 from dataclasses import dataclass
 import os
 from pathlib import Path
 
 from wizlib.class_family import ClassFamily
 from wizlib.command import WizHelpCommand
 from wizlib.super_wrapper import SuperWrapper
-from wizlib.parser import WizParser
+from wizlib.parser import WizArgumentError, WizParser
 from wizlib.ui import UI
 
 
 RED = '\033[91m'
 RESET = '\033[0m'
 
 
@@ -40,15 +41,20 @@
         cls.start(*sys.argv[1:], debug=os.getenv('DEBUG'))
 
     @classmethod
     def start(cls, *args, debug=False):
         """Call this from a Python entrypoint"""
         try:
             cls.initialize()
-            ns = cls.parser.parse_args(args)
+            try:
+                ns = cls.parser.parse_args(args)
+                if (ns.command is None) and (not hasattr(ns, 'help')):
+                    ns = cls.dparser.parse_args(args)
+            except ArgumentError as e:
+                ns = cls.dparser.parse_args(args)
             app = cls(**vars(ns))
             app.run(**vars(ns))
         except AppCancellation as cancellation:
             if str(cancellation):
                 print(str(cancellation), file=sys.stderr)
         except BaseException as error:
             if debug:
@@ -59,22 +65,25 @@
                       f"{error}{RESET}", file=sys.stderr)
                 sys.exit(1)
 
     @classmethod
     def initialize(cls):
         """Set up the parser for the app class"""
         cls.parser = WizParser(prog=cls.name)
-        for handler in cls.handlers:
-            handler.add_args(cls.parser)
         subparsers = cls.parser.add_subparsers(dest='command')
         for command in cls.base.family_members('name'):
             key = command.get_member_attr('key')
             aliases = [key] if key else []
             subparser = subparsers.add_parser(command.name, aliases=aliases)
+            if command.name == cls.base.default:
+                cls.dparser = subparser
             command.add_args(subparser)
+        for handler in cls.handlers:
+            handler.add_args(cls.parser)
+            handler.add_args(cls.dparser)
 
     def __init__(self, **vals):
         """Create the app. Only interested in the handlers from the parsed
         values passed in"""
         for hcls in self.handlers:
             val = vals[hcls.name] if (hcls.name in vals) else hcls.default
             handler = hcls.setup(val)
@@ -82,20 +91,21 @@
             setattr(self, hcls.name, handler)
 
     def run(self, **vals):
         """Perform a command. May be called more than once. Only interested in
         the command itself and its specific arguments from the values passed
         in."""
         if 'help' in vals:
-            return WizHelpCommand(**vals)
-        c = 'command'
-        cname = (vals.pop(c) if c in vals else None) or self.base.default
-        ccls = self.base.family_member('name', cname)
-        if not ccls:
-            raise Exception(f"Unknown command {cname}")
+            ccls = WizHelpCommand
+        else:
+            c = 'command'
+            cname = (vals.pop(c) if c in vals else None) or self.base.default
+            ccls = self.base.family_member('name', cname)
+            if not ccls:
+                raise Exception(f"Unknown command {cname}")
         command = ccls(self, **vals)
         result = command.execute()
         if result:
             print(result, end='')
             if sys.stdout.isatty():  # pragma: nocover
                 print()
         if command.status:
```

### Comparing `wizlib-3.1.0/wizlib/class_family.py` & `wizlib-3.1.1/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/command.py` & `wizlib-3.1.1/wizlib/command.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/config_handler.py` & `wizlib-3.1.1/wizlib/config_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/parser.py` & `wizlib-3.1.1/wizlib/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from argparse import SUPPRESS
 from contextlib import redirect_stdout
 from io import StringIO
 import sys
 import os
 
 
+# We found the help process a little clumsy
+
 class WizHelpAction(Action):
 
     def __init__(self,
                  option_strings,
                  dest=SUPPRESS,
                  default=SUPPRESS,
                  help=None):
```

### Comparing `wizlib-3.1.0/wizlib/stream_handler.py` & `wizlib-3.1.1/wizlib/stream_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/ui/__init__.py` & `wizlib-3.1.1/wizlib/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/ui/shell/__init__.py` & `wizlib-3.1.1/wizlib/ui/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/ui/shell/line_editor.py` & `wizlib-3.1.1/wizlib/ui/shell/line_editor.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/ui/shell_ui.py` & `wizlib-3.1.1/wizlib/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/wizlib/ui_handler.py` & `wizlib-3.1.1/wizlib/ui_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.1.0/PKG-INFO` & `wizlib-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Framework for flexible and powerful command-line applications
 License: MIT
 Author: Steampunk Wizard
 Author-email: wizlib@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

