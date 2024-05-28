# Comparing `tmp/sphinx-design-elements-0.3.1.tar.gz` & `tmp/sphinx_design_elements-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-design-elements-0.3.1.tar", last modified: Wed Apr 10 13:47:53 2024, max compression
+gzip compressed data, was "sphinx_design_elements-0.3.2.tar", last modified: Tue May 28 18:34:41 2024, max compression
```

## Comparing `sphinx-design-elements-0.3.1.tar` & `sphinx_design_elements-0.3.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.555605 sphinx-design-elements-0.3.1/
--rw-r--r--   0 amo        (501) staff       (20)      768 2024-04-10 13:47:11.000000 sphinx-design-elements-0.3.1/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.3.1/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     8142 2024-04-10 13:47:53.555203 sphinx-design-elements-0.3.1/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.532962 sphinx-design-elements-0.3.1/docs/
--rw-r--r--   0 amo        (501) staff       (20)      772 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.1/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)      768 2024-04-10 13:47:11.000000 sphinx-design-elements-0.3.1/docs/changes.md
--rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.1/docs/css_classes.md
--rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.3.1/docs/get_started.md
--rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.1/docs/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)    33174 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/hyper.md
--rw-r--r--   0 amo        (501) staff       (20)     3835 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/index.md
--rw-r--r--   0 amo        (501) staff       (20)     2163 2024-04-10 04:43:18.000000 sphinx-design-elements-0.3.1/docs/info.md
--rw-r--r--   0 amo        (501) staff       (20)     2996 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.1/docs/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.3.1/docs/project.md
--rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/docs/readme.md
--rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.3.1/docs/sandbox.md
--rw-r--r--   0 amo        (501) staff       (20)    12371 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.1/docs/shield.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.533360 sphinx-design-elements-0.3.1/docs/snippets/
--rw-r--r--   0 amo        (501) staff       (20)       73 2024-03-24 17:03:31.000000 sphinx-design-elements-0.3.1/docs/snippets/index.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.537208 sphinx-design-elements-0.3.1/docs/snippets/myst/
--rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)      643 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/hyper.md
--rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/shield.md
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/tag.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.540413 sphinx-design-elements-0.3.1/docs/snippets/rst/
--rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/dropdown-group.rst
--rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/gridtable.rst
--rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/infocard.rst
--rw-r--r--   0 amo        (501) staff       (20)      201 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/shield.rst
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/tag.rst
--rw-r--r--   0 amo        (501) staff       (20)     2822 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/tag.md
--rw-r--r--   0 amo        (501) staff       (20)     6056 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-10 13:47:53.555696 sphinx-design-elements-0.3.1/setup.cfg
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.546989 sphinx-design-elements-0.3.1/sphinx_design_elements/
--rw-r--r--   0 amo        (501) staff       (20)      434 2024-03-07 23:44:18.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.550291 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/addon.js
--rw-r--r--   0 amo        (501) staff       (20)     1431 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/style.css
--rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/dropdown_group.py
--rw-r--r--   0 amo        (501) staff       (20)     2849 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/extension.py
--rw-r--r--   0 amo        (501) staff       (20)     5218 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/gridtable.py
--rw-r--r--   0 amo        (501) staff       (20)    13371 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/hyper.py
--rw-r--r--   0 amo        (501) staff       (20)     3751 2024-03-20 22:48:06.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/infocard.py
--rw-r--r--   0 amo        (501) staff       (20)     4004 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/shield.py
--rw-r--r--   0 amo        (501) staff       (20)     2006 2024-03-07 23:25:56.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/tag.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.551835 sphinx-design-elements-0.3.1/sphinx_design_elements/util/
--rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     4565 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/directive.py
--rw-r--r--   0 amo        (501) staff       (20)     4482 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/role.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.552546 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     8142 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     1412 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      331 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       29 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.373562 sphinx_design_elements-0.3.2/
+-rw-r--r--   0 amo        (501) staff       (20)      922 2024-05-28 18:32:10.000000 sphinx_design_elements-0.3.2/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx_design_elements-0.3.2/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx_design_elements-0.3.2/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     8144 2024-05-28 18:34:41.372794 sphinx_design_elements-0.3.2/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx_design_elements-0.3.2/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.356701 sphinx_design_elements-0.3.2/docs/
+-rw-r--r--   0 amo        (501) staff       (20)      772 2024-04-06 16:14:56.000000 sphinx_design_elements-0.3.2/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)      922 2024-05-28 18:32:10.000000 sphinx_design_elements-0.3.2/docs/changes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx_design_elements-0.3.2/docs/css_classes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx_design_elements-0.3.2/docs/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx_design_elements-0.3.2/docs/get_started.md
+-rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx_design_elements-0.3.2/docs/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)    33174 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/docs/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)     3835 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/docs/index.md
+-rw-r--r--   0 amo        (501) staff       (20)     2163 2024-04-10 04:43:18.000000 sphinx_design_elements-0.3.2/docs/info.md
+-rw-r--r--   0 amo        (501) staff       (20)     2996 2024-03-24 11:42:42.000000 sphinx_design_elements-0.3.2/docs/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx_design_elements-0.3.2/docs/project.md
+-rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx_design_elements-0.3.2/docs/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx_design_elements-0.3.2/docs/sandbox.md
+-rw-r--r--   0 amo        (501) staff       (20)    12371 2024-04-06 16:14:56.000000 sphinx_design_elements-0.3.2/docs/shield.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.357052 sphinx_design_elements-0.3.2/docs/snippets/
+-rw-r--r--   0 amo        (501) staff       (20)       73 2024-03-24 17:03:31.000000 sphinx_design_elements-0.3.2/docs/snippets/index.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.359317 sphinx_design_elements-0.3.2/docs/snippets/myst/
+-rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)      643 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-06 16:12:43.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/shield.md
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx_design_elements-0.3.2/docs/snippets/myst/tag.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.361133 sphinx_design_elements-0.3.2/docs/snippets/rst/
+-rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx_design_elements-0.3.2/docs/snippets/rst/dropdown-group.rst
+-rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx_design_elements-0.3.2/docs/snippets/rst/gridtable.rst
+-rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx_design_elements-0.3.2/docs/snippets/rst/infocard.rst
+-rw-r--r--   0 amo        (501) staff       (20)      201 2024-04-06 16:12:43.000000 sphinx_design_elements-0.3.2/docs/snippets/rst/shield.rst
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx_design_elements-0.3.2/docs/snippets/rst/tag.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2822 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/docs/tag.md
+-rw-r--r--   0 amo        (501) staff       (20)     6058 2024-05-28 18:30:42.000000 sphinx_design_elements-0.3.2/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-05-28 18:34:41.373793 sphinx_design_elements-0.3.2/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.364240 sphinx_design_elements-0.3.2/sphinx_design_elements/
+-rw-r--r--   0 amo        (501) staff       (20)      434 2024-03-07 23:44:18.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.367462 sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/addon.js
+-rw-r--r--   0 amo        (501) staff       (20)     1431 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/style.css
+-rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/dropdown_group.py
+-rw-r--r--   0 amo        (501) staff       (20)     2849 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/extension.py
+-rw-r--r--   0 amo        (501) staff       (20)     5218 2024-03-24 11:42:42.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/gridtable.py
+-rw-r--r--   0 amo        (501) staff       (20)    13371 2024-04-06 16:14:54.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/hyper.py
+-rw-r--r--   0 amo        (501) staff       (20)     3751 2024-03-20 22:48:06.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/infocard.py
+-rw-r--r--   0 amo        (501) staff       (20)     4004 2024-04-06 16:12:43.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/shield.py
+-rw-r--r--   0 amo        (501) staff       (20)     2006 2024-03-07 23:25:56.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/tag.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.368698 sphinx_design_elements-0.3.2/sphinx_design_elements/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-06 16:12:43.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4565 2024-04-06 16:12:43.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/util/directive.py
+-rw-r--r--   0 amo        (501) staff       (20)     4482 2024-04-10 13:46:31.000000 sphinx_design_elements-0.3.2/sphinx_design_elements/util/role.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-28 18:34:41.369229 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     8144 2024-05-28 18:34:41.000000 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     1412 2024-05-28 18:34:41.000000 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-05-28 18:34:41.000000 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      333 2024-05-28 18:34:41.000000 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       29 2024-05-28 18:34:41.000000 sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/top_level.txt
```

### Comparing `sphinx-design-elements-0.3.1/CHANGES.md` & `sphinx_design_elements-0.3.2/CHANGES.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Change Log
 
 ## Unreleased
 
