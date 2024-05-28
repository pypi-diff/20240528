# Comparing `tmp/libreflow_extensions_anpo_texture_proxies-1.0.0.tar.gz` & `tmp/libreflow_extensions_anpo_texture_proxies-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_texture_proxies-1.0.0.tar", last modified: Mon May 27 16:51:17 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_texture_proxies-1.0.1.tar", last modified: Tue May 28 14:56:11 2024, max compression
```

## Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0.tar` & `libreflow_extensions_anpo_texture_proxies-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.833072 libreflow_extensions_anpo_texture_proxies-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1411 2024-05-27 16:51:17.833072 libreflow_extensions_anpo_texture_proxies-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-27 16:51:17.834072 libreflow_extensions_anpo_texture_proxies-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.828072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.831072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.832072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.832072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.833072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/texture_proxies/
--rw-rw-rw-   0 root         (0) root         (0)     6022 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/texture_proxies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-27 16:51:17.834072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/texture_proxies/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/texture_proxies/create_proxies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:51:17.833072 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1411 2024-05-27 16:51:17.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-27 16:51:17.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:51:17.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-27 16:51:17.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-27 16:51:08.000000 libreflow_extensions_anpo_texture_proxies-1.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.490380 libreflow_extensions_anpo_texture_proxies-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-05-28 14:56:11.490380 libreflow_extensions_anpo_texture_proxies-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-28 14:56:11.490380 libreflow_extensions_anpo_texture_proxies-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.485380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.487380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.488380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.489380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.489380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/texture_proxies/
+-rw-rw-rw-   0 root         (0) root         (0)     8370 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/texture_proxies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-28 14:56:11.491380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/texture_proxies/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/texture_proxies/create_proxies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:56:11.490380 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-05-28 14:56:11.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-28 14:56:11.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 14:56:11.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 14:56:11.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-28 14:56:02.000000 libreflow_extensions_anpo_texture_proxies-1.0.1/versioneer.py
```

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/CHANGELOG.md` & `libreflow_extensions_anpo_texture_proxies-1.0.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,12 +15,17 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+### Added
+
+* An option to overwrite existing proxies (disabled by default).
+* A new action to create textures proxies for the latest textures of all assets of an asset family.
+
 ## [1.0.0] - 2024-05-27
 
 ### Added
 
 * Action to create 1K and 2K versions of the images in a `textures` folder. The generated proxies are placed respectively in the `textures_1k` and `textures_2k` folders (when the target size does not exceed the original one).
```

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/PKG-INFO` & `libreflow_extensions_anpo_texture_proxies-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.texture_proxies
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/texture_proxies
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -35,12 +35,17 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+### Added
+
+* An option to overwrite existing proxies (disabled by default).
+* A new action to create textures proxies for the latest textures of all assets of an asset family.
+
 ## [1.0.0] - 2024-05-27
 
 ### Added
 
 * Action to create 1K and 2K versions of the images in a `textures` folder. The generated proxies are placed respectively in the `textures_1k` and `textures_2k` folders (when the target size does not exceed the original one).
```

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/setup.py` & `libreflow_extensions_anpo_texture_proxies-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow/extensions/anpo/texture_proxies/create_proxies.py` & `libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow/extensions/anpo/texture_proxies/create_proxies.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/PKG-INFO` & `libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.texture_proxies
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/texture_proxies
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -35,12 +35,17 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+### Added
+
+* An option to overwrite existing proxies (disabled by default).
+* A new action to create textures proxies for the latest textures of all assets of an asset family.
+
 ## [1.0.0] - 2024-05-27
 
 ### Added
 
 * Action to create 1K and 2K versions of the images in a `textures` folder. The generated proxies are placed respectively in the `textures_1k` and `textures_2k` folders (when the target size does not exceed the original one).
```

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/src/libreflow.extensions.anpo.texture_proxies.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_texture_proxies-1.0.1/src/libreflow.extensions.anpo.texture_proxies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_texture_proxies-1.0.0/versioneer.py` & `libreflow_extensions_anpo_texture_proxies-1.0.1/versioneer.py`

 * *Files identical despite different names*

