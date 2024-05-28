# Comparing `tmp/dlg_palettegen-0.3.6.tar.gz` & `tmp/dlg_palettegen-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlg_palettegen-0.3.6.tar", last modified: Thu Apr 18 09:41:25 2024, max compression
+gzip compressed data, was "dlg_palettegen-0.3.7.tar", last modified: Tue May 28 08:44:03 2024, max compression
```

## Comparing `dlg_palettegen-0.3.6.tar` & `dlg_palettegen-0.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.553818 dlg_palettegen-0.3.6/dlg_paletteGen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33046 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/module_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    32315 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/source_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.553818 dlg_palettegen-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/PickOne.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_casatask.py
--rw-r--r--   0 runner    (1001) docker     (127)    38003 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_eagle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_oskar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_rascil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_tabascal.py
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:44:03.824390 dlg_palettegen-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 08:44:03.824390 dlg_palettegen-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:44:03.820390 dlg_palettegen-0.3.7/dlg_paletteGen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33046 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/module_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32315 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/source_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/dlg_paletteGen/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:44:03.824390 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 08:44:03.000000 dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:44:03.824390 dlg_palettegen-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:44:03.820390 dlg_palettegen-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:44:03.824390 dlg_palettegen-0.3.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/PickOne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_casatask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38003 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_eagle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_oskar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_rascil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/data/example_tabascal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-05-28 08:43:55.000000 dlg_palettegen-0.3.7/tests/test_base.py
```

### Comparing `dlg_palettegen-0.3.6/HISTORY.md` & `dlg_palettegen-0.3.7/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Changelog
 =========
 
 
-(unreleased)
-------------
+0.3.6 (2024-04-18)
+------------------
+- Release: version 0.3.6 🚀 [Andreas Wicenec]
 - Fixed value of complex types. [Andreas Wicenec]
 
 
 0.3.5 (2024-03-25)
 ------------------
 - Release: version 0.3.5 🚀 [Andreas Wicenec]
 - Release: version 0.3.4 🚀 [Andreas Wicenec]
```

### Comparing `dlg_palettegen-0.3.6/LICENSE` & `dlg_palettegen-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/PKG-INFO` & `dlg_palettegen-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg_paletteGen
-Version: 0.3.6
+Version: 0.3.7
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-benedict
 Requires-Dist: numpy
```

### Comparing `dlg_palettegen-0.3.6/README.md` & `dlg_palettegen-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/classes.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/classes.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/cli.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/cli.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/module_base.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/module_base.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/settings.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/settings.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/source_base.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/source_base.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen/support_functions.py` & `dlg_palettegen-0.3.7/dlg_paletteGen/support_functions.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/PKG-INFO` & `dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg_paletteGen
-Version: 0.3.6
+Version: 0.3.7
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-benedict
 Requires-Dist: numpy
```

### Comparing `dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/SOURCES.txt` & `dlg_palettegen-0.3.7/dlg_paletteGen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/setup.py` & `dlg_palettegen-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/PickOne.py` & `dlg_palettegen-0.3.7/tests/data/PickOne.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_casatask.py` & `dlg_palettegen-0.3.7/tests/data/example_casatask.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_eagle.py` & `dlg_palettegen-0.3.7/tests/data/example_eagle.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_functions.py` & `dlg_palettegen-0.3.7/tests/data/example_functions.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_google.py` & `dlg_palettegen-0.3.7/tests/data/example_google.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_numpy.py` & `dlg_palettegen-0.3.7/tests/data/example_numpy.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_options.py` & `dlg_palettegen-0.3.7/tests/data/example_options.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_oskar.py` & `dlg_palettegen-0.3.7/tests/data/example_oskar.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_rascil.py` & `dlg_palettegen-0.3.7/tests/data/example_rascil.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_rest.py` & `dlg_palettegen-0.3.7/tests/data/example_rest.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/data/example_tabascal.py` & `dlg_palettegen-0.3.7/tests/data/example_tabascal.py`

 * *Files identical despite different names*

### Comparing `dlg_palettegen-0.3.6/tests/test_base.py` & `dlg_palettegen-0.3.7/tests/test_base.py`

 * *Files identical despite different names*

