# Comparing `tmp/trame_jupyter_extension-2.1.0.tar.gz` & `tmp/trame_jupyter_extension-2.1.1.tar.gz`

## Comparing `trame_jupyter_extension-2.1.0.tar` & `trame_jupyter_extension-2.1.1.tar`

### file list

```diff
@@ -1,37 +1,43 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.yarnrc.yml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/RELEASE.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/install.json
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/tsconfig.json
--rw-r--r--   0        0        0   227220 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/yarn.lock
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/interrupt.ipynb
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/requirements.txt
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/simple-test.ipynb
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/test_trame_jupyter_comm.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/untitled.txt
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/vtk_remote_rendering.ipynb
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/vue23.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/jupyter-config/server-config/trame_jupyter_extension.json
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/comm.ts
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/emitter.ts
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/index.ts
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/location.ts
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/manager.ts
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/registry.ts
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/utils.ts
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/websocket.ts
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/index.js
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/LICENSE
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/README.md
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/install.json
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/tsconfig.json
+-rw-r--r--   0        0        0   227220 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/yarn.lock
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/interrupt.ipynb
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/requirements.txt
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/simple-test.ipynb
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/test_trame_jupyter_comm.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/untitled.txt
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/vtk_remote_rendering.ipynb
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/examples/vue23.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/jupyter-config/server-config/trame_jupyter_extension.json
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/comm.ts
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/emitter.ts
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/index.ts
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/location.ts
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/manager.ts
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/registry.ts
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/utils.ts
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/src/websocket.ts
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/style/index.js
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/static/612.f1237fcf4c45cf215a18.js
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/static/728.5b961f2098a059c1e4b9.js
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/static/remoteEntry.39d7b892ed5465b29a60.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/trame_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/README.md
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.1/PKG-INFO
```

### Comparing `trame_jupyter_extension-2.1.0/.copier-answers.yml` & `trame_jupyter_extension-2.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/RELEASE.md` & `trame_jupyter_extension-2.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/package.json` & `trame_jupyter_extension-2.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.1.1'"}*

```diff
@@ -191,9 +191,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.1.0"
+    "version": "2.1.1"
 }
```

### Comparing `trame_jupyter_extension-2.1.0/tsconfig.json` & `trame_jupyter_extension-2.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/yarn.lock` & `trame_jupyter_extension-2.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/examples/interrupt.ipynb` & `trame_jupyter_extension-2.1.1/examples/interrupt.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/examples/simple-test.ipynb` & `trame_jupyter_extension-2.1.1/examples/simple-test.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/examples/test_trame_jupyter_comm.ipynb` & `trame_jupyter_extension-2.1.1/examples/test_trame_jupyter_comm.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/examples/vtk_remote_rendering.ipynb` & `trame_jupyter_extension-2.1.1/examples/vtk_remote_rendering.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/examples/vue23.ipynb` & `trame_jupyter_extension-2.1.1/examples/vue23.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/comm.ts` & `trame_jupyter_extension-2.1.1/src/comm.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/emitter.ts` & `trame_jupyter_extension-2.1.1/src/emitter.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/index.ts` & `trame_jupyter_extension-2.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/location.ts` & `trame_jupyter_extension-2.1.1/src/location.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/manager.ts` & `trame_jupyter_extension-2.1.1/src/manager.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/utils.ts` & `trame_jupyter_extension-2.1.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/src/websocket.ts` & `trame_jupyter_extension-2.1.1/src/websocket.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/trame_jupyter_extension/__init__.py` & `trame_jupyter_extension-2.1.1/trame_jupyter_extension/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 try:
     from ._version import __version__
 except ImportError:
     # Fallback when using the package in dev mode without installing
     # in editable mode with pip. It is highly recommended to install
     # the package from a stable release or in editable mode: https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs
     import warnings
+
     warnings.warn("Importing 'trame_jupyter_extension' outside a proper installation.")
     __version__ = "dev"
 from .handlers import setup_handlers
 
 
 def _jupyter_labextension_paths():
-    return [{
-        "src": "labextension",
-        "dest": "trame-jupyter-extension"
-    }]
+    return [{"src": "labextension", "dest": "trame-jupyter-extension"}]
 
 
 def _jupyter_server_extension_points():
-    return [{
-        "module": "trame_jupyter_extension"
-    }]
+    return [{"module": "trame_jupyter_extension"}]
 
 
 def _load_jupyter_server_extension(server_app):
     """Registers the API handler to receive HTTP requests from the frontend extension.
 
     Parameters
     ----------
     server_app: jupyterlab.labapp.LabApp
         JupyterLab application instance
     """
+    if "headers" not in server_app.web_app.settings:
+        server_app.web_app.settings["headers"] = {}
+    server_app.web_app.settings["headers"].update(
+        {
+            # Allow access to `SharedArrayBuffer`.
+            "Cross-Origin-Opener-Policy": "same-origin",
+            "Cross-Origin-Embedder-Policy": "require-corp",
+        }
+    )
+
     setup_handlers(server_app.web_app)
     name = "trame-jupyter-extension"
     server_app.log.info(f"Registered {name} server extension")
```

### Comparing `trame_jupyter_extension-2.1.0/.gitignore` & `trame_jupyter_extension-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/LICENSE` & `trame_jupyter_extension-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/README.md` & `trame_jupyter_extension-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/pyproject.toml` & `trame_jupyter_extension-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.1.0/PKG-INFO` & `trame_jupyter_extension-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trame-jupyter-extension
-Version: 2.1.0
+Version: 2.1.1
 Dynamic: Keywords
 Summary: A JupyterLab extension for trame communication layer
 Project-URL: Homepage, https://github.com/Kitware/trame-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/Kitware/trame-jupyter-extension/issues
 Project-URL: Repository, https://github.com/Kitware/trame-jupyter-extension.git
 Author-email: "Kitware Inc." <sebastien.jourdain@kitware.com>
 License: BSD 3-Clause License
```

