# Comparing `tmp/sphinxawesome_theme-5.1.4.tar.gz` & `tmp/sphinxawesome_theme-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.1.4.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.1.5.tar", max compression
```

## Comparing `sphinxawesome_theme-5.1.4.tar` & `sphinxawesome_theme-5.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2024-04-23 15:22:40.387702 sphinxawesome_theme-5.1.4/LICENSE
--rw-r--r--   0        0        0     2294 2024-04-23 15:22:40.387702 sphinxawesome_theme-5.1.4/README.md
--rw-r--r--   0        0        0     2682 2024-04-23 15:22:40.391702 sphinxawesome_theme-5.1.4/pyproject.toml
--rw-r--r--   0        0        0     7311 2024-04-23 15:22:40.391702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     4166 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     1394 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2841 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/genindex.html
--rw-r--r--   0        0        0     7675 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12751 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1013 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1192 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5135 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3242 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7816 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      932 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1226 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    21956 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
--rw-r--r--   0        0        0    30184 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
--rw-r--r--   0        0        0    21088 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
--rw-r--r--   0        0        0    28620 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
--rw-r--r--   0        0        0    23072 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
--rw-r--r--   0        0        0    23148 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
--rw-r--r--   0        0        0    30232 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
--rw-r--r--   0        0        0    29416 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
--rw-r--r--   0        0        0    28636 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
--rw-r--r--   0        0        0    22188 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
--rw-r--r--   0        0        0    21820 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
--rw-r--r--   0        0        0     4495 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.css
--rw-r--r--   0        0        0        0 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.js
--rw-r--r--   0        0        0     1338 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.css
--rw-r--r--   0        0        0        0 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.js
--rw-r--r--   0        0        0    27896 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
--rw-r--r--   0        0        0    49637 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.css
--rw-r--r--   0        0        0    56143 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js
--rw-r--r--   0        0        0       93 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      353 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2369 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-28 07:43:51.780524 sphinxawesome_theme-5.1.5/LICENSE
+-rw-r--r--   0        0        0     2294 2024-05-28 07:43:51.780524 sphinxawesome_theme-5.1.5/README.md
+-rw-r--r--   0        0        0     2770 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7311 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     4166 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     1394 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2841 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/genindex.html
+-rw-r--r--   0        0        0     7675 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12745 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1013 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1192 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5135 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3242 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7816 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      932 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1226 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    21956 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
+-rw-r--r--   0        0        0    30184 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
+-rw-r--r--   0        0        0    21088 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
+-rw-r--r--   0        0        0    28620 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
+-rw-r--r--   0        0        0    23072 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
+-rw-r--r--   0        0        0    23148 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
+-rw-r--r--   0        0        0    30232 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
+-rw-r--r--   0        0        0    29416 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
+-rw-r--r--   0        0        0    28636 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
+-rw-r--r--   0        0        0    22188 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
+-rw-r--r--   0        0        0    21820 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
+-rw-r--r--   0        0        0     4495 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.css
+-rw-r--r--   0        0        0        0 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.js
+-rw-r--r--   0        0        0     1338 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.css
+-rw-r--r--   0        0        0        0 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.js
+-rw-r--r--   0        0        0    27896 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
+-rw-r--r--   0        0        0    49637 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.css
+-rw-r--r--   0        0        0    56408 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js
+-rw-r--r--   0        0        0       93 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      353 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2369 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.5/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.1.4/LICENSE` & `sphinxawesome_theme-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/README.md` & `sphinxawesome_theme-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/pyproject.toml` & `sphinxawesome_theme-5.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.1.4"
+version = "5.1.5"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -19,42 +19,45 @@
 packages = [
   { include = "sphinxawesome_theme", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = [
-  { version = "<7.2", python = ">=3.8,<3.9"},
-  { version = "^7.2,<7.3", python = ">=3.9,<3.13"},
+  { version = "<7.2", python = ">=3.8,<3.9" },
+  { version = "^7.2,<7.4", python = ">=3.9,<3.13" },
 ]
 beautifulsoup4 = "^4.9.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = [
-  { version = "^2021", python = ">=3.8,<3.9"},
-  { version = "^2024.2.4", python = ">=3.9,<=3.12"},
+  { version = "^2021", python = ">=3.8,<3.9" },
+  { version = "^2024.2.4", python = ">=3.9,<3.13" },
 ]
 sphinx-sitemap = "^2.2.0"
-sphinx-design = ">=0.4.1,<0.6.0"
-sphinx-docsearch = "^0.0.4"
+sphinx-design = [
+  { version = "^0.5.0", python = ">=3.8,<3.9" },
+  { version = "^0.6.0", python = ">=3.9,<3.13" },
+]
+sphinx-docsearch = "^0.0.6"
 python-dotenv = ">=0.19,<1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8"
 pytest-cov = ">=4,<6"
 coverage = { extras = ["toml"], version = "^7.2" }
-types-docutils = ">=0.19.1.6,<0.21.0.0"
+types-docutils = ">=0.19.1.6,<0.22.0.0"
 mypy = "^1.0"
 
 [tool.poetry.group.lint.dependencies]
 pre-commit = [
   { version = "^3.5", python = ">=3.8,<3.9"},
-  { version = "^3.6", python = ">=3.9,<=3.12"},
+  { version = "^3.6", python = ">=3.9,<3.13"},
 ]
-ruff = ">=0.0.269,<0.4.2"
+ruff = ">=0.0.269,<0.4.6"
 
 [tool.poetry.group.netlify.dependencies]
 nox = {version = ">=2023.4.22,<2025.0.0", python = "3.8"}
 poetry = {version = "^1.4.2", python = "3.8"}
 pipx = {version = "^1.2.0", python = "3.8"}
 pip = {version = ">=23.1.2,<25.0.0", python = "3.8"}
```

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/deprecated.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/genindex.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/highlighting.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,19 +162,19 @@
 
         In contrast to Pygments, use ``<mark>``, ``<ins>``, and ``<del>`` elements.
         """
         for i, (t, value) in enumerate(tokensource):
             if t != 1:
                 yield t, value
             if i + 1 in self.hl_lines:
-                yield 1, "<mark>%s</mark>" % value
+                yield 1, f"<mark>{value}</mark>"
             elif i + 1 in self.added_lines:
-                yield 1, "<ins>%s</ins>" % value
+                yield 1, f"<ins>{value}</ins>"
             elif i + 1 in self.removed_lines:
-                yield 1, "<del>%s</del>" % value
+                yield 1, f"<del>{value}</del>"
             else:
                 yield 1, value
 
     def format_unencoded(
         self: AwesomeHtmlFormatter,
         tokensource: TokenStream,
         outfile: Any,
```

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/logos.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.css` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.css` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.css` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -75,21 +75,21 @@
 
                                     function y(e, t) {
                                         return y = Object.setPrototypeOf || function(e, t) {
                                             return e.__proto__ = t, e
                                         }, y(e, t)
                                     }
 
-                                    function v(e) {
-                                        return v = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                                    function m(e) {
+                                        return m = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                                             return e.__proto__ || Object.getPrototypeOf(e)
-                                        }, v(e)
+                                        }, m(e)
                                     }
 
-                                    function m(e, t) {
+                                    function v(e, t) {
                                         var n = "data-clipboard-".concat(e);
                                         if (t.hasAttribute(n)) return t.getAttribute(n)
                                     }
                                     var g = function(e) {
                                             ! function(e, t) {
                                                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                                                 e.prototype = Object.create(t && t.prototype, {
@@ -106,17 +106,17 @@
                                                 if ("function" == typeof Proxy) return !0;
                                                 try {
                                                     return Date.prototype.toString.call(Reflect.construct(Date, [], (function() {}))), !0
                                                 } catch (e) {
                                                     return !1
                                                 }
                                             }(), function() {
-                                                var e, t, n = v(i);
+                                                var e, t, n = m(i);
                                                 if (o) {
-                                                    var r = v(this).constructor;
+                                                    var r = m(this).constructor;
                                                     e = Reflect.construct(n, arguments, r)
                                                 } else e = n.apply(this, arguments);
                                                 return !(t = e) || "object" !== _(t) && "function" != typeof t ? function(e) {
                                                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                                     return e
                                                 }(this) : t
                                             });
@@ -178,26 +178,26 @@
                                                             t && t.focus(), window.getSelection().removeAllRanges()
                                                         }
                                                     })
                                                 }
                                             }, {
                                                 key: "defaultAction",
                                                 value: function(e) {
-                                                    return m("action", e)
+                                                    return v("action", e)
                                                 }
                                             }, {
                                                 key: "defaultTarget",
                                                 value: function(e) {
-                                                    var t = m("target", e);
+                                                    var t = v("target", e);
                                                     if (t) return document.querySelector(t)
                                                 }
                                             }, {
                                                 key: "defaultText",
                                                 value: function(e) {
-                                                    return m("text", e)
+                                                    return v("text", e)
                                                 }
                                             }, {
                                                 key: "destroy",
                                                 value: function() {
                                                     this.listener.destroy()
                                                 }
                                             }], r = [{
@@ -461,65 +461,65 @@
                         let i = e();
                         JSON.stringify(i), r ? n = i : queueMicrotask((() => {
                             t(i, n), n = i
                         })), r = !1
                     }));
                 return () => a(i)
             }
-            var v = [],
-                m = [],
+            var m = [],
+                v = [],
                 g = [];
 
             function x(e, t) {
-                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, m.push(t))
+                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, v.push(t))
             }
 
             function b(e) {
-                v.push(e)
+                m.push(e)
             }
 
             function w(e, t, n) {
                 e._x_attributeCleanups || (e._x_attributeCleanups = {}), e._x_attributeCleanups[t] || (e._x_attributeCleanups[t] = []), e._x_attributeCleanups[t].push(n)
             }
 
             function E(e, t) {
                 e._x_attributeCleanups && Object.entries(e._x_attributeCleanups).forEach((([n, r]) => {
                     (void 0 === t || t.includes(n)) && (r.forEach((e => e())), delete e._x_attributeCleanups[n])
                 }))
             }
             var S = new MutationObserver(L),
                 A = !1;
 
-            function O() {
+            function k() {
                 S.observe(document, {
                     subtree: !0,
                     childList: !0,
                     attributes: !0,
                     attributeOldValue: !0
                 }), A = !0
             }
 
-            function k() {
+            function O() {
                 ! function() {
                     let e = S.takeRecords();
                     j.push((() => e.length > 0 && L(e)));
                     let t = j.length;
                     queueMicrotask((() => {
                         if (j.length === t)
                             for (; j.length > 0;) j.shift()()
                     }))
                 }(), S.disconnect(), A = !1
             }
             var j = [];
 
             function C(e) {
                 if (!A) return e();
-                k();
+                O();
                 let t = e();
-                return O(), t
+                return k(), t
             }
             var T = !1,
                 $ = [];
 
             function L(e) {
                 if (T) return void($ = $.concat(e));
                 let t = new Set,
@@ -540,17 +540,17 @@
                             l = () => {
                                 i.has(t) || i.set(t, []), i.get(t).push(n)
                             };
                         t.hasAttribute(n) && null === a ? s() : t.hasAttribute(n) ? (l(), s()) : l()
                     } i.forEach(((e, t) => {
                     E(t, e)
                 })), r.forEach(((e, t) => {
-                    v.forEach((n => n(t, e)))
+                    m.forEach((n => n(t, e)))
                 }));
-                for (let e of n) t.has(e) || m.forEach((t => t(e)));
+                for (let e of n) t.has(e) || v.forEach((t => t(e)));
                 t.forEach((e => {
                     e._x_ignoreSelf = !0, e._x_ignore = !0
                 }));
                 for (let e of t) n.has(e) || e.isConnected && (delete e._x_ignoreSelf, delete e._x_ignore, g.forEach((t => t(e))), e._x_ignore = !0, e._x_ignoreSelf = !0);
                 t.forEach((e => {
                     delete e._x_ignoreSelf, delete e._x_ignore
                 })), t = null, n = null, r = null, i = null
@@ -772,16 +772,16 @@
             }
             var re = {};
 
             function ie(e, t) {
                 return re[e] = t, {
                     before(t) {
                         if (!re[t]) return void console.warn(String.raw`Cannot find directive \`${t}\`. \`${e}\` will use the default order of execution`);
