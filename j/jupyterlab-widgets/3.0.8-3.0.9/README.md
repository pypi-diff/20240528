# Comparing `tmp/jupyterlab_widgets-3.0.8.tar.gz` & `tmp/jupyterlab_widgets-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_widgets-3.0.8.tar", last modified: Tue Jul  4 15:06:35 2023, max compression
+gzip compressed data, was "jupyterlab_widgets-3.0.9.tar", last modified: Wed Sep 13 08:01:44 2023, max compression
```

## Comparing `jupyterlab_widgets-3.0.8.tar` & `jupyterlab_widgets-3.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    13847 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/LICENSE
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      383 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/MANIFEST.in
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2741 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/README.md
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      197 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/install.json
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.803618 jupyterlab_widgets-3.0.8/jupyterlab_widgets/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      599 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets/__init__.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      124 2023-07-04 15:06:04.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets/_version.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.805618 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1370 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/not-zip-safe
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       19 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.805618 jupyterlab_widgets-3.0.8/labextension/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3532 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/package.json
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.801618 jupyterlab_widgets-3.0.8/labextension/schemas/
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.801618 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.806618 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3416 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      375 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.810618 jupyterlab_widgets-3.0.8/labextension/static/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   181710 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/113.6113d19fca7ff66ccc66.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      160 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/113.6113d19fca7ff66ccc66.js.LICENSE.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    85828 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/134.b4eddbb09f5fd50a4007.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    87175 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      218 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js.LICENSE.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11738 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/336.9f709c2076672b1bfe2b.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    38492 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/345.17494fea1ff555b26294.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   111313 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/495.b58859516292ffe4bc96.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    24347 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/595.942a65706d9bc281d5ca.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/596.1f32fb4ed861227b46e2.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      187 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/61.21f571face17e35076c2.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    60054 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/644.52a1098a3a5f3e45abff.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    33147 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/699.e966b1425a7d4e8c3f4e.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/965.22fa53da8ad2a8da593a.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    10607 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/remoteEntry.98b8a827bfc5f86e95d2.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      118 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/static/style.js
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    40924 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/third-party-licenses.json
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3359 2023-07-04 15:05:15.000000 jupyterlab_widgets-3.0.8/package.json
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      496 2023-07-04 14:25:30.000000 jupyterlab_widgets-3.0.8/pyproject.toml
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1371 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/setup.cfg
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      907 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/setup.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      310 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/tsconfig.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.329206 jupyterlab_widgets-3.0.9/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    13847 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/LICENSE
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      383 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/MANIFEST.in
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-09-13 08:01:44.329206 jupyterlab_widgets-3.0.9/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2741 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/README.md
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      197 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/install.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.321206 jupyterlab_widgets-3.0.9/jupyterlab_widgets/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      599 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets/__init__.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      124 2023-09-13 08:01:11.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets/_version.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.322206 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-09-13 08:01:44.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1370 2023-09-13 08:01:44.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-09-13 08:01:44.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-09-13 07:59:53.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       19 2023-09-13 08:01:44.000000 jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.322206 jupyterlab_widgets-3.0.9/labextension/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3532 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/package.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.319206 jupyterlab_widgets-3.0.9/labextension/schemas/
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.319206 jupyterlab_widgets-3.0.9/labextension/schemas/@jupyter-widgets/
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.322206 jupyterlab_widgets-3.0.9/labextension/schemas/@jupyter-widgets/jupyterlab-manager/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3416 2023-09-13 07:57:09.000000 jupyterlab_widgets-3.0.9/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      375 2023-09-13 07:57:09.000000 jupyterlab_widgets-3.0.9/labextension/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-09-13 08:01:44.329206 jupyterlab_widgets-3.0.9/labextension/static/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   181710 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/113.e4cfda62b59ddbe550d3.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      160 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/113.e4cfda62b59ddbe550d3.js.LICENSE.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    85829 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/134.a63a8d293fb35a52dc25.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    87175 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/291.cff5ef71b29e18850479.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      218 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/291.cff5ef71b29e18850479.js.LICENSE.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11738 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/336.ebc7a55ea1768712771f.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    38492 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/345.17494fea1ff555b26294.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   111313 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/495.79062b4ce5ec7920dcb1.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    24253 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/595.74686e2543ce21f10975.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/596.df8214a14175baf1ee16.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      187 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/61.21f571face17e35076c2.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    60054 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/644.558670f1aa9ae5791769.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    33147 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/699.e966b1425a7d4e8c3f4e.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/965.9a2bfc1116cea35345ca.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    10608 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/remoteEntry.a37e37c87d212fe85e13.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      118 2023-09-13 07:57:09.000000 jupyterlab_widgets-3.0.9/labextension/static/style.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    40924 2023-09-13 07:57:19.000000 jupyterlab_widgets-3.0.9/labextension/static/third-party-licenses.json
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3359 2023-09-13 07:57:29.000000 jupyterlab_widgets-3.0.9/package.json
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      496 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/pyproject.toml
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1371 2023-09-13 08:01:44.330206 jupyterlab_widgets-3.0.9/setup.cfg
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      907 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/setup.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      310 2023-07-31 12:53:52.000000 jupyterlab_widgets-3.0.9/tsconfig.json
```

### Comparing `jupyterlab_widgets-3.0.8/LICENSE` & `jupyterlab_widgets-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/PKG-INFO` & `jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab_widgets
-Version: 3.0.8
+Name: jupyterlab-widgets
+Version: 3.0.9
 Summary: Jupyter interactive widgets for JupyterLab
 Home-page: https://github.com/jupyter-widgets/ipywidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD-3-Clause
 Keywords: Interactive,Interpreter,Shell,Web,notebook,widgets,Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_widgets-3.0.8/README.md` & `jupyterlab_widgets-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/jupyterlab_widgets/__init__.py` & `jupyterlab_widgets-3.0.9/jupyterlab_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/PKG-INFO` & `jupyterlab_widgets-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab-widgets
-Version: 3.0.8
+Name: jupyterlab_widgets
+Version: 3.0.9
 Summary: Jupyter interactive widgets for JupyterLab
 Home-page: https://github.com/jupyter-widgets/ipywidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD-3-Clause
 Keywords: Interactive,Interpreter,Shell,Web,notebook,widgets,Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/SOURCES.txt` & `jupyterlab_widgets-3.0.9/jupyterlab_widgets.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 jupyterlab_widgets.egg-info/SOURCES.txt
 jupyterlab_widgets.egg-info/dependency_links.txt
 jupyterlab_widgets.egg-info/not-zip-safe
 jupyterlab_widgets.egg-info/top_level.txt
 labextension/package.json
 labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
 labextension/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
