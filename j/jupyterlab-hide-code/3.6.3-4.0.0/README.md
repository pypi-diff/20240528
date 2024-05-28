# Comparing `tmp/jupyterlab_hide_code-3.6.3.tar.gz` & `tmp/jupyterlab_hide_code-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_hide_code-3.6.3.tar", last modified: Fri May 12 07:23:07 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_hide_code-3.6.3.tar` & `jupyterlab_hide_code-4.0.0.tar`

### file list

```diff
@@ -1,52 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/install.json
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-05-12 07:23:04.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/build_log.json
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.131062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    28556 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-12 07:23:04.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/src/__tests__/jupyterlab_hide_code.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/style/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/ui-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/playwright.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/ui-tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/tests/jupyterlab_hide_code.spec.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/babel.config.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jest.config.js
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/tsconfig.test.json
+-rw-r--r--   0        0        0   421581 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/yarn.lock
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/_version.py
+-rw-r--r--   0        0        0    22701 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/build_log.json
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/package.json
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/schemas/jupyterlab_hide_code/package.json.orig
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/schemas/jupyterlab_hide_code/plugin.json
+-rw-r--r--   0        0        0    25274 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/lib_index_js.982c91ab12ef33ba33d4.js
+-rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/lib_index_js.982c91ab12ef33ba33d4.js.map
+-rw-r--r--   0        0        0    28059 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/remoteEntry.3b2ac13a839eb96bd9f4.js
+-rw-r--r--   0        0        0    26850 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/remoteEntry.3b2ac13a839eb96bd9f4.js.map
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/style.js
+-rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/style_index_js.aae21a5a3c7d2c98990c.js
+-rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/style_index_js.aae21a5a3c7d2c98990c.js.map
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/schema/plugin.json
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/src/index.ts
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/src/__tests__/jupyterlab_hide_code.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/style/index.js
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/README.md
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 jupyterlab_hide_code-4.0.0/PKG-INFO
```

### Comparing `jupyterlab_hide_code-3.6.3/LICENSE` & `jupyterlab_hide_code-4.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Dou Du
+Copyright (c) 2024, Dou Du
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_hide_code-3.6.3/PKG-INFO` & `jupyterlab_hide_code-4.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,105 @@
-Metadata-Version: 2.1
-Name: jupyterlab_hide_code
-Version: 3.6.3
-Summary: A JupyterLab extension to run and hide source code.
-Home-page: https://github.com/osscar-org/jupyterlab-hide-code
-Author: Dou Du
-Author-email: dou.du@epfl.ch
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# `jupyterlab-hide-code`: A Button in JupyterLab to Run and Hide Code
 
