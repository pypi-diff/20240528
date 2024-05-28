# Comparing `tmp/liblet-1.7.5.tar.gz` & `tmp/liblet-1.7.6.tar.gz`

## Comparing `liblet-1.7.5.tar` & `liblet-1.7.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/api.rst
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/conf.py
--rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples.ipynb
--rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples.rst
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/index.rst
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/installation.rst
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/stg.svg
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/tree.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_static/custom.css
--rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_static/logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_templates/project.html
--rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_70_0.svg
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_71_0.svg
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_82_0.svg
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_83_0.svg
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_8_0.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.5/src/scripts.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/__init__.py
--rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/antlr.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/automaton.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/const.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/decorators.py
--rw-r--r--   0        0        0    21005 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/display.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/grammar.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/llvm.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/__init__.py
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/antlr_test.py
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/automaton_test.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/decorators_test.py
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/grammar_test.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/run.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/utils_test.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.5/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.5/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.5/LICENSE-GPL.txt
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.5/README.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.5/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/api.rst
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/conf.py
+-rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples.ipynb
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples.rst
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/index.rst
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/installation.rst
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/stg.svg
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/tree.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/_static/custom.css
+-rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/_static/logo.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/_templates/project.html
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples_files/examples_70_0.svg
+-rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples_files/examples_71_0.svg
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples_files/examples_82_0.svg
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples_files/examples_83_0.svg
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.6/docs/examples_files/examples_8_0.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.6/src/scripts.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/__init__.py
+-rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/antlr.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/automaton.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/const.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/decorators.py
+-rw-r--r--   0        0        0    21448 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/display.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/grammar.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/llvm.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 liblet-1.7.6/src/liblet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/__init__.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/antlr_test.py
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/automaton_test.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/decorators_test.py
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/grammar_test.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/run.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.6/src/tests/utils_test.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.6/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.6/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.6/LICENSE-GPL.txt
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.6/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.6/PKG-INFO
```

### Comparing `liblet-1.7.5/docs/api.rst` & `liblet-1.7.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/conf.py` & `liblet-1.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples.ipynb` & `liblet-1.7.6/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples.rst` & `liblet-1.7.6/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/index.rst` & `liblet-1.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/installation.rst` & `liblet-1.7.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/stg.svg` & `liblet-1.7.6/docs/stg.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/tree.svg` & `liblet-1.7.6/docs/tree.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/_static/logo.png` & `liblet-1.7.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/_templates/project.html` & `liblet-1.7.6/docs/_templates/project.html`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples_files/examples_70_0.svg` & `liblet-1.7.6/docs/examples_files/examples_70_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples_files/examples_71_0.svg` & `liblet-1.7.6/docs/examples_files/examples_71_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples_files/examples_82_0.svg` & `liblet-1.7.6/docs/examples_files/examples_82_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples_files/examples_83_0.svg` & `liblet-1.7.6/docs/examples_files/examples_83_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/docs/examples_files/examples_8_0.svg` & `liblet-1.7.6/docs/examples_files/examples_8_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/__init__.py` & `liblet-1.7.6/src/liblet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.7.5'
+__version__ = '1.7.6'
 
 from liblet.antlr import ANTLR, AnnotatedTreeWalker
 from liblet.automaton import (
   Automaton,
   BottomUpInstantaneousDescription,
   InstantaneousDescription,
   TopDownInstantaneousDescription,
```

