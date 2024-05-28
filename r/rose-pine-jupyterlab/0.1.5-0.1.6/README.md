# Comparing `tmp/rose_pine_jupyterlab-0.1.5.tar.gz` & `tmp/rose_pine_jupyterlab-0.1.6.tar.gz`

## Comparing `rose_pine_jupyterlab-0.1.5.tar` & `rose_pine_jupyterlab-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.copier-answers.yml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.yarnrc.yml
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/contributing.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/install.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/license
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/package.json
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/release.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/tsconfig.json
--rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/yarn.lock
--rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine-dawn.png
--rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine-moon.png
--rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine.png
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/examples/example_notebook.ipynb
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/_version.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/517.56cb28c4b8230b0f86c3.js
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/remoteEntry.ad3e3d6d7fd32586ac09.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/index.ts
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/pallettes.d.ts
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/pallettes.ts
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine-dawn.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine-moon.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/templates.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/style/index.css
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.gitignore
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/readme.md
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/.copier-answers.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/.yarnrc.yml
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/contributing.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/install.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/license
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/package.json
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/release.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/tsconfig.json
+-rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/yarn.lock
+-rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/assets/rose-pine-dawn.png
+-rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/assets/rose-pine-moon.png
+-rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/assets/rose-pine.png
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/examples/example_notebook.ipynb
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/_version.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/remoteEntry.b5b05e313715531dc542.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/index.ts
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/pallettes.d.ts
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/pallettes.ts
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/rose-pine-dawn.json
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/rose-pine-moon.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/rose-pine.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/src/templates.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/style/index.css
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/.gitignore
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/readme.md
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.6/PKG-INFO
```

### Comparing `rose_pine_jupyterlab-0.1.5/.pre-commit-config.yaml` & `rose_pine_jupyterlab-0.1.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.4.5
     hooks:
       - id: ruff
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.1.0
     hooks:
```

### Comparing `rose_pine_jupyterlab-0.1.5/CHANGELOG.md` & `rose_pine_jupyterlab-0.1.6/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.6
+
+([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.5...d4e82be3baf220cb46ea2522ef5ca50d7cc94b62))
+
+### Maintenance and upkeep improvements
+
+- fix: :bug: secret var name [#9](https://github.com/aaravind100/jupyterlab/pull/9) ([@aaravind100](https://github.com/aaravind100))
+- chore: :construction_worker: update template to v4.3.1 [#8](https://github.com/aaravind100/jupyterlab/pull/8) ([@aaravind100](https://github.com/aaravind100))
+- update pre commit hooks [#7](https://github.com/aaravind100/jupyterlab/pull/7) ([@aaravind100](https://github.com/aaravind100))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-04-10&to=2024-05-28&type=c))
+
+[@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-04-10..2024-05-28&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.5
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.4...b770b8a44a7348efb306861e7d449108bd7095ea))
 
 ### Maintenance and upkeep improvements
 
 - update template to v4.2.6 [#6](https://github.com/aaravind100/jupyterlab/pull/6) ([@aaravind100](https://github.com/aaravind100))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-01-28&to=2024-04-10&type=c))
 
 [@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-01-28..2024-04-10&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.4
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.3...bb0738f57092f86a380e1e56aced95d4c3c22321))
 
 ### Enhancements made
 
 - refactor: :recycle: Pallette implementation out of loop [#5](https://github.com/aaravind100/jupyterlab/pull/5) ([@aaravind100](https://github.com/aaravind100))
```

### Comparing `rose_pine_jupyterlab-0.1.5/contributing.md` & `rose_pine_jupyterlab-0.1.6/contributing.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/license` & `rose_pine_jupyterlab-0.1.6/license`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/package.json` & `rose_pine_jupyterlab-0.1.6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.6'"}*

```diff
@@ -180,9 +180,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.5/tsconfig.json` & `rose_pine_jupyterlab-0.1.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/yarn.lock` & `rose_pine_jupyterlab-0.1.6/yarn.lock`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/assets/rose-pine-dawn.png` & `rose_pine_jupyterlab-0.1.6/assets/rose-pine-dawn.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/assets/rose-pine-moon.png` & `rose_pine_jupyterlab-0.1.6/assets/rose-pine-moon.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/assets/rose-pine.png` & `rose_pine_jupyterlab-0.1.6/assets/rose-pine.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/examples/example_notebook.ipynb` & `rose_pine_jupyterlab-0.1.6/examples/example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/__init__.py` & `rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/package.json` & `rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b5b05e313715531dc542.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -100,15 +100,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aaravind100/jupyterlab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ad3e3d6d7fd32586ac09.js"
+            "load": "static/remoteEntry.b5b05e313715531dc542.js"
         },
         "extension": true,
         "outputDir": "rose_pine_jupyterlab/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/517.56cb28c4b8230b0f86c3.js` & `rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkrose_pine_jupyterlab = self.webpackChunkrose_pine_jupyterlab || []).push([
     [517], {
         517: (e, p, t) => {
             t.r(p), t.d(p, {
                 default: () => d
             });
-            var l = t(464);
+            var l = t(690);
             const r = JSON.parse('{"name":"Rosé Pine","type":"dark","pallette":{"--rp-plt-base":"#191724","--rp-plt-surface":"#1f1d2e","--rp-plt-overlay":"#26233a","--rp-plt-muted":"#6e6a86","--rp-plt-subtle":"#908caa","--rp-plt-text":"#e0def4","--rp-plt-love":"#eb6f92","--rp-plt-gold":"#f6c177","--rp-plt-rose":"#ebbcba","--rp-plt-pine":"#31748f","--rp-plt-foam":"#9ccfd8","--rp-plt-iris":"#c4a7e7","--rp-plt-highlight-low":"#21202e","--rp-plt-highlight-med":"#403d52","--rp-plt-highlight-high":"#524f67"}}'),
                 a = JSON.parse('{"name":"Rosé Pine Moon","type":"dark","pallette":{"--rp-plt-base":"#232136","--rp-plt-surface":"#2a273f","--rp-plt-overlay":"#393552","--rp-plt-muted":"#6e6a86","--rp-plt-subtle":"#908caa","--rp-plt-text":"#e0def4","--rp-plt-love":"#eb6f92","--rp-plt-gold":"#f6c177","--rp-plt-rose":"#ea9a97","--rp-plt-pine":"#3e8fb0","--rp-plt-foam":"#9ccfd8","--rp-plt-iris":"#c4a7e7","--rp-plt-highlight-low":"#2a283e","--rp-plt-highlight-med":"#44415a","--rp-plt-highlight-high":"#56526e"}}'),
                 i = JSON.parse('{"name":"Rosé Pine Dawn","type":"light","pallette":{"--rp-plt-base":"#faf4ed","--rp-plt-surface":"#fffaf3","--rp-plt-overlay":"#f2e9e1","--rp-plt-muted":"#9893a5","--rp-plt-subtle":"#797593","--rp-plt-text":"#575279","--rp-plt-love":"#b4637a","--rp-plt-gold":"#ea9d34","--rp-plt-rose":"#d7827e","--rp-plt-pine":"#286983","--rp-plt-foam":"#56949f","--rp-plt-iris":"#907aa9","--rp-plt-highlight-low":"#f4ede8","--rp-plt-highlight-med":"#dfdad9","--rp-plt-highlight-high":"#cecacd"}}');
             class s {
                 constructor(e, p, t) {
                     this.name = e, this.type = p, this.pallette = t
                 }
```

### Comparing `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/remoteEntry.ad3e3d6d7fd32586ac09.js` & `rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/static/remoteEntry.b5b05e313715531dc542.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, l, s, f, p, d, c, h, v, g = {
+    var e, r, t, n, o, i, a, u, l, s, f, p, d, c, h, v, b = {
             368: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(517).then((() => () => t(517))),
                         "./extension": () => t.e(517).then((() => () => t(517)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,30 +20,30 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => i
                 })
             }
         },
-        b = {};
+        g = {};
 
     function m(e) {
-        var r = b[e];
+        var r = g[e];
         if (void 0 !== r) return r.exports;
-        var t = b[e] = {
+        var t = g[e] = {
             exports: {}
         };
-        return g[e](t, t.exports, m), t.exports
+        return b[e](t, t.exports, m), t.exports
     }
-    m.m = g, m.c = b, m.d = (e, r) => {
+    m.m = b, m.c = g, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".56cb28c4b8230b0f86c3.js?v=56cb28c4b8230b0f86c3", m.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".da5b8c1b3fb547fc39bf.js?v=da5b8c1b3fb547fc39bf", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "rose_pine_jupyterlab:", m.l = (t, n, o, i) => {
@@ -93,15 +93,15 @@
                     var o = i[e] = i[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
                         get: () => m.e(517).then((() => () => m(517))),
                         from: a,
                         eager: !1
                     })
-                })("rose_pine_jupyterlab", "0.1.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("rose_pine_jupyterlab", "0.1.6"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -195,17 +195,17 @@
         return i(n, o) || f(l(e, t, o, n)), p(e[t][o])
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var i = m.I(r);
         return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, h = {
-        464: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 6])
+        690: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 1])
     }, v = {
-        517: [464]
+        517: [690]
     }, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