-# **jupyterlab-hide-code**: A JupyterLab Extension to Run and Hide Source Code
-
-![Build](https://github.com/osscar-org/jupyterlab-hide-code/workflows/Build/badge.svg)
-[![PyPI version](https://badge.fury.io/py/jupyterlab-hide-code.svg)](https://badge.fury.io/py/jupyterlab-hide-code)
+[![Github Actions Status](https://github.com/osscar-org/jupyterlab-hide-code/workflows/Build/badge.svg)](https://github.com/osscar-org/jupyterlab-hide-code/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/osscar-org/jupyterlab-hide-code/main?urlpath=lab)
 
 A button in JupyterLab to run the code cells and then to hide the code cells.
-This JupyterLab extension was inspired by the
-[jlab-hide-code](https://github.com/AixViPMaP/jlab-hide-code) JupyterLab
-extension from Aachen (Aix) Virtual Platform for Materials Processing.
 
-![demo](./docs/hide-input.gif)
+![demo](./binder/demo.gif)
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
+To install the extension, execute:
+
 ```bash
-pip install jupyterlab-hide-code
+pip install jupyterlab_hide_code
 ```
 
 ## Uninstall
 
+To remove the extension, execute:
+
 ```bash
-pip uninstall jupyterlab-hide-code
+pip uninstall jupyterlab_hide_code
 ```
 
 ## Contributing
 
-### Build
+### Development install
+
+Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Move to jupyterlab-hide-code directory
-# Install dependencies
-jlpm
-# Build Typescript source
-jlpm build
+# Change directory to the jupyterlab_hide_code directory
+# Install package in development mode
+pip install -e "."
 # Link your development version of the extension with JupyterLab
-jupyter labextension link .
-# Rebuild Typescript source after making changes
+jupyter labextension develop . --overwrite
+# Rebuild extension Typescript source after making changes
 jlpm build
-# Rebuild JupyterLab after making any changes
-jupyter lab build
 ```
 
-You can watch the source directory and run JupyterLab in watch mode to watch for changes in the extension's source and automatically rebuild the extension and application.
+You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
-# Watch the source directory in another terminal tab
+# Watch the source directory in one terminal, automatically rebuilding when needed
 jlpm watch
-# Run jupyterlab in watch mode in one terminal tab
-jupyter lab --watch
+# Run JupyterLab in another terminal
+jupyter lab
+```
+
+With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
+
+By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
+
+```bash
+jupyter lab build --minimize=False
+```
+
+### Development uninstall
+
+```bash
+pip uninstall jupyterlab_hide_code
+```
+
+In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
+command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
+folder is located. Then you can remove the symlink named `jupyterlab_hide_code` within that folder.
+
+### Testing the extension
+
+#### Frontend tests
+
+This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
+
+To execute them, execute:
+
+```sh
+jlpm
+jlpm test
 ```
 
-## Acknowlegements
+#### Integration tests
+
+This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
+
+More information are provided within the [ui-tests](./ui-tests/README.md) README.
+
+### Packaging the extension
+
+See [RELEASE](RELEASE.md)
+
+## Acknowledgements
 
 We acknowledge support from the EPFL Open Science Fund via the [OSSCAR](http://www.osscar.org) project.
 
-<img src='https://www.osscar.org/_images/logos.png' width='700'>
+<img src='https://www.osscar.org/_images/logos.png' width='1200'>
```

### Comparing `jupyterlab_hide_code-3.6.3/RELEASE.md` & `jupyterlab_hide_code-4.0.0/RELEASE.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,39 @@
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
 
-This extension can be distributed as Python
-packages. All of the Python
-packaging instructions in the `pyproject.toml` file to wrap your extension in a
-Python package. Before generating a package, we first need to install `build`.
+This extension can be distributed as Python packages. All of the Python
+packaging instructions are in the `pyproject.toml` file to wrap your extension in a
+Python package. Before generating a package, you first need to install some tools:
 
 ```bash
-pip install build twine
+pip install build twine hatch
+```
+
+Bump the version using `hatch`. By default this will create a tag.
+See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
+
+```bash
+hatch version <new-version>
+```
+
+Make sure to clean up all the development files before building the package:
+
+```bash
+jlpm clean:all
+```
+
+You could also clean up the local git repository:
+
+```bash
+git clean -dfX
 ```
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
 python -m build
 ```
@@ -38,24 +56,22 @@
 npm publish --access public
 ```
 
 ## Automated releases with the Jupyter Releaser
 
 The extension repository should already be compatible with the Jupyter Releaser.
 
-Check out the [workflow documentation](https://github.com/jupyter-server/jupyter_releaser#typical-workflow) for more information.
+Check out the [workflow documentation](https://jupyter-releaser.readthedocs.io/en/latest/get_started/making_release_from_repo.html) for more information.
 
 Here is a summary of the steps to cut a new release:
 
-- Fork the [`jupyter-releaser` repo](https://github.com/jupyter-server/jupyter_releaser)
-- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the Github Secrets in the fork
+- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the [Github Secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets) in the repository
 - Go to the Actions panel
-- Run the "Draft Changelog" workflow
-- Merge the Changelog PR
-- Run the "Draft Release" workflow
-- Run the "Publish Release" workflow
+- Run the "Step 1: Prep Release" workflow
+- Check the draft changelog
+- Run the "Step 2: Publish Release" workflow
 
 ## Publishing to `conda-forge`
 
 If the package is not on conda forge yet, check the documentation to learn how to add it: https://conda-forge.org/docs/maintainer/adding_pkgs.html
 
 Otherwise a bot should pick up the new version publish to PyPI, and open a new PR on the feedstock repository automatically.
```

### Comparing `jupyterlab_hide_code-3.6.3/jest.config.js` & `jupyterlab_hide_code-4.0.0/jest.config.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,28 @@
 const jestJupyterLab = require('@jupyterlab/testutils/lib/jest-config');
 
 const esModules = [
+    '@codemirror',
+    '@jupyter/ydoc',
     '@jupyterlab/',
     'lib0',
-    'y\\-protocols',
-    'y\\-websocket',
+    'nanoid',
+    'vscode-ws-jsonrpc',
+    'y-protocols',
+    'y-websocket',
     'yjs'
 ].join('|');
 
-const jlabConfig = jestJupyterLab(__dirname);
-
-const {
-    moduleFileExtensions,
-    moduleNameMapper,
-    preset,
-    setupFilesAfterEnv,
-    setupFiles,
-    testPathIgnorePatterns,
-    transform
-} = jlabConfig;
+const baseConfig = jestJupyterLab(__dirname);
 
 module.exports = {
-    moduleFileExtensions,
-    moduleNameMapper,
-    preset,
-    setupFilesAfterEnv,
-    setupFiles,
-    testPathIgnorePatterns,
-    transform,
+    ...baseConfig,
     automock: false,
-    collectCoverageFrom: ['src/**/*.{ts,tsx}', '!src/**/*.d.ts'],
-    coverageDirectory: 'coverage',
+    collectCoverageFrom: [
+        'src/**/*.{ts,tsx}',
+        '!src/**/*.d.ts',
+        '!src/**/.ipynb_checkpoints/*'
+    ],
     coverageReporters: ['lcov', 'text'],
-    globals: {
-        'ts-jest': {
-            tsconfig: 'tsconfig.json'
-        }
-    },
     testRegex: 'src/.*/.*.spec.ts[x]?$',
     transformIgnorePatterns: [`/node_modules/(?!${esModules}).+`]
 };
```

### Comparing `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/build_log.json` & `jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/build_log.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9421726336132951%*

 * *Differences: {'0': "{'module': {'rules': {1: {'test': '/(?<!\\\\.raw)\\\\.css$/', 'use': "*

 * *      "['/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/style-loader/dist/cjs.js', "*

 * *      "'/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/css-loader/dist/cjs.js']}, "*

 * *      "2: {'test': '/\\\\.txt$/', 'type': 'asset/source', delete: ['use']}, 3: {'test': "*

 * *      "'/\\\\.md$/', 'type': 'asset/source', delete: ['use']}, 4: {'test': "*

 * *      "'/\\\\.(jpg|png|gif)$/', 'type': 'asset/resou […]*

```diff
@@ -3,656 +3,712 @@
         "bail": true,
         "devtool": "source-map",
         "entry": {},
         "mode": "development",
         "module": {
             "rules": [
                 {
-                    "test": {},
+                    "test": "/\\.raw\\.css$/",
+                    "type": "asset/source"
+                },
+                {
+                    "test": "/(?<!\\.raw)\\.css$/",
                     "use": [
-                        "style-loader",
-                        "css-loader"
+                        "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/style-loader/dist/cjs.js",
+                        "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/css-loader/dist/cjs.js"
                     ]
                 },
                 {
-                    "test": {},
-                    "use": "raw-loader"
+                    "test": "/\\.txt$/",
+                    "type": "asset/source"
                 },
                 {
-                    "test": {},
-                    "use": "raw-loader"
+                    "test": "/\\.md$/",
+                    "type": "asset/source"
                 },
                 {
-                    "test": {},
-                    "use": "file-loader"
+                    "test": "/\\.(jpg|png|gif)$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "test": {},
-                    "use": "file-loader"
+                    "test": "/\\.js.map$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "test": {},
-                    "use": "url-loader?limit=10000&mimetype=application/font-woff"
+                    "test": "/\\.woff2(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "test": {},
-                    "use": "url-loader?limit=10000&mimetype=application/font-woff"
+                    "test": "/\\.woff(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "test": {},
-                    "use": "url-loader?limit=10000&mimetype=application/octet-stream"
+                    "test": "/\\.ttf(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "test": {},
-                    "use": "file-loader"
+                    "test": "/\\.eot(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset/resource"
                 },
                 {
-                    "issuer": {},
-                    "test": {},
-                    "use": {
-                        "loader": "svg-url-loader",
-                        "options": {
-                            "encoding": "none",
-                            "limit": 10000
-                        }
-                    }
+                    "generator": {},
+                    "issuer": "/\\.css$/",
+                    "test": "/\\.svg(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset"
                 },
                 {
-                    "issuer": {},
-                    "test": {},
-                    "use": {
-                        "loader": "raw-loader"
-                    }
+                    "issuer": "/\\.js$/",
+                    "test": "/\\.svg(\\?v=\\d+\\.\\d+\\.\\d+)?$/",
+                    "type": "asset/source"
                 },
                 {
-                    "test": {},
+                    "test": "/\\.m?js$/",
                     "type": "javascript/auto"
                 },
                 {
                     "resolve": {
                         "fullySpecified": false
                     },
-                    "test": {}
+                    "test": "/\\.m?js/"
                 },
                 {
                     "resolve": {
                         "fullySpecified": false
                     },
-                    "test": {}
+                    "test": "/\\.c?js/"
                 },
                 {
-                    "test": {},
-                    "type": "file-loader"
+                    "test": "/\\.html$/",
+                    "type": "asset/resource"
                 },
                 {
                     "enforce": "pre",
-                    "test": {},
+                    "test": "/\\.js$/",
                     "use": [
-                        "source-map-loader"
+                        "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/@jupyterlab/builder/node_modules/source-map-loader/dist/cjs.js"
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/jupyterlab_hide_code/labextension/static",
+            "path": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/jupyterlab_hide_code/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/lib/index.js",
-                        "./index": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/lib/index.js",
-                        "./style": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/style/index.js"
+                        "./extension": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/lib/index.js",
+                        "./index": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/lib/index.js",
+                        "./style": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
-                            "jupyterlab-hide-code"
+                            "jupyterlab_hide_code"
                         ],
                         "type": "var"
                     },
-                    "name": "jupyterlab-hide-code",
+                    "name": "jupyterlab_hide_code",
                     "shared": {
+                        "@codemirror/language": {
+                            "import": false,
+                            "requiredVersion": "^6.0.0",
+                            "singleton": true
+                        },
+                        "@codemirror/state": {
+                            "import": false,
+                            "requiredVersion": "^6.2.0",
+                            "singleton": true
+                        },
+                        "@codemirror/view": {
+                            "import": false,
+                            "requiredVersion": "^6.9.6",
+                            "singleton": true
+                        },
+                        "@jupyter/react-components": {
+                            "import": false,
+                            "requiredVersion": "^0.15.3",
+                            "singleton": true
+                        },
+                        "@jupyter/web-components": {
+                            "import": false,
+                            "requiredVersion": "^0.15.3",
+                            "singleton": true
+                        },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^0.2.3",
+                            "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.3.1",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
-                        },
-                        "@jupyterlab/celltags": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
-                        },
-                        "@jupyterlab/collaboration": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3",
-                            "singleton": true
-                        },
-                        "@jupyterlab/collaboration-extension": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^6.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
-                        },
-                        "@jupyterlab/docprovider": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3",
-                            "singleton": true
-                        },
-                        "@jupyterlab/docprovider-extension": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@jupyterlab/lsp": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
+                        },
+                        "@jupyterlab/lsp-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
-                        "@jupyterlab/mathjax2": {
+                        "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
-                        "@jupyterlab/mathjax2-extension": {
+                        "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@jupyterlab/mermaid": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
+                        },
+                        "@jupyterlab/mermaid-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@jupyterlab/metadataform": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
+                        },
+                        "@jupyterlab/metadataform-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.6.3"
+                            "requiredVersion": "^5.2.1"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@jupyterlab/pluginmanager": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
+                        },
+                        "@jupyterlab/pluginmanager-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.10.1",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.6.3",
+                            "requiredVersion": "^7.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
-                            "singleton": true
-                        },
-                        "@jupyterlab/shared-models": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^5.0.1"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@jupyterlab/theme-dark-high-contrast-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^6.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.6.3"
+                            "requiredVersion": "^6.2.1"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^4.2.1",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
-                        "@jupyterlab/vdom": {
+                        "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
                         },
-                        "@jupyterlab/vdom-extension": {
+                        "@jupyterlab/workspaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1",
+                            "singleton": true
                         },
-                        "@jupyterlab/vega5-extension": {
+                        "@jupyterlab/workspaces-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^4.2.1"
+                        },
+                        "@lezer/common": {
+                            "import": false,
+                            "requiredVersion": "^1.0.0",
+                            "singleton": true
+                        },
+                        "@lezer/highlight": {
+                            "import": false,
+                            "requiredVersion": "^1.0.0",
+                            "singleton": true
                         },
                         "@lumino/algorithm": {
                             "import": false,
-                            "requiredVersion": "^1.9.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.31.4",
+                            "requiredVersion": "^2.3.0-alpha.0",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
-                            "requiredVersion": "^1.19.0",
+                            "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@lumino/coreutils": {
                             "import": false,
-                            "requiredVersion": "^1.11.0",
+                            "requiredVersion": "^2.0.0",
+                            "singleton": true
+                        },
+                        "@lumino/datagrid": {
+                            "import": false,
+                            "requiredVersion": "^2.3.0-alpha.0",
                             "singleton": true
                         },
                         "@lumino/disposable": {
                             "import": false,
-                            "requiredVersion": "^1.10.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/domutils": {
                             "import": false,
-                            "requiredVersion": "^1.8.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/dragdrop": {
                             "import": false,
-                            "requiredVersion": "^1.13.0",
+                            "requiredVersion": "^2.0.0",
+                            "singleton": true
+                        },
+                        "@lumino/keyboard": {
+                            "import": false,
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/messaging": {
                             "import": false,
-                            "requiredVersion": "^1.10.0",
+                            "requiredVersion": "^2.0.0",
+                            "singleton": true
+                        },
+                        "@lumino/polling": {
+                            "import": false,
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/properties": {
                             "import": false,
-                            "requiredVersion": "^1.8.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/signaling": {
                             "import": false,
-                            "requiredVersion": "^1.10.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/virtualdom": {
                             "import": false,
-                            "requiredVersion": "^1.14.0",
+                            "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.37.2",
+                            "requiredVersion": "^2.3.1-alpha.0",
+                            "singleton": true
+                        },
+                        "@microsoft/fast-element": {
+                            "import": false,
+                            "requiredVersion": "^1.12.0",
                             "singleton": true
                         },
-                        "jupyterlab-hide-code": {
-                            "import": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/lib/index.js",
+                        "@microsoft/fast-foundation": {
+                            "import": false,
+                            "requiredVersion": "^2.49.2",
+                            "singleton": true
+                        },
+                        "jupyterlab_hide_code": {
+                            "import": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/lib/index.js",
                             "singleton": true,
-                            "version": "3.6.2"
+                            "version": "4.0.0"
                         },
                         "react": {
                             "import": false,
-                            "requiredVersion": "^17.0.1",
+                            "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
-                            "requiredVersion": "^17.0.1",
+                            "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "yjs": {
                             "import": false,
-                            "requiredVersion": "^13.5.17",
+                            "requiredVersion": "^13.5.40",
                             "singleton": true
                         }
                     }
                 }
             },
             {}
         ],
         "resolve": {
-            "alias": {
-                "@phosphor/algorithm$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/algorithm/dist/index.js",
-                "@phosphor/application$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/application/dist/index.js",
-                "@phosphor/commands$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/commands/dist/index.js",
-                "@phosphor/coreutils$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/coreutils/dist/index.node.js",
-                "@phosphor/disposable$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/disposable/dist/index.js",
-                "@phosphor/domutils$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/domutils/dist/index.js",
-                "@phosphor/dragdrop$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/dragdrop/dist/index.js",
-                "@phosphor/dragdrop/style": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/widgets/style",
-                "@phosphor/messaging$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/messaging/dist/index.js",
-                "@phosphor/properties$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/properties/dist/index.js",
-                "@phosphor/signaling": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/signaling/dist/index.js",
-                "@phosphor/virtualdom$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/virtualdom/dist/index.js",
-                "@phosphor/widgets$": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/widgets/dist/index.js",
-                "@phosphor/widgets/style": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/@lumino/widgets/style"
-            },
             "fallback": {
                 "buffer": false,
                 "crypto": false,
-                "path": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/path-browserify/index.js",
-                "process": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/node_modules/process/browser.js",
+                "path": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/path-browserify/index.js",
+                "process": "/home/dou/Project/osscar/extensions/jupyterlab-hide-code/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/package.json` & `jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/schemas/jupyterlab_hide_code/package.json.orig`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6590170940170939%*

 * *Differences: {"'author'": "{'email': 'dou.du@icloud.com'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/docregistry', "*

 * *                   "'@jupyterlab/notebook', '@jupyterlab/services']}",*

 * * "'description'": "'A button in JupyterLab to run the code cells and then to hide the code cells.'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@jupyterlab/testutils': '^4.0.0', "*

 * *                 […]*

```diff
@@ -1,95 +1,151 @@
 {
     "author": {
-        "email": "dou.du@epfl.ch",
+        "email": "dou.du@icloud.com",
         "name": "Dou Du"
     },
     "bugs": {
         "url": "https://github.com/osscar-org/jupyterlab-hide-code/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.3",
-        "@jupyterlab/apputils": "3.6.3",
-        "@jupyterlab/docregistry": "3.6.3",
-        "@jupyterlab/notebook": "3.6.3",
-        "@jupyterlab/services": "6.6.3"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab extension to run and hide source code.",
+    "description": "A button in JupyterLab to run the code cells and then to hide the code cells.",
     "devDependencies": {
-        "@babel/core": "^7.21.8",
-        "@babel/preset-env": "^7.21.5",
-        "@jupyterlab/builder": "^3.6.3",
-        "@jupyterlab/testutils": "^3.6.3",
-        "@types/jest": "^29.5.1",
-        "@typescript-eslint/eslint-plugin": "^5.59.5",
-        "@typescript-eslint/parser": "^5.59.5",
-        "eslint": "^8.40.0",
-        "eslint-config-prettier": "^8.8.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "jest": "^29.5.0",
+        "jest": "^29.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.8",
-        "rimraf": "^5.0.0",
-        "stylelint": "^14.16.1",
-        "stylelint-config-prettier": "^9.0.5",
-        "stylelint-config-recommended": "^9.0.0",
-        "stylelint-config-standard": "~29.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^29.1.0",
-        "typescript": "4.3.5"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/naming-convention": [
+                "error",
+                {
+                    "custom": {
+                        "match": true,
+                        "regex": "^I[A-Z]"
+                    },
+                    "format": [
+                        "PascalCase"
+                    ],
+                    "selector": "interface"
+                }
+            ],
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
+    },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/*.json"
     ],
     "homepage": "https://github.com/osscar-org/jupyterlab-hide-code",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
-        }
-    },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.10c1996eae06db73781b.js",
-            "style": "./style"
-        },
         "extension": true,
-        "outputDir": "jupyterlab_hide_code/labextension"
+        "outputDir": "jupyterlab_hide_code/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-hide-code",
+    "name": "jupyterlab_hide_code",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/osscar-org/jupyterlab-hide-code.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_hide_code/labextension",
+        "clean:labextension": "rimraf jupyterlab_hide_code/labextension jupyterlab_hide_code/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -97,18 +153,33 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "rules": {
+            "property-no-vendor-prefix": null,
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "3.6.2"
+    "version": "4.0.0",
+    "workspaces": [
+        "ui-tests"
+    ]
 }
```

### Comparing `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js` & `jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/remoteEntry.3b2ac13a839eb96bd9f4.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,30 +3,30 @@
 (() => { // webpackBootstrap
     /******/
     "use strict";
     /******/
     var __webpack_modules__ = ({
 
         /***/
-        "webpack/container/entry/jupyterlab-hide-code":
+        "webpack/container/entry/jupyterlab_hide_code":
             /*!***********************!*\
               !*** container entry ***!
               \***********************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
                 var moduleMap = {
                     "./index": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
+                        return __webpack_require__.e("style_index_js").then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -182,17 +182,16 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "b56891ccedf3d2237715",
-                "lib_index_js": "d1df23bd25080bd06288",
-                "style_index_js": "b7522e42ae3acc6f5e3c"
+                "lib_index_js": "982c91ab12ef33ba33d4",
+                "style_index_js": "aae21a5a3c7d2c98990c"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -230,15 +229,15 @@
     /******/
     /* webpack/runtime/load script */
     /******/
     (() => {
         /******/
         var inProgress = {};
         /******/
-        var dataWebpackPrefix = "jupyterlab-hide-code:";
+        var dataWebpackPrefix = "jupyterlab_hide_code:";
         /******/ // loadScript function to load a script via script tag
         /******/
         __webpack_require__.l = (url, done, key, chunkId) => {
             /******/
             if (inProgress[url]) {
                 inProgress[url].push(done);
                 return;
@@ -278,14 +277,15 @@
                     /******/
                     script.setAttribute("nonce", __webpack_require__.nc);
                     /******/
                 }
                 /******/
                 script.setAttribute("data-webpack", dataWebpackPrefix + key);
                 /******/
+                /******/
                 script.src = url;
                 /******/
             }
             /******/
             inProgress[url] = [done];
             /******/
             var onScriptComplete = (prev, event) => {
@@ -381,15 +381,15 @@
             /******/
             var warn = (msg) => {
                 /******/
                 if (typeof console !== "undefined" && console.warn) console.warn(msg);
                 /******/
             };
             /******/
-            var uniqueName = "jupyterlab-hide-code";
+            var uniqueName = "jupyterlab_hide_code";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
                 var activeVersion = versions[version];
                 /******/
@@ -427,15 +427,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-hide-code", "3.6.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_hide_code", "4.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -468,15 +468,15 @@
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
                 if (scripts.length) {
                     /******/
                     var i = scripts.length - 1;
                     /******/
-                    while (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;
+                    while (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;
                     /******/
                 }
                 /******/
             }
             /******/
         }
         /******/ // When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration
@@ -828,19 +828,19 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@lumino/disposable": () => (loadSingletonVersionCheck("default", "@lumino/disposable", [1, 1, 10, 0])),
+            "webpack/sharing/consume/default/@lumino/disposable": () => (loadSingletonVersionCheck("default", "@lumino/disposable", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 3, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 3]))
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 2, 1]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -851,62 +851,70 @@
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/notebook"
                 /******/
             ]
             /******/
         };
         /******/
+        var startedInstallModules = {};
+        /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
             if (__webpack_require__.o(chunkMapping, chunkId)) {
                 /******/
                 chunkMapping[chunkId].forEach((id) => {
                     /******/
                     if (__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);
                     /******/
-                    var onFactory = (factory) => {
-                        /******/
-                        installedModules[id] = 0;
+                    if (!startedInstallModules[id]) {
                         /******/
-                        __webpack_require__.m[id] = (module) => {
+                        var onFactory = (factory) => {
                             /******/
-                            delete __webpack_require__.c[id];
+                            installedModules[id] = 0;
                             /******/
-                            module.exports = factory();
+                            __webpack_require__.m[id] = (module) => {
+                                /******/
+                                delete __webpack_require__.c[id];
+                                /******/
+                                module.exports = factory();
+                                /******/
+                            }
                             /******/
-                        }
-                        /******/
-                    };
-                    /******/
-                    var onError = (error) => {
+                        };
                         /******/
-                        delete installedModules[id];
+                        startedInstallModules[id] = true;
                         /******/
-                        __webpack_require__.m[id] = (module) => {
+                        var onError = (error) => {
                             /******/
-                            delete __webpack_require__.c[id];
+                            delete installedModules[id];
                             /******/
-                            throw error;
+                            __webpack_require__.m[id] = (module) => {
+                                /******/
+                                delete __webpack_require__.c[id];
+                                /******/
+                                throw error;
+                                /******/
+                            }
                             /******/
-                        }
-                        /******/
-                    };
-                    /******/
-                    try {
-                        /******/
-                        var promise = moduleToHandlerMapping[id]();
+                        };
                         /******/
-                        if (promise.then) {
+                        try {
+                            /******/
+                            var promise = moduleToHandlerMapping[id]();
                             /******/
-                            promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
+                            if (promise.then) {
+                                /******/
+                                promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
+                                /******/
+                            } else onFactory(promise);
                             /******/
-                        } else onFactory(promise);
+                        } catch (e) {
+                            onError(e);
+                        }
                         /******/
-                    } catch (e) {
-                        onError(e);
                     }
                     /******/
                 });
                 /******/
             }
             /******/
         }
@@ -921,15 +929,15 @@
         /******/
         /******/ // object to store loaded and loading chunks
         /******/ // undefined = chunk not loaded, null = chunk preloaded/prefetched
         /******/ // [resolve, reject, Promise] = chunk loading, 0 = chunk loaded
         /******/
         var installedChunks = {
             /******/
-            "jupyterlab-hide-code": 0
+            "jupyterlab_hide_code": 0
             /******/
         };
         /******/
         /******/
         __webpack_require__.f.j = (chunkId, promises) => {
             /******/ // JSONP chunk loading for javascript
             /******/
@@ -1074,14 +1082,14 @@
     /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
-    var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-hide-code");
+    var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_hide_code");
     /******/
-    (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-hide-code"] = __webpack_exports__;
+    (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_hide_code = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.10c1996eae06db73781b.js.map
+//# sourceMappingURL=remoteEntry.3b2ac13a839eb96bd9f4.js.map
```

### Comparing `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js.map` & `jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/remoteEntry.3b2ac13a839eb96bd9f4.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7417582417582418%*

 * *Differences: {"'file'": "'remoteEntry.3b2ac13a839eb96bd9f4.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "file": "remoteEntry.10c1996eae06db73781b.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.3b2ac13a839eb96bd9f4.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WClLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://jupyterlab-hide-code/webpack/container-entry",
-        "webpack://jupyterlab-hide-code/webpack/bootstrap",
-        "webpack://jupyterlab-hide-code/webpack/runtime/compat get default export",
-        "webpack://jupyterlab-hide-code/webpack/runtime/define property getters",
-        "webpack://jupyterlab-hide-code/webpack/runtime/ensure chunk",
-        "webpack://jupyterlab-hide-code/webpack/runtime/get javascript chunk filename",
-        "webpack://jupyterlab-hide-code/webpack/runtime/global",
-        "webpack://jupyterlab-hide-code/webpack/runtime/hasOwnProperty shorthand",
-        "webpack://jupyterlab-hide-code/webpack/runtime/load script",
-        "webpack://jupyterlab-hide-code/webpack/runtime/make namespace object",
-        "webpack://jupyterlab-hide-code/webpack/runtime/sharing",
-        "webpack://jupyterlab-hide-code/webpack/runtime/publicPath",
-        "webpack://jupyterlab-hide-code/webpack/runtime/consumes",
-        "webpack://jupyterlab-hide-code/webpack/runtime/jsonp chunk loading",
-        "webpack://jupyterlab-hide-code/webpack/runtime/nonce",
-        "webpack://jupyterlab-hide-code/webpack/before-startup",
-        "webpack://jupyterlab-hide-code/webpack/startup",
-        "webpack://jupyterlab-hide-code/webpack/after-startup"
+        "webpack://jupyterlab_hide_code/webpack/container-entry",
+        "webpack://jupyterlab_hide_code/webpack/bootstrap",
+        "webpack://jupyterlab_hide_code/webpack/runtime/compat get default export",
+        "webpack://jupyterlab_hide_code/webpack/runtime/define property getters",
+        "webpack://jupyterlab_hide_code/webpack/runtime/ensure chunk",
+        "webpack://jupyterlab_hide_code/webpack/runtime/get javascript chunk filename",
+        "webpack://jupyterlab_hide_code/webpack/runtime/global",
+        "webpack://jupyterlab_hide_code/webpack/runtime/hasOwnProperty shorthand",
+        "webpack://jupyterlab_hide_code/webpack/runtime/load script",
+        "webpack://jupyterlab_hide_code/webpack/runtime/make namespace object",
+        "webpack://jupyterlab_hide_code/webpack/runtime/sharing",
+        "webpack://jupyterlab_hide_code/webpack/runtime/publicPath",
+        "webpack://jupyterlab_hide_code/webpack/runtime/consumes",
+        "webpack://jupyterlab_hide_code/webpack/runtime/jsonp chunk loading",
+        "webpack://jupyterlab_hide_code/webpack/runtime/nonce",
+        "webpack://jupyterlab_hide_code/webpack/before-startup",
+        "webpack://jupyterlab_hide_code/webpack/startup",
+        "webpack://jupyterlab_hide_code/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"b56891ccedf3d2237715\",\"lib_index_js\":\"d1df23bd25080bd06288\",\"style_index_js\":\"b7522e42ae3acc6f5e3c\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"982c91ab12ef33ba33d4\",\"style_index_js\":\"aae21a5a3c7d2c98990c\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-hide-code:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_hide_code:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-hide-code\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-hide-code\", \"3.6.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-hide-code\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_hide_code\"] = self[\"webpackChunkjupyterlab_hide_code\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_hide_code\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_hide_code\", \"4.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,3,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,2,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_hide_code\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_hide_code\"] = self[\"webpackChunkjupyterlab_hide_code\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
-        "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-hide-code\");\n",
+        "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_hide_code\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map` & `jupyterlab_hide_code-4.0.0/jupyterlab_hide_code/labextension/static/style_index_js.aae21a5a3c7d2c98990c.js.map`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'file'": "'style_index_js.aae21a5a3c7d2c98990c.js'",*

 * * "'mappings'": "';;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,KAAK;AACL;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,iBAAiB;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,qBAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sFAAsF,qBAAqB;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA, […]*

```diff
@@ -1,17 +1,33 @@
 {
-    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js",
-    "mappings": ";;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;;AAEjB;AACA;AACA;;AAEA;AACA,4CAA4C,qBAAqB;AACjE;;AAEA;AACA,KAAK;AACL,KAAK;AACL;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA,sBAAsB,iBAAiB;AACvC;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA,qBAAqB,qBAAqB;AAC1C;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;;;;;;;;;ACjEa;;AAEb,kCAAkC;;AAElC,8BAA8B;;AAE9B,kDAAkD,gBAAgB,gEAAgE,wDAAwD,6DAA6D,sDAAsD;;AAE7S,uCAAuC,uDAAuD,uCAAuC,SAAS,OAAO,oBAAoB;;AAEzK,yCAAyC,8FAA8F,wBAAwB,eAAe,eAAe,gBAAgB,YAAY,MAAM,wBAAwB,+BAA+B,aAAa,qBAAqB,uCAAuC,cAAc,WAAW,YAAY,UAAU,MAAM,mDAAmD,UAAU,sBAAsB;;AAEve,gCAAgC;;AAEhC;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA,KAAK;AACL;AACA;;AAEA;AACA;;;;;;;;;;ACnCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;AACA;AACA;AACA;AACA,wDAAwD;;AAExD;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;;AAEA;AACA;;AAEA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA,OAAO;AACP;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA,gBAAgB,KAAwC,GAAG,sBAAiB,GAAG,CAAI;;AAEnF;AACA;AACA;AACA;;AAEA;AACA;AACA,GAAG;;AAEH;AACA;AACA,IAAI;AACJ;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;;AAED;AACA,qEAAqE,qBAAqB,cAAc;;AAExG;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA,yDAAyD;AACzD,IAAI;;AAEJ;;;AAGA;AACA;AACA,IAAI;AACJ;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA,2BAA2B;AAC3B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;;AAEA;;AAEA,qBAAqB,6BAA6B;AAClD;;AAEA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA",
+    "file": "style_index_js.aae21a5a3c7d2c98990c.js",
+    "mappings": ";;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,KAAK;AACL;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,iBAAiB;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,qBAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sFAAsF,qBAAqB;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,iDAAiD,qBAAqB;AACtE;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sDAAsD,qBAAqB;AAC3E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACpFa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA;AACA;;;;;;;;;;ACfa;;AAEb;AACA;AACA;AACA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA,OAAO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;AACA;AACA,qBAAqB,6BAA6B;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACnFa;;AAEb;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACjCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA,cAAc,KAAwC,GAAG,sBAAiB,GAAG,CAAI;AACjF;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA;AACA,0CAA0C;AAC1C;AACA;AACA;AACA,iFAAiF;AACjF;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,yDAAyD;AACzD;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,kCAAkC;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;AC5Da;;AAEb;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;ACboB;;;;;;;;;;;;;;;;;;;ACApB;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA;AACA;;AAEA;AACA;AACA,OAAO,oFAAoF,2LAA2L;AACtR;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACXvC,MAA+F;AAC/F,MAAqF;AACrF,MAA4F;AAC5F,MAA+G;AAC/G,MAAwG;AACxG,MAAwG;AACxG,MAAkG;AAClG;AACA;;AAEA;;AAEA,4BAA4B,qGAAmB;AAC/C,wBAAwB,kHAAa;;AAErC,uBAAuB,uGAAa;AACpC;AACA,iBAAiB,+FAAM;AACvB,6BAA6B,sGAAkB;;AAE/C,aAAa,0GAAG,CAAC,qFAAO;;;;AAI4C;AACpE,OAAO,iEAAe,qFAAO,IAAI,qFAAO,UAAU,qFAAO,mBAAmB,EAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://jupyterlab-hide-code/./node_modules/css-loader/dist/runtime/api.js",
-        "webpack://jupyterlab-hide-code/./node_modules/css-loader/dist/runtime/cssWithMappingToString.js",
-        "webpack://jupyterlab-hide-code/./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js"
+        "webpack://jupyterlab_hide_code/./node_modules/css-loader/dist/runtime/api.js",
+        "webpack://jupyterlab_hide_code/./node_modules/css-loader/dist/runtime/sourceMaps.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/insertBySelector.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/insertStyleElement.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/styleDomAPI.js",
+        "webpack://jupyterlab_hide_code/./node_modules/style-loader/dist/runtime/styleTagTransform.js",
+        "webpack://jupyterlab_hide_code/./style/index.js",
+        "webpack://jupyterlab_hide_code/./style/base.css",
+        "webpack://jupyterlab_hide_code/./style/base.css?1944"
     ],
     "sourcesContent": [
-        "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\n// css base code, injected by the css-loader\n// eslint-disable-next-line func-names\nmodule.exports = function (cssWithMappingToString) {\n  var list = []; // return the list of modules as css string\n\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = cssWithMappingToString(item);\n\n      if (item[2]) {\n        return \"@media \".concat(item[2], \" {\").concat(content, \"}\");\n      }\n\n      return content;\n    }).join(\"\");\n  }; // import a list of modules into the list\n  // eslint-disable-next-line func-names\n\n\n  list.i = function (modules, mediaQuery, dedupe) {\n    if (typeof modules === \"string\") {\n      // eslint-disable-next-line no-param-reassign\n      modules = [[null, modules, \"\"]];\n    }\n\n    var alreadyImportedModules = {};\n\n    if (dedupe) {\n      for (var i = 0; i < this.length; i++) {\n        // eslint-disable-next-line prefer-destructuring\n        var id = this[i][0];\n\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n\n    for (var _i = 0; _i < modules.length; _i++) {\n      var item = [].concat(modules[_i]);\n\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        // eslint-disable-next-line no-continue\n        continue;\n      }\n\n      if (mediaQuery) {\n        if (!item[2]) {\n          item[2] = mediaQuery;\n        } else {\n          item[2] = \"\".concat(mediaQuery, \" and \").concat(item[2]);\n        }\n      }\n\n      list.push(item);\n    }\n  };\n\n  return list;\n};",
-        "\"use strict\";\n\nfunction _slicedToArray(arr, i) { return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest(); }\n\nfunction _nonIterableRest() { throw new TypeError(\"Invalid attempt to destructure non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\"); }\n\nfunction _unsupportedIterableToArray(o, minLen) { if (!o) return; if (typeof o === \"string\") return _arrayLikeToArray(o, minLen); var n = Object.prototype.toString.call(o).slice(8, -1); if (n === \"Object\" && o.constructor) n = o.constructor.name; if (n === \"Map\" || n === \"Set\") return Array.from(o); if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen); }\n\nfunction _arrayLikeToArray(arr, len) { if (len == null || len > arr.length) len = arr.length; for (var i = 0, arr2 = new Array(len); i < len; i++) { arr2[i] = arr[i]; } return arr2; }\n\nfunction _iterableToArrayLimit(arr, i) { var _i = arr && (typeof Symbol !== \"undefined\" && arr[Symbol.iterator] || arr[\"@@iterator\"]); if (_i == null) return; var _arr = []; var _n = true; var _d = false; var _s, _e; try { for (_i = _i.call(arr); !(_n = (_s = _i.next()).done); _n = true) { _arr.push(_s.value); if (i && _arr.length === i) break; } } catch (err) { _d = true; _e = err; } finally { try { if (!_n && _i[\"return\"] != null) _i[\"return\"](); } finally { if (_d) throw _e; } } return _arr; }\n\nfunction _arrayWithHoles(arr) { if (Array.isArray(arr)) return arr; }\n\nmodule.exports = function cssWithMappingToString(item) {\n  var _item = _slicedToArray(item, 4),\n      content = _item[1],\n      cssMapping = _item[3];\n\n  if (!cssMapping) {\n    return content;\n  }\n\n  if (typeof btoa === \"function\") {\n    // eslint-disable-next-line no-undef\n    var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));\n    var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n    var sourceMapping = \"/*# \".concat(data, \" */\");\n    var sourceURLs = cssMapping.sources.map(function (source) {\n      return \"/*# sourceURL=\".concat(cssMapping.sourceRoot || \"\").concat(source, \" */\");\n    });\n    return [content].concat(sourceURLs).concat([sourceMapping]).join(\"\\n\");\n  }\n\n  return [content].join(\"\\n\");\n};",
-        "\"use strict\";\n\nvar isOldIE = function isOldIE() {\n  var memo;\n  return function memorize() {\n    if (typeof memo === 'undefined') {\n      // Test for IE <= 9 as proposed by Browserhacks\n      // @see http://browserhacks.com/#hack-e71d8692f65334173fee715c222cb805\n      // Tests for existence of standard globals is to allow style-loader\n      // to operate correctly into non-standard environments\n      // @see https://github.com/webpack-contrib/style-loader/issues/177\n      memo = Boolean(window && document && document.all && !window.atob);\n    }\n\n    return memo;\n  };\n}();\n\nvar getTarget = function getTarget() {\n  var memo = {};\n  return function memorize(target) {\n    if (typeof memo[target] === 'undefined') {\n      var styleTarget = document.querySelector(target); // Special case to return head of iframe instead of iframe itself\n\n      if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n        try {\n          // This will throw an exception if access to iframe is blocked\n          // due to cross-origin restrictions\n          styleTarget = styleTarget.contentDocument.head;\n        } catch (e) {\n          // istanbul ignore next\n          styleTarget = null;\n        }\n      }\n\n      memo[target] = styleTarget;\n    }\n\n    return memo[target];\n  };\n}();\n\nvar stylesInDom = [];\n\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n\n  for (var i = 0; i < stylesInDom.length; i++) {\n    if (stylesInDom[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n\n  return result;\n}\n\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var index = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3]\n    };\n\n    if (index !== -1) {\n      stylesInDom[index].references++;\n      stylesInDom[index].updater(obj);\n    } else {\n      stylesInDom.push({\n        identifier: identifier,\n        updater: addStyle(obj, options),\n        references: 1\n      });\n    }\n\n    identifiers.push(identifier);\n  }\n\n  return identifiers;\n}\n\nfunction insertStyleElement(options) {\n  var style = document.createElement('style');\n  var attributes = options.attributes || {};\n\n  if (typeof attributes.nonce === 'undefined') {\n    var nonce = typeof __webpack_nonce__ !== 'undefined' ? __webpack_nonce__ : null;\n\n    if (nonce) {\n      attributes.nonce = nonce;\n    }\n  }\n\n  Object.keys(attributes).forEach(function (key) {\n    style.setAttribute(key, attributes[key]);\n  });\n\n  if (typeof options.insert === 'function') {\n    options.insert(style);\n  } else {\n    var target = getTarget(options.insert || 'head');\n\n    if (!target) {\n      throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n    }\n\n    target.appendChild(style);\n  }\n\n  return style;\n}\n\nfunction removeStyleElement(style) {\n  // istanbul ignore if\n  if (style.parentNode === null) {\n    return false;\n  }\n\n  style.parentNode.removeChild(style);\n}\n/* istanbul ignore next  */\n\n\nvar replaceText = function replaceText() {\n  var textStore = [];\n  return function replace(index, replacement) {\n    textStore[index] = replacement;\n    return textStore.filter(Boolean).join('\\n');\n  };\n}();\n\nfunction applyToSingletonTag(style, index, remove, obj) {\n  var css = remove ? '' : obj.media ? \"@media \".concat(obj.media, \" {\").concat(obj.css, \"}\") : obj.css; // For old IE\n\n  /* istanbul ignore if  */\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = replaceText(index, css);\n  } else {\n    var cssNode = document.createTextNode(css);\n    var childNodes = style.childNodes;\n\n    if (childNodes[index]) {\n      style.removeChild(childNodes[index]);\n    }\n\n    if (childNodes.length) {\n      style.insertBefore(cssNode, childNodes[index]);\n    } else {\n      style.appendChild(cssNode);\n    }\n  }\n}\n\nfunction applyToTag(style, options, obj) {\n  var css = obj.css;\n  var media = obj.media;\n  var sourceMap = obj.sourceMap;\n\n  if (media) {\n    style.setAttribute('media', media);\n  } else {\n    style.removeAttribute('media');\n  }\n\n  if (sourceMap && typeof btoa !== 'undefined') {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  } // For old IE\n\n  /* istanbul ignore if  */\n\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = css;\n  } else {\n    while (style.firstChild) {\n      style.removeChild(style.firstChild);\n    }\n\n    style.appendChild(document.createTextNode(css));\n  }\n}\n\nvar singleton = null;\nvar singletonCounter = 0;\n\nfunction addStyle(obj, options) {\n  var style;\n  var update;\n  var remove;\n\n  if (options.singleton) {\n    var styleIndex = singletonCounter++;\n    style = singleton || (singleton = insertStyleElement(options));\n    update = applyToSingletonTag.bind(null, style, styleIndex, false);\n    remove = applyToSingletonTag.bind(null, style, styleIndex, true);\n  } else {\n    style = insertStyleElement(options);\n    update = applyToTag.bind(null, style, options);\n\n    remove = function remove() {\n      removeStyleElement(style);\n    };\n  }\n\n  update(obj);\n  return function updateStyle(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap) {\n        return;\n      }\n\n      update(obj = newObj);\n    } else {\n      remove();\n    }\n  };\n}\n\nmodule.exports = function (list, options) {\n  options = options || {}; // Force single-tag solution on IE6-9, which has a hard limit on the # of <style>\n  // tags it will allow on a page\n\n  if (!options.singleton && typeof options.singleton !== 'boolean') {\n    options.singleton = isOldIE();\n  }\n\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n\n    if (Object.prototype.toString.call(newList) !== '[object Array]') {\n      return;\n    }\n\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDom[index].references--;\n    }\n\n    var newLastIdentifiers = modulesToDom(newList, options);\n\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n\n      var _index = getIndexByIdentifier(_identifier);\n\n      if (stylesInDom[_index].references === 0) {\n        stylesInDom[_index].updater();\n\n        stylesInDom.splice(_index, 1);\n      }\n    }\n\n    lastIdentifiers = newLastIdentifiers;\n  };\n};"
+        "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\nmodule.exports = function (cssWithMappingToString) {\n  var list = [];\n\n  // return the list of modules as css string\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = \"\";\n      var needLayer = typeof item[5] !== \"undefined\";\n      if (item[4]) {\n        content += \"@supports (\".concat(item[4], \") {\");\n      }\n      if (item[2]) {\n        content += \"@media \".concat(item[2], \" {\");\n      }\n      if (needLayer) {\n        content += \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\");\n      }\n      content += cssWithMappingToString(item);\n      if (needLayer) {\n        content += \"}\";\n      }\n      if (item[2]) {\n        content += \"}\";\n      }\n      if (item[4]) {\n        content += \"}\";\n      }\n      return content;\n    }).join(\"\");\n  };\n\n  // import a list of modules into the list\n  list.i = function i(modules, media, dedupe, supports, layer) {\n    if (typeof modules === \"string\") {\n      modules = [[null, modules, undefined]];\n    }\n    var alreadyImportedModules = {};\n    if (dedupe) {\n      for (var k = 0; k < this.length; k++) {\n        var id = this[k][0];\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n    for (var _k = 0; _k < modules.length; _k++) {\n      var item = [].concat(modules[_k]);\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        continue;\n      }\n      if (typeof layer !== \"undefined\") {\n        if (typeof item[5] === \"undefined\") {\n          item[5] = layer;\n        } else {\n          item[1] = \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\").concat(item[1], \"}\");\n          item[5] = layer;\n        }\n      }\n      if (media) {\n        if (!item[2]) {\n          item[2] = media;\n        } else {\n          item[1] = \"@media \".concat(item[2], \" {\").concat(item[1], \"}\");\n          item[2] = media;\n        }\n      }\n      if (supports) {\n        if (!item[4]) {\n          item[4] = \"\".concat(supports);\n        } else {\n          item[1] = \"@supports (\".concat(item[4], \") {\").concat(item[1], \"}\");\n          item[4] = supports;\n        }\n      }\n      list.push(item);\n    }\n  };\n  return list;\n};",
+        "\"use strict\";\n\nmodule.exports = function (item) {\n  var content = item[1];\n  var cssMapping = item[3];\n  if (!cssMapping) {\n    return content;\n  }\n  if (typeof btoa === \"function\") {\n    var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));\n    var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n    var sourceMapping = \"/*# \".concat(data, \" */\");\n    return [content].concat([sourceMapping]).join(\"\\n\");\n  }\n  return [content].join(\"\\n\");\n};",
+        "\"use strict\";\n\nvar stylesInDOM = [];\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n  for (var i = 0; i < stylesInDOM.length; i++) {\n    if (stylesInDOM[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n  return result;\n}\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var indexByIdentifier = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3],\n      supports: item[4],\n      layer: item[5]\n    };\n    if (indexByIdentifier !== -1) {\n      stylesInDOM[indexByIdentifier].references++;\n      stylesInDOM[indexByIdentifier].updater(obj);\n    } else {\n      var updater = addElementStyle(obj, options);\n      options.byIndex = i;\n      stylesInDOM.splice(i, 0, {\n        identifier: identifier,\n        updater: updater,\n        references: 1\n      });\n    }\n    identifiers.push(identifier);\n  }\n  return identifiers;\n}\nfunction addElementStyle(obj, options) {\n  var api = options.domAPI(options);\n  api.update(obj);\n  var updater = function updater(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap && newObj.supports === obj.supports && newObj.layer === obj.layer) {\n        return;\n      }\n      api.update(obj = newObj);\n    } else {\n      api.remove();\n    }\n  };\n  return updater;\n}\nmodule.exports = function (list, options) {\n  options = options || {};\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDOM[index].references--;\n    }\n    var newLastIdentifiers = modulesToDom(newList, options);\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n      var _index = getIndexByIdentifier(_identifier);\n      if (stylesInDOM[_index].references === 0) {\n        stylesInDOM[_index].updater();\n        stylesInDOM.splice(_index, 1);\n      }\n    }\n    lastIdentifiers = newLastIdentifiers;\n  };\n};",
+        "\"use strict\";\n\nvar memo = {};\n\n/* istanbul ignore next  */\nfunction getTarget(target) {\n  if (typeof memo[target] === \"undefined\") {\n    var styleTarget = document.querySelector(target);\n\n    // Special case to return head of iframe instead of iframe itself\n    if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n      try {\n        // This will throw an exception if access to iframe is blocked\n        // due to cross-origin restrictions\n        styleTarget = styleTarget.contentDocument.head;\n      } catch (e) {\n        // istanbul ignore next\n        styleTarget = null;\n      }\n    }\n    memo[target] = styleTarget;\n  }\n  return memo[target];\n}\n\n/* istanbul ignore next  */\nfunction insertBySelector(insert, style) {\n  var target = getTarget(insert);\n  if (!target) {\n    throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n  }\n  target.appendChild(style);\n}\nmodule.exports = insertBySelector;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction insertStyleElement(options) {\n  var element = document.createElement(\"style\");\n  options.setAttributes(element, options.attributes);\n  options.insert(element, options.options);\n  return element;\n}\nmodule.exports = insertStyleElement;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction setAttributesWithoutAttributes(styleElement) {\n  var nonce = typeof __webpack_nonce__ !== \"undefined\" ? __webpack_nonce__ : null;\n  if (nonce) {\n    styleElement.setAttribute(\"nonce\", nonce);\n  }\n}\nmodule.exports = setAttributesWithoutAttributes;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction apply(styleElement, options, obj) {\n  var css = \"\";\n  if (obj.supports) {\n    css += \"@supports (\".concat(obj.supports, \") {\");\n  }\n  if (obj.media) {\n    css += \"@media \".concat(obj.media, \" {\");\n  }\n  var needLayer = typeof obj.layer !== \"undefined\";\n  if (needLayer) {\n    css += \"@layer\".concat(obj.layer.length > 0 ? \" \".concat(obj.layer) : \"\", \" {\");\n  }\n  css += obj.css;\n  if (needLayer) {\n    css += \"}\";\n  }\n  if (obj.media) {\n    css += \"}\";\n  }\n  if (obj.supports) {\n    css += \"}\";\n  }\n  var sourceMap = obj.sourceMap;\n  if (sourceMap && typeof btoa !== \"undefined\") {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  }\n\n  // For old IE\n  /* istanbul ignore if  */\n  options.styleTagTransform(css, styleElement, options.options);\n}\nfunction removeStyleElement(styleElement) {\n  // istanbul ignore if\n  if (styleElement.parentNode === null) {\n    return false;\n  }\n  styleElement.parentNode.removeChild(styleElement);\n}\n\n/* istanbul ignore next  */\nfunction domAPI(options) {\n  if (typeof document === \"undefined\") {\n    return {\n      update: function update() {},\n      remove: function remove() {}\n    };\n  }\n  var styleElement = options.insertStyleElement(options);\n  return {\n    update: function update(obj) {\n      apply(styleElement, options, obj);\n    },\n    remove: function remove() {\n      removeStyleElement(styleElement);\n    }\n  };\n}\nmodule.exports = domAPI;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction styleTagTransform(css, styleElement) {\n  if (styleElement.styleSheet) {\n    styleElement.styleSheet.cssText = css;\n  } else {\n    while (styleElement.firstChild) {\n      styleElement.removeChild(styleElement.firstChild);\n    }\n    styleElement.appendChild(document.createTextNode(css));\n  }\n}\nmodule.exports = styleTagTransform;",
+        "import './base.css';\n",
+        "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/sourceMaps.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, `/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n`, \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
+        "\n      import API from \"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n      import domAPI from \"!../node_modules/style-loader/dist/runtime/styleDomAPI.js\";\n      import insertFn from \"!../node_modules/style-loader/dist/runtime/insertBySelector.js\";\n      import setAttributes from \"!../node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js\";\n      import insertStyleElement from \"!../node_modules/style-loader/dist/runtime/insertStyleElement.js\";\n      import styleTagTransformFn from \"!../node_modules/style-loader/dist/runtime/styleTagTransform.js\";\n      import content, * as namedExport from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n      \n      \n\nvar options = {};\n\noptions.styleTagTransform = styleTagTransformFn;\noptions.setAttributes = setAttributes;\n\n      options.insert = insertFn.bind(null, \"head\");\n    \noptions.domAPI = domAPI;\noptions.insertStyleElement = insertStyleElement;\n\nvar update = API(content, options);\n\n\n\nexport * from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n       export default content && content.locals ? content.locals : undefined;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_hide_code-3.6.3/package.json` & `jupyterlab_hide_code-4.0.0/package.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6574145299145298%*

 * *Differences: {"'author'": "{'email': 'dou.du@icloud.com'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/docregistry', "*

 * *                   "'@jupyterlab/notebook', '@jupyterlab/services']}",*

 * * "'description'": "'A button in JupyterLab to run the code cells and then to hide the code cells.'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@jupyterlab/testutils': '^4.0.0', "*

 * *                 […]*

```diff
@@ -1,90 +1,152 @@
 {
     "author": {
-        "email": "dou.du@epfl.ch",
+        "email": "dou.du@icloud.com",
         "name": "Dou Du"
     },
     "bugs": {
         "url": "https://github.com/osscar-org/jupyterlab-hide-code/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.3",
-        "@jupyterlab/apputils": "3.6.3",
-        "@jupyterlab/docregistry": "3.6.3",
-        "@jupyterlab/notebook": "3.6.3",
-        "@jupyterlab/services": "6.6.3"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab extension to run and hide source code.",
+    "description": "A button in JupyterLab to run the code cells and then to hide the code cells.",
     "devDependencies": {
-        "@babel/core": "^7.21.8",
-        "@babel/preset-env": "^7.21.5",
-        "@jupyterlab/builder": "^3.6.3",
-        "@jupyterlab/testutils": "^3.6.3",
-        "@types/jest": "^29.5.1",
-        "@typescript-eslint/eslint-plugin": "^5.59.5",
-        "@typescript-eslint/parser": "^5.59.5",
-        "eslint": "^8.40.0",
-        "eslint-config-prettier": "^8.8.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "jest": "^29.5.0",
+        "jest": "^29.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.8",
-        "rimraf": "^5.0.0",
-        "stylelint": "^14.16.1",
-        "stylelint-config-prettier": "^9.0.5",
-        "stylelint-config-recommended": "^9.0.0",
-        "stylelint-config-standard": "~29.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^29.1.0",
-        "typescript": "4.3.5"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/naming-convention": [
+                "error",
+                {
+                    "custom": {
+                        "match": true,
+                        "regex": "^I[A-Z]"
+                    },
+                    "format": [
+                        "PascalCase"
+                    ],
+                    "selector": "interface"
+                }
+            ],
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
+    },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/*.json"
     ],
     "homepage": "https://github.com/osscar-org/jupyterlab-hide-code",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
-        }
-    },
     "jupyterlab": {
         "extension": true,
-        "outputDir": "jupyterlab_hide_code/labextension"
+        "outputDir": "jupyterlab_hide_code/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
-        "jupyterlab-extension"
+        "jupyterlab-extension",
+        "osscar"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-hide-code",
+    "name": "jupyterlab_hide_code",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/osscar-org/jupyterlab-hide-code.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_hide_code/labextension",
+        "clean:labextension": "rimraf jupyterlab_hide_code/labextension jupyterlab_hide_code/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -92,18 +154,33 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "rules": {
+            "property-no-vendor-prefix": null,
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "3.6.3"
+    "version": "4.0.0",
+    "workspaces": [
+        "ui-tests"
+    ]
 }
```

### Comparing `jupyterlab_hide_code-3.6.3/src/index.ts` & `jupyterlab_hide_code-4.0.0/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,24 @@
   NotebookPanel,
   INotebookModel
 } from '@jupyterlab/notebook';
 
 import '../style/index.css';
 
 /**
- * Initialization data for the jupyterlab-hide-code extension.
+ * Initialization data for the jupyterlab_hide_code extension.
  */
-const extension: JupyterFrontEndPlugin<void> = {
-  id: 'jupyterlab-hide-code',
+const plugin: JupyterFrontEndPlugin<void> = {
+  id: 'jupyterlab_hide_code:plugin',
+  description:
+    'A button in JupyterLab to run the code cells and then to hide the code cells.',
   autoStart: true,
   activate: (app: JupyterFrontEnd) => {
     app.docRegistry.addWidgetExtension('Notebook', new ButtonExtension());
-    console.log('JupyterLab extension jupyterlab-hide-code is activated!');
+    console.log('JupyterLab extension jupyterlab_hide_code is activated!');
   }
 };
 
 export class ButtonExtension
   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
 {
   createNew(
@@ -84,8 +86,8 @@
     return new DisposableDelegate(() => {
       buttonHideInput.dispose();
       buttonShowInput.dispose();
     });
   }
 }
 
-export default extension;
+export default plugin;
```

### Comparing `jupyterlab_hide_code-3.6.3/tsconfig.json` & `jupyterlab_hide_code-4.0.0/tsconfig.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018'}"}*

```diff
@@ -13,15 +13,15 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2018",
+        "target": "ES2018",
         "types": [
             "jest"
         ]
     },
     "include": [
         "src/*"
     ]
```

