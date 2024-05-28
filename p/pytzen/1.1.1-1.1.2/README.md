# Comparing `tmp/pytzen-1.1.1.tar.gz` & `tmp/pytzen-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytzen-1.1.1.tar", last modified: Mon May 20 11:40:47 2024, max compression
+gzip compressed data, was "pytzen-1.1.2.tar", last modified: Tue May 28 15:21:46 2024, max compression
```

## Comparing `pytzen-1.1.1.tar` & `pytzen-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-20 11:40:38.000000 pytzen-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-20 11:40:38.000000 pytzen-1.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-20 11:40:47.752894 pytzen-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-20 11:40:38.000000 pytzen-1.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-20 11:40:38.000000 pytzen-1.1.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-20 11:40:47.752894 pytzen-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/pytzen/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-20 11:40:38.000000 pytzen-1.1.1/src/pytzen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/pytzen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:46.663515 pytzen-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-05-28 15:21:46.663515 pytzen-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24650 2024-05-28 15:21:34.000000 pytzen-1.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-28 15:21:34.000000 pytzen-1.1.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-28 15:21:46.663515 pytzen-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:46.659515 pytzen-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:46.663515 pytzen-1.1.2/src/pytzen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-28 15:21:34.000000 pytzen-1.1.2/src/pytzen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:46.663515 pytzen-1.1.2/src/pytzen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-05-28 15:21:46.000000 pytzen-1.1.2/src/pytzen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 15:21:46.000000 pytzen-1.1.2/src/pytzen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:21:46.000000 pytzen-1.1.2/src/pytzen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 15:21:46.000000 pytzen-1.1.2/src/pytzen.egg-info/top_level.txt
```

### Comparing `pytzen-1.1.1/src/pytzen/__init__.py` & `pytzen-1.1.2/src/pytzen/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PYTZEN is designed to sketch out data pipelines.
+github.com/pytzen/pytzen/blob/main/pytzen_package/src/pytzen/__init__.py
 """
 
 import json
 import sys
 import importlib.util
 import os
 from datetime import datetime
```