-labextension/static/113.6113d19fca7ff66ccc66.js
-labextension/static/113.6113d19fca7ff66ccc66.js.LICENSE.txt
-labextension/static/134.b4eddbb09f5fd50a4007.js
+labextension/static/113.e4cfda62b59ddbe550d3.js
+labextension/static/113.e4cfda62b59ddbe550d3.js.LICENSE.txt
+labextension/static/134.a63a8d293fb35a52dc25.js
 labextension/static/291.cff5ef71b29e18850479.js
 labextension/static/291.cff5ef71b29e18850479.js.LICENSE.txt
-labextension/static/336.9f709c2076672b1bfe2b.js
+labextension/static/336.ebc7a55ea1768712771f.js
 labextension/static/345.17494fea1ff555b26294.js
-labextension/static/495.b58859516292ffe4bc96.js
-labextension/static/595.942a65706d9bc281d5ca.js
-labextension/static/596.1f32fb4ed861227b46e2.js
+labextension/static/495.79062b4ce5ec7920dcb1.js
+labextension/static/595.74686e2543ce21f10975.js
+labextension/static/596.df8214a14175baf1ee16.js
 labextension/static/61.21f571face17e35076c2.js
-labextension/static/644.52a1098a3a5f3e45abff.js
+labextension/static/644.558670f1aa9ae5791769.js
 labextension/static/699.e966b1425a7d4e8c3f4e.js
-labextension/static/965.22fa53da8ad2a8da593a.js
-labextension/static/remoteEntry.98b8a827bfc5f86e95d2.js
+labextension/static/965.9a2bfc1116cea35345ca.js
+labextension/static/remoteEntry.a37e37c87d212fe85e13.js
 labextension/static/style.js
 labextension/static/third-party-licenses.json
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/package.json` & `jupyterlab_widgets-3.0.9/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9352777777777779%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.6', '@jupyter-widgets/base-manager': '^1.0.7', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.7', '@jupyter-widgets/output': '^6.0.6'}",*

 * * "'gitHead'": "'17f68ed1b50f1c8b6843cb33f6b08161be89d3ea'",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'5.0.9'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.5",
-        "@jupyter-widgets/base-manager": "^1.0.6",
-        "@jupyter-widgets/controls": "^5.0.6",
-        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyter-widgets/base": "^6.0.6",
+        "@jupyter-widgets/base-manager": "^1.0.7",
+        "@jupyter-widgets/controls": "^5.0.7",
+        "@jupyter-widgets/output": "^6.0.6",
         "@jupyterlab/application": "^3.0.0 || ^4.0.0",
         "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
         "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
         "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
         "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
         "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
         "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
@@ -49,21 +49,17 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
-    "gitHead": "5e86a96c0138b837a1b0e609f02dd79de71f5bd6",
+    "gitHead": "17f68ed1b50f1c8b6843cb33f6b08161be89d3ea",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.98b8a827bfc5f86e95d2.js"
-        },
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -93,9 +89,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.8"
+    "version": "5.0.9"
 }
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig` & `jupyterlab_widgets-3.0.9/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9144444444444445%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.6', '@jupyter-widgets/base-manager': '^1.0.7', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.7', '@jupyter-widgets/output': '^6.0.6'}",*

 * * "'version'": "'5.0.9'",*

 * * 'delete': "['gitHead']"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.5",
-        "@jupyter-widgets/base-manager": "^1.0.6",
-        "@jupyter-widgets/controls": "^5.0.6",
-        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyter-widgets/base": "^6.0.6",
+        "@jupyter-widgets/base-manager": "^1.0.7",
+        "@jupyter-widgets/controls": "^5.0.7",
+        "@jupyter-widgets/output": "^6.0.6",
         "@jupyterlab/application": "^3.0.0 || ^4.0.0",
         "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
         "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
         "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
         "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
         "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
         "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
@@ -49,15 +49,14 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
-    "gitHead": "5e86a96c0138b837a1b0e609f02dd79de71f5bd6",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
@@ -89,9 +88,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.8"
+    "version": "5.0.9"
 }
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/113.6113d19fca7ff66ccc66.js` & `jupyterlab_widgets-3.0.9/labextension/static/113.e4cfda62b59ddbe550d3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 113.6113d19fca7ff66ccc66.js.LICENSE.txt */
+/*! For license information please see 113.e4cfda62b59ddbe550d3.js.LICENSE.txt */
 (self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || []).push([
     [113], {
         5766: (e, t) => {
             "use strict";
             t.b$ = function(e) {
                 var t, r, s = function(e) {
                         var t = e.length;
@@ -3888,15 +3888,15 @@
                             m = {};
                         for (o = 0; o < n.length; o++) l = (a = n[o])[a.length - 1], c = a.substring(0, a.length - 1), u = parseInt(c, 10), h = parseFloat(c), d.test(c) && "w" === l ? ((t || r) && (p = !0), 0 === u ? p = !0 : t = u) : f.test(c) && "x" === l ? ((t || r || s) && (p = !0), h < 0 ? p = !0 : r = h) : d.test(c) && "h" === l ? ((s || r) && (p = !0), 0 === u ? p = !0 : s = u) : p = !0;
                         p ? console && console.log && console.log("Invalid srcset descriptor found in '" + e + "' at '" + a + "'.") : (m.url = i, t && (m.w = t), r && (m.d = r), s && (m.h = s), g.push(m))
                     }
                 }
             }) ? r.apply(t, []) : r) || (e.exports = i)
         },
