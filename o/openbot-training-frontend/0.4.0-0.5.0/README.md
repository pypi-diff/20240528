# Comparing `tmp/openbot_training_frontend-0.4.0.tar.gz` & `tmp/openbot_training_frontend-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbot_training_frontend-0.4.0.tar", last modified: Tue May 28 04:53:22 2024, max compression
+gzip compressed data, was "openbot_training_frontend-0.5.0.tar", last modified: Tue May 28 05:10:01 2024, max compression
```

## Comparing `openbot_training_frontend-0.4.0.tar` & `openbot_training_frontend-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.122319 openbot_training_frontend-0.4.0/
--rw-r--r--   0 hardikgarg   (501) staff       (20)       61 2024-05-28 04:47:54.000000 openbot_training_frontend-0.4.0/MANIFEST.in
--rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-28 04:53:22.122052 openbot_training_frontend-0.4.0/PKG-INFO
--rw-r--r--   0 hardikgarg   (501) staff       (20)     1002 2024-01-23 07:24:42.000000 openbot_training_frontend-0.4.0/README.md
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.111816 openbot_training_frontend-0.4.0/openbot-training-frontend/
--rw-r--r--   0 hardikgarg   (501) staff       (20)      154 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/__init__.py
--rw-r--r--   0 hardikgarg   (501) staff       (20)      517 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/asset-manifest.json
--rw-r--r--   0 hardikgarg   (501) staff       (20)     3870 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/favicon.ico
--rw-r--r--   0 hardikgarg   (501) staff       (20)      656 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/index.html
--rw-r--r--   0 hardikgarg   (501) staff       (20)     5347 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/logo192.png
--rw-r--r--   0 hardikgarg   (501) staff       (20)     9664 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/logo512.png
--rw-r--r--   0 hardikgarg   (501) staff       (20)      492 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/manifest.json
--rw-r--r--   0 hardikgarg   (501) staff       (20)       67 2024-05-28 04:53:11.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/robots.txt
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.110127 openbot_training_frontend-0.4.0/openbot-training-frontend/static/
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.112383 openbot_training_frontend-0.4.0/openbot-training-frontend/static/css/
--rw-r--r--   0 hardikgarg   (501) staff       (20)   580316 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/css/main.24e9152c.css
--rw-r--r--   0 hardikgarg   (501) staff       (20)   823000 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/css/main.24e9152c.css.map
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.114410 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/
--rw-r--r--   0 hardikgarg   (501) staff       (20)     3393 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/422.9175c467.chunk.js
--rw-r--r--   0 hardikgarg   (501) staff       (20)     7840 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/422.9175c467.chunk.js.map
--rw-r--r--   0 hardikgarg   (501) staff       (20)  1035223 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js
--rw-r--r--   0 hardikgarg   (501) staff       (20)     8145 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js.LICENSE.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)  5852296 2024-05-28 04:53:21.000000 openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js.map
-drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 04:53:22.121743 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/
--rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-28 04:53:22.000000 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/PKG-INFO
--rw-r--r--   0 hardikgarg   (501) staff       (20)      995 2024-05-28 04:53:22.000000 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 04:53:22.000000 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 04:48:36.000000 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/not-zip-safe
--rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 04:53:22.000000 openbot_training_frontend-0.4.0/openbot_training_frontend.egg-info/top_level.txt
--rw-r--r--   0 hardikgarg   (501) staff       (20)       38 2024-05-28 04:53:22.122374 openbot_training_frontend-0.4.0/setup.cfg
--rw-r--r--   0 hardikgarg   (501) staff       (20)      432 2024-05-28 04:50:44.000000 openbot_training_frontend-0.4.0/setup.py
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.316553 openbot_training_frontend-0.5.0/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       61 2024-05-28 05:07:17.000000 openbot_training_frontend-0.5.0/MANIFEST.in
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-28 05:10:01.316275 openbot_training_frontend-0.5.0/PKG-INFO
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     1002 2024-01-23 07:24:42.000000 openbot_training_frontend-0.5.0/README.md
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.307090 openbot_training_frontend-0.5.0/openbot_training_frontend/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      154 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/__init__.py
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      517 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/asset-manifest.json
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     3870 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/favicon.ico
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      656 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/index.html
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     5347 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/logo192.png
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     9664 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/logo512.png
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      492 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/manifest.json
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       67 2024-05-28 05:09:49.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/robots.txt
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.304660 openbot_training_frontend-0.5.0/openbot_training_frontend/static/
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.309269 openbot_training_frontend-0.5.0/openbot_training_frontend/static/css/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)   580316 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/css/main.24e9152c.css
+-rw-r--r--   0 hardikgarg   (501) staff       (20)   823000 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/css/main.24e9152c.css.map
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.312194 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     3393 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/422.9175c467.chunk.js
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     7840 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/422.9175c467.chunk.js.map
+-rw-r--r--   0 hardikgarg   (501) staff       (20)  1035223 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js
+-rw-r--r--   0 hardikgarg   (501) staff       (20)     8145 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js.LICENSE.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)  5852296 2024-05-28 05:10:00.000000 openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js.map
+drwxr-xr-x   0 hardikgarg   (501) staff       (20)        0 2024-05-28 05:10:01.315947 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      229 2024-05-28 05:10:01.000000 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      995 2024-05-28 05:10:01.000000 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 05:10:01.000000 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 05:10:01.000000 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 hardikgarg   (501) staff       (20)        1 2024-05-28 05:10:01.000000 openbot_training_frontend-0.5.0/openbot_training_frontend.egg-info/top_level.txt
+-rw-r--r--   0 hardikgarg   (501) staff       (20)       38 2024-05-28 05:10:01.316640 openbot_training_frontend-0.5.0/setup.cfg
+-rw-r--r--   0 hardikgarg   (501) staff       (20)      432 2024-05-28 05:08:30.000000 openbot_training_frontend-0.5.0/setup.py
```

### Comparing `openbot_training_frontend-0.4.0/README.md` & `openbot_training_frontend-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/asset-manifest.json` & `openbot_training_frontend-0.5.0/openbot_training_frontend/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/favicon.ico` & `openbot_training_frontend-0.5.0/openbot_training_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/index.html` & `openbot_training_frontend-0.5.0/openbot_training_frontend/index.html`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/logo192.png` & `openbot_training_frontend-0.5.0/openbot_training_frontend/logo192.png`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/logo512.png` & `openbot_training_frontend-0.5.0/openbot_training_frontend/logo512.png`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/css/main.24e9152c.css` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/css/main.24e9152c.css`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/css/main.24e9152c.css.map` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/css/main.24e9152c.css.map`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/422.9175c467.chunk.js` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/422.9175c467.chunk.js`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/422.9175c467.chunk.js.map` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/422.9175c467.chunk.js.map`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js.LICENSE.txt` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openbot_training_frontend-0.4.0/openbot-training-frontend/static/js/main.c7b656db.js.map` & `openbot_training_frontend-0.5.0/openbot_training_frontend/static/js/main.c7b656db.js.map`

 * *Files identical despite different names*

