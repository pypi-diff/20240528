# Comparing `tmp/jupyterlab_gallery-0.1.2.tar.gz` & `tmp/jupyterlab_gallery-0.1.3.tar.gz`

## Comparing `jupyterlab_gallery-0.1.2.tar` & `jupyterlab_gallery-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/babel.config.js
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/conftest.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jest.config.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/junit.xml
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/tsconfig.test.json
--rw-r--r--   0        0        0   374798 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyter-config/server-config/jupyterlab_gallery.json
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/_version.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/gitpuller.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/handlers.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/package.json
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/plugin.json
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/274.65854fd2800238c6f003.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/remoteEntry.7e7867bc630c8abba4aa.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/tests/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/jupyterlab_gallery/tests/test_handlers.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/schema/plugin.json
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/gallery.tsx
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/handler.ts
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/icons.ts
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/index.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/svg.d.ts
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/types.ts
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/src/__tests__/jupyterlab_gallery.spec.ts
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/style/icons/md/LICENSE
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/style/icons/md/gallery.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/yarn.lock
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/ui-tests/tests/jupyterlab_gallery.spec.ts
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/LICENSE
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/README.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/babel.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/conftest.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jest.config.js
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/junit.xml
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/tsconfig.test.json
+-rw-r--r--   0        0        0   382329 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyter-config/server-config/jupyterlab_gallery.json
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/_version.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/app.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/gitpuller.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/handlers.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/manager.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/package.json
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/plugin.json
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/274.78ff9c1bf7688afa9147.js
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/728.8ac417a035c29c0e6d2f.js
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/remoteEntry.cddf7f3b6d80e2c2c00f.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/tests/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/jupyterlab_gallery/tests/test_handlers.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/schema/plugin.json
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/gallery.tsx
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/handler.ts
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/icons.ts
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/index.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/svg.d.ts
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/types.ts
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/src/__tests__/jupyterlab_gallery.spec.ts
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/style/icons/md/gallery.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/README.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/ui-tests/tests/jupyterlab_gallery.spec.ts
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/README.md
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 jupyterlab_gallery-0.1.3/PKG-INFO
```

### Comparing `jupyterlab_gallery-0.1.2/.copier-answers.yml` & `jupyterlab_gallery-0.1.3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/RELEASE.md` & `jupyterlab_gallery-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/jest.config.js` & `jupyterlab_gallery-0.1.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/package.json` & `jupyterlab_gallery-0.1.3/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9776785714285715%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/launcher': '^4.0.0', 'jupyterlab-new-launcher': '^0.4.0'}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -11,26 +11,28 @@
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "A JupyterLab gallery extension for presenting and downloading examples from remote repositories",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.8.0",
         "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "jupyterlab-new-launcher": "^0.4.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^3.0.0",
         "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
         "stylelint": "^15.10.1",
@@ -202,9 +204,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_gallery-0.1.2/tsconfig.json` & `jupyterlab_gallery-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/yarn.lock` & `jupyterlab_gallery-0.1.3/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -2152,14 +2152,43 @@
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.12.1
   checksum: 96f4f9055c464fb6f0e2545d21623b9500936da44cd7bafa9c1154164f6fc1846a518bc637ef46d6a082d208d12acf737d8aa679ce5546427ac04f068cf10cd5
   languageName: node
   linkType: hard
 
+"@jupyterlab/apputils@npm:^4.3.1":
+  version: 4.3.1
+  resolution: "@jupyterlab/apputils@npm:4.3.1"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.2.1
+    "@jupyterlab/observables": ^5.2.1
+    "@jupyterlab/rendermime-interfaces": ^3.10.1
+    "@jupyterlab/services": ^7.2.1
+    "@jupyterlab/settingregistry": ^4.2.1
+    "@jupyterlab/statedb": ^4.2.1
+    "@jupyterlab/statusbar": ^4.2.1
+    "@jupyterlab/translation": ^4.2.1
+    "@jupyterlab/ui-components": ^4.2.1
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.3.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.2
+    "@types/react": ^18.0.26
+    react: ^18.2.0
+    sanitize-html: ~2.12.1
+  checksum: 380d9059dd14ee47bb50a821515e0b4a92a2b60b6fed2bf15fb73b9192a2e95d1e6c97337f11d0c26870dba2dc89ee19604f068483df505e78d798510a61bf01
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/attachments@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/attachments@npm:4.2.0"
   dependencies:
     "@jupyterlab/nbformat": ^4.2.0
     "@jupyterlab/observables": ^5.2.0
     "@jupyterlab/rendermime": ^4.2.0
@@ -2323,14 +2352,28 @@
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
   checksum: 1975f19f567b63484055b0d1d10757b2bf66274814083e50702bb6017af22341cc3f5924d0ec7da408feacd652120b476aaaf50286a5401f798f257e899aed91
   languageName: node
   linkType: hard
 
+"@jupyterlab/coreutils@npm:^6.2.1":
+  version: 6.2.1
+  resolution: "@jupyterlab/coreutils@npm:6.2.1"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    minimist: ~1.2.0
+    path-browserify: ^1.0.0
+    url-parse: ~1.5.4
+  checksum: c8167bd8d4472471297e5669d6b3ee7c9d5c1246e8413680713b15f8a81926d2c97bc6a3c0b26c16603b197b412e01b443cc74b02a3676adea5690aac41964be
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/docmanager@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/docmanager@npm:4.2.0"
   dependencies:
     "@jupyterlab/apputils": ^4.3.0
     "@jupyterlab/coreutils": ^6.2.0
     "@jupyterlab/docregistry": ^4.2.0
@@ -2421,14 +2464,32 @@
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.2
     react: ^18.2.0
   checksum: d80fdb55c25472cae56852c6ce8633a9899430e784ff60fbac956c17db60bc3eb92fdc5cf4e7b1c06e1fd5b7e37c3c4f9992e4ed7d4d800cd5c65eac43d5ac08
   languageName: node
   linkType: hard
 
