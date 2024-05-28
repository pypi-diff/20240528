# Comparing `tmp/hashinator-0.1.1.tar.gz` & `tmp/hashinator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashinator-0.1.1.tar", last modified: Tue May 28 19:16:50 2024, max compression
+gzip compressed data, was "hashinator-0.1.2.tar", last modified: Tue May 28 19:21:01 2024, max compression
```

## Comparing `hashinator-0.1.1.tar` & `hashinator-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 19:16:50.209380 hashinator-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-05-28 18:52:44.000000 hashinator-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      241 2024-05-28 19:16:50.207754 hashinator-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-28 19:16:36.000000 hashinator-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 19:16:50.209380 hashinator-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 19:16:50.161042 hashinator-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 19:16:50.171994 hashinator-0.1.1/src/hashinator/
--rw-rw-rw-   0        0        0        0 2024-05-28 18:24:57.000000 hashinator-0.1.1/src/hashinator/__init__.py
--rw-rw-rw-   0        0        0    12452 2024-05-28 18:25:39.000000 hashinator-0.1.1/src/hashinator/hashes.py
--rw-rw-rw-   0        0        0     3306 2024-05-28 18:22:10.000000 hashinator-0.1.1/src/hashinator/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 19:16:50.205396 hashinator-0.1.1/src/hashinator.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-28 19:16:50.000000 hashinator-0.1.1/src/hashinator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-28 19:16:50.000000 hashinator-0.1.1/src/hashinator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 19:16:50.000000 hashinator-0.1.1/src/hashinator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-28 19:16:50.000000 hashinator-0.1.1/src/hashinator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-28 19:16:50.000000 hashinator-0.1.1/src/hashinator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.799077 hashinator-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-28 18:52:44.000000 hashinator-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      241 2024-05-28 19:21:01.783469 hashinator-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-28 19:20:49.000000 hashinator-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 19:21:01.799077 hashinator-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.735890 hashinator-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.747494 hashinator-0.1.2/src/hashinator/
+-rw-rw-rw-   0        0        0        0 2024-05-28 18:24:57.000000 hashinator-0.1.2/src/hashinator/__init__.py
+-rw-rw-rw-   0        0        0    12452 2024-05-28 18:25:39.000000 hashinator-0.1.2/src/hashinator/hashes.py
+-rw-rw-rw-   0        0        0     3306 2024-05-28 18:22:10.000000 hashinator-0.1.2/src/hashinator/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.783469 hashinator-0.1.2/src/hashinator.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/top_level.txt
```

### Comparing `hashinator-0.1.1/LICENSE` & `hashinator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hashinator-0.1.1/src/hashinator/hashes.py` & `hashinator-0.1.2/src/hashinator/hashes.py`

 * *Files identical despite different names*

### Comparing `hashinator-0.1.1/src/hashinator/utils.py` & `hashinator-0.1.2/src/hashinator/utils.py`

 * *Files identical despite different names*

