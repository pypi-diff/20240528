# Comparing `tmp/TemDataBrowser-1.0.4.tar.gz` & `tmp/temdatabrowser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TemDataBrowser-1.0.4.tar", last modified: Tue Dec  5 21:16:05 2023, max compression
+gzip compressed data, was "temdatabrowser-1.0.5.tar", last modified: Tue May 28 16:55:05 2024, max compression
```

## Comparing `TemDataBrowser-1.0.4.tar` & `temdatabrowser-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 21:16:05.561329 TemDataBrowser-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      359 2023-12-05 21:16:05.561329 TemDataBrowser-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-11-27 18:30:49.000000 TemDataBrowser-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 21:16:05.557329 TemDataBrowser-1.0.4/TemDataBrowser/
--rw-r--r--   0 root         (0) root         (0)    17327 2023-12-05 21:11:15.000000 TemDataBrowser-1.0.4/TemDataBrowser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 21:16:05.557329 TemDataBrowser-1.0.4/TemDataBrowser/images/
--rw-r--r--   0 root         (0) root         (0)   696897 2023-11-27 18:30:49.000000 TemDataBrowser-1.0.4/TemDataBrowser/images/TemDataBrowser_window.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 21:16:05.561329 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      359 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-12-05 21:16:05.000000 TemDataBrowser-1.0.4/TemDataBrowser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      482 2023-12-05 21:13:57.000000 TemDataBrowser-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      125 2023-11-27 18:30:49.000000 TemDataBrowser-1.0.4/run_TemDataBrowser.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-05 21:16:05.561329 TemDataBrowser-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.936317 temdatabrowser-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.932317 temdatabrowser-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.932317 temdatabrowser-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-28 16:55:05.936317 temdatabrowser-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.932317 temdatabrowser-1.0.5/TemDataBrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)    17327 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/TemDataBrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.936317 temdatabrowser-1.0.5/TemDataBrowser/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   696897 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/TemDataBrowser/images/TemDataBrowser_window.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:55:05.936317 temdatabrowser-1.0.5/TemDataBrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 16:55:05.000000 temdatabrowser-1.0.5/TemDataBrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 16:55:01.000000 temdatabrowser-1.0.5/run_TemDataBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:55:05.936317 temdatabrowser-1.0.5/setup.cfg
```

### Comparing `TemDataBrowser-1.0.4/README.md` & `temdatabrowser-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # TemDataBrowser
 A graphical user interface based on ScopeFoundry for viewing TEM data.
 
-![GUI example](https://github.com/ercius/TemDataBrowser/blob/main/TemDataBrowser/images/TemDataBrowser_window.png?raw=true)
+![GUI example](TemDataBrowser/images/TemDataBrowser_window.png)
 
 # Installation
 First install QT bindings. For example:
 
 `$ pip install PyQt5`
 
 Then install this package and the rest of the dependencies:
```

### Comparing `TemDataBrowser-1.0.4/TemDataBrowser/__init__.py` & `temdatabrowser-1.0.5/TemDataBrowser/__init__.py`

 * *Files identical despite different names*

### Comparing `TemDataBrowser-1.0.4/TemDataBrowser/images/TemDataBrowser_window.png` & `temdatabrowser-1.0.5/TemDataBrowser/images/TemDataBrowser_window.png`

 * *Files identical despite different names*