+"@jupyterlab/launcher@npm:^4.0.0":
+  version: 4.2.1
+  resolution: "@jupyterlab/launcher@npm:4.2.1"
+  dependencies:
+    "@jupyterlab/apputils": ^4.3.1
+    "@jupyterlab/translation": ^4.2.1
+    "@jupyterlab/ui-components": ^4.2.1
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.3.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/widgets": ^2.3.2
+    react: ^18.2.0
+  checksum: cb376579427da1e6be1f2d5aa159430df5c984421e61abe167244da384c8598bfe96523150e3a303a200e5e3a1bbb1c2e176d81aa0425ecb5cfda20764b604a8
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/lsp@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/lsp@npm:4.2.0"
   dependencies:
     "@jupyterlab/apputils": ^4.3.0
     "@jupyterlab/codeeditor": ^4.2.0
     "@jupyterlab/codemirror": ^4.2.0
@@ -2453,14 +2514,23 @@
   resolution: "@jupyterlab/nbformat@npm:4.2.0"
   dependencies:
     "@lumino/coreutils": ^2.1.2
   checksum: adecadcb63de48f09aeb54eebfed8b77ab322c478fd903001e09780a01e7cf68f93716a2598631d4426d8ad9d3dc6349e8892db12575f74c8daea33f63b9c111
   languageName: node
   linkType: hard
 
+"@jupyterlab/nbformat@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/nbformat@npm:4.2.1"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+  checksum: 192167e2a9019bf91e1e7088c9eaaae7b1037f5e7b5db15b97687b052323e6e75913b301ca7a9783d0e59aa36f18ddff90fc71a90a8153e0c89e32fd92b2519c
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/notebook@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/notebook@npm:4.2.0"
   dependencies:
     "@jupyter/ydoc": ^2.0.1
     "@jupyterlab/apputils": ^4.3.0
     "@jupyterlab/cells": ^4.2.0
@@ -2504,14 +2574,27 @@
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
   checksum: 98460d55d8ac559c79be87fe5e105cc200556e87276daed739fd89e8393c74ba9b03f67c8ecf7a02e8d8ee1fd8a60031ced6c1b7884ab5f10c8bdb876f150c5f
   languageName: node
   linkType: hard
 
+"@jupyterlab/observables@npm:^5.2.1":
+  version: 5.2.1
+  resolution: "@jupyterlab/observables@npm:5.2.1"
+  dependencies:
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+  checksum: 3833d3ad0640a6160fdc5254ec08a600e628e235103e311ca8ee90ade11b73e045ab78b82282153da700f9ae796a99ef36da223baad6c21ad7af0ea84b9514b6
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/outputarea@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/outputarea@npm:4.2.0"
   dependencies:
     "@jupyterlab/apputils": ^4.3.0
     "@jupyterlab/nbformat": ^4.2.0
     "@jupyterlab/observables": ^5.2.0
@@ -2536,14 +2619,24 @@
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
     "@lumino/widgets": ^1.37.2 || ^2.3.2
   checksum: 08999b64a6896a4d58869ec00ca64a1b3931e01b438d471a0ad1404407f6231667f686b823a9cb482349f3d774693368320d2d4463c23fdd1de81cb4ddf34f20
   languageName: node
   linkType: hard
 
+"@jupyterlab/rendermime-interfaces@npm:^3.10.1":
+  version: 3.10.1
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.10.1"
+  dependencies:
+    "@lumino/coreutils": ^1.11.0 || ^2.1.2
+    "@lumino/widgets": ^1.37.2 || ^2.3.2
+  checksum: 537fe7d96f8e157d89de0035149bf98bfaf1b9fde92d4f58c1e879ce87cab586311aa18dfb02a218bd24aa3cd1f24122e256a70cb2a0a437cc4fea1c9a3f2fa1
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/rendermime@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/rendermime@npm:4.2.0"
   dependencies:
     "@jupyterlab/apputils": ^4.3.0
     "@jupyterlab/coreutils": ^6.2.0
     "@jupyterlab/nbformat": ^4.2.0
@@ -2575,14 +2668,33 @@
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
   checksum: edc93389913d792841b615cd0a317e16c77621cd5cb35e67c40f7a58bcf0e31c77718ae7abcf643621ba86ce78c795d6008a9413d84ecad2b42e39bd52db1447
   languageName: node
   linkType: hard
 
+"@jupyterlab/services@npm:^7.2.1":
+  version: 7.2.1
+  resolution: "@jupyterlab/services@npm:7.2.1"
+  dependencies:
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/coreutils": ^6.2.1
+    "@jupyterlab/nbformat": ^4.2.1
+    "@jupyterlab/settingregistry": ^4.2.1
+    "@jupyterlab/statedb": ^4.2.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    ws: ^8.11.0
+  checksum: f07be2f3a174466c17ab5c22f8ef622fc623e8c61f2220b8bfb465a263971313cb9129e84bba32606e6ab7d1e0be3a9754b97f98e173e9c95eaf0b1c6cd8110a
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/settingregistry@npm:^4.0.0, @jupyterlab/settingregistry@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/settingregistry@npm:4.2.0"
   dependencies:
     "@jupyterlab/nbformat": ^4.2.0
     "@jupyterlab/statedb": ^4.2.0
     "@lumino/commands": ^2.3.0
@@ -2594,27 +2706,59 @@
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
   checksum: fc60490e9e977e38b14b27a9e3896b47a28930a76a84888dd86180105b9ab6d1e68544f1184bdba72b4c5aa003cb13f10c8e5ca60685827fe6f893302483a109
   languageName: node
   linkType: hard
 