+## v0.3.2 - 2024-05-28
+- Dependencies: Use sphinx-design 0.5
+  sphinx-design 0.6 introduced CSS changes downstream projects might not
+  be prepared for.
+
 ## v0.3.1 - 2024-04-10
 - Fix compatibility issue with Python 3.8
 
 ## v0.3.0 - 2024-04-06
 - Accept more options on grid table's `sd-item` directive
 - Add `shield` directive, to render badges through Shields.io
 - Add `hyper` role, to render different kinds of hyperlinks
```

### Comparing `sphinx-design-elements-0.3.1/LICENSE` & `sphinx_design_elements-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/PKG-INFO` & `sphinx_design_elements-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -68,26 +68,26 @@
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sphinx<7.2
-Requires-Dist: sphinx-design<1
+Requires-Dist: sphinx-design<0.6
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
-Requires-Dist: mypy<1.10; extra == "develop"
-Requires-Dist: poethepoet<0.26; extra == "develop"
-Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff<0.4; extra == "develop"
+Requires-Dist: mypy<1.11; extra == "develop"
+Requires-Dist: poethepoet<0.27; extra == "develop"
+Requires-Dist: pyproject-fmt<2.2; extra == "develop"
+Requires-Dist: ruff<0.5; extra == "develop"
 Requires-Dist: types-docutils==0.20.0.3; extra == "develop"