-        1794: e => {
+        4470: e => {
             var t = String,
                 r = function() {
                     return {
                         isColorSupported: !1,
                         reset: t,
                         bold: t,
                         dim: t,
@@ -4134,15 +4134,15 @@
                 "atrule" === e.type ? Object.setPrototypeOf(e, s.prototype) : "rule" === e.type ? Object.setPrototypeOf(e, n.prototype) : "decl" === e.type ? Object.setPrototypeOf(e, c.prototype) : "comment" === e.type ? Object.setPrototypeOf(e, u.prototype) : "root" === e.type && Object.setPrototypeOf(e, o.prototype), e[l] = !0, e.nodes && e.nodes.forEach((e => {
                     f.rebuild(e)
                 }))
             }
         },
         9452: (e, t, r) => {
             "use strict";
-            let i = r(1794),
+            let i = r(4470),
                 n = r(764);
             class s extends Error {
                 constructor(e, t, r, i, n, o) {
                     super(e), this.name = "CssSyntaxError", this.reason = e, n && (this.file = n), i && (this.source = i), o && (this.plugin = o), void 0 !== t && void 0 !== r && ("number" == typeof t ? (this.line = t, this.column = r) : (this.line = t.line, this.column = t.column, this.endLine = r.line, this.endColumn = r.column)), this.setMessage(), Error.captureStackTrace && Error.captureStackTrace(this, s)
                 }
                 setMessage() {
                     this.message = this.plugin ? this.plugin + ": " : "", this.message += this.file ? this.file : "<css input>", void 0 !== this.line && (this.message += ":" + this.line + ":" + this.column), this.message += ": " + this.reason
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/134.b4eddbb09f5fd50a4007.js` & `jupyterlab_widgets-3.0.9/labextension/static/134.a63a8d293fb35a52dc25.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -240,19 +240,19 @@
             });
             var i = {};
             t.r(i), t.d(i, {
                 OUTPUT_WIDGET_VERSION: () => P,
                 OutputModel: () => U,
                 OutputView: () => k
             });
-            var r = t(56),
-                o = t(1919),
-                a = t(4826),
-                d = t(4470),
-                s = t(9350),
+            var r = t(1426),
+                o = t(2212),
+                a = t(9450),
+                d = t(7463),
+                s = t(5243),
                 l = t(6697),
                 g = t(7717),
                 p = t(3004),
                 c = t(7930),
                 u = t(8778);
             class w extends u.Panel {
                 constructor(e, n) {
@@ -285,16 +285,16 @@
                 dispose() {
                     this.isDisposed || (this._manager = null, super.dispose())
                 }
                 _rerender() {
                     this._rerenderMimeModel && (this.node.textContent = "", this.removeClass("jupyter-widgets"), this.renderModel(this._rerenderMimeModel))
                 }
             }
-            var h = t(9890),
-                E = t(7482),
+            var h = t(4869),
+                E = t(7631),
                 b = t(4901),
                 j = t(9e3);
             class y {
                 constructor() {
                     this._cache = Object.create(null)
                 }
                 set(e, n, t) {
@@ -523,16 +523,16 @@
                 async clear_state() {
                     await super.clear_state(), this.setDirty()
                 }
                 setDirty() {
                     this._settings.saveState && (this._context.model.dirty = !0)
                 }
             }
-            var x = t(8409),
-                C = t(3363),
+            var x = t(8177),
+                C = t(4339),
                 R = t(2994),
                 A = t.n(R);
             const P = x.OUTPUT_WIDGET_VERSION;
             class U extends x.OutputModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         msg_id: "",
@@ -622,16 +622,16 @@
                 V = t.n(F),
                 G = t(937),
                 Y = {};
             Y.styleTagTransform = V(), Y.setAttributes = L(), Y.insert = N().bind(null, "head"), Y.domAPI = _(), Y.insertStyleElement = H(), B()(G.Z, Y), G.Z && G.Z.locals && G.Z.locals;
             var Z = t(5309),
                 K = {};
             K.styleTagTransform = V(), K.setAttributes = L(), K.insert = N().bind(null, "head"), K.domAPI = _(), K.insertStyleElement = H(), B()(Z.Z, K), Z.Z && Z.Z.locals && Z.Z.locals;
-            var J = t(4238),
-                $ = t(926);
+            var J = t(2380),
+                $ = t(452);
             const X = [],
                 q = {
                     saveState: !1
                 };
 
             function* Q(e) {
                 for (const n of e.widgets)
@@ -748,15 +748,15 @@
                     autoStart: !0,
                     activate: (e, n) => {
                         n.registerWidget({
                             name: "@jupyter-widgets/controls",
                             version: I.N,
                             exports: () => new Promise(((e, n) => {
                                 t.e(863).then((n => {
-                                    e(t(6530))
+                                    e(t(342))
                                 }).bind(null, t)).catch((e => {
                                     n(e)
                                 }))
                             }))
                         })
                     }
                 },
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js` & `jupyterlab_widgets-3.0.9/labextension/static/291.cff5ef71b29e18850479.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/336.9f709c2076672b1bfe2b.js` & `jupyterlab_widgets-3.0.9/labextension/static/336.ebc7a55ea1768712771f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
                 ManagerBase: () => v,
                 base64ToBuffer: () => d,
                 bufferToBase64: () => m,
                 bufferToHex: () => a,
                 hexToBuffer: () => i,
                 serialize_state: () => b
             });
-            var s = o(9890),
+            var s = o(4869),
                 n = o(7930),
                 r = o(5766);
             const l = ["00", "01", "02", "03", "04", "05", "06", "07", "08", "09", "0A", "0B", "0C", "0D", "0E", "0F", "10", "11", "12", "13", "14", "15", "16", "17", "18", "19", "1A", "1B", "1C", "1D", "1E", "1F", "20", "21", "22", "23", "24", "25", "26", "27", "28", "29", "2A", "2B", "2C", "2D", "2E", "2F", "30", "31", "32", "33", "34", "35", "36", "37", "38", "39", "3A", "3B", "3C", "3D", "3E", "3F", "40", "41", "42", "43", "44", "45", "46", "47", "48", "49", "4A", "4B", "4C", "4D", "4E", "4F", "50", "51", "52", "53", "54", "55", "56", "57", "58", "59", "5A", "5B", "5C", "5D", "5E", "5F", "60", "61", "62", "63", "64", "65", "66", "67", "68", "69", "6A", "6B", "6C", "6D", "6E", "6F", "70", "71", "72", "73", "74", "75", "76", "77", "78", "79", "7A", "7B", "7C", "7D", "7E", "7F", "80", "81", "82", "83", "84", "85", "86", "87", "88", "89", "8A", "8B", "8C", "8D", "8E", "8F", "90", "91", "92", "93", "94", "95", "96", "97", "98", "99", "9A", "9B", "9C", "9D", "9E", "9F", "A0", "A1", "A2", "A3", "A4", "A5", "A6", "A7", "A8", "A9", "AA", "AB", "AC", "AD", "AE", "AF", "B0", "B1", "B2", "B3", "B4", "B5", "B6", "B7", "B8", "B9", "BA", "BB", "BC", "BD", "BE", "BF", "C0", "C1", "C2", "C3", "C4", "C5", "C6", "C7", "C8", "C9", "CA", "CB", "CC", "CD", "CE", "CF", "D0", "D1", "D2", "D3", "D4", "D5", "D6", "D7", "D8", "D9", "DA", "DB", "DC", "DD", "DE", "DF", "E0", "E1", "E2", "E3", "E4", "E5", "E6", "E7", "E8", "E9", "EA", "EB", "EC", "ED", "EE", "EF", "F0", "F1", "F2", "F3", "F4", "F5", "F6", "F7", "F8", "F9", "FA", "FB", "FC", "FD", "FE", "FF"];
 
             function a(e) {
                 const t = new Uint8Array(e),
                     o = [];
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/345.17494fea1ff555b26294.js` & `jupyterlab_widgets-3.0.9/labextension/static/345.17494fea1ff555b26294.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/495.b58859516292ffe4bc96.js` & `jupyterlab_widgets-3.0.9/labextension/static/495.79062b4ce5ec7920dcb1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -151,15 +151,15 @@
                 serialize_naive: () => ge,
                 serialize_time: () => ie,
                 time_serializers: () => le,
                 typeset: () => a,
                 uuid: () => i.uuid,
                 version: () => ws
             });
-            var i = s(9890);
+            var i = s(4869);
 
             function a(e, t) {
                 void 0 !== t && (e.textContent = t), void 0 !== window.MathJax && MathJax.Hub.Queue(["Typeset", MathJax.Hub, e])
             }
 
             function l(e) {
                 const t = document.createElement("div");
@@ -3816,12 +3816,12 @@
                 warning: ["mod-warning"],
                 danger: ["mod-danger"]
             };
             const ws = s(7021).i8
         },
         7021: e => {
             e.exports = {
-                i8: "5.0.6"
+                i8: "5.0.7"
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/595.942a65706d9bc281d5ca.js` & `jupyterlab_widgets-3.0.9/labextension/static/595.74686e2543ce21f10975.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,43 +1,43 @@
 "use strict";
 (self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || []).push([
     [595], {
         9185: (e, t, s) => {
             s.r(t), s.d(t, {
                 BROKEN_FILE_SVG_ICON: () => f,
-                DOMWidgetModel: () => W,
-                DOMWidgetView: () => J,
-                ErrorWidgetView: () => K,
-                IJupyterWidgetRegistry: () => q,
+                DOMWidgetModel: () => z,
+                DOMWidgetView: () => V,
+                ErrorWidgetView: () => q,
+                IJupyterWidgetRegistry: () => H,
                 JUPYTER_WIDGETS_VERSION: () => x,
-                JupyterLuminoPanelWidget: () => I,
-                JupyterLuminoWidget: () => N,
-                JupyterPhosphorWidget: () => V,
-                LayoutModel: () => U,
-                LayoutView: () => $,
+                JupyterLuminoPanelWidget: () => N,
+                JupyterLuminoWidget: () => W,
+                JupyterPhosphorWidget: () => T,
+                LayoutModel: () => J,
+                LayoutView: () => D,
                 PROTOCOL_VERSION: () => S,
-                StyleModel: () => R,
-                StyleView: () => B,
-                ViewList: () => G,
-                WidgetModel: () => A,
-                WidgetView: () => T,
+                StyleModel: () => U,
+                StyleView: () => $,
+                ViewList: () => B,
+                WidgetModel: () => C,
+                WidgetView: () => A,
                 assign: () => a,
-                createErrorWidgetModel: () => F,
-                createErrorWidgetView: () => Y,
+                createErrorWidgetModel: () => G,
+                createErrorWidgetView: () => F,
                 difference: () => r,
                 isEqual: () => l,
                 isObject: () => m,
                 isSerializable: () => _,
-                pack_models: () => z,
+                pack_models: () => L,
                 put_buffers: () => u,
                 reject: () => d,
                 remove_buffers: () => g,
                 resolvePromisesDict: () => h,
-                shims: () => H,
-                unpack_models: () => C,
+                shims: () => R,
+                unpack_models: () => P,
                 uuid: () => c
             });
             var i = s(7930),
                 n = s(8149),
                 o = s.n(n);
 
             function r(e, t) {
@@ -219,46 +219,44 @@
                     return this
                 }
             }
             var O = s(5633),
                 E = s(8778);
             const x = "2.0.0",
                 S = "2.1.0",
-                M = "IPY_MODEL_",
-                P = e => JSON.parse(JSON.stringify(e)),
-                L = globalThis.structuredClone || P;
+                M = "IPY_MODEL_";
 
-            function C(e, t) {
+            function P(e, t) {
                 if (Array.isArray(e)) {
                     const s = [];
-                    for (const i of e) s.push(C(i, t));
+                    for (const i of e) s.push(P(i, t));
                     return Promise.all(s)
                 }
                 if (e instanceof Object && "string" != typeof e) {
                     const s = {};
-                    for (const [i, n] of Object.entries(e)) s[i] = C(n, t);
+                    for (const [i, n] of Object.entries(e)) s[i] = P(n, t);
                     return h(s)
                 }
                 return "string" == typeof e && e.slice(0, 10) === M ? t.get_model(e.slice(10, e.length)) : Promise.resolve(e)
             }
 
-            function z(e, t) {
+            function L(e, t) {
                 if (Array.isArray(e)) {
                     const s = [];
-                    for (const i of e) s.push(z(i, t));
+                    for (const i of e) s.push(L(i, t));
                     return s
                 }
-                if (e instanceof A) return `${M}${e.model_id}`;
+                if (e instanceof C) return `${M}${e.model_id}`;
                 if (!(e instanceof Object && "string" != typeof e)) return e;
                 {
                     const s = {};
-                    for (const [i, n] of Object.entries(e)) s[i] = z(n, t)
+                    for (const [i, n] of Object.entries(e)) s[i] = L(n, t)
                 }
             }
-            class A extends v.Model {
+            class C extends v.Model {
                 defaults() {
                     return {
                         _model_module: "@jupyter-widgets/base",
                         _model_name: "WidgetModel",
                         _model_module_version: x,
                         _view_module: "@jupyter-widgets/base",
                         _view_name: null,
@@ -403,19 +401,15 @@
                     this._attrsToUpdate.forEach((t => {
                         this._expectedEchoMsgIds.set(t, e)
                     })), this._attrsToUpdate = new Set
                 }
                 serialize(e) {
                     const t = this.constructor.serializers || i.JSONExt.emptyObject;
                     for (const s of Object.keys(e)) try {
-                        const n = t[s] || i.JSONExt.emptyObject;
-                        let {
-                            serialize: o
-                        } = n;
-                        null == o && n.deserialize === C && (o = P), e[s] = o ? o(e[s], this) : L(e[s]), e[s] && e[s].toJSON && (e[s] = e[s].toJSON())
+                        t[s] && t[s].serialize ? e[s] = t[s].serialize(e[s], this) : e[s] = JSON.parse(JSON.stringify(e[s])), e[s] && e[s].toJSON && (e[s] = e[s].toJSON())
                     } catch (e) {
                         throw console.error("Error serializing widget state attribute: ", s), e
                     }
                     return e
                 }
                 send_sync_message(e, t = {}) {
                     if (!this.comm) return "";
@@ -462,32 +456,32 @@
                     if (s) {
                         i = {};
                         for (const n in e) s[n] && s[n].deserialize ? i[n] = s[n].deserialize(e[n], t) : i[n] = e[n]
                     } else i = e;
                     return h(i)
                 }
             }
-            class W extends A {
+            class z extends C {
                 defaults() {
                     return a(super.defaults(), {
                         _dom_classes: [],
                         tabbable: null,
                         tooltip: null
                     })
                 }
             }
-            W.serializers = Object.assign(Object.assign({}, A.serializers), {
+            z.serializers = Object.assign(Object.assign({}, C.serializers), {
                 layout: {
-                    deserialize: C
+                    deserialize: P
                 },
                 style: {
-                    deserialize: C
+                    deserialize: P
                 }
             });
-            class T extends j {
+            class A extends j {
                 constructor(e) {
                     super(e)
                 }
                 initialize(e) {
                     this.listenTo(this.model, "change", ((e, t) => {
                         const s = Object.keys(this.model.changedAttributes() || {});
                         "_view_count" === s[0] && 1 === s.length || this.update(t)
@@ -518,41 +512,41 @@
                 touch() {
                     this.model.save_changes(this.callbacks())
                 }
                 remove() {
                     return super.remove(), this.trigger("remove"), this
                 }
             }
-            class N extends E.Widget {
+            class W extends E.Widget {
                 constructor(e) {
                     const t = e.view;
                     delete e.view, super(e), this._view = t
                 }
                 dispose() {
                     this.isDisposed || (super.dispose(), this._view.remove(), this._view = null)
                 }
                 processMessage(e) {
                     super.processMessage(e), this._view.processLuminoMessage(e)
                 }
             }
-            const V = N;
-            class I extends E.Panel {
+            const T = W;
+            class N extends E.Panel {
                 constructor(e) {
                     const t = e.view;
                     delete e.view, super(e), this._view = t
                 }
                 processMessage(e) {
                     super.processMessage(e), this._view.processLuminoMessage(e)
                 }
                 dispose() {
                     var e;
                     this.isDisposed || (super.dispose(), null === (e = this._view) || void 0 === e || e.remove(), this._view = null)
                 }
             }
-            class J extends T {
+            class V extends A {
                 initialize(e) {
                     super.initialize(e), this.listenTo(this.model, "change:_dom_classes", ((e, t) => {
                         const s = e.previous("_dom_classes");
                         this.update_classes(s, t)
                     })), this.layoutPromise = Promise.resolve(), this.listenTo(this.model, "change:layout", ((e, t) => {
                         this.setLayout(t, e.previous("layout"))
                     })), this.stylePromise = Promise.resolve(), this.listenTo(this.model, "change:style", ((e, t) => {
@@ -591,15 +585,15 @@
                 }
                 set_mapped_classes(e, t, s) {
                     const i = this.model.get(t),
                         n = e[i] ? e[i] : [];
                     this.update_classes([], n, s || this.el)
                 }
                 _setElement(e) {
-                    this.luminoWidget && this.luminoWidget.dispose(), this.$el = e instanceof y() ? e : y()(e), this.el = this.$el[0], this.luminoWidget = new N({
+                    this.luminoWidget && this.luminoWidget.dispose(), this.$el = e instanceof y() ? e : y()(e), this.el = this.$el[0], this.luminoWidget = new W({
                         node: e,
                         view: this
                     })
                 }
                 remove() {
                     return this.luminoWidget && this.luminoWidget.dispose(), super.remove()
                 }
@@ -619,15 +613,15 @@
                     const e = this.model.get("tabbable");
                     !0 === e ? this.el.setAttribute("tabIndex", "0") : !1 === e ? this.el.setAttribute("tabIndex", "-1") : null === e && this.el.removeAttribute("tabIndex")
                 }
                 get pWidget() {
                     return this.luminoWidget
                 }
             }
-            const D = {
+            const I = {
                 align_content: null,
                 align_items: null,
                 align_self: null,
                 border_top: null,
                 border_right: null,
                 border_bottom: null,
                 border_left: null,
@@ -660,26 +654,26 @@
                 grid_template_rows: null,
                 grid_template_columns: null,
                 grid_template_areas: null,
                 grid_row: null,
                 grid_column: null,
                 grid_area: null
             };
-            class U extends A {
+            class J extends C {
                 defaults() {
                     return a(super.defaults(), {
                         _model_name: "LayoutModel",
                         _view_name: "LayoutView"
-                    }, D)
+                    }, I)
                 }
             }
-            class $ extends T {
+            class D extends A {
                 initialize(e) {
                     this._traitNames = [], super.initialize(e);
-                    for (const e of Object.keys(D)) this.registerTrait(e)
+                    for (const e of Object.keys(I)) this.registerTrait(e)
                 }
                 registerTrait(e) {
                     this._traitNames.push(e), this.listenTo(this.model, "change:" + e, ((t, s) => {
                         this.handleChange(e, s)
                     })), this.handleChange(e, this.model.get(e))
                 }
                 css_name(e) {
@@ -692,25 +686,25 @@
                 unlayout() {
                     const e = this.options.parent;
                     this._traitNames.forEach((t => {
                         e ? e.el.style.removeProperty(this.css_name(t)) : console.warn("Style not removed because a parent view does not exist")
                     }), this)
                 }
             }
-            class R extends A {
+            class U extends C {
                 defaults() {
                     const e = this.constructor;
                     return a(super.defaults(), {
                         _model_name: "StyleModel",
                         _view_name: "StyleView"
                     }, Object.keys(e.styleProperties).reduce(((t, s) => (t[s] = e.styleProperties[s].default, t)), {}))
                 }
             }
-            R.styleProperties = {};
-            class B extends T {
+            U.styleProperties = {};
+            class $ extends A {
                 initialize(e) {
                     this._traitNames = [], super.initialize(e);
                     const t = this.model.constructor;
                     for (const e of Object.keys(t.styleProperties)) this.registerTrait(e);
                     this.style()
                 }
                 registerTrait(e) {
@@ -743,15 +737,15 @@
                                 n = t[s].selector,
                                 o = n ? e.el.querySelectorAll(n) : [e.el];
                             for (let e = 0; e !== o.length; ++e) o[e].style.removeProperty(i)
                         } else console.warn("Style not removed because a parent view does not exist")
                     }), this)
                 }
             }
-            var H;
+            var R;
             ! function(e) {
                 let t;
                 ! function(e) {
                     e.CommManager = class {
                         constructor(e) {
                             this.targets = Object.create(null), this.comms = Object.create(null), this.init_kernel(e)
                         }
@@ -827,16 +821,16 @@
                                         t.iopub.output(e)
                                 }
                             })
                         }
                     }
                     e.Comm = t
                 }(t = e.services || (e.services = {}))
-            }(H || (H = {}));
-            class G {
+            }(R || (R = {}));
+            class B {
                 constructor(e, t, s) {
                     this.initialize(e, t, s)
                 }
                 initialize(e, t, s) {
                     this._handler_context = s || this, this._models = [], this.views = [], this._create_view = e, this._remove_view = t || function(e) {
                         e.remove()
                     }
@@ -860,31 +854,31 @@
                         e.forEach((e => this._remove_view.call(this._handler_context, e))), this.views = [], this._models = []
                     }))
                 }
                 dispose() {
                     this.views = null, this._models = null
                 }
             }
-            const q = new i.Token("jupyter.extensions.jupyterWidgetRegistry");
+            const H = new i.Token("jupyter.extensions.jupyterWidgetRegistry");
 
-            function F(e, t) {
-                return class extends W {
+            function G(e, t) {
+                return class extends z {
                     constructor(s, i) {
                         super(s = Object.assign(Object.assign({}, s), {
                             _view_name: "ErrorWidgetView",
                             _view_module: "@jupyter-widgets/base",
                             _model_module_version: x,
                             _view_module_version: x,
                             msg: t,
                             error: e
                         }), i), this.comm_live = !0
                     }
                 }
             }
-            class K extends J {
+            class q extends V {
                 generateErrorMessage() {
                     return {
                         msg: this.model.get("msg"),
                         stack: String(this.model.get("error").stack)
                     }
                 }
                 render() {
@@ -901,16 +895,16 @@
                         s.classList.contains("icon-error") && (o = o || s.clientHeight, n = n || s.clientWidth, s.classList.remove("icon-error"), s.innerHTML = `\n        <pre>[Open Browser Console for more detailed log - Double click to close this message]\n${e}\n${t}</pre>\n        `, s.style.height = `${o}px`, s.style.width = `${n}px`, s.classList.add("text-error"))
                     }, this.el.ondblclick = () => {
                         s.classList.contains("text-error") && (s.classList.remove("text-error"), s.innerHTML = f, s.append(i), s.classList.add("icon-error"))
                     }
                 }
             }
 
-            function Y(e, t) {
-                return class extends K {
+            function F(e, t) {
+                return class extends q {
                     generateErrorMessage() {
                         return {
                             msg: t,
                             stack: String(e instanceof Error ? e.stack : e)
                         }
                     }
                 }
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/596.1f32fb4ed861227b46e2.js` & `jupyterlab_widgets-3.0.9/labextension/static/596.df8214a14175baf1ee16.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     [596, 965], {
         2965: (e, t, u) => {
             u.r(t), u.d(t, {
                 OUTPUT_WIDGET_VERSION: () => _,
                 OutputModel: () => d,
                 OutputView: () => l
             });
-            var s = u(9890);
+            var s = u(4869);
             const _ = "1.0.0";
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: "OutputModel",
                         _view_name: "OutputView",
                         _model_module: "@jupyter-widgets/output",
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/644.52a1098a3a5f3e45abff.js` & `jupyterlab_widgets-3.0.9/labextension/static/644.558670f1aa9ae5791769.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1052,15 +1052,15 @@
                     n = null == t ? 0 : t.length;
                 for (this.__data__ = new r; ++e < n;) this.add(t[e])
             }
             s.prototype.add = s.prototype.push = i, s.prototype.has = o, t.exports = s
         },
         6571: (t, e, n) => {
             var r = n(235),
-                i = n(5243),
+                i = n(9777),
                 o = n(2858),
                 s = n(4417),
                 a = n(8605),
                 u = n(1418);
 
             function c(t) {
                 var e = this.__data__ = new r(t);
@@ -1675,15 +1675,15 @@
                 var e = -1,
                     n = Array(t.size);
                 return t.forEach((function(t) {
                     n[++e] = t
                 })), n
             }
         },
-        5243: (t, e, n) => {
+        9777: (t, e, n) => {
             var r = n(235);
             t.exports = function() {
                 this.__data__ = new r, this.size = 0
             }
         },
         2858: t => {
             t.exports = function(t) {
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/699.e966b1425a7d4e8c3f4e.js` & `jupyterlab_widgets-3.0.9/labextension/static/699.e966b1425a7d4e8c3f4e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/965.22fa53da8ad2a8da593a.js` & `jupyterlab_widgets-3.0.9/labextension/static/965.9a2bfc1116cea35345ca.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     [965, 596], {
         2965: (e, t, u) => {
             u.r(t), u.d(t, {
                 OUTPUT_WIDGET_VERSION: () => _,
                 OutputModel: () => d,
                 OutputView: () => l
             });
-            var s = u(9890);
+            var s = u(4869);
             const _ = "1.0.0";
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: "OutputModel",
                         _view_name: "OutputView",
                         _model_module: "@jupyter-widgets/output",
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/remoteEntry.98b8a827bfc5f86e95d2.js` & `jupyterlab_widgets-3.0.9/labextension/static/remoteEntry.a37e37c87d212fe85e13.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, u, l, f, d, s, c, p, b, h, m, g, v, y, j, w, P, S, k = {
+    var e, r, t, a, n, o, i, u, l, d, f, s, c, p, b, h, m, g, v, y, j, w, P, S, k = {
             5348: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(890), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134))),
-                        "./extension": () => Promise.all([t.e(890), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134)))
+                        "./index": () => Promise.all([t.e(869), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134))),
+                        "./extension": () => Promise.all([t.e(869), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var a = "default",
@@ -45,65 +45,65 @@
         for (var t in r) _.o(r, t) && !_.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => (863 === e ? "@jupyter-widgets/controls" : e) + "." + {
         61: "21f571face17e35076c2",
         67: "760f0b2ce7647388b914",
-        113: "6113d19fca7ff66ccc66",
-        134: "b4eddbb09f5fd50a4007",
+        113: "e4cfda62b59ddbe550d3",
+        134: "a63a8d293fb35a52dc25",
         291: "cff5ef71b29e18850479",
-        336: "9f709c2076672b1bfe2b",
+        336: "ebc7a55ea1768712771f",
         345: "17494fea1ff555b26294",
         388: "7b9bc65ab3b0b744fe93",
-        495: "b58859516292ffe4bc96",
-        595: "942a65706d9bc281d5ca",
-        596: "1f32fb4ed861227b46e2",
+        495: "79062b4ce5ec7920dcb1",
+        595: "74686e2543ce21f10975",
+        596: "df8214a14175baf1ee16",
         633: "2cbcc5998e25c5521f72",
-        644: "52a1098a3a5f3e45abff",
+        644: "558670f1aa9ae5791769",
         699: "e966b1425a7d4e8c3f4e",
         863: "f3d34622f50c9be50b4f",
-        890: "147c36e3b30d7baedc95",
+        869: "19bd6b2dbf5f1e6c9f81",
         930: "b32c52301e934bfecc7d",
-        965: "22fa53da8ad2a8da593a"
+        965: "9a2bfc1116cea35345ca"
     } [e] + ".js?v=" + {
         61: "21f571face17e35076c2",
         67: "760f0b2ce7647388b914",
-        113: "6113d19fca7ff66ccc66",
-        134: "b4eddbb09f5fd50a4007",
+        113: "e4cfda62b59ddbe550d3",
+        134: "a63a8d293fb35a52dc25",
         291: "cff5ef71b29e18850479",
-        336: "9f709c2076672b1bfe2b",
+        336: "ebc7a55ea1768712771f",
         345: "17494fea1ff555b26294",
         388: "7b9bc65ab3b0b744fe93",
-        495: "b58859516292ffe4bc96",
-        595: "942a65706d9bc281d5ca",
-        596: "1f32fb4ed861227b46e2",
+        495: "79062b4ce5ec7920dcb1",
+        595: "74686e2543ce21f10975",
+        596: "df8214a14175baf1ee16",
         633: "2cbcc5998e25c5521f72",
-        644: "52a1098a3a5f3e45abff",
+        644: "558670f1aa9ae5791769",
         699: "e966b1425a7d4e8c3f4e",
         863: "f3d34622f50c9be50b4f",
-        890: "147c36e3b30d7baedc95",
+        869: "19bd6b2dbf5f1e6c9f81",
         930: "b32c52301e934bfecc7d",
-        965: "22fa53da8ad2a8da593a"
+        965: "9a2bfc1116cea35345ca"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-widgets/jupyterlab-manager:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, u;
             if (void 0 !== n)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var f = l[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
             var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
@@ -139,15 +139,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@jupyter-widgets/base-manager", "1.0.6", (() => Promise.all([_.e(113), _.e(890), _.e(930), _.e(336)]).then((() => () => _(6110))))), u("@jupyter-widgets/base", "6.0.5", (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))), u("@jupyter-widgets/controls", "5.0.6", (() => Promise.all([_.e(345), _.e(890), _.e(67), _.e(633), _.e(495), _.e(388), _.e(61)]).then((() => () => _(2495))))), u("@jupyter-widgets/jupyterlab-manager", "5.0.8", (() => Promise.all([_.e(890), _.e(67), _.e(930), _.e(388), _.e(134)]).then((() => () => _(134))))), u("@jupyter-widgets/output", "6.0.5", (() => Promise.all([_.e(890), _.e(965)]).then((() => () => _(2965))))), u("jquery", "3.7.0", (() => _.e(291).then((() => () => _(8291))))), u("semver", "7.5.1", (() => _.e(699).then((() => () => _(7699)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupyter-widgets/base-manager", "1.0.7", (() => Promise.all([_.e(113), _.e(869), _.e(930), _.e(336)]).then((() => () => _(6110))))), u("@jupyter-widgets/base", "6.0.6", (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))), u("@jupyter-widgets/controls", "5.0.7", (() => Promise.all([_.e(345), _.e(869), _.e(67), _.e(633), _.e(495), _.e(388), _.e(61)]).then((() => () => _(2495))))), u("@jupyter-widgets/jupyterlab-manager", "5.0.9", (() => Promise.all([_.e(869), _.e(67), _.e(930), _.e(388), _.e(134)]).then((() => () => _(134))))), u("@jupyter-widgets/output", "6.0.6", (() => Promise.all([_.e(869), _.e(965)]).then((() => () => _(2965))))), u("jquery", "3.7.0", (() => _.e(291).then((() => () => _(8291))))), u("semver", "7.5.1", (() => _.e(699).then((() => () => _(7699)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -197,31 +197,31 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > a && !n : "" == s != n);
-                if ("u" == d) {
+                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == s ? u > a && !n : "" == s != n);
+                if ("u" == f) {
                     if (!l || "u" != s) return !1
                 } else if (l)
-                    if (s == d)
+                    if (s == f)
                         if (u <= a) {
-                            if (f != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (n ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (n ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= a || d < s != n) return !1;
+                    if (u <= a || f < s != n) return !1;
                     l = !1
                 } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
@@ -235,66 +235,66 @@
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
+    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = l(e, t);
-        return o(a, n) || p(f(e, t, n, a)), h(e[t][n])
+        return o(a, n) || p(d(e, t, n, a)), h(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, c = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, b = (e, r, t, a) => {
         p(c(e, r, t, a))
     }, h = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, a, n) {
         var o = _.I(r);
         return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
-    })(((e, r, t, a) => r && _.o(r, t) ? h(u(r, t)) : a())), v = m(((e, r, t, a) => (i(e, t), h(s(r, t, a) || b(r, e, t, a) || u(r, t))))), y = m(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), j = m(((e, r, t, a, n) => {
+    })(((e, r, t, a) => r && _.o(r, t) ? h(u(r, t)) : a())), v = m(((e, r, t, a) => (i(e, t), h(s(r, t, a) || b(r, e, t, a) || u(r, t))))), y = m(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), j = m(((e, r, t, a, n) => {
         var o = r && _.o(r, t) && s(r, t, a);
         return o ? h(o) : n()
     })), w = {}, P = {
-        9890: () => j("default", "@jupyter-widgets/base", [1, 6, 0, 5], (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))),
+        4869: () => j("default", "@jupyter-widgets/base", [1, 6, 0, 6], (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))),
         2994: () => j("default", "jquery", [1, 3, 1, 1], (() => _.e(291).then((() => () => _(8291))))),
         8778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
         7930: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
         6697: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
-        56: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
-        926: () => y("default", "@jupyterlab/translation", [1, 4, 0, 2]),
-        1919: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 2]),
+        452: () => y("default", "@jupyterlab/translation", [1, 4, 0, 5]),
+        1426: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 5]),
+        2212: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 5]),
+        2380: () => y("default", "@jupyterlab/services", [1, 7, 0, 5]),
         3004: () => y("default", "@lumino/properties", [1, 2, 0, 0]),
-        3363: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 2]),
-        4238: () => y("default", "@jupyterlab/services", [1, 7, 0, 2]),
-        4470: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 2]),
-        4826: () => y("default", "@jupyterlab/mainmenu", [1, 4, 0, 2]),
-        7482: () => j("default", "@jupyter-widgets/base-manager", [1, 1, 0, 6], (() => Promise.all([_.e(113), _.e(336)]).then((() => () => _(6110))))),
+        4339: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 5]),
+        5243: () => y("default", "@jupyterlab/logconsole", [1, 4, 0, 5]),
+        7463: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 5]),
+        7631: () => j("default", "@jupyter-widgets/base-manager", [1, 1, 0, 7], (() => Promise.all([_.e(113), _.e(336)]).then((() => () => _(6110))))),
         7717: () => y("default", "@lumino/disposable", [1, 2, 0, 0]),
-        8409: () => j("default", "@jupyter-widgets/output", [1, 6, 0, 5], (() => _.e(596).then((() => () => _(2965))))),
+        8177: () => j("default", "@jupyter-widgets/output", [1, 6, 0, 6], (() => _.e(596).then((() => () => _(2965))))),
         9e3: () => j("default", "semver", [1, 7, 3, 5], (() => _.e(699).then((() => () => _(7699))))),
-        9350: () => y("default", "@jupyterlab/logconsole", [1, 4, 0, 2]),
+        9450: () => y("default", "@jupyterlab/mainmenu", [1, 4, 0, 5]),
         5633: () => y("default", "@lumino/messaging", [1, 2, 0, 0]),
         8830: () => g("default", "jquery", (() => _.e(291).then((() => () => _(8291))))),
         5593: () => y("default", "@lumino/domutils", [1, 2, 0, 0]),
-        6530: () => j("default", "@jupyter-widgets/controls", [1, 5, 0, 6], (() => Promise.all([_.e(345), _.e(633), _.e(495)]).then((() => () => _(2495)))))
+        342: () => j("default", "@jupyter-widgets/controls", [1, 5, 0, 7], (() => Promise.all([_.e(345), _.e(633), _.e(495)]).then((() => () => _(2495)))))
     }, S = {
         67: [2994, 8778],
-        134: [56, 926, 1919, 3004, 3363, 4238, 4470, 4826, 7482, 7717, 8409, 9e3, 9350],
+        134: [452, 1426, 2212, 2380, 3004, 4339, 5243, 7463, 7631, 7717, 8177, 9e3, 9450],
         388: [4901, 6697],
         495: [5593],
         595: [8830],
         633: [5633],
-        863: [6530],
-        890: [9890],
+        863: [342],
+        869: [4869],
         930: [7930]
     }, _.f.consumes = (e, r) => {
         _.o(S, e) && S[e].forEach((e => {
             if (_.o(w, e)) return r.push(w[e]);
             var t = r => {
                     w[e] = 0, _.m[e] = t => {
                         delete _.c[e], t.exports = r()
@@ -317,15 +317,15 @@
         var e = {
             513: 0
         };
         _.f.j = (r, t) => {
             var a = _.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(388|633|67|863|890|930)$/.test(r)) e[r] = 0;
+                else if (/^(86[39]|388|633|67|930)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = _.p + _.u(r),
                     i = new Error;
                 _.l(o, (t => {
                     if (_.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
```

### Comparing `jupyterlab_widgets-3.0.8/labextension/static/third-party-licenses.json` & `jupyterlab_widgets-3.0.9/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.0.6'}, 1: {'versionInfo': '1.0.7'}, 2: {'versionInfo': "*

 * *               "'5.0.7'}, 3: {'versionInfo': '6.0.6'}}"}*

```diff
@@ -1,32 +1,32 @@
 {
     "packages": [
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/base",
-            "versionInfo": "6.0.5"
+            "versionInfo": "6.0.6"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/base-manager",
-            "versionInfo": "1.0.6"
+            "versionInfo": "1.0.7"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/controls",
-            "versionInfo": "5.0.6"
+            "versionInfo": "5.0.7"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/output",
-            "versionInfo": "6.0.5"
+            "versionInfo": "6.0.6"
         },
         {
             "extractedText": "Copyright (c) 2010-2019 Jeremy Ashkenas, DocumentCloud\n\nPermission is hereby granted, free of charge, to any person\nobtaining a copy of this software and associated documentation\nfiles (the \"Software\"), to deal in the Software without\nrestriction, including without limitation the rights to use,\ncopy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the\nSoftware is furnished to do so, subject to the following\nconditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES\nOF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT\nHOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR\nOTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "backbone",
             "versionInfo": "1.4.0"
         },
```

### Comparing `jupyterlab_widgets-3.0.8/package.json` & `jupyterlab_widgets-3.0.9/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9075000000000001%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.6', '@jupyter-widgets/base-manager': '^1.0.7', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.7', '@jupyter-widgets/output': '^6.0.6'}",*

 * * "'gitHead'": "'17f68ed1b50f1c8b6843cb33f6b08161be89d3ea'",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.a37e37c87d212fe85e13.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'5.0.9'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.5",
-        "@jupyter-widgets/base-manager": "^1.0.6",
-        "@jupyter-widgets/controls": "^5.0.6",
-        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyter-widgets/base": "^6.0.6",
+        "@jupyter-widgets/base-manager": "^1.0.7",
+        "@jupyter-widgets/controls": "^5.0.7",
+        "@jupyter-widgets/output": "^6.0.6",
         "@jupyterlab/application": "^3.0.0 || ^4.0.0",
         "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
         "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
         "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
         "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
         "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
         "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
@@ -49,16 +49,21 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
+    "gitHead": "17f68ed1b50f1c8b6843cb33f6b08161be89d3ea",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.a37e37c87d212fe85e13.js"
+        },
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -88,9 +93,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.8"
+    "version": "5.0.9"
 }
```

### Comparing `jupyterlab_widgets-3.0.8/setup.cfg` & `jupyterlab_widgets-3.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.8/setup.py` & `jupyterlab_widgets-3.0.9/setup.py`

 * *Files identical despite different names*