+"@jupyterlab/settingregistry@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/settingregistry@npm:4.2.1"
+  dependencies:
+    "@jupyterlab/nbformat": ^4.2.1
+    "@jupyterlab/statedb": ^4.2.1
+    "@lumino/commands": ^2.3.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@rjsf/utils": ^5.13.4
+    ajv: ^8.12.0
+    json5: ^2.2.3
+  peerDependencies:
+    react: ">=16"
+  checksum: 794e5ecde19a40e1b95c0d636eed7b56bbdc46857c8f3b4ef446c1bc90e8ea660c2ccf8f36a238bc312002f106a5a8522bb057742d9c0d674b2974ef21a786d7
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/statedb@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/statedb@npm:4.2.0"
   dependencies:
     "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
   checksum: 69620478aa7bf452d7440b9433b6411edef537cd7d9f72f87f70bd6fc0c8fc50003d02ab8d9d4b0746383f98cb7035b093ce5e596e6560e3c35c5a0fe434dce4
   languageName: node
   linkType: hard
 
+"@jupyterlab/statedb@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/statedb@npm:4.2.1"
+  dependencies:
+    "@lumino/commands": ^2.3.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+  checksum: 51e07db85269883bcd58fc5ba890db122e260e8d1ce4046f0b188453726694c2d909f27ca069ee3cd6944a93d70fcb8360074f87cdb13d611af2e24f6b14af30
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/statusbar@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/statusbar@npm:4.2.0"
   dependencies:
     "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
@@ -2623,14 +2767,30 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.2
     react: ^18.2.0
   checksum: 1ab4bfab3d6b37f0ff93ffd8b747b90ec7e532c554c8203716931923bcd97c61ad1b34c07b9973517022f022879014b57614a27f7417996697a5c97cad814c3b
   languageName: node
   linkType: hard
 
+"@jupyterlab/statusbar@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/statusbar@npm:4.2.1"
+  dependencies:
+    "@jupyterlab/ui-components": ^4.2.1
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.2
+    react: ^18.2.0
+  checksum: 65a0e4e0fa29ddd088d8dd2ee007a5166f783aa2852acd4217f2ed52fa04f492119c6e5b6e4f83884766fe7cfed3135ddd8c89b564ac3cc34ed6559457994885
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/testing@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/testing@npm:4.2.0"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
     "@jupyterlab/coreutils": ^6.2.0
@@ -2694,14 +2854,27 @@
     "@jupyterlab/services": ^7.2.0
     "@jupyterlab/statedb": ^4.2.0
     "@lumino/coreutils": ^2.1.2
   checksum: 0b2d4d3827946bf5b12db5e98356d15dc7721279bb791a46f2927b20b49b597fd717b0d24b84ae4c7b96540f99a0eed82ba0609c186675daf80b343df9792a21
   languageName: node
   linkType: hard
 
+"@jupyterlab/translation@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/translation@npm:4.2.1"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.2.1
+    "@jupyterlab/rendermime-interfaces": ^3.10.1
+    "@jupyterlab/services": ^7.2.1
+    "@jupyterlab/statedb": ^4.2.1
+    "@lumino/coreutils": ^2.1.2
+  checksum: 509c9fd8790f852faaa7f956c2ac660247a8d1610cb9f08fd5a357f784a7f32f838ac388a47626da66ee207769253d16ea72235d608112d560dbc10417d9b8e4
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/ui-components@npm:^4.2.0":
   version: 4.2.0
   resolution: "@jupyterlab/ui-components@npm:4.2.0"
   dependencies:
     "@jupyter/react-components": ^0.15.3
     "@jupyter/web-components": ^0.15.3
     "@jupyterlab/coreutils": ^6.2.0
@@ -2725,14 +2898,45 @@
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
   checksum: 9352c9d5d4df2671999a79bcc0434c50731bc78e89b5d94cfcf1e91f55fb14dbe4670576f49b8c53f9c7bb3995e72455c9062ad6953411c188c8bb85edee0a00
   languageName: node
   linkType: hard
 
+"@jupyterlab/ui-components@npm:^4.2.1":
+  version: 4.2.1
+  resolution: "@jupyterlab/ui-components@npm:4.2.1"
+  dependencies:
+    "@jupyter/react-components": ^0.15.3
+    "@jupyter/web-components": ^0.15.3
+    "@jupyterlab/coreutils": ^6.2.1
+    "@jupyterlab/observables": ^5.2.1
+    "@jupyterlab/rendermime-interfaces": ^3.10.1
+    "@jupyterlab/translation": ^4.2.1
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.3.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.2
+    "@rjsf/core": ^5.13.4
+    "@rjsf/utils": ^5.13.4
+    react: ^18.2.0
+    react-dom: ^18.2.0
+    typestyle: ^2.0.4
+  peerDependencies:
+    react: ^18.2.0
+  checksum: 7032d7755a7b69e98acc6378d9dedcc56d016cd0d4d6091bda3593baf89876a5e00f84116ab2a5ab5cc68439e07c2194eb7d211b6b3cff0a03cdfd11b03951bd
+  languageName: node
+  linkType: hard
+
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
   version: 1.2.1
   resolution: "@lezer/common@npm:1.2.1"
   checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
   languageName: node
   linkType: hard
 
@@ -7242,28 +7446,30 @@
 "jupyterlab-gallery@workspace:.":
   version: 0.0.0-use.local
   resolution: "jupyterlab-gallery@workspace:."
   dependencies:
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/launcher": ^4.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/settingregistry": ^4.0.0
     "@jupyterlab/testutils": ^4.0.0
     "@types/jest": ^29.2.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@types/react-addons-linked-state-mixin": ^0.14.22
     "@typescript-eslint/eslint-plugin": ^6.1.0
     "@typescript-eslint/parser": ^6.1.0
     css-loader: ^6.7.1
     eslint: ^8.36.0
     eslint-config-prettier: ^8.8.0
     eslint-plugin-prettier: ^5.0.0
     jest: ^29.2.0
+    jupyterlab-new-launcher: ^0.4.0
     mkdirp: ^1.0.3
     npm-run-all: ^4.1.5
     prettier: ^3.0.0
     rimraf: ^5.0.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
     stylelint: ^15.10.1
@@ -7272,14 +7478,25 @@
     stylelint-csstree-validator: ^3.0.0
     stylelint-prettier: ^4.0.0
     typescript: ~5.0.2
     yjs: ^13.5.0
   languageName: unknown
   linkType: soft
 
