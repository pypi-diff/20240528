# Comparing `tmp/quokka-project-0.5.6.tar.gz` & `tmp/quokka-project-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka-project-0.5.6.tar", last modified: Thu May 16 11:55:14 2024, max compression
+gzip compressed data, was "quokka-project-0.5.7.tar", last modified: Tue May 28 21:13:56 2024, max compression
```

## Comparing `quokka-project-0.5.6.tar` & `quokka-project-0.5.7.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.886572 quokka-project-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-16 11:55:13.000000 quokka-project-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-16 11:55:14.886572 quokka-project-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-16 11:55:13.000000 quokka-project-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.882572 quokka-project-0.5.6/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.882572 quokka-project-0.5.6/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.886572 quokka-project-0.5.6/bindings/python/quokka/
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/addresser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.886572 quokka-project-0.5.6/bindings/python/quokka/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/calling_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/replacer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.886572 quokka-project-0.5.6/bindings/python/quokka/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/backends/capstone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/backends/pypcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)    23300 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/program.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25403 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/quokka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 11:55:13.000000 quokka-project-0.5.6/bindings/python/quokka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:55:14.886572 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-16 11:55:14.000000 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 11:55:14.000000 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:55:14.000000 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-16 11:55:14.000000 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 11:55:14.000000 quokka-project-0.5.6/bindings/python/quokka_project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 11:55:13.000000 quokka-project-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:55:14.886572 quokka-project-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-16 11:55:13.000000 quokka-project-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.407917 quokka-project-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-28 21:13:54.000000 quokka-project-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-28 21:13:56.407917 quokka-project-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-28 21:13:54.000000 quokka-project-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.399917 quokka-project-0.5.7/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.399917 quokka-project-0.5.7/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.403917 quokka-project-0.5.7/bindings/python/quokka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/addresser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.403917 quokka-project-0.5.7/bindings/python/quokka/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/calling_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/replacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.403917 quokka-project-0.5.7/bindings/python/quokka/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/backends/capstone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/backends/pypcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23449 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/quokka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-28 21:13:54.000000 quokka-project-0.5.7/bindings/python/quokka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:13:56.407917 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 21:13:56.000000 quokka-project-0.5.7/bindings/python/quokka_project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-28 21:13:54.000000 quokka-project-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:13:56.407917 quokka-project-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-28 21:13:54.000000 quokka-project-0.5.7/setup.py
```

### Comparing `quokka-project-0.5.6/LICENSE` & `quokka-project-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/PKG-INFO` & `quokka-project-0.5.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.6
+Version: 0.5.7
 Summary: Quokka: A Fast and Accurate Binary Exporter
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/quokka/
 Project-URL: Repository, https://github.com/quarkslab/quokka/
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
@@ -89,14 +89,25 @@
 ```
 
 Note: We are using `idat64` and not `ida64` to increase the export speed
 because we don't need the graphical interface.
 
 - Using the plugin shortcut inside IDA: (by default) Alt+A
 
+### Export a file in batch
+
+One can write its own bash script run multiple `idat64` in parallel. However,
+Quokka provides an utility tool to automatically export all executable files
+of a given directory in parallel. An example to automate the export using 8 threads:
+
+```commandline
+$ quokka-cli -t 8 dir/
+```
+
+
 ### Load an export file
 
 ```python
 import quokka
 
 # Directly from the binary (requires the IDA plugin to be installed)
 ls = quokka.Program.from_binary("/bin/ls")
```

### Comparing `quokka-project-0.5.6/README.md` & `quokka-project-0.5.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -71,14 +71,25 @@
 ```
 
 Note: We are using `idat64` and not `ida64` to increase the export speed
 because we don't need the graphical interface.
 
 - Using the plugin shortcut inside IDA: (by default) Alt+A
 
+### Export a file in batch
+
+One can write its own bash script run multiple `idat64` in parallel. However,
+Quokka provides an utility tool to automatically export all executable files
+of a given directory in parallel. An example to automate the export using 8 threads:
+
+```commandline
+$ quokka-cli -t 8 dir/
+```
+
+
 ### Load an export file
 
 ```python
 import quokka
 
 # Directly from the binary (requires the IDA plugin to be installed)
 ls = quokka.Program.from_binary("/bin/ls")
```

### Comparing `quokka-project-0.5.6/bindings/python/quokka/__init__.py` & `quokka-project-0.5.7/bindings/python/quokka/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/addresser.py` & `quokka-project-0.5.7/bindings/python/quokka/addresser.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/__init__.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/arch.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/arch.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/calling_convention.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/calling_convention.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/env.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/env.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/replacer.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/replacer.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/analysis/utils.py` & `quokka-project-0.5.7/bindings/python/quokka/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/backends/__init__.py` & `quokka-project-0.5.7/bindings/python/quokka/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/backends/capstone.py` & `quokka-project-0.5.7/bindings/python/quokka/backends/capstone.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/backends/pypcode.py` & `quokka-project-0.5.7/bindings/python/quokka/backends/pypcode.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/block.py` & `quokka-project-0.5.7/bindings/python/quokka/block.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/data.py` & `quokka-project-0.5.7/bindings/python/quokka/data.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/exc.py` & `quokka-project-0.5.7/bindings/python/quokka/exc.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/executable.py` & `quokka-project-0.5.7/bindings/python/quokka/executable.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/function.py` & `quokka-project-0.5.7/bindings/python/quokka/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,25 +544,27 @@
     Arguments:
         func: Protobuf data
         program: Program reference
 
     Attributes:
         start: Start address
         name: Function name
