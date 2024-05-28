# Comparing `tmp/ipymario-0.0.0.tar.gz` & `tmp/ipymario-0.1.0.tar.gz`

## Comparing `ipymario-0.0.0.tar` & `ipymario-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ipymario-0.0.0/.DS_Store
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 ipymario-0.0.0/demo.ipynb
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ipymario-0.0.0/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ipymario-0.0.0/src/ipymario/.DS_Store
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 ipymario-0.0.0/src/ipymario/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ipymario-0.0.0/src/ipymario/static/widget.css
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ipymario-0.0.0/src/ipymario/static/widget.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipymario-0.0.0/.gitignore
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ipymario-0.0.0/README.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ipymario-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ipymario-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 ipymario-0.1.0/demo.ipynb
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ipymario-0.1.0/src/ipymario/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ipymario-0.1.0/src/ipymario/static/widget.css
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 ipymario-0.1.0/src/ipymario/static/widget.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipymario-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ipymario-0.1.0/LICENSE
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ipymario-0.1.0/README.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ipymario-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 ipymario-0.1.0/PKG-INFO
```

### Comparing `ipymario-0.0.0/demo.ipynb` & `ipymario-0.1.0/demo.ipynb`

 * *Files identical despite different names*

### Comparing `ipymario-0.0.0/src/ipymario/__init__.py` & `ipymario-0.1.0/src/ipymario/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import importlib.metadata
 import pathlib
 
 import anywidget
-import traitlets
 import numpy as np
+import traitlets
 
 try:
     __version__ = importlib.metadata.version("ipymario")
 except importlib.metadata.PackageNotFoundError:
     __version__ = "unknown"
 
 
 colors = {
-  'O': [0, 0, 0, 255],
-  'X': [247, 82, 0, 255],
-  ' ': [247, 186, 119, 255],
+    "O": [0, 0, 0, 255],
+    "X": [247, 82, 0, 255],
+    " ": [247, 186, 119, 255],
 }
 
+# fmt: off
 box = [
     ['O', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'X', 'O'],
     ['X', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', 'O', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', 'O', ' ', 'O'],
     ['X', ' ', ' ', ' ', ' ', 'X', 'X', 'X', 'X', 'X', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', ' ', ' ', 'X', 'X', 'O', 'O', 'O', 'X', 'X', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', ' ', ' ', 'X', 'X', 'O', ' ', ' ', 'X', 'X', 'O', ' ', ' ', ' ', 'O'],
@@ -31,21 +32,23 @@
     ['X', ' ', ' ', ' ', ' ', ' ', ' ', ' ', 'O', 'O', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', ' ', ' ', ' ', ' ', ' ', 'X', 'X', ' ', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', ' ', ' ', ' ', ' ', ' ', 'X', 'X', 'O', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['X', ' ', 'O', ' ', ' ', ' ', ' ', ' ', 'O', 'O', ' ', ' ', ' ', 'O', ' ', 'O'],
     ['X', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', 'O'],
     ['O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O'],
 ]
+# fmt: on
 
 np_box = np.array([[colors[c] for c in row] for row in box], dtype=np.uint8)
 
+
 class Widget(anywidget.AnyWidget):
     _esm = pathlib.Path(__file__).parent / "static" / "widget.js"
     _css = pathlib.Path(__file__).parent / "static" / "widget.css"
     _box = traitlets.Bytes(np_box.tobytes()).tag(sync=True)
     gain = traitlets.Float(0.1).tag(sync=True)
     duration = traitlets.Float(1.0).tag(sync=True)
     size = traitlets.Int(30).tag(sync=True)
     animate = traitlets.Bool(True).tag(sync=True)
 
     def click(self):
-        self.send({ "type": "click" })
+        self.send({"type": "click"})
```

