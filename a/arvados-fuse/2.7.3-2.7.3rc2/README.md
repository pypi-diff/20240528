# Comparing `tmp/arvados_fuse-2.7.3.tar.gz` & `tmp/arvados_fuse-2.7.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvados_fuse-2.7.3.tar", last modified: Tue May 28 13:36:14 2024, max compression
+gzip compressed data, was "arvados_fuse-2.7.3rc2.tar", last modified: Tue May 28 17:54:39 2024, max compression
```

## Comparing `arvados_fuse-2.7.3.tar` & `arvados_fuse-2.7.3rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:14.663302 arvados_fuse-2.7.3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2024-05-28 13:36:14.647300 arvados_fuse-2.7.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2495 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/README.rst
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/agpl-3.0.txt
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:14.615297 arvados_fuse-2.7.3/arvados_fuse/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35946 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    25796 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/command.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/crunchstat.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4009 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/fresh.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    56792 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/fusedir.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4584 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/fusefile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7328 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_fuse/unmount.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:14.647300 arvados_fuse-2.7.3/arvados_fuse.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      145 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2024-05-28 13:36:14.000000 arvados_fuse-2.7.3/arvados_fuse.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:14.647300 arvados_fuse-2.7.3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/bin/arv-mount
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 13:36:14.663302 arvados_fuse-2.7.3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1882 2024-05-28 13:36:08.000000 arvados_fuse-2.7.3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3554 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2495 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/README.rst
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/agpl-3.0.txt
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/arvados_fuse/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35946 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2024-05-28 17:54:38.000000 arvados_fuse-2.7.3rc2/arvados_fuse/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    25796 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/command.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/crunchstat.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4009 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/fresh.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    56792 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/fusedir.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4584 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/fusefile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7328 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_fuse/unmount.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3554 2024-05-28 17:54:39.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2024-05-28 17:54:39.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 17:54:39.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      148 2024-05-28 17:54:39.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2024-05-28 17:54:39.000000 arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/bin/arv-mount
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 17:54:39.191709 arvados_fuse-2.7.3rc2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1882 2024-05-28 17:54:34.000000 arvados_fuse-2.7.3rc2/setup.py
```

### Comparing `arvados_fuse-2.7.3/PKG-INFO` & `arvados_fuse-2.7.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados_fuse
-Version: 2.7.3
+Version: 2.7.3rc2
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.7.3/README.rst` & `arvados_fuse-2.7.3rc2/README.rst`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/agpl-3.0.txt` & `arvados_fuse-2.7.3rc2/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/__init__.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/command.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/command.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/crunchstat.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/crunchstat.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/fresh.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/fresh.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/fusedir.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/fusedir.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/fusefile.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/fusefile.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse/unmount.py` & `arvados_fuse-2.7.3rc2/arvados_fuse/unmount.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/arvados_fuse.egg-info/PKG-INFO` & `arvados_fuse-2.7.3rc2/arvados_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-fuse
-Version: 2.7.3
+Version: 2.7.3rc2
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.7.3/arvados_version.py` & `arvados_fuse-2.7.3rc2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.3/setup.py` & `arvados_fuse-2.7.3rc2/setup.py`

 * *Files identical despite different names*

