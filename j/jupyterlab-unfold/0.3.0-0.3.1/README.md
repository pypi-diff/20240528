# Comparing `tmp/jupyterlab_unfold-0.3.0.tar.gz` & `tmp/jupyterlab_unfold-0.3.1.tar.gz`

## Comparing `jupyterlab_unfold-0.3.0.tar` & `jupyterlab_unfold-0.3.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/.copier-answers.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/.prettierignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/.stylelintrc.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/.yarnrc.yml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/babel.config.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/environment.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jest.config.js
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/setup.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/tsconfig.test.json
--rw-r--r--   0        0        0   369864 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/yarn.lock
--rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/images/screenshot.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/_version.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/package.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/jupyterlab-unfold-settings.json
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/plugin.json
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/874.b754c9a07ec6ba2ba607.js
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/remoteEntry.6e3a0c2dd12e1cd0ae76.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/schema/jupyterlab-unfold-settings.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/schema/plugin.json
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/src/index.ts
--rw-r--r--   0        0        0    16466 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/src/unfold.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/src/__tests__/jupyterlab_unfold.spec.ts
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/style/icons/folder-open.svg
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   151934 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/test_structure/file0.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/test_structure/dir1/file11.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/test_structure/dir1/file12.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/test_structure/dir2/file21.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/test_structure/dir2/dir3/file211.txt
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png
--rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png
--rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/LICENSE
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/README.md
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.copier-answers.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.prettierignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.stylelintrc.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.yarnrc.yml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/babel.config.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/environment.yml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jest.config.js
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/setup.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/tsconfig.test.json
+-rw-r--r--   0        0        0   369864 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/yarn.lock
+-rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/images/screenshot.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/_version.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/package.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/jupyterlab-unfold-settings.json
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/plugin.json
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/874.2dab0411ca57be43f175.js
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/remoteEntry.51e9d38969fad5feb467.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/schema/jupyterlab-unfold-settings.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/schema/plugin.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/index.ts
+-rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/unfold.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/__tests__/jupyterlab_unfold.spec.ts
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/icons/folder-open.svg
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   151934 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/file0.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir1/file11.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir1/file12.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir2/file21.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir2/dir3/file211.txt
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png
+-rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png
+-rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/README.md
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/PKG-INFO
```

### Comparing `jupyterlab_unfold-0.3.0/.stylelintrc.yaml` & `jupyterlab_unfold-0.3.1/.stylelintrc.yaml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/RELEASE.md` & `jupyterlab_unfold-0.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/jest.config.js` & `jupyterlab_unfold-0.3.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/package.json` & `jupyterlab_unfold-0.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -194,9 +194,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_unfold-0.3.0/tsconfig.json` & `jupyterlab_unfold-0.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/yarn.lock` & `jupyterlab_unfold-0.3.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/images/screenshot.png` & `jupyterlab_unfold-0.3.1/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/package.json` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.51e9d38969fad5feb467.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -116,15 +116,15 @@
         "style/**/*.{css,svg}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-unfold",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6e3a0c2dd12e1cd0ae76.js",
+            "load": "static/remoteEntry.51e9d38969fad5feb467.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_unfold/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -199,9 +199,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -194,9 +194,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/874.b754c9a07ec6ba2ba607.js` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/874.2dab0411ca57be43f175.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,25 +6,25 @@
                 DirTreeListing: () => y,
                 FileTreeBrowser: () => w,
                 FileTreeRenderer: () => f,
                 FilterFileTreeBrowserModel: () => _,
                 default: () => C,
                 folderOpenIcon: () => v
             });
-            var i = s(322),
-                o = s(527),
-                n = s(609),
-                r = s(426),
-                a = s(452),
-                l = s(86),
+            var i = s(779),
+                o = s(786),
+                n = s(690),
+                r = s(386),
+                a = s(954),
+                l = s(233),
                 h = s(697),
                 c = s(593),
                 d = s(930),
