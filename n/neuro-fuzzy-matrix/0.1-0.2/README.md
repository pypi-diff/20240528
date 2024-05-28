# Comparing `tmp/neuro_fuzzy_matrix-0.1.tar.gz` & `tmp/neuro_fuzzy_matrix-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro_fuzzy_matrix-0.1.tar", last modified: Sun Apr  7 17:25:30 2024, max compression
+gzip compressed data, was "neuro_fuzzy_matrix-0.2.tar", last modified: Tue May 28 11:27:47 2024, max compression
```

## Comparing `neuro_fuzzy_matrix-0.1.tar` & `neuro_fuzzy_matrix-0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.348219 neuro_fuzzy_matrix-0.1/
--rw-rw-rw-   0        0        0      127 2024-04-07 17:25:30.348219 neuro_fuzzy_matrix-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4099 2024-03-26 17:51:24.000000 neuro_fuzzy_matrix-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.331378 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/
--rw-rw-rw-   0        0        0    22957 2024-04-07 17:24:26.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/__init__.py
--rw-rw-rw-   0        0        0      547 2024-03-26 16:57:26.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/test_save.py
--rw-rw-rw-   0        0        0     1960 2024-03-26 14:31:04.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_full.py
--rw-rw-rw-   0        0        0     2820 2024-03-26 16:55:01.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_not_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.346224 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/
--rw-rw-rw-   0        0        0      127 2024-04-07 17:25:29.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 17:25:29.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 17:25:30.350214 neuro_fuzzy_matrix-0.1/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-03-28 09:49:21.000000 neuro_fuzzy_matrix-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:27:47.525605 neuro_fuzzy_matrix-0.2/
+-rw-rw-rw-   0        0        0      127 2024-05-28 11:27:47.526601 neuro_fuzzy_matrix-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4099 2024-03-26 17:51:24.000000 neuro_fuzzy_matrix-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 11:27:47.494089 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/
+-rw-rw-rw-   0        0        0    16999 2024-05-28 09:41:36.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/__init__.py
+-rw-rw-rw-   0        0        0     3278 2024-05-27 11:49:37.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/test.py
+-rw-rw-rw-   0        0        0      547 2024-03-26 16:57:26.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/test_save.py
+-rw-rw-rw-   0        0        0     1960 2024-03-26 14:31:04.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/tests_full.py
+-rw-rw-rw-   0        0        0     2820 2024-03-26 16:55:01.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/tests_not_rules.py
+-rw-rw-rw-   0        0        0     1057 2024-05-23 18:25:36.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/tests_save.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:27:47.522612 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/
+-rw-rw-rw-   0        0        0      127 2024-05-28 11:27:46.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-28 11:27:46.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:27:46.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 17:25:29.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-05-28 11:27:46.000000 neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:27:47.528214 neuro_fuzzy_matrix-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-05-28 11:19:25.000000 neuro_fuzzy_matrix-0.2/setup.py
```

### Comparing `neuro_fuzzy_matrix-0.1/README.md` & `neuro_fuzzy_matrix-0.2/README.md`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/test_save.py` & `neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/test_save.py`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_full.py` & `neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/tests_full.py`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_not_rules.py` & `neuro_fuzzy_matrix-0.2/neuro_fuzzy_matrix/tests_not_rules.py`

 * *Files identical despite different names*