-Requires-Dist: validate-pyproject<0.17; extra == "develop"
+Requires-Dist: validate-pyproject<0.19; extra == "develop"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
-Requires-Dist: myst-parser[linkify]<3,>=0.18; extra == "docs"
+Requires-Dist: myst-parser[linkify]<4,>=0.18; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: keyring; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
```

### Comparing `sphinx-design-elements-0.3.1/README.md` & `sphinx_design_elements-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/backlog.md` & `sphinx_design_elements-0.3.2/docs/backlog.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/changes.md` & `sphinx_design_elements-0.3.2/docs/changes.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Change Log
 
 ## Unreleased
 
+## v0.3.2 - 2024-05-28
+- Dependencies: Use sphinx-design 0.5
+  sphinx-design 0.6 introduced CSS changes downstream projects might not
+  be prepared for.
+
 ## v0.3.1 - 2024-04-10
 - Fix compatibility issue with Python 3.8
 
 ## v0.3.0 - 2024-04-06
 - Accept more options on grid table's `sd-item` directive
 - Add `shield` directive, to render badges through Shields.io
 - Add `hyper` role, to render different kinds of hyperlinks
```

### Comparing `sphinx-design-elements-0.3.1/docs/css_classes.md` & `sphinx_design_elements-0.3.2/docs/css_classes.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/dropdown-group.md` & `sphinx_design_elements-0.3.2/docs/dropdown-group.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/get_started.md` & `sphinx_design_elements-0.3.2/docs/get_started.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/gridtable.md` & `sphinx_design_elements-0.3.2/docs/gridtable.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/hyper.md` & `sphinx_design_elements-0.3.2/docs/hyper.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/index.md` & `sphinx_design_elements-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/info.md` & `sphinx_design_elements-0.3.2/docs/info.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/infocard.md` & `sphinx_design_elements-0.3.2/docs/infocard.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/readme.md` & `sphinx_design_elements-0.3.2/docs/readme.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/sandbox.md` & `sphinx_design_elements-0.3.2/docs/sandbox.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/shield.md` & `sphinx_design_elements-0.3.2/docs/shield.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/snippets/myst/hyper.md` & `sphinx_design_elements-0.3.2/docs/snippets/myst/hyper.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/snippets/rst/infocard.rst` & `sphinx_design_elements-0.3.2/docs/snippets/rst/infocard.rst`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/docs/tag.md` & `sphinx_design_elements-0.3.2/docs/tag.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/pyproject.toml` & `sphinx_design_elements-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -82,29 +82,29 @@
   "Topic :: Text Processing :: Markup :: reStructuredText",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "sphinx<7.2",
-  "sphinx-design<1",
+  "sphinx-design<0.6",
 ]
 [project.optional-dependencies]
 develop = [
   "black<25",
-  "mypy<1.10",
-  "poethepoet<0.26",
-  "pyproject-fmt<1.8",
-  "ruff<0.4",
+  "mypy<1.11",
+  "poethepoet<0.27",
+  "pyproject-fmt<2.2",
+  "ruff<0.5",
   "types-docutils==0.20.0.3",
-  "validate-pyproject<0.17",
+  "validate-pyproject<0.19",
 ]
 docs = [
   "furo",
-  "myst-parser[linkify]<3,>=0.18",
+  "myst-parser[linkify]>=0.18,<4",
   "sphinx-autobuild",
   "sphinx-copybutton",
 ]
 release = [
   "build<2",
   "keyring",
   "twine<6",
```

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/addon.js` & `sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/addon.js`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/style.css` & `sphinx_design_elements-0.3.2/sphinx_design_elements/compiled/style.css`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/extension.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/gridtable.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/gridtable.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/hyper.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/hyper.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/infocard.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/infocard.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/shield.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/shield.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/tag.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/tag.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/util/directive.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/util/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements/util/role.py` & `sphinx_design_elements-0.3.2/sphinx_design_elements/util/role.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/PKG-INFO` & `sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -68,26 +68,26 @@
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sphinx<7.2
-Requires-Dist: sphinx-design<1
+Requires-Dist: sphinx-design<0.6
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
-Requires-Dist: mypy<1.10; extra == "develop"
-Requires-Dist: poethepoet<0.26; extra == "develop"
-Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff<0.4; extra == "develop"
+Requires-Dist: mypy<1.11; extra == "develop"
+Requires-Dist: poethepoet<0.27; extra == "develop"
+Requires-Dist: pyproject-fmt<2.2; extra == "develop"
+Requires-Dist: ruff<0.5; extra == "develop"
 Requires-Dist: types-docutils==0.20.0.3; extra == "develop"
-Requires-Dist: validate-pyproject<0.17; extra == "develop"
+Requires-Dist: validate-pyproject<0.19; extra == "develop"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
-Requires-Dist: myst-parser[linkify]<3,>=0.18; extra == "docs"
+Requires-Dist: myst-parser[linkify]<4,>=0.18; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: keyring; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
```

### Comparing `sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/SOURCES.txt` & `sphinx_design_elements-0.3.2/sphinx_design_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