```

### Comparing `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css` & `rose_pine_jupyterlab-0.1.6/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/index.ts` & `rose_pine_jupyterlab-0.1.6/src/index.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/pallettes.ts` & `rose_pine_jupyterlab-0.1.6/src/pallettes.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/rose-pine-dawn.json` & `rose_pine_jupyterlab-0.1.6/src/rose-pine-dawn.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/rose-pine-moon.json` & `rose_pine_jupyterlab-0.1.6/src/rose-pine-moon.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/rose-pine.json` & `rose_pine_jupyterlab-0.1.6/src/rose-pine.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/src/templates.json` & `rose_pine_jupyterlab-0.1.6/src/templates.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/style/variables.css` & `rose_pine_jupyterlab-0.1.6/style/variables.css`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/.gitignore` & `rose_pine_jupyterlab-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/pyproject.toml` & `rose_pine_jupyterlab-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,19 @@
 [tool.check-wheel-contents]
 ignore = ["W002"]
 
 [tool.ruff]
 target-version = "py311"
 line-length = 88
 indent-width = 4
+extend-include = ["*.ipynb"]
 
 [tool.ruff.lint]
-select = ["A", "B", "C", "E", "F", "I", "W"]
+select = ["A", "B", "C", "D", "E", "F", "I", "S", "W", "UP", "RUF"]
+ignore = ["D203", "D213"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["D104", "F401"]
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
```

### Comparing `rose_pine_jupyterlab-0.1.5/readme.md` & `rose_pine_jupyterlab-0.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.5/PKG-INFO` & `rose_pine_jupyterlab-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rose_pine_jupyterlab
-Version: 0.1.5
+Version: 0.1.6
 Dynamic: Keywords
 Summary: Soho Vibes for JupyterLab
 Project-URL: Homepage, https://github.com/aaravind100/jupyterlab
 Project-URL: Bug Tracker, https://github.com/aaravind100/jupyterlab/issues
 Project-URL: Repository, https://github.com/aaravind100/jupyterlab.git
 Author-email: Ajith Aravind <ajith.aravind100@gmail.com>
 License: BSD 3-Clause License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: rose_pine_jupyterlab Version: 0.1.5 Dynamic:
+Metadata-Version: 2.3 Name: rose_pine_jupyterlab Version: 0.1.6 Dynamic:
 Keywords Summary: Soho Vibes for JupyterLab Project-URL: Homepage, https://
 github.com/aaravind100/jupyterlab Project-URL: Bug Tracker, https://github.com/
 aaravind100/jupyterlab/issues Project-URL: Repository, https://github.com/
 aaravind100/jupyterlab.git Author-email: Ajith Aravind
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ajith Aravind All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
```

