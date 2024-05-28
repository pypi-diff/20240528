# Comparing `tmp/pixyverse_render_html-0.1.2.tar.gz` & `tmp/pixyverse_render_html-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixyverse_render_html-0.1.2.tar", max compression
+gzip compressed data, was "pixyverse_render_html-0.1.3.tar", max compression
```

## Comparing `pixyverse_render_html-0.1.2.tar` & `pixyverse_render_html-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11356 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/LICENSE
--rw-r--r--   0        0        0      267 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/README.md
--rw-r--r--   0        0        0     1969 2024-05-28 18:11:07.994989 pixyverse_render_html-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/src/pixyverse/render_html/__init__.py
--rw-r--r--   0        0        0      738 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/src/pixyverse/render_html/render.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/LICENSE
+-rw-r--r--   0        0        0      267 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/README.md
+-rw-r--r--   0        0        0     1969 2024-05-28 19:48:06.079665 pixyverse_render_html-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/src/pixyverse/render_html/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/src/pixyverse/render_html/render.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.3/PKG-INFO
```

### Comparing `pixyverse_render_html-0.1.2/LICENSE` & `pixyverse_render_html-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixyverse_render_html-0.1.2/pyproject.toml` & `pixyverse_render_html-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 license = {file = "LICENSE"}
 keywords = ["templating","web","parser","jsx","html"]
 dependencies = [
-"pixyverse-pixy == ^0.0.8"
+
 ]
 
 [project.optional-dependencies]
 dev = [
   "build",
   "pre-commit",
   "poetry",
@@ -53,22 +53,23 @@
 [[tool.poetry.source]]
 name = "test-pypi"
 url = "https://test.pypi.org/simple/"
 priority = "explicit"
 
 [tool.poetry]
 name = "pixyverse.render_html"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package to render pixy (.pix) files to HTML"
 authors = ["Pradeep Roark <pradeep.roark@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pixyverse/render_html", from="src/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+pixyverse-pixy = "^0.0.8"
 
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.13.2"
 build = "^1.2.1"
 pre-commit = "^3.7.0"
 black = "^24.3.0"
```

### Comparing `pixyverse_render_html-0.1.2/src/pixyverse/render_html/render.py` & `pixyverse_render_html-0.1.3/src/pixyverse/render_html/render.py`

 * *Files identical despite different names*

### Comparing `pixyverse_render_html-0.1.2/PKG-INFO` & `pixyverse_render_html-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pixyverse.render_html
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to render pixy (.pix) files to HTML
 Author: Pradeep Roark
 Author-email: pradeep.roark@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pixyverse-pixy (>=0.0.8,<0.0.9)
 Description-Content-Type: text/markdown
 
 Render-HTML
 --------------
 
 What is Render-HTML
 --------------------
```