-                        const n = me.indexOf(t);
-                        me.splice(n >= 0 ? n : me.indexOf("DEFAULT"), 0, e)
+                        const n = ve.indexOf(t);
+                        ve.splice(n >= 0 ? n : ve.indexOf("DEFAULT"), 0, e)
                     }
                 }
             }
 
             function oe(e, t, n) {
                 if (t = Array.from(t), e._x_virtualDirectives) {
                     let n = Object.entries(e._x_virtualDirectives).map((([e, t]) => ({
@@ -888,21 +888,21 @@
 
             function he({
                 name: e
             }) {
                 return ye().test(e)
             }
             var ye = () => new RegExp(`^${te}([^:^.]+)\\b`),
-                ve = "DEFAULT",
-                me = ["ignore", "ref", "data", "id", "anchor", "bind", "init", "for", "model", "modelable", "transition", "show", "if", ve, "teleport"];
+                me = "DEFAULT",
+                ve = ["ignore", "ref", "data", "id", "anchor", "bind", "init", "for", "model", "modelable", "transition", "show", "if", me, "teleport"];
 
             function ge(e, t) {
-                let n = -1 === me.indexOf(e.type) ? ve : e.type,
-                    r = -1 === me.indexOf(t.type) ? ve : t.type;
-                return me.indexOf(n) - me.indexOf(r)
+                let n = -1 === ve.indexOf(e.type) ? me : e.type,
+                    r = -1 === ve.indexOf(t.type) ? me : t.type;
+                return ve.indexOf(n) - ve.indexOf(r)
             }
 
             function xe(e, t, n = {}) {
                 e.dispatchEvent(new CustomEvent(t, {
                     detail: n,
                     bubbles: !0,
                     composed: !0,
@@ -921,33 +921,33 @@
             function we(e, ...t) {
                 console.warn(`Alpine Warning: ${e}`, ...t)
             }
             var Ee = !1,
                 Se = [],
                 Ae = [];
 
-            function Oe() {
+            function ke() {
                 return Se.map((e => e()))
             }
 
-            function ke() {
+            function Oe() {
                 return Se.concat(Ae).map((e => e()))
             }
 
             function je(e) {
                 Se.push(e)
             }
 
             function Ce(e) {
                 Ae.push(e)
             }
 
             function Te(e, t = !1) {
                 return $e(e, (e => {
-                    if ((t ? ke() : Oe()).some((t => e.matches(t)))) return !0
+                    if ((t ? Oe() : ke()).some((t => e.matches(t)))) return !0
                 }))
             }
 
             function $e(e, t) {
                 if (e) {
                     if (t(e)) return e;
                     if (e._x_teleportBack && (e = e._x_teleportBack), e.parentElement) return $e(e.parentElement, t)
@@ -1223,15 +1223,15 @@
                     e._x_transition.out((() => {}), (() => t(r))), e._x_transitioning && e._x_transitioning.beforeCancel((() => n({
                         isFromCancelledTransition: !0
                     })))
                 })) : Promise.resolve(r), queueMicrotask((() => {
                     let t = We(e);
                     t ? (t._x_hideChildren || (t._x_hideChildren = []), t._x_hideChildren.push(e)) : i((() => {
                         let t = e => {
-                            let n = Promise.all([e._x_hidePromise, ...(e._x_hideChildren || []).map(t)]).then((([e]) => e()));
+                            let n = Promise.all([e._x_hidePromise, ...(e._x_hideChildren || []).map(t)]).then((([e]) => e?.()));
                             return delete e._x_hidePromise, delete e._x_hideChildren, n
                         };
                         t(e).catch((e => {
                             if (!e.isFromCancelledTransition) throw e
                         }))
                     }))
                 })))
@@ -1400,24 +1400,24 @@
                     },
                     get effect() {
                         return o
                     },
                     get raw() {
                         return s
                     },
-                    version: "3.13.9",
+                    version: "3.14.0",
                     flushAndStopDeferringMutations: function() {
                         T = !1, L($), $ = []
                     },
                     dontAutoEvaluateFunctions: Z,
                     disableEffectScheduling: function(e) {
                         _ = !1, e(), _ = !0
                     },
-                    startObservingMutations: O,
-                    stopObservingMutations: k,
+                    startObservingMutations: k,
+                    stopObservingMutations: O,
                     setReactivityEngine: function(e) {
                         i = e.reactive, a = e.release, o = t => e.effect(t, {
                             scheduler: e => {
                                 _ ? function(e) {
                                     var t;
                                     t = e, u.includes(t) || u.push(t), c || l || (l = !0, queueMicrotask(p))
                                 }(e) : e()
@@ -1480,17 +1480,17 @@
                     magic: H,
                     store: function(e, t) {
                         if (ut || (ct = i(ct), ut = !0), void 0 === t) return ct[e];
                         ct[e] = t, "object" == typeof t && null !== t && t.hasOwnProperty("init") && "function" == typeof t.init && ct[e].init(), D(ct[e])
                     },
                     start: function() {
                         var e;
-                        Ee && we("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), Ee = !0, document.body || we("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), xe(document, "alpine:init"), xe(document, "alpine:initializing"), O(), e = e => Me(e, be), g.push(e), x((e => Ne(e))), b(((e, t) => {
+                        Ee && we("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), Ee = !0, document.body || we("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), xe(document, "alpine:init"), xe(document, "alpine:initializing"), k(), e = e => Me(e, be), g.push(e), x((e => Ne(e))), b(((e, t) => {
                             oe(e, t).forEach((e => e()))
-                        })), Array.from(document.querySelectorAll(ke().join(","))).filter((e => !Te(e.parentElement, !0))).forEach((e => {
+                        })), Array.from(document.querySelectorAll(Oe().join(","))).filter((e => !Te(e.parentElement, !0))).forEach((e => {
                             Me(e)
                         })), xe(document, "alpine:initialized"), setTimeout((() => {
                             [
                                 ["ui", "dialog", ["[x-dialog], [x-popover]"]],
                                 ["anchor", "anchor", ["[x-anchor]"]],
                                 ["sort", "sort", ["[x-sort]"]]
                             ].forEach((([e, t, n]) => {
@@ -1504,15 +1504,15 @@
                     clone: function(e, t) {
                         t._x_dataStack || (t._x_dataStack = e._x_dataStack), Ke = !0, Ye = !0, Ge((() => {
                             ! function(e) {
                                 let t = !1;
                                 Me(e, ((e, n) => {
                                     be(e, ((e, r) => {
                                         if (t && function(e) {
-                                                return Oe().some((t => e.matches(t)))
+                                                return ke().some((t => e.matches(t)))
                                             }(e)) return r();
                                         t = !0, n(e, r)
                                     }))
                                 }))
                             }(t)
                         })), Ke = !1, Ye = !1
                     },
@@ -1540,25 +1540,25 @@
 
             function ht(e, t) {
                 const n = Object.create(null),
                     r = e.split(",");
                 for (let e = 0; e < r.length; e++) n[r[e]] = !0;
                 return t ? e => !!n[e.toLowerCase()] : e => !!n[e]
             }
-            var yt, vt = Object.freeze({}),
-                mt = (Object.freeze([]), Object.prototype.hasOwnProperty),
-                gt = (e, t) => mt.call(e, t),
+            var yt, mt = Object.freeze({}),
+                vt = (Object.freeze([]), Object.prototype.hasOwnProperty),
+                gt = (e, t) => vt.call(e, t),
                 xt = Array.isArray,
                 bt = e => "[object Map]" === At(e),
                 wt = e => "symbol" == typeof e,
                 Et = e => null !== e && "object" == typeof e,
                 St = Object.prototype.toString,
                 At = e => St.call(e),
-                Ot = e => At(e).slice(8, -1),
-                kt = e => "string" == typeof e && "NaN" !== e && "-" !== e[0] && "" + parseInt(e, 10) === e,
+                kt = e => At(e).slice(8, -1),
+                Ot = e => "string" == typeof e && "NaN" !== e && "-" !== e[0] && "" + parseInt(e, 10) === e,
                 jt = e => {
                     const t = Object.create(null);
                     return n => t[n] || (t[n] = e(n))
                 },
                 Ct = /-(\w)/g,
                 Tt = (jt((e => e.replace(Ct, ((e, t) => t ? t.toUpperCase() : "")))), /\B([A-Z])/g),
                 $t = (jt((e => e.replace(Tt, "-$1").toLowerCase())), jt((e => e.charAt(0).toUpperCase() + e.slice(1)))),
@@ -1610,15 +1610,15 @@
                     };
                 if ("clear" === t) a.forEach(l);
                 else if ("length" === n && xt(e)) a.forEach(((e, t) => {
                     ("length" === t || t >= r) && l(e)
                 }));
                 else switch (void 0 !== n && l(a.get(n)), t) {
                     case "add":
-                        xt(e) ? kt(n) && l(a.get("length")) : (l(a.get(Pt)), bt(e) && l(a.get(Rt)));
+                        xt(e) ? Ot(n) && l(a.get("length")) : (l(a.get(Pt)), bt(e) && l(a.get(Rt)));
                         break;
                     case "delete":
                         xt(e) || (l(a.get(Pt)), bt(e) && l(a.get(Rt)));
                         break;
                     case "set":
                         bt(e) && l(a.get(Pt))
                 }
@@ -1658,27 +1658,27 @@
                 })), e
             }
 
             function Xt(e = !1, t = !1) {
                 return function(n, r, i) {
                     if ("__v_isReactive" === r) return !e;
                     if ("__v_isReadonly" === r) return e;
-                    if ("__v_raw" === r && i === (e ? t ? kn : On : t ? An : Sn).get(n)) return n;
+                    if ("__v_raw" === r && i === (e ? t ? On : kn : t ? An : Sn).get(n)) return n;
                     const o = xt(n);
                     if (!e && o && gt(Zt, r)) return Reflect.get(Zt, r, i);
                     const a = Reflect.get(n, r, i);
-                    return (wt(r) ? Vt.has(r) : Wt(r)) ? a : (e || Ft(n, "get", r), t ? a : Ln(a) ? o && kt(r) ? a : a.value : Et(a) ? e ? Cn(a) : jn(a) : a)
+                    return (wt(r) ? Vt.has(r) : Wt(r)) ? a : (e || Ft(n, "get", r), t ? a : Ln(a) ? o && Ot(r) ? a : a.value : Et(a) ? e ? Cn(a) : jn(a) : a)
                 }
             }
 
             function Yt(e = !1) {
                 return function(t, n, r, i) {
                     let o = t[n];
                     if (!e && (r = $n(r), o = $n(o), !xt(t) && Ln(o) && !Ln(r))) return o.value = r, !0;
-                    const a = xt(t) && kt(n) ? Number(n) < t.length : gt(t, n),
+                    const a = xt(t) && Ot(n) ? Number(n) < t.length : gt(t, n),
                         s = Reflect.set(t, n, r, i);
                     return t === $n(i) && (a ? Lt(r, o) && Ht(t, "set", n, r, o) : Ht(t, "add", n, r)), s
                 }
             }
             var Gt = {
                     get: Ut,
                     set: Yt(),
@@ -1882,45 +1882,45 @@
                         clear: _n("clear"),
                         forEach: dn(!0, !0)
                     };
                 return ["keys", "values", "entries", Symbol.iterator].forEach((i => {
                     e[i] = pn(i, !1, !1), n[i] = pn(i, !0, !1), t[i] = pn(i, !1, !0), r[i] = pn(i, !0, !0)
                 })), [e, n, t, r]
             }
-            var [yn, vn, mn, gn] = hn();
+            var [yn, mn, vn, gn] = hn();
 
             function xn(e, t) {
-                const n = t ? e ? gn : mn : e ? vn : yn;
+                const n = t ? e ? gn : vn : e ? mn : yn;
                 return (t, r, i) => "__v_isReactive" === r ? !e : "__v_isReadonly" === r ? e : "__v_raw" === r ? t : Reflect.get(gt(n, r) && r in t ? n : t, r, i)
             }
             var bn = {
                     get: xn(!1, !1)
                 },
                 wn = {
                     get: xn(!0, !1)
                 };
 
             function En(e, t, n) {
                 const r = $n(n);
                 if (r !== n && t.call(e, r)) {
-                    const t = Ot(e);
+                    const t = kt(e);
                     console.warn(`Reactive ${t} contains both the raw and reactive versions of the same object${"Map"===t?" as keys":""}, which can lead to inconsistencies. Avoid differentiating between the raw and reactive versions of an object and only use the reactive version if possible.`)
                 }
             }
             var Sn = new WeakMap,
                 An = new WeakMap,
-                On = new WeakMap,
-                kn = new WeakMap;
+                kn = new WeakMap,
+                On = new WeakMap;
 
             function jn(e) {
                 return e && e.__v_isReadonly ? e : Tn(e, !1, Gt, bn, Sn)
             }
 
             function Cn(e) {
-                return Tn(e, !0, Qt, wn, On)
+                return Tn(e, !0, Qt, wn, kn)
             }
 
             function Tn(e, t, n, r, i) {
                 if (!Et(e)) return console.warn(`value cannot be made reactive: ${String(e)}`), e;
                 if (e.__v_raw && (!t || !e.__v_isReactive)) return e;
                 const o = i.get(e);
                 if (o) return o;
@@ -1933,15 +1933,15 @@
                         case "Set":
                         case "WeakMap":
                         case "WeakSet":
                             return 2;
                         default:
                             return 0
                     }
-                }(Ot(s));
+                }(kt(s));
                 var s;
                 if (0 === a) return e;
                 const l = new Proxy(e, 2 === a ? r : n);
                 return i.set(e, l), l
             }
 
             function $n(e) {
@@ -2051,15 +2051,17 @@
                         t.stopPropagation(), e.dispatchEvent(new t.constructor(t.type, t))
                     }))
                 })), N(o, {}, e);
                 let a = (e, t, n) => {
                     n.includes("prepend") ? t.parentNode.insertBefore(e, t) : n.includes("append") ? t.parentNode.insertBefore(e, t.nextSibling) : t.appendChild(e)
                 };
                 C((() => {
-                    a(o, i, t), Me(o), o._x_ignore = !0
+                    a(o, i, t), Ze((() => {
+                        Me(o), o._x_ignore = !0
+                    }))()
                 })), e._x_teleportPutBack = () => {
                     let r = qn(n);
                     C((() => {
                         a(e._x_teleport, r, t)
                     }))
                 }, r((() => o.remove()))
             }));
@@ -2092,42 +2094,50 @@
                     t.stopPropagation(), e(t)
                 }))), n.includes("once") && (o = s(o, ((e, n) => {
                     e(n), i.removeEventListener(t, o, a)
                 }))), (n.includes("away") || n.includes("outside")) && (i = document, o = s(o, ((t, n) => {
                     e.contains(n.target) || !1 !== n.target.isConnected && (e.offsetWidth < 1 && e.offsetHeight < 1 || !1 !== e._x_isShown && t(n))
                 }))), n.includes("self") && (o = s(o, ((t, n) => {
                     n.target === e && t(n)
-                }))), o = s(o, ((e, r) => {
-                    (function(e) {
-                        return ["keydown", "keyup"].includes(e)
-                    })(t) && function(e, t) {
-                        let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture"].includes(e)));
+                }))), (function(e) {
+                    return ["keydown", "keyup"].includes(e)
+                }(t) || Bn(t)) && (o = s(o, ((e, t) => {
+                    (function(e, t) {
+                        let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture", "self", "away", "outside", "passive"].includes(e)));
                         if (n.includes("debounce")) {
                             let e = n.indexOf("debounce");
                             n.splice(e, zn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
                         }
                         if (n.includes("throttle")) {
                             let e = n.indexOf("throttle");
                             n.splice(e, zn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
                         }
                         if (0 === n.length) return !1;
-                        if (1 === n.length && Bn(e.key).includes(n[0])) return !1;
+                        if (1 === n.length && Fn(e.key).includes(n[0])) return !1;
                         const r = ["ctrl", "shift", "alt", "meta", "cmd", "super"].filter((e => n.includes(e)));
-                        return n = n.filter((e => !r.includes(e))), !(r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length && Bn(e.key).includes(n[0]))
-                    }(r, n) || e(r)
-                })), i.addEventListener(t, o, a), () => {
+                        if (n = n.filter((e => !r.includes(e))), r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length) {
+                            if (Bn(e.type)) return !1;
+                            if (Fn(e.key).includes(n[0])) return !1
+                        }
+                        return !0
+                    })(t, n) || e(t)
+                }))), i.addEventListener(t, o, a), () => {
                     i.removeEventListener(t, o, a)
                 }
             }
 
             function zn(e) {
                 return !Array.isArray(e) && !isNaN(e)
             }
 
             function Bn(e) {
+                return ["contextmenu", "click", "mouse"].some((t => e.includes(t)))
+            }
+
+            function Fn(e) {
                 if (!e) return [];
                 var t;
                 e = [" ", "_"].includes(t = e) ? t : t.replace(/([a-z])([A-Z])/g, "$1-$2").replace(/[_\s]/, "-").toLowerCase();
                 let n = {
                     ctrl: "control",
                     slash: "/",
                     space: " ",
@@ -2135,48 +2145,49 @@
                     cmd: "meta",
                     esc: "escape",
                     up: "arrow-up",
                     down: "arrow-down",
                     left: "arrow-left",
                     right: "arrow-right",
                     period: ".",
+                    comma: ",",
                     equal: "=",
                     minus: "-",
                     underscore: "_"
                 };
                 return n[e] = e, Object.keys(n).map((t => {
                     if (n[t] === e) return t
                 })).filter((e => e))
             }
 
