# Comparing `tmp/consoleiotools-4.6.0.tar.gz` & `tmp/consoleiotools-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleiotools-4.6.0.tar", last modified: Tue May 28 08:47:05 2024, max compression
+gzip compressed data, was "consoleiotools-4.6.1.tar", last modified: Tue May 28 09:32:21 2024, max compression
```

## Comparing `consoleiotools-4.6.0.tar` & `consoleiotools-4.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:47:05.589783 consoleiotools-4.6.0/
--rw-rw-rw-   0        0        0     1092 2021-03-17 11:22:04.000000 consoleiotools-4.6.0/LICENSE
--rw-rw-rw-   0        0        0     7835 2024-05-28 08:47:05.587784 consoleiotools-4.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5691 2024-05-28 08:46:07.000000 consoleiotools-4.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 08:47:05.554222 consoleiotools-4.6.0/consoleiotools/
--rw-rw-rw-   0        0        0    11816 2024-05-28 08:40:53.000000 consoleiotools-4.6.0/consoleiotools/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-06-21 03:15:10.000000 consoleiotools-4.6.0/consoleiotools/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:47:05.585783 consoleiotools-4.6.0/consoleiotools.egg-info/
--rw-rw-rw-   0        0        0     7835 2024-05-28 08:47:05.000000 consoleiotools-4.6.0/consoleiotools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-05-28 08:47:05.000000 consoleiotools-4.6.0/consoleiotools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:47:05.000000 consoleiotools-4.6.0/consoleiotools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 08:47:05.000000 consoleiotools-4.6.0/consoleiotools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-28 08:47:05.000000 consoleiotools-4.6.0/consoleiotools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1308 2024-03-16 08:38:13.000000 consoleiotools-4.6.0/pyproject.toml
--rw-rw-rw-   0        0        0        6 2024-03-16 08:36:32.000000 consoleiotools-4.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 08:47:05.589783 consoleiotools-4.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 08:47:05.583783 consoleiotools-4.6.0/tests/
--rw-rw-rw-   0        0        0    13023 2024-05-28 08:45:36.000000 consoleiotools-4.6.0/tests/test_consoleiotools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:32:21.650892 consoleiotools-4.6.1/
+-rw-rw-rw-   0        0        0     1092 2021-03-17 11:22:04.000000 consoleiotools-4.6.1/LICENSE
+-rw-rw-rw-   0        0        0     8213 2024-05-28 09:32:21.649891 consoleiotools-4.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6069 2024-05-28 09:31:51.000000 consoleiotools-4.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:32:21.621129 consoleiotools-4.6.1/consoleiotools/
+-rw-rw-rw-   0        0        0    11923 2024-05-28 09:23:19.000000 consoleiotools-4.6.1/consoleiotools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-06-21 03:15:10.000000 consoleiotools-4.6.1/consoleiotools/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:32:21.648893 consoleiotools-4.6.1/consoleiotools.egg-info/
+-rw-rw-rw-   0        0        0     8213 2024-05-28 09:32:21.000000 consoleiotools-4.6.1/consoleiotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-05-28 09:32:21.000000 consoleiotools-4.6.1/consoleiotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:32:21.000000 consoleiotools-4.6.1/consoleiotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 09:32:21.000000 consoleiotools-4.6.1/consoleiotools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-28 09:32:21.000000 consoleiotools-4.6.1/consoleiotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1308 2024-03-16 08:38:13.000000 consoleiotools-4.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0        6 2024-03-16 08:36:32.000000 consoleiotools-4.6.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:32:21.652404 consoleiotools-4.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 09:32:21.647894 consoleiotools-4.6.1/tests/
+-rw-rw-rw-   0        0        0    13024 2024-05-28 09:24:39.000000 consoleiotools-4.6.1/tests/test_consoleiotools.py
```

### Comparing `consoleiotools-4.6.0/LICENSE` & `consoleiotools-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.0/PKG-INFO` & `consoleiotools-4.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleiotools
-Version: 4.6.0
+Version: 4.6.1
 Summary: Console tools for inputs and outputs in Python
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,20 +74,29 @@
 
 >>> cit.echo("Hello World")
 | Hello World
 
 >>> cit.echo("Hello World", pre="say", bar="!")
 ! (Say) Hello World
 
