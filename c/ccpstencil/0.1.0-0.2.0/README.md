# Comparing `tmp/ccpstencil-0.1.0.tar.gz` & `tmp/ccpstencil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpstencil-0.1.0.tar", last modified: Fri May 24 18:44:25 2024, max compression
+gzip compressed data, was "ccpstencil-0.2.0.tar", last modified: Tue May 28 16:01:34 2024, max compression
```

## Comparing `ccpstencil-0.1.0.tar` & `ccpstencil-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.181828 ccpstencil-0.1.0/ccpstencil/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.181828 ccpstencil-0.1.0/ccpstencil/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.181828 ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.181828 ccpstencil-0.1.0/ccpstencil/context/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/context/_alviss.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/context/_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/context/_kwarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/ccpstencil/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/renderer/_string.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/stencils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/ccpstencil/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/ccpstencil/structs/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/interfaces/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/interfaces/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/structs/interfaces/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/ccpstencil/template/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/template/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/template/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/ccpstencil/template/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/ccpstencil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 18:44:25.000000 ccpstencil-0.1.0/ccpstencil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:44:25.189828 ccpstencil-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:44:25.185828 ccpstencil-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-24 18:44:11.000000 ccpstencil-0.1.0/tests/test_some_basic_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/context/_alviss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/context/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/context/_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/jinjaext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/jinjaext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.090314 ccpstencil-0.2.0/ccpstencil/jinjaext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/jinjaext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/jinjaext/extensions/_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.094313 ccpstencil-0.2.0/ccpstencil/jinjaext/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/jinjaext/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/jinjaext/filters/_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.094313 ccpstencil-0.2.0/ccpstencil/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/renderer/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.094313 ccpstencil-0.2.0/ccpstencil/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/shortcuts/_render_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/stencils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.094313 ccpstencil-0.2.0/ccpstencil/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.094313 ccpstencil-0.2.0/ccpstencil/structs/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/interfaces/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/interfaces/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/structs/interfaces/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/ccpstencil/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/template/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/template/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/template/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/ccpstencil/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/ccpstencil/utils/_guessers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/ccpstencil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 16:01:34.000000 ccpstencil-0.2.0/ccpstencil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:01:34.098314 ccpstencil-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 16:01:25.000000 ccpstencil-0.2.0/tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.1.0/LICENSE` & `ccpstencil-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/PKG-INFO` & `ccpstencil-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.1.0
+Version: 0.2.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.1.0/README.md` & `ccpstencil-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/_runner.py` & `ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/_runner.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/ccpstencil/cli/ccp_stencil/main.py` & `ccpstencil-0.2.0/ccpstencil/cli/ccp_stencil/main.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/ccpstencil/context/_alviss.py` & `ccpstencil-0.2.0/ccpstencil/context/_alviss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 __all__ = [
     'AlvissContext',
 ]
 
 from ccpstencil.structs import *
 from alviss import quickloader
 from ccptools.tpu import iters
+from pathlib import Path
 import logging
 log = logging.getLogger(__file__)
 
 
 class AlvissContext(IContext):
-    def __init__(self, file_name: str, **kwargs):
-        self._file_name = file_name
+    def __init__(self, file_name: Union[str, Path], **kwargs):
+        self._file_name = str(file_name)
         self._data = quickloader.autoload(file_name)
         self._update_map: Dict[Tuple[str], Any] = {}
 
     def update(self, key: str, value: Any):
         self._data[key] = value
 
     def nested_update(self, key_tuple: Union[str, Tuple[str]], value: Any):
```

### Comparing `ccpstencil-0.1.0/ccpstencil/context/_dict.py` & `ccpstencil-0.2.0/ccpstencil/context/_dict.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/ccpstencil/renderer/_file.py` & `ccpstencil-0.2.0/ccpstencil/renderer/_file.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/ccpstencil/structs/_errors.py` & `ccpstencil-0.2.0/ccpstencil/structs/_errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     'ContextError',
 
     'RenderError',
     'NoTemplateSetError',
     'InvalidContextTypeForRendererError',
     'InvalidTemplateTypeForRendererError',
     'OutputFileExistsError',
+    'EmbedFileNotFound',
 ]
 
 
 class StencilError(Exception):
     pass
 
 
@@ -44,7 +45,11 @@
 
 class InvalidTemplateTypeForRendererError(RenderError, TypeError):
     pass
 
 
 class OutputFileExistsError(RenderError, FileExistsError):
     pass
