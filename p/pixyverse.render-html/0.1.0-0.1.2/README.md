# Comparing `tmp/pixyverse_render_html-0.1.0.tar.gz` & `tmp/pixyverse_render_html-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixyverse_render_html-0.1.0.tar", max compression
+gzip compressed data, was "pixyverse_render_html-0.1.2.tar", max compression
```

## Comparing `pixyverse_render_html-0.1.0.tar` & `pixyverse_render_html-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11356 2024-05-20 18:55:43.610313 pixyverse_render_html-0.1.0/LICENSE
--rw-r--r--   0        0        0      267 2024-05-20 18:55:43.610313 pixyverse_render_html-0.1.0/README.md
--rw-r--r--   0        0        0     1794 2024-05-20 18:55:43.614313 pixyverse_render_html-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 18:55:43.614313 pixyverse_render_html-0.1.0/src/pixyverse/render_html/__init__.py
--rw-r--r--   0        0        0      731 2024-05-20 18:55:43.614313 pixyverse_render_html-0.1.0/src/pixyverse/render_html/render.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/LICENSE
+-rw-r--r--   0        0        0      267 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/README.md
+-rw-r--r--   0        0        0     1969 2024-05-28 18:11:07.994989 pixyverse_render_html-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/src/pixyverse/render_html/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-28 18:10:54.682800 pixyverse_render_html-0.1.2/src/pixyverse/render_html/render.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pixyverse_render_html-0.1.2/PKG-INFO
```

### Comparing `pixyverse_render_html-0.1.0/LICENSE` & `pixyverse_render_html-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pixyverse_render_html-0.1.0/pyproject.toml` & `pixyverse_render_html-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -20,25 +20,26 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 license = {file = "LICENSE"}
 keywords = ["templating","web","parser","jsx","html"]
 dependencies = [
-  
+"pixyverse-pixy == ^0.0.8"
 ]
 
 [project.optional-dependencies]
 dev = [
   "build",
   "pre-commit",
   "poetry",
   "black",
   "flake8",
-  "mypy"
+  "mypy",
+  "isort"
 ]
 publish = ["twine"]
 
 
 [tool.black]
 line-length = 88
 target-version = ['py310','py311','py312']
@@ -52,27 +53,32 @@
 [[tool.poetry.source]]
 name = "test-pypi"
 url = "https://test.pypi.org/simple/"
 priority = "explicit"
 
 [tool.poetry]
 name = "pixyverse.render_html"
-version = "0.1.0"
+version = "0.1.2"
 description = "A package to render pixy (.pix) files to HTML"
 authors = ["Pradeep Roark <pradeep.roark@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pixyverse/render_html", from="src/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pixyverse-pixy = "^0.0.6"
+
 
 [tool.poetry.group.dev.dependencies]
+isort = "^5.13.2"
 build = "^1.2.1"
 pre-commit = "^3.7.0"
 black = "^24.3.0"
 flake8 = "^7.0.0"
 mypy = "^1.10.0"
 
+
+[tool.poetry-dynamic-versioning]
+enable = false
+pattern = "rel-(?P<base>\\d.\\d.\\d)"
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pixyverse_render_html-0.1.0/src/pixyverse/render_html/render.py` & `pixyverse_render_html-0.1.2/src/pixyverse/render_html/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 def map_prop_name(name: str):
     if name in safeKeyNames.keys():
         return safeKeyNames[name]
     return name
 
 
-id = lambda x: x
+def id(x):
+    return x
 
 
 def flat_map(f, xs: Iterable):
     ys: List = []
     for x in xs:
         ys.extend(f(x))
     return ys
@@ -25,8 +26,10 @@
 
 def create_element(
     elem: str,
     props: dict[str, str] = {},
     children: Iterable[str] | Iterable[Iterable[str]] = [],
 ):
     render_children = "".join(flat_map(id, children))
-    return f"""<{elem}{''.join(f' {underscoreToHyphen(map_prop_name(key))}={value}' for key, value in props.items())}>{render_children}</{elem}>"""
+    return f"<{elem}\
+{''.join(f' {underscoreToHyphen(map_prop_name(key))}={value}' for key, value in props.items())}>\
+{render_children}</{elem}>"
```

### Comparing `pixyverse_render_html-0.1.0/PKG-INFO` & `pixyverse_render_html-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pixyverse.render_html
-Version: 0.1.0
+Version: 0.1.2
 Summary: A package to render pixy (.pix) files to HTML
 Author: Pradeep Roark
 Author-email: pradeep.roark@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pixyverse-pixy (>=0.0.6,<0.0.7)
 Description-Content-Type: text/markdown
 
 Render-HTML
 --------------
 
 What is Render-HTML
 --------------------
```