->>> cit.echo("Hello World", indent=1)  # indent level
+>>> cit.echo("Hello World", indent="+")  # indent, `+` means 1 level of indents
 | +-- Hello World
 
->>> cit.echo("Hello World", indent=-1)  # level < 0 means this is the last line of indents.
+>>> cit.echo("Hello World", indent="-")  # `-` means last line of indents.
 | `-- Hello World
 
+>>> cit.echo("Hello World", indent="+-+-")  # 4 levels of indents
+| |       |   `-- Hello World
+# |   |   |   |   |
+# |   |   |   |   `-- The content
+# |   |   |   `------ The last char `-` in `indent=`
+# |   |   `---------- The 3rd char `+` in `indent=`
+# |   `-------------- The 2nd char `-` in `indent=`
+# `------------------ The 1st char `+` in `indent=`
+
 >>> cit.ask("Hello World")
 | (?) Hello World
 
 >>> cit.info("Hello World")
 | (Info) Hello World
 
 >>> cit.warn("Hello World")
```

### Comparing `consoleiotools-4.6.0/README.md` & `consoleiotools-4.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,29 @@
 
 >>> cit.echo("Hello World")
 | Hello World
 
 >>> cit.echo("Hello World", pre="say", bar="!")
 ! (Say) Hello World
 
->>> cit.echo("Hello World", indent=1)  # indent level
+>>> cit.echo("Hello World", indent="+")  # indent, `+` means 1 level of indents
 | +-- Hello World
 
->>> cit.echo("Hello World", indent=-1)  # level < 0 means this is the last line of indents.
+>>> cit.echo("Hello World", indent="-")  # `-` means last line of indents.
 | `-- Hello World
 
+>>> cit.echo("Hello World", indent="+-+-")  # 4 levels of indents
+| |       |   `-- Hello World
+# |   |   |   |   |
+# |   |   |   |   `-- The content
+# |   |   |   `------ The last char `-` in `indent=`
+# |   |   `---------- The 3rd char `+` in `indent=`
+# |   `-------------- The 2nd char `-` in `indent=`
+# `------------------ The 1st char `+` in `indent=`
+
 >>> cit.ask("Hello World")
 | (?) Hello World
 
 >>> cit.info("Hello World")
 | (Info) Hello World
 
 >>> cit.warn("Hello World")
```

### Comparing `consoleiotools-4.6.0/consoleiotools/__init__.py` & `consoleiotools-4.6.1/consoleiotools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import rich.panel
 import rich.text
 import rich.progress
 import rich.traceback
 import rich.markdown
 import rich.box
 