+        mangled_name: Function mangled name (it might be equal to the function name)
         program: Program reference
         type: Function type
         index_to_address: Mapping of Chunks to Protobuf indexes
         func: Protobuf data
     """
 
     def __init__(self, func: "quokka.pb.Quokka.Function", program: quokka.Program):
         """Constructor"""
         super(dict, self).__init__()
         self.start: int = program.addresser.absolute(func.offset)
         self.name: str = func.name
+        self.mangled_name: str = func.mangled_name or func.name
 
         self.program: quokka.Program = program
 
         self.type: "FunctionType" = FunctionType.from_proto(func.function_type)
         if self.type == FunctionType.NORMAL:
             segment = self.program.get_segment(self.start)
             if segment and segment.type == SegmentType.EXTERN:
```

### Comparing `quokka-project-0.5.6/bindings/python/quokka/instruction.py` & `quokka-project-0.5.7/bindings/python/quokka/instruction.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/program.py` & `quokka-project-0.5.7/bindings/python/quokka/program.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/reference.py` & `quokka-project-0.5.7/bindings/python/quokka/reference.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/segment.py` & `quokka-project-0.5.7/bindings/python/quokka/segment.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/structure.py` & `quokka-project-0.5.7/bindings/python/quokka/structure.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/types.py` & `quokka-project-0.5.7/bindings/python/quokka/types.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/utils.py` & `quokka-project-0.5.7/bindings/python/quokka/utils.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.6/bindings/python/quokka/version.py` & `quokka-project-0.5.7/bindings/python/quokka/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
```

### Comparing `quokka-project-0.5.6/bindings/python/quokka_project.egg-info/PKG-INFO` & `quokka-project-0.5.7/bindings/python/quokka_project.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.6
+Version: 0.5.7
 Summary: Quokka: A Fast and Accurate Binary Exporter
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/quokka/
 Project-URL: Repository, https://github.com/quarkslab/quokka/
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
@@ -89,14 +89,25 @@
 ```
 
 Note: We are using `idat64` and not `ida64` to increase the export speed
 because we don't need the graphical interface.
 
 - Using the plugin shortcut inside IDA: (by default) Alt+A
 
+### Export a file in batch
+
+One can write its own bash script run multiple `idat64` in parallel. However,
+Quokka provides an utility tool to automatically export all executable files
+of a given directory in parallel. An example to automate the export using 8 threads:
+
+```commandline
+$ quokka-cli -t 8 dir/
+```
+
+
 ### Load an export file
 
 ```python
 import quokka
 
 # Directly from the binary (requires the IDA plugin to be installed)
 ls = quokka.Program.from_binary("/bin/ls")
```

### Comparing `quokka-project-0.5.6/bindings/python/quokka_project.egg-info/SOURCES.txt` & `quokka-project-0.5.7/bindings/python/quokka_project.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 bindings/python/quokka/__init__.py
+bindings/python/quokka/__main__.py
 bindings/python/quokka/addresser.py
 bindings/python/quokka/block.py
 bindings/python/quokka/data.py
 bindings/python/quokka/exc.py
 bindings/python/quokka/executable.py
 bindings/python/quokka/function.py
 bindings/python/quokka/instruction.py
@@ -27,9 +28,10 @@
 bindings/python/quokka/analysis/utils.py
 bindings/python/quokka/backends/__init__.py
 bindings/python/quokka/backends/capstone.py
 bindings/python/quokka/backends/pypcode.py
 bindings/python/quokka_project.egg-info/PKG-INFO
 bindings/python/quokka_project.egg-info/SOURCES.txt
 bindings/python/quokka_project.egg-info/dependency_links.txt
+bindings/python/quokka_project.egg-info/entry_points.txt
 bindings/python/quokka_project.egg-info/requires.txt
 bindings/python/quokka_project.egg-info/top_level.txt
```

### Comparing `quokka-project-0.5.6/pyproject.toml` & `quokka-project-0.5.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,34 @@
 [project]
 name = "quokka-project"
 description = "Quokka: A Fast and Accurate Binary Exporter"
 authors = [{ name = "Quarkslab", email = "diffing@quarkslab.com" }]
 license = { text = "Apache Software License (Apache License, Version 2)" }
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
-dependencies = ["capstone>=4.0.2", "networkx>=2.4", "protobuf>=3.12.2"]
+dependencies = [
+    "capstone>=4.0.2",
+    "networkx>=2.4",
+    "protobuf>=3.12.2",
+
+    # Wait for python-magic to solve/merge https://github.com/ahupp/python-magic/pull/294
+    "python-magic; os_name!='nt'",
+    "python-magic-bin; os_name=='nt'",
+]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/quarkslab/quokka/"
 Repository = "https://github.com/quarkslab/quokka/"
 Documentation = "https://quarkslab.github.io/quokka/"
 "Bug Tracker" = "https://github.com/quarkslab/quokka/issues"
 
+[project.scripts]
+quokka-cli = 'quokka.__main__:main'
+
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-mock",
     "pytest-cov",
     "coverage[toml]",
     "pypcode>=2.0.0",
```

### Comparing `quokka-project-0.5.6/setup.py` & `quokka-project-0.5.7/setup.py`

 * *Files identical despite different names*