-            function Fn(e, t, n, r) {
+            function Hn(e, t, n, r) {
                 return C((() => {
                     if (n instanceof CustomEvent && void 0 !== n.detail) return null !== n.detail && void 0 !== n.detail ? n.detail : n.target.value;
                     if ("checkbox" === e.type) {
                         if (Array.isArray(r)) {
                             let e = null;
-                            return e = t.includes("number") ? Hn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : n.target.value, n.target.checked ? r.concat([e]) : r.filter((t => !(t == e)))
+                            return e = t.includes("number") ? Wn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : n.target.value, n.target.checked ? r.includes(e) ? r : r.concat([e]) : r.filter((t => !(t == e)))
                         }
                         return n.target.checked
                     }
-                    if ("select" === e.tagName.toLowerCase() && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map((e => Hn(e.value || e.text))) : t.includes("boolean") ? Array.from(n.target.selectedOptions).map((e => nt(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text));
+                    if ("select" === e.tagName.toLowerCase() && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map((e => Wn(e.value || e.text))) : t.includes("boolean") ? Array.from(n.target.selectedOptions).map((e => nt(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text));
                     {
                         let i;
-                        return i = "radio" === e.type ? n.target.checked ? n.target.value : r : n.target.value, t.includes("number") ? Hn(i) : t.includes("boolean") ? nt(i) : t.includes("trim") ? i.trim() : i
+                        return i = "radio" === e.type ? n.target.checked ? n.target.value : r : n.target.value, t.includes("number") ? Wn(i) : t.includes("boolean") ? nt(i) : t.includes("trim") ? i.trim() : i
                     }
                 }))
             }
 
-            function Hn(e) {
+            function Wn(e) {
                 let t = e ? parseFloat(e) : null;
                 return n = t, Array.isArray(n) || isNaN(n) ? e : t;
                 var n
             }
 
-            function Wn(e) {
+            function Vn(e) {
                 return null !== e && "object" == typeof e && "function" == typeof e.get && "function" == typeof e.set
             }
             In.inline = (e, {
                 modifiers: t
             }, {
                 cleanup: n
             }) => {
@@ -2198,38 +2209,40 @@
             }) => {
                 let o = e;
                 t.includes("parent") && (o = e.parentNode);
                 let a, s = X(o, n);
                 a = "string" == typeof n ? X(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? X(o, `${n()} = __placeholder`) : () => {};
                 let l = () => {
                         let e;
-                        return s((t => e = t)), Wn(e) ? e.get() : e
+                        return s((t => e = t)), Vn(e) ? e.get() : e
                     },
                     c = e => {
                         let t;
-                        s((e => t = e)), Wn(t) ? t.set(e) : a((() => {}), {
+                        s((e => t = e)), Vn(t) ? t.set(e) : a((() => {}), {
                             scope: {
                                 __placeholder: e
                             }
                         })
                     };
                 "string" == typeof n && "radio" === e.type && C((() => {
                     e.hasAttribute("name") || e.setAttribute("name", n)
                 }));
                 var u = "select" === e.tagName.toLowerCase() || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
                 let f = Ke ? () => {} : Dn(e, u, t, (n => {
-                    c(Fn(e, t, n, l()))
+                    c(Hn(e, t, n, l()))
                 }));
-                if (t.includes("fill") && ([void 0, null, ""].includes(l()) || "checkbox" === e.type && Array.isArray(l())) && c(Fn(e, t, {
+                if (t.includes("fill") && ([void 0, null, ""].includes(l()) || "checkbox" === e.type && Array.isArray(l()) || "select" === e.tagName.toLowerCase() && e.multiple) && c(Hn(e, t, {
                         target: e
                     }, l())), e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = f, i((() => e._x_removeModelListeners.default())), e.form) {
-                    let t = Dn(e.form, "reset", [], (t => {
-                        qe((() => e._x_model && e._x_model.set(e.value)))
+                    let n = Dn(e.form, "reset", [], (n => {
+                        qe((() => e._x_model && e._x_model.set(Hn(e, t, {
+                            target: e
+                        }, l()))))
                     }));
-                    i((() => t()))
+                    i((() => n()))
                 }
                 e._x_model = {
                     get() {
                         return l()
                     },
                     set(e) {
                         c(e)
@@ -2269,15 +2282,15 @@
                     i((t => {
                         C((() => {
                             e.innerHTML = t, e._x_ignoreSelf = !0, Me(e), delete e._x_ignoreSelf
                         }))
                     }))
                 }))
             })), _e(fe(":", ne("bind:")));
-            var Vn = (e, {
+            var Un = (e, {
                 value: t,
                 modifiers: n,
                 expression: r,
                 original: i
             }, {
                 effect: o,
                 cleanup: a
@@ -2305,38 +2318,38 @@
                 o((() => l((i => {
                     void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), C((() => Qe(e, t, i, n)))
                 })))), a((() => {
                     e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedStyles && e._x_undoAddedStyles()
                 }))
             };
 
-            function Un(e, t, n, r) {
+            function Kn(e, t, n, r) {
                 let i = {};
                 return /^\[.*\]$/.test(e.item) && Array.isArray(t) ? e.item.replace("[", "").replace("]", "").split(",").map((e => e.trim())).forEach(((e, n) => {
                     i[e] = t[n]
                 })) : /^\{.*\}$/.test(e.item) && !Array.isArray(t) && "object" == typeof t ? e.item.replace("{", "").replace("}", "").split(",").map((e => e.trim())).forEach((e => {
                     i[e] = t[e]
                 })) : i[e.item] = t, e.index && (i[e.index] = n), e.collection && (i[e.collection] = r), i
             }
 
-            function Kn() {}
+            function Zn() {}
 
-            function Zn(e, t, n) {
+            function Jn(e, t, n) {
                 ie(t, (r => we(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
             }
-            Vn.inline = (e, {
+            Un.inline = (e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }) => {
                 t && (e._x_inlineBindings || (e._x_inlineBindings = {}), e._x_inlineBindings[t] = {
                     expression: r,
                     extract: !1
                 })
-            }, ie("bind", Vn), je((() => `[${ne("data")}]`)), ie("data", ((e, {
+            }, ie("bind", Un), je((() => `[${ne("data")}]`)), ie("data", ((e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
                 if (function(e) {
                         return !!Ke && (!!Ye || e.hasAttribute("data-has-alpine-state"))
                     }(e)) return;
@@ -2420,25 +2433,25 @@
                         a = n, !Array.isArray(a) && !isNaN(a) && n >= 0 && (n = Array.from(Array(n).keys(), (e => e + 1))), void 0 === n && (n = []);
                         let s = e._x_lookup,
                             l = e._x_prevKeys,
                             c = [],
                             u = [];
                         if ("object" != typeof(f = n) || Array.isArray(f))
                             for (let i = 0; i < n.length; i++) {
-                                let o = Un(t, n[i], i, n);
+                                let o = Kn(t, n[i], i, n);
                                 r((t => {
                                     u.includes(t) && we("Duplicate key on x-for", e), u.push(t)
                                 }), {
                                     scope: {
                                         index: i,
                                         ...o
                                     }
                                 }), c.push(o)
                             } else n = Object.entries(n).map((([i, o]) => {
-                                let a = Un(t, o, i, n);
+                                let a = Kn(t, o, i, n);
                                 r((t => {
                                     u.includes(t) && we("Duplicate key on x-for", e), u.push(t)
                                 }), {
                                     scope: {
                                         index: i,
                                         ...a
                                     }
@@ -2449,25 +2462,25 @@
                             _ = [],
                             h = [],
                             y = [];
                         for (let e = 0; e < l.length; e++) {
                             let t = l[e]; - 1 === u.indexOf(t) && h.push(t)
                         }
                         l = l.filter((e => !h.includes(e)));
-                        let v = "template";
+                        let m = "template";
                         for (let e = 0; e < u.length; e++) {
                             let t = u[e],
                                 n = l.indexOf(t);
-                            if (-1 === n) l.splice(e, 0, t), p.push([v, e]);
+                            if (-1 === n) l.splice(e, 0, t), p.push([m, e]);
                             else if (n !== e) {
                                 let t = l.splice(e, 1)[0],
                                     r = l.splice(n - 1, 1)[0];
                                 l.splice(e, 0, r), l.splice(n, 0, t), _.push([t, r])
                             } else y.push(t);
-                            v = t
+                            m = t
                         }
                         for (let e = 0; e < h.length; e++) {
                             let t = h[e];
                             s[t]._x_effects && s[t]._x_effects.forEach(d), s[t].remove(), s[t] = null, delete s[t]
                         }
                         for (let e = 0; e < _.length; e++) {
                             let [t, n] = _[e], r = s[t], i = s[n], a = document.createElement("div");
@@ -2492,22 +2505,22 @@
                         }
                         for (let e = 0; e < y.length; e++) s[y[e]]._x_refreshXForScope(c[u.indexOf(y[e])]);
                         o._x_prevKeys = u
                     }))
                 }(e, o, a, s))), r((() => {
                     Object.values(e._x_lookup).forEach((e => e.remove())), delete e._x_prevKeys, delete e._x_lookup
                 }))
-            })), Kn.inline = (e, {
+            })), Zn.inline = (e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
                 let r = Te(e);
                 r._x_refs || (r._x_refs = {}), r._x_refs[t] = e, n((() => delete r._x_refs[t]))
-            }, ie("ref", Kn), ie("if", ((e, {
+            }, ie("ref", Zn), ie("if", ((e, {
                 expression: t
             }, {
                 effect: n,
                 cleanup: r
             }) => {
                 "template" !== e.tagName.toLowerCase() && we("x-if can only be used on a <template> tag", e);
                 let i = X(e, t);
@@ -2548,17 +2561,17 @@
                         scope: {
                             $event: e
                         },
                         params: [e]
                     })
                 }));
                 i((() => a()))
-            }))), Zn("Collapse", "collapse", "collapse"), Zn("Intersect", "intersect", "intersect"), Zn("Focus", "trap", "focus"), Zn("Mask", "mask", "mask"), _t.setEvaluator(G), _t.setReactivityEngine({
+            }))), Jn("Collapse", "collapse", "collapse"), Jn("Intersect", "intersect", "intersect"), Jn("Focus", "trap", "focus"), Jn("Mask", "mask", "mask"), _t.setEvaluator(G), _t.setReactivityEngine({
                 reactive: jn,
-                effect: function(e, t = vt) {
+                effect: function(e, t = mt) {
                     (function(e) {
                         return e && !0 === e._isEffect
                     })(e) && (e = e.raw);
                     const n = function(e, t) {
                         const n = function() {
                             if (!n.active) return e();
                             if (!Nt.includes(n)) {
@@ -2575,22 +2588,22 @@
                     return t.lazy || n(), n
                 },
                 release: function(e) {
                     e.active && (It(e), e.options.onStop && e.options.onStop(), e.active = !1)
                 },
                 raw: $n
             });
-            var Jn = _t,
-                Xn = n(122),
-                Yn = n.n(Xn);
+            var Xn = _t,
+                Yn = n(122),
+                Gn = n.n(Yn);
 
-            function Gn(e, t) {
+            function Qn(e, t) {
                 e.classList.remove("scale-100"), t.classList.add("scale-100"), e.classList.add("scale-0"), t.classList.remove("scale-0")
             }
-            window.Alpine = Jn, Jn.plugin((function(t) {
+            window.Alpine = Xn, Xn.plugin((function(t) {
                 t.directive("intersect", t.skipDuringClone(((t, {
                     value: n,
                     expression: i,
                     modifiers: o
                 }, {
                     evaluateLater: a,
                     cleanup: s
@@ -2605,35 +2618,35 @@
                                 e.isIntersecting !== ("leave" === n) && (l(), o.includes("once") && u.disconnect())
                             }))
                         }), c);
                     u.observe(t), s((() => {
                         u.disconnect()
                     }))
                 })))
-            })), Jn.start(), window.addEventListener("DOMContentLoaded", (() => {
+            })), Xn.start(), window.addEventListener("DOMContentLoaded", (() => {
                 ! function() {
                     const e = document.querySelectorAll(".highlight");
                     if (!e) return;
                     e.forEach((e => {
                         const t = e.querySelector("pre");
                         if (t) {
                             const e = '<button class="copy z-20 inline-flex h-6 w-6 items-center justify-center rounded-md border border-border bg-background opacity-0 focus:opacity-100 text-sm font-medium transition-all hover:bg-muted absolute right-4 top-4 tooltipped tooltipped-n" data-tooltip="Copy code" type="button"><span class="sr-only">Copy code</span><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-icon h-[14px] w-[14px] transition-all transform scale-100 absolute"><path d="M200 976q-33 0-56.5-23.5T120 896V376q0-17 11.5-28.5T160 336q17 0 28.5 11.5T200 376v520h400q17 0 28.5 11.5T640 936q0 17-11.5 28.5T600 976H200Zm160-160q-33 0-56.5-23.5T280 736V256q0-33 23.5-56.5T360 176h360q33 0 56.5 23.5T800 256v480q0 33-23.5 56.5T720 816H360Zm0-80h360V256H360v480Zm0 0V256v480Z"/></svg><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-success-icon h-[14px] w-[14px] transition-all transform scale-0 absolute"><path d="M382 799q-8 0-15-2.5t-13-8.5L182 616q-11-11-10.5-28.5T183 559q11-11 28-11t28 11l143 143 339-339q11-11 28.5-11t28.5 11q11 11 11 28.5T778 420L410 788q-6 6-13 8.5t-15 2.5Z"/></svg></button>';
                             t.insertAdjacentHTML("beforeend", e)
                         }
                     }));
-                    const t = new(Yn())("button.copy", {
+                    const t = new(Gn())("button.copy", {
                         target: e => e.previousElementSibling
                     });
                     t.on("success", (({
                         trigger: e
                     }) => {
                         const t = e.getAttribute("data-tooltip"),
                             n = e.querySelector(".copy-icon"),
                             r = e.querySelector(".copy-success-icon");
-                        Gn(n, r), e.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
-                            Gn(r, n), e.setAttribute("data-tooltip", t)
+                        Qn(n, r), e.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
+                            Qn(r, n), e.setAttribute("data-tooltip", t)
                         }), 2e3)
                     }))
                 }()
             }))
         }()
 }();
```

### Comparing `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.4/PKG-INFO` & `sphinxawesome_theme-5.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.1.4
+Version: 5.1.5
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: sphinx (<7.2) ; python_version >= "3.8" and python_version < "3.9"
-Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and python_version < "3.13"
+Requires-Dist: sphinx (>=7.2,<7.4) ; python_version >= "3.9" and python_version < "3.13"
 Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
 
 <h1 align="center">Sphinx awesome theme</h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.4 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.5 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx Classifier: Topic :: Software
 Development :: Documentation Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: sphinx (<7.2) ; python_version >= "3.8" and python_version <
-"3.9" Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and
+"3.9" Requires-Dist: sphinx (>=7.2,<7.4) ; python_version >= "3.9" and
 python_version < "3.13" Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
                       ************ SSpphhiinnxx aawweessoommee tthheemmee ************
       [MIT license][PyPI version][Netlify Deploy][GitHub Workflow Status]
  Create beautiful and awesome documentation websites with _S_p_h_i_n_x. See how the
                     theme looks like on _s_p_h_i_n_x_a_w_e_s_o_m_e_._x_y_z.
```

