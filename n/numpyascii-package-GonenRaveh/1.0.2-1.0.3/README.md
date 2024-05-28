# Comparing `tmp/numpyascii_package_gonenraveh-1.0.2.tar.gz` & `tmp/numpyascii_package_gonenraveh-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyascii_package_gonenraveh-1.0.2.tar", last modified: Tue May 28 12:34:15 2024, max compression
+gzip compressed data, was "numpyascii_package_gonenraveh-1.0.3.tar", last modified: Tue May 28 12:36:41 2024, max compression
```

## Comparing `numpyascii_package_gonenraveh-1.0.2.tar` & `numpyascii_package_gonenraveh-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 12:34:15.523568 numpyascii_package_gonenraveh-1.0.2/
--rw-rw-rw-   0        0        0     1093 2024-05-28 05:19:24.000000 numpyascii_package_gonenraveh-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2945 2024-05-28 12:34:15.519574 numpyascii_package_gonenraveh-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2024-05-28 05:18:37.000000 numpyascii_package_gonenraveh-1.0.2/README.md
--rw-rw-rw-   0        0        0      649 2024-05-28 12:28:21.000000 numpyascii_package_gonenraveh-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 12:34:15.524568 numpyascii_package_gonenraveh-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 12:34:15.448485 numpyascii_package_gonenraveh-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 12:34:15.478569 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_GonenRaveh/
--rw-rw-rw-   0        0        0        0 2024-05-28 05:08:22.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_GonenRaveh/__init__.py
--rw-rw-rw-   0        0        0    13884 2024-05-28 12:33:10.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_GonenRaveh/numpyascii.py
-drwxrwxrwx   0        0        0        0 2024-05-28 12:34:15.513577 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/
--rw-rw-rw-   0        0        0     2945 2024-05-28 12:34:15.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-28 12:34:15.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 12:34:15.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 12:34:15.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-28 12:34:15.000000 numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 12:34:15.507568 numpyascii_package_gonenraveh-1.0.2/tests/
--rw-rw-rw-   0        0        0      391 2024-05-28 12:33:55.000000 numpyascii_package_gonenraveh-1.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.184369 numpyascii_package_gonenraveh-1.0.3/
+-rw-rw-rw-   0        0        0     1093 2024-05-28 05:19:24.000000 numpyascii_package_gonenraveh-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2945 2024-05-28 12:36:41.179367 numpyascii_package_gonenraveh-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1170 2024-05-28 05:18:37.000000 numpyascii_package_gonenraveh-1.0.3/README.md
+-rw-rw-rw-   0        0        0      649 2024-05-28 12:36:30.000000 numpyascii_package_gonenraveh-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:36:41.185377 numpyascii_package_gonenraveh-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.100837 numpyascii_package_gonenraveh-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.134370 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/
+-rw-rw-rw-   0        0        0        0 2024-05-28 05:08:22.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/__init__.py
+-rw-rw-rw-   0        0        0    13884 2024-05-28 12:33:10.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/numpyascii.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.171378 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/
+-rw-rw-rw-   0        0        0     2945 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-28 12:36:41.000000 numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 12:36:41.166381 numpyascii_package_gonenraveh-1.0.3/tests/
+-rw-rw-rw-   0        0        0      391 2024-05-28 12:33:55.000000 numpyascii_package_gonenraveh-1.0.3/tests/test.py
```

### Comparing `numpyascii_package_gonenraveh-1.0.2/LICENSE` & `numpyascii_package_gonenraveh-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `numpyascii_package_gonenraveh-1.0.2/PKG-INFO` & `numpyascii_package_gonenraveh-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyascii_package_GonenRaveh
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper Python packages for 1D, 2D and 3D numpy matrices
 Author-email: Gonen Raveh <gonen.raveh@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `numpyascii_package_gonenraveh-1.0.2/README.md` & `numpyascii_package_gonenraveh-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `numpyascii_package_gonenraveh-1.0.2/pyproject.toml` & `numpyascii_package_gonenraveh-1.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numpyascii_package_GonenRaveh"
-version = "1.0.2"
+version = "1.0.3"
 dependencies = [
   "numpy"
 ]
 authors = [
   { name="Gonen Raveh", email="gonen.raveh@gmail.com" },
 ]
 description = "Helper Python packages for 1D, 2D and 3D numpy matrices"
```

### Comparing `numpyascii_package_gonenraveh-1.0.2/src/numpyascii_GonenRaveh/numpyascii.py` & `numpyascii_package_gonenraveh-1.0.3/src/numpyascii_GonenRaveh/numpyascii.py`

 * *Files identical despite different names*

### Comparing `numpyascii_package_gonenraveh-1.0.2/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO` & `numpyascii_package_gonenraveh-1.0.3/src/numpyascii_package_GonenRaveh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyascii_package_GonenRaveh
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper Python packages for 1D, 2D and 3D numpy matrices
 Author-email: Gonen Raveh <gonen.raveh@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