+"jupyterlab-new-launcher@npm:^0.4.0":
+  version: 0.4.0
+  resolution: "jupyterlab-new-launcher@npm:0.4.0"
+  dependencies:
+    "@jupyterlab/application": ^4.0.0
+    "@jupyterlab/launcher": ^4.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+  checksum: a963895f4f651bb69cf5cc50b5f61810f6643920ae7faad2a6e0a971769b5804b2d1e778cda8a10610303ddb3d0dee382b2c1d158960e69f59d0ea122c191e1b
+  languageName: node
+  linkType: hard
+
 "keyv@npm:^4.5.3":
   version: 4.5.4
   resolution: "keyv@npm:4.5.4"
   dependencies:
     json-buffer: 3.0.1
   checksum: 74a24395b1c34bd44ad5cb2b49140d087553e170625240b86755a6604cd65aa16efdbdeae5cdb17ba1284a0fbb25ad06263755dbc71b8d8b06f74232ce3cdd72
   languageName: node
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/__init__.py` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,16 @@
     # Fallback when using the package in dev mode without installing
     # in editable mode with pip. It is highly recommended to install
     # the package from a stable release or in editable mode: https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs
     import warnings
 
     warnings.warn("Importing 'jupyterlab_gallery' outside a proper installation.")
     __version__ = "dev"
-from .handlers import setup_handlers
+from .app import GalleryApp
 
 
 def _jupyter_labextension_paths():
     return [{"src": "labextension", "dest": "jupyterlab-gallery"}]
 
 
 def _jupyter_server_extension_points():
-    return [{"module": "jupyterlab_gallery"}]
-
-
-def _load_jupyter_server_extension(server_app):
-    """Registers the API handler to receive HTTP requests from the frontend extension.
-
-    Parameters
-    ----------
-    server_app: jupyterlab.labapp.LabApp
-        JupyterLab application instance
-    """
-    setup_handlers(server_app.web_app, server_app)
-    name = "jupyterlab_gallery"
-    server_app.log.info(f"Registered {name} server extension")
+    return [{"module": "jupyterlab_gallery", "app": GalleryApp}]
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/package.json` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9773313492063492%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/launcher': '^4.0.0', 'jupyterlab-new-launcher': '^0.4.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.cddf7f3b6d80e2c2c00f.js'}}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -11,26 +11,28 @@
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "A JupyterLab gallery extension for presenting and downloading examples from remote repositories",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.8.0",
         "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "jupyterlab-new-launcher": "^0.4.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^3.0.0",
         "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
         "stylelint": "^15.10.1",
@@ -110,15 +112,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-gallery",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7e7867bc630c8abba4aa.js",
+            "load": "static/remoteEntry.cddf7f3b6d80e2c2c00f.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_gallery"
                 },
@@ -207,9 +209,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/schemas/jupyterlab-gallery/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9776785714285715%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/launcher': '^4.0.0', 'jupyterlab-new-launcher': '^0.4.0'}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -11,26 +11,28 @@
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "A JupyterLab gallery extension for presenting and downloading examples from remote repositories",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.8.0",
         "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "jupyterlab-new-launcher": "^0.4.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^3.0.0",
         "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
         "stylelint": "^15.10.1",