-                p = s(519),
-                m = s(888);
+                p = s(705),
+                m = s(764);
             const u = "jp-mod-dropTarget",
                 g = "application/x-jupyter-icontents",
                 v = new m.LabIcon({
                     name: "ui-components:folder-open",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 576 512"><path class="jp-icon3 jp-icon-selectable" fill="#616161" d="M572.694 292.093L500.27 416.248A63.997 63.997 0 0 1 444.989 448H45.025c-18.523 0-30.064-20.093-20.731-36.093l72.424-124.155A64 64 0 0 1 152 256h399.964c18.523 0 30.064 20.093 20.73 36.093zM152 224h328v-48c0-26.51-21.49-48-48-48H272l-64-64H48C21.49 64 0 85.49 0 112v278.046l69.077-118.418C86.214 242.25 117.989 224 152 224z"></path></svg>\n'
                 });
             class f extends i.DirListing.Renderer {
@@ -158,15 +158,21 @@
                 constructor(t) {
                     super(t), this._isRestored = new d.PromiseDelegate, this._savedState = null, this._stateKey = null, this.openState = {}, this.contentManager = this.manager.services.contents, this._savedState = t.state || null, this._path = this.rootPath
                 }
                 get path() {
                     return this._path
                 }
                 set path(t) {
-                    this._path = t
+                    const e = this.pathChanged,
+                        s = this._path;
+                    this._path = t, e.emit({
+                        name: "path",
+                        oldValue: s,
+                        newValue: t
+                    })
                 }
                 async cd(t = this.rootPath) {
                     const e = await this.fetchContent(this.rootPath, t);
                     this.handleContents({
                         name: this.rootPath,
                         path: this.rootPath,
                         type: "directory",
@@ -277,14 +283,19 @@
                                     model: h,
                                     restore: !0,
                                     translator: s,
                                     app: t
                                 });
                             return c.listing.singleClickToUnfold = r.get("singleClickToUnfold").composite, r.changed.connect((() => {
                                 c.listing.singleClickToUnfold = r.get("singleClickToUnfold").composite
+                            })), t.restored.then((() => {
+                                const t = window.location.pathname;
+                                let s = t.indexOf("/tree/"),
+                                    i = t.substring(s + 6);
+                                i = decodeURIComponent(i), e.open(i)
                             })), a.add(c), c
                         },
                         tracker: a
                     }
                 }
             }
         }
```

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/remoteEntry.6e3a0c2dd12e1cd0ae76.js` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/remoteEntry.51e9d38969fad5feb467.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, f, d, s, p, c, h, v, b = {
-            796: (e, r, t) => {
+            533: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(874).then((() => () => t(874))),
                         "./extension": () => t.e(874).then((() => () => t(874))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -44,18 +44,18 @@
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
         747: "85bcc3e88490fafaddb5",
-        874: "b754c9a07ec6ba2ba607"
+        874: "2dab0411ca57be43f175"
     } [e] + ".js?v=" + {
         747: "85bcc3e88490fafaddb5",
-        874: "b754c9a07ec6ba2ba607"
+        874: "2dab0411ca57be43f175"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(874).then((() => () => m(874))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-unfold", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-unfold", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -208,27 +208,27 @@
         return a(n, o) || d(l(e, t, o, n)), s(e[t][o])
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
-        86: () => p("default", "@jupyterlab/statedb", [1, 4, 0, 5]),
-        322: () => p("default", "@jupyterlab/filebrowser", [1, 4, 0, 5]),
-        426: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 5]),
-        452: () => p("default", "@jupyterlab/translation", [1, 4, 0, 5]),
-        519: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 5]),
-        527: () => p("default", "@jupyterlab/docmanager", [1, 4, 0, 5]),
+        233: () => p("default", "@jupyterlab/statedb", [1, 4, 2, 1]),
+        386: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 1]),
         593: () => p("default", "@lumino/domutils", [1, 2, 0, 0]),
-        609: () => p("default", "@jupyterlab/apputils", [1, 4, 1, 5]),
+        690: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 1]),
         697: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
-        888: () => p("default", "@jupyterlab/ui-components", [1, 4, 0, 5]),
-        930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0])
+        705: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 1]),
+        764: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
+        779: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 1]),
+        786: () => p("default", "@jupyterlab/docmanager", [1, 4, 2, 1]),
+        930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        954: () => p("default", "@jupyterlab/translation", [1, 4, 2, 1])
     }, v = {
-        874: [86, 322, 426, 452, 519, 527, 593, 609, 697, 888, 930]
+        874: [233, 386, 593, 690, 697, 705, 764, 779, 786, 930, 954]
     }, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