-__version__ = "4.6.0"
+__version__ = "4.6.1"
 __ascii__ = False
 theme = rich.theme.Theme({
     "echo": "bright_white",
     "echo-bar": "",
     "echo-pre": "dim bright_white",
     "echo-indent": "dim",
     "info": "",
@@ -107,32 +107,32 @@
 
 
 def br(count=1):
     """print 1 to N blank lines"""
     print("\n" * (count - 1))
 
 
-def echo(*args, pre: str = "", bar: str = "|" if __ascii__ else "│", style: str = "echo", indent: int = 0, **options):
+def echo(*args, pre: str = "", bar: str = "|" if __ascii__ else "│", style: str = "echo", indent: str = "", **options):
     txt = rich.text.Text()
     if bar:
         txt.append(f"{bar}", style=f"{style}-bar" if f"{style}-bar" in theme.styles else style)
         txt.append(" ")
     if pre:
         txt.append(f"({pre.capitalize()})", style=f"{style}-pre" if f"{style}-pre" in theme.styles else style)
         txt.append(" ")
     if indent:
-        indent_char = "-" if __ascii__ else "─"
-        if indent < 0:
-            indent = -indent
-            indent_char_start = "`" if __ascii__ else "╰"
-        else:
-            indent_char_start = "+" if __ascii__ else "├"
-        indent_deco = f"{indent_char_start}{indent_char * (indent * 4 - 2)}"
+        indent_char_stem = "|   " if __ascii__ else "│   "
+        indent_char_branch = "+-- " if __ascii__ else "├── "
+        indent_char_leaf = "`-- " if __ascii__ else "╰── "
+        indent_deco = ""
+        for level in indent[:-1]:
+            indent_deco += indent_char_stem if level == "+" else "    "
+        else:  # when success
+            indent_deco += indent_char_branch if indent[-1] == "+" else indent_char_leaf
         txt.append(f"{indent_deco}", style=f"{style}-indent" if f"{style}-indent" in theme.styles else style)
-        txt.append(" ")
     contents = rich.text.Text(" ").join(rich.text.Text.from_markup(f"{arg}") for arg in args)
     contents.stylize(style)
     txt.append(contents)
     console.print(txt, **options)
 
 
 def title(*args, **options):
```

### Comparing `consoleiotools-4.6.0/consoleiotools/__main__.py` & `consoleiotools-4.6.1/consoleiotools/__main__.py`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.0/consoleiotools.egg-info/PKG-INFO` & `consoleiotools-4.6.1/consoleiotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleiotools
-Version: 4.6.0
+Version: 4.6.1
 Summary: Console tools for inputs and outputs in Python
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,20 +74,29 @@
 
 >>> cit.echo("Hello World")
 | Hello World
 
 >>> cit.echo("Hello World", pre="say", bar="!")
 ! (Say) Hello World
 
->>> cit.echo("Hello World", indent=1)  # indent level
+>>> cit.echo("Hello World", indent="+")  # indent, `+` means 1 level of indents
 | +-- Hello World
 
->>> cit.echo("Hello World", indent=-1)  # level < 0 means this is the last line of indents.
+>>> cit.echo("Hello World", indent="-")  # `-` means last line of indents.
 | `-- Hello World
 
+>>> cit.echo("Hello World", indent="+-+-")  # 4 levels of indents
+| |       |   `-- Hello World
+# |   |   |   |   |
+# |   |   |   |   `-- The content
+# |   |   |   `------ The last char `-` in `indent=`
+# |   |   `---------- The 3rd char `+` in `indent=`
+# |   `-------------- The 2nd char `-` in `indent=`
+# `------------------ The 1st char `+` in `indent=`
+
 >>> cit.ask("Hello World")
 | (?) Hello World
 
 >>> cit.info("Hello World")
 | (Info) Hello World
 
 >>> cit.warn("Hello World")
```

### Comparing `consoleiotools-4.6.0/pyproject.toml` & `consoleiotools-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.0/tests/test_consoleiotools.py` & `consoleiotools-4.6.1/tests/test_consoleiotools.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,26 +59,26 @@
     def test_echo_bar(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
             cit.echo("ABC", bar="BAR")
             self.assertEqual(fake_out.getvalue(), "BAR ABC\n")
 
     def test_echo_indent(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC", indent=1)
+            cit.echo("ABC", indent="+")
             self.assertEqual(fake_out.getvalue(), "│ ├── ABC\n")
 
-    def test_echo_indent_level(self):
+    def test_echo_indent_leaf(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC", indent=2)
-            self.assertEqual(fake_out.getvalue(), "│ ├────── ABC\n")
+            cit.echo("ABC", indent="-")
+            self.assertEqual(fake_out.getvalue(), "│ ╰── ABC\n")
 
-    def test_echo_indent_closure(self):
+    def test_echo_indent_stem(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC", indent=-1)
-            self.assertEqual(fake_out.getvalue(), "│ ╰── ABC\n")
+            cit.echo("ABC", indent="+-+")
+            self.assertEqual(fake_out.getvalue(), "│ │       ├── ABC\n")
 
     def test_markdown(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
             cit.markdown("### ABC")
             self.assertEqual(fake_out.getvalue().strip(), "ABC")
 
     def test_panel(self):
```