@@ -202,9 +204,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/728.3bf722b918aa1abe3220.js` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/728.8ac417a035c29c0e6d2f.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,198 +1,198 @@
 "use strict";
 (self.webpackChunkjupyterlab_gallery = self.webpackChunkjupyterlab_gallery || []).push([
     [728], {
-        475: (e, n, t) => {
-            t.d(n, {
+        475: (n, e, t) => {
+            t.d(e, {
                 A: () => s
             });
             var r = t(601),
-                a = t.n(r),
-                o = t(314),
-                i = t.n(o)()(a());
-            i.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.jp-Exhibit {\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  margin: 12px;\n  padding: 4px 8px;\n  max-width: 200px;\n}\n\n.jp-Exhibit-title {\n  margin: 2px 4px;\n}\n\n.jp-Exhibit-description {\n  padding: 2px;\n}\n\n.jp-Exhibit-icon {\n  max-width: 100%;\n}\n", ""]);
+                o = t.n(r),
+                a = t(314),
+                i = t.n(a)()(o());
+            i.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.jp-Exhibit {\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  margin: 12px;\n  padding: 4px 8px;\n  max-width: 200px;\n}\n\n.jp-Exhibit-title {\n  margin: 2px 4px;\n}\n\n.jp-Exhibit-description {\n  padding: 2px;\n  height: 2.15em;\n  overflow: hidden;\n}\n\n.jp-Exhibit-icon > img {\n  max-width: 100%;\n}\n\n.jp-Exhibit-icon {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n}\n\n.jp-Launcher-openExample .jp-Gallery {\n  display: contents;\n}\n\n.jp-Exhibit-progressbar-filler {\n  background: var(--jp-success-color2);\n  height: 1em;\n  transition: width 1s;\n}\n\n.jp-Exhibit-progressbar {\n  border: 1px solid var(--jp-layout-color3);\n  background: var(--jp-layout-color2);\n  width: 100%;\n  margin-bottom: 10px;\n  border-radius: 2px;\n  position: relative;\n}\n\n.jp-Exhibit-progressbar-filler > .jp-Exhibit-progressbar-error {\n  background: var(--jp-error-color1);\n}\n\n.jp-Exhibit-progressMessage {\n  color: black;\n  max-height: 1.2em;\n  font-size: 85%;\n  position: absolute;\n  top: 0;\n  padding: 0 2px;\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n\n.jp-Exhibit-buttons .jp-Button:disabled {\n  opacity: 0.3;\n}\n", ""]);
             const s = i
         },
-        314: e => {
-            e.exports = function(e) {
-                var n = [];
-                return n.toString = function() {
-                    return this.map((function(n) {
+        314: n => {
+            n.exports = function(n) {
+                var e = [];
+                return e.toString = function() {
+                    return this.map((function(e) {
                         var t = "",
-                            r = void 0 !== n[5];
-                        return n[4] && (t += "@supports (".concat(n[4], ") {")), n[2] && (t += "@media ".concat(n[2], " {")), r && (t += "@layer".concat(n[5].length > 0 ? " ".concat(n[5]) : "", " {")), t += e(n), r && (t += "}"), n[2] && (t += "}"), n[4] && (t += "}"), t
+                            r = void 0 !== e[5];
+                        return e[4] && (t += "@supports (".concat(e[4], ") {")), e[2] && (t += "@media ".concat(e[2], " {")), r && (t += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), t += n(e), r && (t += "}"), e[2] && (t += "}"), e[4] && (t += "}"), t
                     })).join("")
-                }, n.i = function(e, t, r, a, o) {
-                    "string" == typeof e && (e = [
-                        [null, e, void 0]
+                }, e.i = function(n, t, r, o, a) {
+                    "string" == typeof n && (n = [
+                        [null, n, void 0]
                     ]);
                     var i = {};
                     if (r)
                         for (var s = 0; s < this.length; s++) {
                             var c = this[s][0];
                             null != c && (i[c] = !0)
                         }
-                    for (var u = 0; u < e.length; u++) {
-                        var p = [].concat(e[u]);
-                        r && i[p[0]] || (void 0 !== o && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = o), t && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = t) : p[2] = t), a && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = a) : p[4] = "".concat(a)), n.push(p))
+                    for (var p = 0; p < n.length; p++) {
+                        var l = [].concat(n[p]);
+                        r && i[l[0]] || (void 0 !== a && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = a), t && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = t) : l[2] = t), o && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = o) : l[4] = "".concat(o)), e.push(l))
                     }
-                }, n
+                }, e
             }
         },
-        601: e => {
-            e.exports = function(e) {
-                return e[1]
+        601: n => {
+            n.exports = function(n) {
+                return n[1]
             }
         },
-        72: e => {
-            var n = [];
+        72: n => {
+            var e = [];
 
-            function t(e) {
-                for (var t = -1, r = 0; r < n.length; r++)
-                    if (n[r].identifier === e) {
+            function t(n) {
+                for (var t = -1, r = 0; r < e.length; r++)
+                    if (e[r].identifier === n) {
                         t = r;
                         break
                     } return t
             }
 
-            function r(e, r) {
-                for (var o = {}, i = [], s = 0; s < e.length; s++) {
-                    var c = e[s],
-                        u = r.base ? c[0] + r.base : c[0],
-                        p = o[u] || 0,
-                        l = "".concat(u, " ").concat(p);
-                    o[u] = p + 1;
-                    var d = t(l),
+            function r(n, r) {
+                for (var a = {}, i = [], s = 0; s < n.length; s++) {
+                    var c = n[s],
+                        p = r.base ? c[0] + r.base : c[0],
+                        l = a[p] || 0,
+                        u = "".concat(p, " ").concat(l);
+                    a[p] = l + 1;
+                    var d = t(u),
                         f = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3],
                             supports: c[4],
                             layer: c[5]
                         };
-                    if (-1 !== d) n[d].references++, n[d].updater(f);
+                    if (-1 !== d) e[d].references++, e[d].updater(f);
                     else {
-                        var v = a(f, r);
-                        r.byIndex = s, n.splice(s, 0, {
-                            identifier: l,
-                            updater: v,
+                        var h = o(f, r);
+                        r.byIndex = s, e.splice(s, 0, {
+                            identifier: u,
+                            updater: h,
                             references: 1
                         })
                     }
-                    i.push(l)
+                    i.push(u)
                 }
                 return i
             }
 
-            function a(e, n) {
-                var t = n.domAPI(n);
-                return t.update(e),
-                    function(n) {
-                        if (n) {
-                            if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap && n.supports === e.supports && n.layer === e.layer) return;
-                            t.update(e = n)
+            function o(n, e) {
+                var t = e.domAPI(e);
+                return t.update(n),
+                    function(e) {
+                        if (e) {
+                            if (e.css === n.css && e.media === n.media && e.sourceMap === n.sourceMap && e.supports === n.supports && e.layer === n.layer) return;
+                            t.update(n = e)
                         } else t.remove()
                     }
             }
-            e.exports = function(e, a) {
-                var o = r(e = e || [], a = a || {});
-                return function(e) {
-                    e = e || [];
-                    for (var i = 0; i < o.length; i++) {
-                        var s = t(o[i]);
-                        n[s].references--
-                    }
-                    for (var c = r(e, a), u = 0; u < o.length; u++) {
-                        var p = t(o[u]);
-                        0 === n[p].references && (n[p].updater(), n.splice(p, 1))
+            n.exports = function(n, o) {
+                var a = r(n = n || [], o = o || {});
+                return function(n) {
+                    n = n || [];
+                    for (var i = 0; i < a.length; i++) {
+                        var s = t(a[i]);
+                        e[s].references--
+                    }
+                    for (var c = r(n, o), p = 0; p < a.length; p++) {
+                        var l = t(a[p]);
+                        0 === e[l].references && (e[l].updater(), e.splice(l, 1))
                     }
-                    o = c
+                    a = c
                 }
             }
         },
-        659: e => {
-            var n = {};
-            e.exports = function(e, t) {
-                var r = function(e) {
-                    if (void 0 === n[e]) {
-                        var t = document.querySelector(e);
+        659: n => {
+            var e = {};
+            n.exports = function(n, t) {
+                var r = function(n) {
+                    if (void 0 === e[n]) {
+                        var t = document.querySelector(n);
                         if (window.HTMLIFrameElement && t instanceof window.HTMLIFrameElement) try {
                             t = t.contentDocument.head
-                        } catch (e) {
+                        } catch (n) {
                             t = null
                         }
-                        n[e] = t
+                        e[n] = t
                     }
-                    return n[e]
-                }(e);
+                    return e[n]
+                }(n);
                 if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                 r.appendChild(t)
             }
         },
-        540: e => {
-            e.exports = function(e) {
-                var n = document.createElement("style");
-                return e.setAttributes(n, e.attributes), e.insert(n, e.options), n
+        540: n => {
+            n.exports = function(n) {
+                var e = document.createElement("style");
+                return n.setAttributes(e, n.attributes), n.insert(e, n.options), e
             }
         },
-        56: (e, n, t) => {
-            e.exports = function(e) {
-                var n = t.nc;
-                n && e.setAttribute("nonce", n)
+        56: (n, e, t) => {
+            n.exports = function(n) {
+                var e = t.nc;
+                e && n.setAttribute("nonce", e)
             }
         },
-        206: e => {
-            e.exports = function(e) {
+        825: n => {
+            n.exports = function(n) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
-                var n = e.insertStyleElement(e);
+                var e = n.insertStyleElement(n);
                 return {
                     update: function(t) {
-                        ! function(e, n, t) {
+                        ! function(n, e, t) {
                             var r = "";
                             t.supports && (r += "@supports (".concat(t.supports, ") {")), t.media && (r += "@media ".concat(t.media, " {"));
-                            var a = void 0 !== t.layer;
-                            a && (r += "@layer".concat(t.layer.length > 0 ? " ".concat(t.layer) : "", " {")), r += t.css, a && (r += "}"), t.media && (r += "}"), t.supports && (r += "}");
-                            var o = t.sourceMap;
-                            o && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), n.styleTagTransform(r, e, n.options)
-                        }(n, e, t)
+                            var o = void 0 !== t.layer;
+                            o && (r += "@layer".concat(t.layer.length > 0 ? " ".concat(t.layer) : "", " {")), r += t.css, o && (r += "}"), t.media && (r += "}"), t.supports && (r += "}");
+                            var a = t.sourceMap;
+                            a && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleTagTransform(r, n, e.options)
+                        }(e, n, t)
                     },
                     remove: function() {
-                        ! function(e) {
-                            if (null === e.parentNode) return !1;
-                            e.parentNode.removeChild(e)
-                        }(n)
+                        ! function(n) {
+                            if (null === n.parentNode) return !1;
+                            n.parentNode.removeChild(n)
+                        }(e)
                     }
                 }
             }
         },
-        113: e => {
-            e.exports = function(e, n) {
-                if (n.styleSheet) n.styleSheet.cssText = e;
+        113: n => {
+            n.exports = function(n, e) {
+                if (e.styleSheet) e.styleSheet.cssText = n;
                 else {
-                    for (; n.firstChild;) n.removeChild(n.firstChild);
-                    n.appendChild(document.createTextNode(e))
+                    for (; e.firstChild;) e.removeChild(e.firstChild);
+                    e.appendChild(document.createTextNode(n))
                 }
             }
         },
-        728: (e, n, t) => {
-            t.r(n);
+        728: (n, e, t) => {
+            t.r(e);
             var r = t(72),
-                a = t.n(r),
-                o = t(206),
-                i = t.n(o),
+                o = t.n(r),
+                a = t(825),
+                i = t.n(a),
                 s = t(659),
                 c = t.n(s),
-                u = t(56),
-                p = t.n(u),
-                l = t(540),
-                d = t.n(l),
+                p = t(56),
+                l = t.n(p),
+                u = t(540),
+                d = t.n(u),
                 f = t(113),
-                v = t.n(f),
-                h = t(475),
-                m = {};
-            m.styleTagTransform = v(), m.setAttributes = p(), m.insert = c().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = d(), a()(h.A, m), h.A && h.A.locals && h.A.locals
+                h = t.n(f),
+                v = t(475),
+                b = {};
+            b.styleTagTransform = h(), b.setAttributes = l(), b.insert = c().bind(null, "head"), b.domAPI = i(), b.insertStyleElement = d(), o()(v.A, b), v.A && v.A.locals && v.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/remoteEntry.7e7867bc630c8abba4aa.js` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/remoteEntry.cddf7f3b6d80e2c2c00f.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, f, s, p, d, c, h, v, b, g = {
+    var e, r, t, n, a, o, i, l, u, f, s, d, p, c, h, v, g, y = {
             607: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(274).then((() => () => t(274))),
                         "./extension": () => t.e(274).then((() => () => t(274))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -21,41 +21,41 @@
                     };
                 t.d(r, {
                     get: () => a,
                     init: () => o
                 })
             }
         },
