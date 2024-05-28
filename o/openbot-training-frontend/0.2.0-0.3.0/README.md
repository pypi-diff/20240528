# Comparing `tmp/openbot_training_frontend-0.2.0.tar.gz` & `tmp/openbot_training_frontend-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbot_training_frontend-0.2.0.tar", last modified: Mon May 27 16:48:56 2024, max compression
+gzip compressed data, was "openbot_training_frontend-0.3.0.tar", last modified: Mon May 27 17:41:22 2024, max compression
```

## Comparing `openbot_training_frontend-0.2.0.tar` & `openbot_training_frontend-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,31 @@
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 16:48:56.148175 openbot_training_frontend-0.2.0/
--rw-r--r--   0 hardikgarg   (501) staff       (20)       52 2024-01-23 07:24:42.000000 openbot_training_frontend-0.2.0/MANIFEST.in
--rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-27 16:48:56.147966 openbot_training_frontend-0.2.0/PKG-INFO
--rw-r--r--   0 hardikgarg   (501) staff       (20)     1002 2024-01-23 07:24:42.000000 openbot_training_frontend-0.2.0/README.md
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 16:48:56.147769 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/
--rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-27 16:48:56.000000 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/PKG-INFO
--rw-r--r--   0 hardikgarg   (501) staff       (20)      274 2024-05-27 16:48:56.000000 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 16:48:56.000000 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 12:07:10.000000 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/not-zip-safe
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 16:48:56.000000 openbot_training_frontend-0.2.0/openbot_training_frontend.egg-info/top_level.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)       38 2024-05-27 16:48:56.148221 openbot_training_frontend-0.2.0/setup.cfg
--rw-r--r--   0 hardikgarg   (501) staff       (20)      432 2024-05-27 16:48:34.000000 openbot_training_frontend-0.2.0/setup.py
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.573947 openbot_training_frontend-0.3.0/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       61 2024-05-27 17:15:33.000000 openbot_training_frontend-0.3.0/MANIFEST.in
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-27 17:41:22.573735 openbot_training_frontend-0.3.0/PKG-INFO
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     1002 2024-01-23 07:24:42.000000 openbot_training_frontend-0.3.0/README.md
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.567008 openbot_training_frontend-0.3.0/openbot_training_frontend/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      154 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/__init__.py
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      517 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/asset-manifest.json
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     3870 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/favicon.ico
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      656 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/index.html
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     5347 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/logo192.png
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     9664 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/logo512.png
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      492 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/manifest.json
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       67 2024-05-27 17:41:11.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/robots.txt
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.565429 openbot_training_frontend-0.3.0/openbot_training_frontend/static/
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.568299 openbot_training_frontend-0.3.0/openbot_training_frontend/static/css/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)   580316 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/css/main.24e9152c.css
+-rw-r--r--   0 hardikgarg   (501) staff       (20)   823000 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/css/main.24e9152c.css.map
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.570075 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     3393 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/422.9175c467.chunk.js
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     7840 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/422.9175c467.chunk.js.map
+-rw-r--r--   0 hardikgarg   (501) staff       (20)  1035223 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/main.c7b656db.js
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     8145 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/main.c7b656db.js.LICENSE.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)  5852296 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend/static/js/main.c7b656db.js.map
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-27 17:41:22.573507 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      995 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 12:07:10.000000 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-27 17:41:22.000000 openbot_training_frontend-0.3.0/openbot_training_frontend.egg-info/top_level.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       38 2024-05-27 17:41:22.573994 openbot_training_frontend-0.3.0/setup.cfg
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      432 2024-05-27 17:41:02.000000 openbot_training_frontend-0.3.0/setup.py
```

### Comparing `openbot_training_frontend-0.2.0/README.md` & `openbot_training_frontend-0.3.0/README.md`

 * *Files identical despite different names*

