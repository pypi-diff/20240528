# Comparing `tmp/numpyascii_package_gonenraveh-1.0.3.tar.gz` & `tmp/numpyascii_package_gonenraveh-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyascii_package_gonenraveh-1.0.3.tar", last modified: Tue May 28 12:36:41 2024, max compression
+gzip compressed data, was "numpyascii_package_gonenraveh-1.0.4.tar", last modified: Tue May 28 12:42:05 2024, max compression
```

## Comparing `numpyascii_package_gonenraveh-1.0.3.tar` & `numpyascii_package_gonenraveh-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.184369 numpyascii_package_gonenraveh-1.0.3/
--rw-rw-rw-   0        0        0     1093 2024-05-28 05:19:24.000000 numpyascii_package_gonenraveh-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2945 2024-05-28 12:36:41.179367 numpyascii_package_gonenraveh-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2024-05-28 05:18:37.000000 numpyascii_package_gonenraveh-1.0.3/README.md
--rw-rw-rw-   0        0        0      649 2024-05-28 12:36:30.000000 numpyascii_package_gonenraveh-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 12:36:41.185377 numpyascii_package_gonenraveh-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.100837 numpyascii_package_gonenraveh-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.134370 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/
--rw-rw-rw-   0        0        0        0 2024-05-28 05:08:22.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/__init__.py
--rw-rw-rw-   0        0        0    13884 2024-05-28 12:33:10.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/numpyascii.py
-drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.171378 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/
--rw-rw-rw-   0        0        0     2945 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.166381 numpyascii_package_gonenraveh-1.0.3/tests/
--rw-rw-rw-   0        0        0      391 2024-05-28 12:33:55.000000 numpyascii_package_gonenraveh-1.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:42:05.241138 numpyascii_package_gonenraveh-1.0.4/
+-rw-rw-rw-   0        0        0     1093 2024-05-28 05:19:24.000000 numpyascii_package_gonenraveh-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1864 2024-05-28 12:42:05.238138 numpyascii_package_gonenraveh-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2024-05-28 12:41:35.000000 numpyascii_package_gonenraveh-1.0.4/README.md
+-rw-rw-rw-   0        0        0      649 2024-05-28 12:41:46.000000 numpyascii_package_gonenraveh-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:42:05.242138 numpyascii_package_gonenraveh-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 12:42:05.176138 numpyascii_package_gonenraveh-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 12:42:05.195150 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_GonenRaveh/
+-rw-rw-rw-   0        0        0        0 2024-05-28 05:08:22.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_GonenRaveh/__init__.py
+-rw-rw-rw-   0        0        0    13884 2024-05-28 12:33:10.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_GonenRaveh/numpyascii.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:42:05.230138 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/
+-rw-rw-rw-   0        0        0     1864 2024-05-28 12:42:05.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-28 12:42:05.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:42:05.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 12:42:05.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-28 12:42:05.000000 numpyascii_package_gonenraveh-1.0.4/src/numpyascii_package_GonenRaveh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 12:42:05.225139 numpyascii_package_gonenraveh-1.0.4/tests/
+-rw-rw-rw-   0        0        0      391 2024-05-28 12:33:55.000000 numpyascii_package_gonenraveh-1.0.4/tests/test.py
```

### Comparing `numpyascii_package_gonenraveh-1.0.3/LICENSE` & `numpyascii_package_gonenraveh-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `numpyascii_package_gonenraveh-1.0.3/pyproject.toml` & `numpyascii_package_gonenraveh-1.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numpyascii_package_GonenRaveh"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = [
   "numpy"
 ]
 authors = [
   { name="Gonen Raveh", email="gonen.raveh@gmail.com" },
 ]
 description = "Helper Python packages for 1D, 2D and 3D numpy matrices"
```

### Comparing `numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/numpyascii.py` & `numpyascii_package_gonenraveh-1.0.4/src/numpyascii_GonenRaveh/numpyascii.py`

 * *Files identical despite different names*