@@ -275,10 +275,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyterlab_unfold = self.webpackChunkjupyterlab_unfold || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
-    var y = m(796);
+    var y = m(533);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-unfold"] = y
 })();
```

### Comparing `jupyterlab_unfold-0.3.0/jupyterlab_unfold/labextension/static/third-party-licenses.json` & `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/src/index.ts` & `jupyterlab_unfold-0.3.1/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,23 @@
       widget.listing.singleClickToUnfold = setting.get('singleClickToUnfold')
         .composite as boolean;
 
       setting.changed.connect(() => {
         widget.listing.singleClickToUnfold = setting.get('singleClickToUnfold')
           .composite as boolean;
       });
+   
+      // check the url in iframe and open
+      app.restored.then(() => {
+        const windowPathname = window.location.pathname;
+        let treeIndex = windowPathname.indexOf('/tree/');
+        let path = windowPathname.substring(treeIndex + '/tree/'.length);
+        path = decodeURIComponent(path);
+        docManager.open(path);
+      });
 
       // Track the newly created file browser.
       void tracker.add(widget);
 
       return widget;
     };
```

### Comparing `jupyterlab_unfold-0.3.0/src/unfold.ts` & `jupyterlab_unfold-0.3.1/src/unfold.ts`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 import { ArrayExt, toArray } from '@lumino/algorithm';
 
 import { ElementExt } from '@lumino/domutils';
 
 import { PromiseDelegate, ReadonlyJSONObject } from '@lumino/coreutils';
 
+import { Signal } from '@lumino/signaling';
+
 import { DOMUtils, showErrorMessage } from '@jupyterlab/apputils';
 
 import { JupyterFrontEnd } from '@jupyterlab/application';
 
 import { Contents } from '@jupyterlab/services';
 
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 
 import { renameFile } from '@jupyterlab/docmanager';
 
-import { PathExt } from '@jupyterlab/coreutils';
+import { PathExt, IChangedArgs } from '@jupyterlab/coreutils';
 
 import {
   DirListing,
   FileBrowser,
   FilterFileBrowserModel
 } from '@jupyterlab/filebrowser';
 
@@ -422,15 +424,24 @@
   }
 
   get path(): string {
     return this._path;
   }
 
   set path(value: string) {
+    const pathChanged = this.pathChanged as Signal<this, IChangedArgs<string>>;
+    const oldValue = this._path;
+
     this._path = value;
+
+    pathChanged.emit({
+      name: 'path',
+      oldValue,
+      newValue: value
+    });
   }
 
   /**
    * Change directory.
    *
    * @param path - The path to the file or directory.
    *
```

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/README.md` & `jupyterlab_unfold-0.3.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/yarn.lock` & `jupyterlab_unfold-0.3.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png` & `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/.gitignore` & `jupyterlab_unfold-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/LICENSE` & `jupyterlab_unfold-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/README.md` & `jupyterlab_unfold-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 An IDE-like file browser
 
 ![jupyterlab-unfold](https://raw.githubusercontent.com/jupyterlab-contrib/jupyterlab-unfold/master/images/screenshot.png)
 
 ## Requirements
 
-- JupyterLab >= 3.1.0,<4.0
+- JupyterLab >= 4.0.0,<5.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab-unfold
```

### Comparing `jupyterlab_unfold-0.3.0/pyproject.toml` & `jupyterlab_unfold-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.0/PKG-INFO` & `jupyterlab_unfold-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab-unfold
-Version: 0.3.0
+Version: 0.3.1
+Dynamic: Keywords
 Summary: A vscode-like file browser
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-unfold
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-unfold/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-unfold.git
 Author-email: Martin Renou <martin.renou@gmail.com>
 License: BSD 3-Clause License
         
@@ -61,15 +62,15 @@
 
 An IDE-like file browser
 
 ![jupyterlab-unfold](https://raw.githubusercontent.com/jupyterlab-contrib/jupyterlab-unfold/master/images/screenshot.png)
 
 ## Requirements
 
-- JupyterLab >= 3.1.0,<4.0
+- JupyterLab >= 4.0.0,<5.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab-unfold
```