### Comparing `liblet-1.7.5/src/liblet/antlr.py` & `liblet-1.7.6/src/liblet/antlr.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/automaton.py` & `liblet-1.7.6/src/liblet/automaton.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/decorators.py` & `liblet-1.7.6/src/liblet/decorators.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/display.py` & `liblet-1.7.6/src/liblet/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,46 +293,58 @@
 
   def _repr_svg_(self):
     return self._gv_graph_()._repr_svg_()
 
   def with_threads(self, threads):
     """Draws a *threaded* and *annotated* tree (as a graph).
 
-    Tree *threads* are arcs among tree nodes (or special nodes), more
-    precisely, a :obj:`dict` mapping annotated tree *source* nodes to a
-    :obj:`dict` whose values are *destinations* tree nodes; arcs are
-    represented as dotted arrows. Special nodes are: the *start* tree (an
-    annotated tree whose root contains the ``(type, <START>)`` item), the
-    *join* trees (annotated trees whose root contains the ``(type, <JOIN>)``
-    item) and the ``None`` value; such special nodes are represented as red
-    dots.
+    Tree *threads* are arcs among tree nodes (or special nodes), more precisely,
+    a :obj:`dict` mapping annotated tree *source* nodes to a :obj:`dict` whose
+    values are *destinations* tree nodes; arcs are represented as dotted arrows.
+    Special nodes are: the *begin* tree (an annotated tree whose root contains
+    the ``(type, <BEGIN>)`` item), the *join* trees (annotated trees whose root
+    contains the ``(type, <JOIN>)`` item) and the *end* node  (annotated trees
+    whose root contains the ``(type, <END>)`` item); such special nodes are
+    represented as red dots.
 
 
     Args: threads (dict): a dictionary representing the threads.
     """
 
     G = self._gv_graph_()
     del G.wrapped_graph().edge_attr['dir']
     G.wrapped_graph().edge_attr['arrowsize'] = '.5'
 
     node_args = {'shape': 'point', 'width': '.07', 'height': '.07', 'color': 'red'}
     edge_args = {'dir': 'forward', 'arrowhead': 'vee', 'arrowsize': '.5', 'style': 'dashed', 'color': 'red'}
 
     for node in threads:
-      if 'type' in node.root and node.root['type'] in ('<START>', '<JOIN>'):
+      if 'type' in node.root and node.root['type'] in ('<BEGIN>', '<JOIN>', '<END>'):
         G.node((node.root, node), gv_args=node_args)
-    G.node((None, None), gv_args=node_args)
 
     for node, info in threads.items():
       for nxt in info:
-        G.edge(
-          (node.root if node else None, node),
-          (info[nxt].root if info[nxt] else None, info[nxt]),
-          gv_args=edge_args,
-        )
+        if nxt == 'next':
+          G.edge(
+            (node.root, node),
+            (info[nxt].root, info[nxt]),
+            gv_args=edge_args
+          )
+        else:
+          G.node((nxt, (1, node)), gv_args={'color': 'red', 'fontcolor': 'red', 'fontsize': '10', 'width': '.04', 'height': '.04'})
+          G.edge(
+            (node.root, node),
+            (nxt, (1, node)),
+            gv_args=edge_args | {'arrowhead': 'none'}
+          )
+          G.edge(
+            (nxt, (1, node)),
+            (info[nxt].root, info[nxt]),
+            gv_args=edge_args
+          )
 
     return G
 
 
 class Graph:
   def __init__(self, arcs, sep=None):
     self.G = GVWrapper(
```

### Comparing `liblet-1.7.5/src/liblet/grammar.py` & `liblet-1.7.6/src/liblet/grammar.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/llvm.py` & `liblet-1.7.6/src/liblet/llvm.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/liblet/utils.py` & `liblet-1.7.6/src/liblet/utils.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/tests/antlr_test.py` & `liblet-1.7.6/src/tests/antlr_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/tests/automaton_test.py` & `liblet-1.7.6/src/tests/automaton_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/tests/decorators_test.py` & `liblet-1.7.6/src/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/tests/grammar_test.py` & `liblet-1.7.6/src/tests/grammar_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/src/tests/utils_test.py` & `liblet-1.7.6/src/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/LICENSE-CC.txt` & `liblet-1.7.6/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/LICENSE-GPL.txt` & `liblet-1.7.6/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/README.md` & `liblet-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/pyproject.toml` & `liblet-1.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liblet-1.7.5/PKG-INFO` & `liblet-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liblet
-Version: 1.7.5
+Version: 1.7.6
 Summary: A teaching aid library for formal languages and compiler courses.
 Project-URL: Documentation, https://liblet.readthedocs.io/
 Project-URL: Source code, https://github.com/let-unimi/liblet
 Project-URL: Changelog, https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt
 Project-URL: Bug Tracker, https://github.com/let-unimi/liblet/issues
 Author-email: Massimo Santini <massimo.santini@unimi.it>
 License-File: LICENSE-CC.txt
```

