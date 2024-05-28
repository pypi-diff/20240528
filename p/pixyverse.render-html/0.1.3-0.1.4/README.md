# Comparing `tmp/pixyverse_render_html-0.1.3.tar.gz` & `tmp/pixyverse_render_html-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixyverse_render_html-0.1.3.tar", max compression
+gzip compressed data, was "pixyverse_render_html-0.1.4.tar", max compression
```

## Comparing `pixyverse_render_html-0.1.3.tar` & `pixyverse_render_html-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11356 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/LICENSE
--rw-r--r--   0        0        0      267 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/README.md
--rw-r--r--   0        0        0     1969 2024-05-28 19:48:06.079665 pixyverse_render_html-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/src/pixyverse/render_html/__init__.py
--rw-r--r--   0        0        0      738 2024-05-28 19:48:01.827647 pixyverse_render_html-0.1.3/src/pixyverse/render_html/render.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-28 20:24:42.544237 pixyverse_render_html-0.1.4/LICENSE
+-rw-r--r--   0        0        0      267 2024-05-28 20:24:42.544237 pixyverse_render_html-0.1.4/README.md
+-rw-r--r--   0        0        0     1969 2024-05-28 20:24:52.028298 pixyverse_render_html-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 20:24:42.544237 pixyverse_render_html-0.1.4/src/pixyverse/render_html/__init__.py
+-rw-r--r--   0        0        0      854 2024-05-28 20:24:42.548237 pixyverse_render_html-0.1.4/src/pixyverse/render_html/render.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.4/PKG-INFO
```

### Comparing `pixyverse_render_html-0.1.3/LICENSE` & `pixyverse_render_html-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixyverse_render_html-0.1.3/pyproject.toml` & `pixyverse_render_html-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 [[tool.poetry.source]]
 name = "test-pypi"
 url = "https://test.pypi.org/simple/"
 priority = "explicit"
 
 [tool.poetry]
 name = "pixyverse.render_html"
-version = "0.1.3"
+version = "0.1.4"
 description = "A package to render pixy (.pix) files to HTML"
 authors = ["Pradeep Roark <pradeep.roark@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pixyverse/render_html", from="src/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pixyverse_render_html-0.1.3/PKG-INFO` & `pixyverse_render_html-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixyverse.render_html
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to render pixy (.pix) files to HTML
 Author: Pradeep Roark
 Author-email: pradeep.roark@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