+
+
+class EmbedFileNotFound(RenderError, FileNotFoundError):
+    pass
```

### Comparing `ccpstencil-0.1.0/ccpstencil/structs/interfaces/_renderer.py` & `ccpstencil-0.2.0/ccpstencil/structs/interfaces/_renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,15 @@
     def render(self):
         pass
 
     @property
     @abc.abstractmethod
     def jinja_environment(self) -> jinja2.Environment:
         pass
+
+    @abc.abstractmethod
+    def is_template_loadable(self, template_name: str) -> bool:
+        pass
+
+    @abc.abstractmethod
+    def get_embed(self, file_path: str, source_file: Optional[str] = None, alviss: bool = False, env: bool = False) -> str:
+        pass
```

### Comparing `ccpstencil-0.1.0/ccpstencil/template/_file.py` & `ccpstencil-0.2.0/ccpstencil/template/_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 __all__ = [
     'FileTemplate',
 ]
 
 from ccpstencil.structs import *
 from pathlib import Path
 
-from ._string import *
+from ._base import *
 
 
-class FileTemplate(StringTemplate):
-    def __init__(self, file_path: Union[str, Path], **kwargs):
-        if isinstance(file_path, str):
-            file_path = Path(file_path)
-        self._file_path: Path = file_path
-        super().__init__(template_string=self._read_file(), **kwargs)
+class FileTemplate(_BaseTemplate):
+    def __init__(self, file_path: T_PATH, **kwargs):
+        super().__init__(**kwargs)
+        self._file_path: T_PATH = file_path
 
     def _read_file(self) -> str:
-        if not self._file_path.exists():
-            raise TemplateNotFoundError(f'File {self._file_path} does not exist')
+        if isinstance(self._file_path, str):
+            as_path = Path(self._file_path)
+        else:
+            as_path = self._file_path
+        if not as_path.exists():
+            raise TemplateNotFoundError(f'File {as_path} does not exist')
 
-        with open(self._file_path, 'r') as fin:
+        with open(as_path, 'r') as fin:
             return fin.read()
+
+    def get_jinja_template(self) -> jinja2.Template:
+        if isinstance(self._file_path, str):
+            try:
+                return self.renderer.jinja_environment.get_template(self._file_path)
+            except jinja2.exceptions.TemplateNotFound:
+                pass
+        template_string = self._read_file()
+        return self.renderer.jinja_environment.from_string(template_string)
```

### Comparing `ccpstencil-0.1.0/ccpstencil.egg-info/PKG-INFO` & `ccpstencil-0.2.0/ccpstencil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.1.0
+Version: 0.2.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.1.0/ccpstencil.egg-info/SOURCES.txt` & `ccpstencil-0.2.0/ccpstencil.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,25 +14,37 @@
 ccpstencil/cli/ccp_stencil/__init__.py
 ccpstencil/cli/ccp_stencil/_runner.py
 ccpstencil/cli/ccp_stencil/main.py
 ccpstencil/context/__init__.py
 ccpstencil/context/_alviss.py
 ccpstencil/context/_dict.py
 ccpstencil/context/_kwarg.py
+ccpstencil/jinjaext/__init__.py
+ccpstencil/jinjaext/extensions/__init__.py
+ccpstencil/jinjaext/extensions/_embed.py
+ccpstencil/jinjaext/filters/__init__.py
+ccpstencil/jinjaext/filters/_base64.py
 ccpstencil/renderer/__init__.py
 ccpstencil/renderer/_base.py
 ccpstencil/renderer/_dir.py
 ccpstencil/renderer/_file.py
 ccpstencil/renderer/_stdout.py
 ccpstencil/renderer/_string.py
+ccpstencil/shortcuts/__init__.py
+ccpstencil/shortcuts/_render_stencil.py
 ccpstencil/structs/__init__.py
+ccpstencil/structs/_aliases.py
 ccpstencil/structs/_base.py
 ccpstencil/structs/_errors.py
 ccpstencil/structs/interfaces/__init__.py
 ccpstencil/structs/interfaces/_context.py
 ccpstencil/structs/interfaces/_renderer.py
 ccpstencil/structs/interfaces/_template.py
 ccpstencil/template/__init__.py
 ccpstencil/template/_base.py
 ccpstencil/template/_file.py
 ccpstencil/template/_string.py
+ccpstencil/utils/__init__.py
+ccpstencil/utils/_guessers.py
+tests/test_embed.py
+tests/test_filters.py
 tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.1.0/pyproject.toml` & `ccpstencil-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.1.0/tests/test_some_basic_stuff.py` & `ccpstencil-0.2.0/tests/test_some_basic_stuff.py`

 * *Files identical despite different names*

