# Comparing `tmp/autoDATA-prep-1.0.tar.gz` & `tmp/autoDATA-prep-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoDATA-prep-1.0.tar", last modified: Tue May 28 17:10:18 2024, max compression
+gzip compressed data, was "dist/autoDATA-prep-1.3.0.tar", last modified: Tue May 28 18:09:50 2024, max compression
```

## Comparing `autoDATA-prep-1.0.tar` & `autoDATA-prep-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      263 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-28 17:10:13.000000 autoDATA-prep-1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA-prep/
--rw-r--r--   0 root         (0) root         (0)     7632 2024-05-28 00:48:36.000000 autoDATA-prep-1.0/autoDATA-prep/python_code.py
--rw-r--r--   0 root         (0) root         (0)        0 2018-06-02 00:07:44.000000 autoDATA-prep-1.0/autoDATA-prep/__init__.py
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-12 16:12:04.000000 autoDATA-prep-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/
--rw-r--r--   0 root         (0) root         (0)      257 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      263 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:10:18.000000 autoDATA-prep-1.0/autoDATA_prep.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/assets/
+-rw-r--r--   0 root         (0) root         (0)   113880 2024-05-28 17:43:23.000000 autoDATA-prep-1.3.0/assets/data-preprocessing-cover.png
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-28 17:58:45.000000 autoDATA-prep-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      692 2024-05-28 18:08:53.000000 autoDATA-prep-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA-prep/
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-05-28 00:48:36.000000 autoDATA-prep-1.3.0/autoDATA-prep/python_code.py
+-rw-r--r--   0 root         (0) root         (0)        0 2018-06-02 00:07:44.000000 autoDATA-prep-1.3.0/autoDATA-prep/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-28 18:08:03.000000 autoDATA-prep-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/dependency_links.txt
```

### Comparing `autoDATA-prep-1.0/autoDATA-prep/python_code.py` & `autoDATA-prep-1.3.0/autoDATA-prep/python_code.py`

 * *Files identical despite different names*

