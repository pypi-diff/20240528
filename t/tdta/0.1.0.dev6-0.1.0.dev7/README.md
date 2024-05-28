# Comparing `tmp/tdta-0.1.0.dev6.tar.gz` & `tmp/tdta-0.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdta-0.1.0.dev6.tar", last modified: Thu May  2 10:31:32 2024, max compression
+gzip compressed data, was "tdta-0.1.0.dev7.tar", last modified: Tue May 28 13:17:00 2024, max compression
```

## Comparing `tdta-0.1.0.dev6.tar` & `tdta-0.1.0.dev7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.448557 tdta-0.1.0.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.448557 tdta-0.1.0.dev6/src/tdta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/anndata_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/purl_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/tdt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/src/tdta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.545024 tdta-0.1.0.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/src/tdta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/anndata_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/purl_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/tdt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/src/tdta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/top_level.txt
```

### Comparing `tdta-0.1.0.dev6/LICENSE` & `tdta-0.1.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/PKG-INFO` & `tdta-0.1.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tdta-0.1.0.dev6/src/tdta/__main__.py` & `tdta-0.1.0.dev7/src/tdta/__main__.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/src/tdta/anndata_export.py` & `tdta-0.1.0.dev7/src/tdta/anndata_export.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/src/tdta/purl_publish.py` & `tdta-0.1.0.dev7/src/tdta/purl_publish.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/src/tdta/tdt_export.py` & `tdta-0.1.0.dev7/src/tdta/tdt_export.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/src/tdta/utils.py` & `tdta-0.1.0.dev7/src/tdta/utils.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev6/src/tdta.egg-info/PKG-INFO` & `tdta-0.1.0.dev7/src/tdta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

