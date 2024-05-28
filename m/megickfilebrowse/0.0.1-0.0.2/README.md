# Comparing `tmp/megickfilebrowse-0.0.1.tar.gz` & `tmp/megickfilebrowse-0.0.2.tar.gz`

## Comparing `megickfilebrowse-0.0.1.tar` & `megickfilebrowse-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/__init__.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/megickfilebrowse.py
--rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/megickfilebrowse.pyi
--rw-r--r--   0        0        0    84721 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/component/index.js
--rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/component/style.css
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/example/index.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/demo/__init__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/demo/css.css
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/demo/requirements.txt
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/demo/space.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/Example.svelte
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/Index.svelte
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/gradio.config.js
--rw-r--r--   0        0        0   171521 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/package-lock.json
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/package.json
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/icons/light-file.svg
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/icons/light-folder.svg
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/shared/ArrowIcon.svelte
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/shared/Checkbox.svelte
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/shared/DirectoryExplorer.svelte
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/shared/FileTree.svelte
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/frontend/shared/types.ts
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/.gitignore
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/README.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/__init__.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/megickfilebrowse.py
+-rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/megickfilebrowse.pyi
+-rw-r--r--   0        0        0    84721 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/component/index.js
+-rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/component/style.css
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/example/index.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/demo/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/demo/css.css
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/demo/requirements.txt
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/demo/space.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/Example.svelte
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/Index.svelte
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/gradio.config.js
+-rw-r--r--   0        0        0   171521 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/package.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/icons/light-file.svg
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/icons/light-folder.svg
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/shared/ArrowIcon.svelte
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/shared/Checkbox.svelte
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/shared/DirectoryExplorer.svelte
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/shared/FileTree.svelte
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/frontend/shared/types.ts
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/README.md
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 megickfilebrowse-0.0.2/PKG-INFO
```

### Comparing `megickfilebrowse-0.0.1/backend/megickfilebrowse/megickfilebrowse.py` & `megickfilebrowse-0.0.2/backend/megickfilebrowse/megickfilebrowse.py`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/backend/megickfilebrowse/megickfilebrowse.pyi` & `megickfilebrowse-0.0.2/backend/megickfilebrowse/megickfilebrowse.pyi`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/component/index.js` & `megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/component/style.css` & `megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/backend/megickfilebrowse/templates/example/index.js` & `megickfilebrowse-0.0.2/backend/megickfilebrowse/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/demo/css.css` & `megickfilebrowse-0.0.2/demo/css.css`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/demo/space.py` & `megickfilebrowse-0.0.2/demo/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `megickfilebrowse`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/megickfilebrowse/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/megickfilebrowse"></a>  
 </div>
 
 An extension of Gradio's FileExplorer, with more customization.
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
```

### Comparing `megickfilebrowse-0.0.1/frontend/Example.svelte` & `megickfilebrowse-0.0.2/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/Index.svelte` & `megickfilebrowse-0.0.2/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/package-lock.json` & `megickfilebrowse-0.0.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/package.json` & `megickfilebrowse-0.0.2/frontend/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'name'": "'megickfilebrowse'", "'version'": "'0.0.2'"}*

```diff
@@ -18,12 +18,12 @@
     "exports": {
         ".": "./Index.svelte",
         "./example": "./Example.svelte",
         "./package.json": "./package.json"
     },
     "license": "apache-2.0",
     "main_changeset": true,
-    "name": "gradio_megickfilebrowse",
+    "name": "megickfilebrowse",
     "private": true,
     "type": "module",
-    "version": "0.1.1"
+    "version": "0.0.2"
 }
```

### Comparing `megickfilebrowse-0.0.1/frontend/icons/light-folder.svg` & `megickfilebrowse-0.0.2/frontend/icons/light-folder.svg`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/shared/ArrowIcon.svelte` & `megickfilebrowse-0.0.2/frontend/shared/ArrowIcon.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/shared/Checkbox.svelte` & `megickfilebrowse-0.0.2/frontend/shared/Checkbox.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/shared/DirectoryExplorer.svelte` & `megickfilebrowse-0.0.2/frontend/shared/DirectoryExplorer.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/frontend/shared/FileTree.svelte` & `megickfilebrowse-0.0.2/frontend/shared/FileTree.svelte`

 * *Files identical despite different names*

### Comparing `megickfilebrowse-0.0.1/README.md` & `megickfilebrowse-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `megickfilebrowse`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/megickfilebrowse/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/megickfilebrowse"></a>  
 
 An extension of Gradio's FileExplorer, with more customization.
 
 ## Installation
 
 ```bash
 pip install megickfilebrowse
```

### Comparing `megickfilebrowse-0.0.1/pyproject.toml` & `megickfilebrowse-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,28 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "megickfilebrowse"
-version = "0.0.1"
+version = "0.0.2"
 description = "An extension of Gradio's FileExplorer, with more customization."
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.10"
-authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
+authors = [{ name = "Mejikan", email = "mejikan@example.com" }]
 keywords = ["gradio-custom-component", "gradio-template-FileExplorer", "file"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
-  'Programming Language :: Python :: 3.8',
-  'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Topic :: Scientific/Engineering',
   'Topic :: Scientific/Engineering :: Artificial Intelligence',
   'Topic :: Scientific/Engineering :: Visualization',
 ]
```

### Comparing `megickfilebrowse-0.0.1/PKG-INFO` & `megickfilebrowse-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.3
 Name: megickfilebrowse
-Version: 0.0.1
+Version: 0.0.2
 Summary: An extension of Gradio's FileExplorer, with more customization.
-Author-email: YOUR NAME <YOUREMAIL@domain.com>
+Author-email: Mejikan <mejikan@example.com>
 License-Expression: Apache-2.0
 Keywords: file,gradio-custom-component,gradio-template-FileExplorer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.10
 Requires-Dist: gradio<5.0,>=4.0
@@ -31,15 +29,15 @@
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `megickfilebrowse`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/megickfilebrowse/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/megickfilebrowse"></a>  
 
 An extension of Gradio's FileExplorer, with more customization.
 
 ## Installation
 
 ```bash
 pip install megickfilebrowse
```