-        y = {};
+        b = {};
 
     function m(e) {
-        var r = y[e];
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = b[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, m), t.exports
+        return y[e](t, t.exports, m), t.exports
     }
-    m.m = g, m.c = y, m.n = e => {
+    m.m = y, m.c = b, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return m.d(r, {
             a: r
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        274: "65854fd2800238c6f003",
-        728: "3bf722b918aa1abe3220"
+        274: "78ff9c1bf7688afa9147",
+        728: "8ac417a035c29c0e6d2f"
     } [e] + ".js?v=" + {
-        274: "65854fd2800238c6f003",
-        728: "3bf722b918aa1abe3220"
+        274: "78ff9c1bf7688afa9147",
+        728: "8ac417a035c29c0e6d2f"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -68,24 +68,24 @@
                     var s = u[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
                         i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         l = a[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
                         get: () => m.e(274).then((() => () => m(274))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-gallery", "0.1.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jupyterlab-gallery", "0.1.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,79 +164,80 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == p ? l > n && !a : "" == p != a);
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
                 if ("u" == s) {
-                    if (!u || "u" != p) return !1
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (p == s)
+                    if (d == s)
                         if (l <= n) {
                             if (f != e[l]) return !1
                         } else {
                             if (a ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != d && "n" != d) {
                     if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < p != a) return !1;
+                    if (l <= n || s < d != a) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || s(u(e, t, a, n)), p(e[t][a])
+        return o(n, a) || s(u(e, t, a, n)), d(e[t][a])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
-        265: () => d("default", "@jupyterlab/translation", [1, 4, 2, 0]),
-        345: () => d("default", "react", [1, 18, 2, 0]),
-        527: () => d("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
-        670: () => d("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
-        702: () => d("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
-        825: () => d("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
-        861: () => d("default", "@jupyterlab/services", [1, 7, 2, 0]),
-        923: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 0])
+        107: () => p("default", "@jupyterlab/launcher", [1, 4, 2, 1]),
+        218: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 1]),
+        345: () => p("default", "react", [1, 18, 2, 0]),
+        420: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 1]),
+        445: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 1]),
+        450: () => p("default", "@jupyterlab/translation", [1, 4, 2, 1]),
+        590: () => p("default", "@jupyterlab/services", [1, 7, 2, 1]),
+        602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
+        760: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
+        989: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 1])
     }, v = {
-        274: [265, 345, 527, 602, 670, 702, 825, 861, 923]
-    }, b = {}, m.f.consumes = (e, r) => {
+        274: [107, 218, 345, 420, 445, 450, 590, 602, 760, 989]
+    }, g = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
-            if (!b[e]) {
+            if (!g[e]) {
                 var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 };
-                b[e] = !0;
+                g[e] = !0;
                 var n = r => {
                     delete c[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
                 try {
                     var a = h[e]();
```

### Comparing `jupyterlab_gallery-0.1.2/jupyterlab_gallery/labextension/static/third-party-licenses.json` & `jupyterlab_gallery-0.1.3/jupyterlab_gallery/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/src/handler.ts` & `jupyterlab_gallery-0.1.3/src/handler.ts`

 * *Files 10% similar despite different names*

```diff
@@ -41,36 +41,47 @@
   if (!response.ok) {
     throw new ServerConnection.ResponseError(response, data.message || data);
   }
 
   return data;
 }
 
-export interface IStreamMessage {
+export interface IProgress {
+  progress: number;
+  message: string;
+}
+
+export interface IProgressStreamMessage {
+  output: IProgress;
+  phase: 'progress';
+  exhibit_id: number;
+}
+
+export interface ITextStreamMessage {
   output?: string;
-  phase: string;
+  phase: 'error' | 'finished' | 'syncing';
   exhibit_id: number;
 }
 
+export type IStreamMessage = IProgressStreamMessage | ITextStreamMessage;
+
 export function eventStream(
   endPoint = '',
   onStream: (message: IStreamMessage) => void,
   onError: (error: Event) => void
-) {
+): EventSource {
   const settings = ServerConnection.makeSettings();
   const requestUrl = URLExt.join(
     settings.baseUrl,
     'jupyterlab-gallery', // API Namespace
     endPoint
   );
   const eventSource = new EventSource(requestUrl);
   eventSource.addEventListener('message', event => {
     const data = JSON.parse(event.data);
-    if (data.phase === 'finished' || data.phase === 'error') {
-      eventSource.close();
-    }
     onStream(data);
   });
   eventSource.addEventListener('error', error => {
     onError(error);
   });
+  return eventSource;
 }
```

### Comparing `jupyterlab_gallery-0.1.2/src/index.ts` & `jupyterlab_gallery-0.1.3/src/index.ts`

 * *Files 24% similar despite different names*

```diff
@@ -2,55 +2,91 @@
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { ITranslator, nullTranslator } from '@jupyterlab/translation';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IFileBrowserCommands } from '@jupyterlab/filebrowser';
 
+import { ILauncher } from '@jupyterlab/launcher';
+import type { INewLauncher } from 'jupyterlab-new-launcher/lib/types';
+
 import { GalleryWidget } from './gallery';
 import { galleryIcon } from './icons';
+import { IGalleryReply } from './types';
+import { requestAPI } from './handler';
+
+function isNewLauncher(launcher: ILauncher): launcher is INewLauncher {
+  return 'addSection' in launcher;
+}
 
 /**
  * Initialization data for the jupyterlab-gallery extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab-gallery:plugin',
   description:
     'A JupyterLab gallery extension for presenting and downloading examples from remote repositories',
   autoStart: true,
   requires: [ISettingRegistry],
-  optional: [IFileBrowserCommands, ITranslator],
+  optional: [IFileBrowserCommands, ITranslator, ILauncher],
   activate: async (
     app: JupyterFrontEnd,
     settingRegistry: ISettingRegistry,
     fileBrowserCommands: IFileBrowserCommands | null,
-    translator: ITranslator | null
+    translator: ITranslator | null,
+    launcher: ILauncher | null
   ) => {
     console.log('JupyterLab extension jupyterlab-gallery is activated!');
 
     translator = translator ?? nullTranslator;
     const trans = translator.load('jupyterlab-gallery');
     const widget = new GalleryWidget({
       trans,
       openPath: (path: string) => {
         if (!fileBrowserCommands) {
           // TODO: Notebook v7 support
           throw Error('filebrowser not available');
         }
         app.commands.execute(fileBrowserCommands.openPath, { path });
+      },
+      fileChanged: app.serviceManager.contents.fileChanged,
+      refreshFileBrowser: () => {
+        return app.commands.execute('filebrowser:refresh');
       }
     });
 
-    // TODO: should we put it in the sidebar, or in the main area?
+    const data = await requestAPI<IGalleryReply>('gallery');
+    const expectedVersion = '1.0';
+    if (data.apiVersion !== expectedVersion) {
+      console.warn(
+        `jupyter-gallery API version out of sync, expected ${expectedVersion}, got ${data.apiVersion}`
+      );
+    }
+
+    const title = data.title === 'Gallery' ? trans.__('Gallery') : data.title;
     // add the widget to sidebar before waiting for server reply to reduce UI jitter
-    widget.id = 'jupyterlab-gallery:sidebar';
-    widget.title.icon = galleryIcon;
-    widget.title.caption = trans.__('Gallery');
-    widget.show();
-    app.shell.add(widget, 'left', { rank: 850 });
+    if (launcher && isNewLauncher(launcher)) {
+      launcher.addSection({
+        title,
+        className: 'jp-Launcher-openExample',
+        icon: galleryIcon,
+        id: 'gallery',
+        rank: 2.5,
+        render: () => {
+          return widget.render();
+        }
+      });
+    } else {
+      // fallback to placing it in the sidebar if new launcher is not installed
+      widget.id = 'jupyterlab-gallery:sidebar';
+      widget.title.icon = galleryIcon;
+      widget.title.caption = title;
+      widget.show();
+      app.shell.add(widget, 'left', { rank: 850 });
+    }
 
     try {
       const settings = await settingRegistry.load(plugin.id);
       console.log('jupyterlab-gallery settings loaded:', settings.composite);
     } catch (reason) {
       console.error('Failed to load settings for jupyterlab-gallery.', reason);
       return;
```

### Comparing `jupyterlab_gallery-0.1.2/style/icons/md/LICENSE` & `jupyterlab_gallery-0.1.3/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/ui-tests/README.md` & `jupyterlab_gallery-0.1.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/ui-tests/tests/jupyterlab_gallery.spec.ts` & `jupyterlab_gallery-0.1.3/ui-tests/tests/jupyterlab_gallery.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/.gitignore` & `jupyterlab_gallery-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/LICENSE` & `jupyterlab_gallery-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_gallery-0.1.2/README.md` & `jupyterlab_gallery-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,46 @@
 
 A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 
 This extension is composed of a Python package named `jupyterlab-gallery`
 for the server extension and a NPM package named `jupyterlab-gallery`
 for the frontend extension.
 
+When [`jupyterlab-new-launcher`](https://github.com/nebari-dev/jupyterlab-new-launcher) is installed, the gallery will be added as a "Gallery" section in the launcher; otherwise it will be shown in the left sidebar.
+
+## Configuration
+
+You can configure the gallery with the following traitlets:
+
+- `GalleryManager.exhibits`: controls the tiles shown in the gallery
+- `GalleryManager.destination`: defined the path into which the exhibits will be cloned (by default `/gallery`)
+- `GalleryManager.title`: the display name of the widget (by default "Gallery")
+
+These traitlets can be passed from the command line, a JSON file (`.json`) or a Python file (`.py`).
+
+You must name the file `jupyter_gallery_config.py` or `jupyter_gallery_config.json` and place it in one of the paths returned by `jupyter --paths` under the `config` section.
+
+An example Python file would include:
+
+```python
+c.GalleryManager.title = "Examples"
+c.GalleryManager.destination = "examples"
+c.GalleryManager.exhibits = [
+    {
+        "git": "https://github.com/jupyterlab/jupyterlab.git",
+        "repository": "https://github.com/jupyterlab/jupyterlab/",
+        "title": "JupyterLab",
+        "description": "JupyterLab is a highly extensible, feature-rich notebook authoring application and editing environment.",
+        "icon": "https://raw.githubusercontent.com/jupyterlab/jupyterlab/main/packages/ui-components/style/icons/jupyter/jupyter.svg"
+    }
+]
+```
+
+Using the Python file enables including the PAT access token in the `git` stanza (note: while the `git` value is never exposed to the user, the `repository` is and should not contain the secret if you do not want it to be shared with the users).
+
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
```

### Comparing `jupyterlab_gallery-0.1.2/pyproject.toml` & `jupyterlab_gallery-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "jupyter_server>=2.0.1,<3",
-    "nbgitpuller>=1.2.1"
+    "nbgitpuller>=1.2.1",
+    "GitPython>=3.1.43"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
```

### Comparing `jupyterlab_gallery-0.1.2/PKG-INFO` & `jupyterlab_gallery-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-gallery
-Version: 0.1.2
+Version: 0.1.3
 Dynamic: Keywords
 Summary: A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-gallery
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-gallery/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-gallery.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Requires-Dist: gitpython>=3.1.43
 Requires-Dist: jupyter-server<3,>=2.0.1
 Requires-Dist: nbgitpuller>=1.2.1
 Provides-Extra: dev
 Requires-Dist: ruff==0.4.4; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
@@ -71,14 +72,46 @@
 
 A JupyterLab gallery extension for presenting and downloading examples from remote repositories
 
 This extension is composed of a Python package named `jupyterlab-gallery`
 for the server extension and a NPM package named `jupyterlab-gallery`
 for the frontend extension.
 
+When [`jupyterlab-new-launcher`](https://github.com/nebari-dev/jupyterlab-new-launcher) is installed, the gallery will be added as a "Gallery" section in the launcher; otherwise it will be shown in the left sidebar.
+
+## Configuration
+
+You can configure the gallery with the following traitlets:
+
+- `GalleryManager.exhibits`: controls the tiles shown in the gallery
+- `GalleryManager.destination`: defined the path into which the exhibits will be cloned (by default `/gallery`)
+- `GalleryManager.title`: the display name of the widget (by default "Gallery")
+
+These traitlets can be passed from the command line, a JSON file (`.json`) or a Python file (`.py`).
+
+You must name the file `jupyter_gallery_config.py` or `jupyter_gallery_config.json` and place it in one of the paths returned by `jupyter --paths` under the `config` section.
+
+An example Python file would include:
+
+```python
+c.GalleryManager.title = "Examples"
+c.GalleryManager.destination = "examples"
+c.GalleryManager.exhibits = [
+    {
+        "git": "https://github.com/jupyterlab/jupyterlab.git",
+        "repository": "https://github.com/jupyterlab/jupyterlab/",
+        "title": "JupyterLab",
+        "description": "JupyterLab is a highly extensible, feature-rich notebook authoring application and editing environment.",
+        "icon": "https://raw.githubusercontent.com/jupyterlab/jupyterlab/main/packages/ui-components/style/icons/jupyter/jupyter.svg"
+    }
+]
+```
+
+Using the Python file enables including the PAT access token in the `git` stanza (note: while the `git` value is never exposed to the user, the `repository` is and should not contain the secret if you do not want it to be shared with the users).
+
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
```

