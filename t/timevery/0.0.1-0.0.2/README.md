# Comparing `tmp/timevery-0.0.1.tar.gz` & `tmp/timevery-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timevery-0.0.1.tar", last modified: Tue May 21 09:23:10 2024, max compression
+gzip compressed data, was "timevery-0.0.2.tar", last modified: Tue May 28 02:57:53 2024, max compression
```

## Comparing `timevery-0.0.1.tar` & `timevery-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:23:10.630471 timevery-0.0.1/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-13 10:37:19.000000 timevery-0.0.1/LICENSE
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     1704 2024-05-21 09:23:10.630471 timevery-0.0.1/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       55 2024-05-21 09:22:51.000000 timevery-0.0.1/README.md
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      509 2024-05-21 09:22:42.000000 timevery-0.0.1/pyproject.toml
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:23:10.630471 timevery-0.0.1/setup.cfg
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:18:30.000000 timevery-0.0.1/setup.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:23:10.630471 timevery-0.0.1/src/
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:23:10.630471 timevery-0.0.1/src/timevery/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        0 2024-05-13 10:41:57.000000 timevery-0.0.1/src/timevery/__init__.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1806 2024-05-13 10:49:10.000000 timevery-0.0.1/src/timevery/timer.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:23:10.630471 timevery-0.0.1/src/timevery.egg-info/
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     1704 2024-05-21 09:23:10.000000 timevery-0.0.1/src/timevery.egg-info/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      232 2024-05-21 09:23:10.000000 timevery-0.0.1/src/timevery.egg-info/SOURCES.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-21 09:23:10.000000 timevery-0.0.1/src/timevery.egg-info/dependency_links.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-21 09:23:10.000000 timevery-0.0.1/src/timevery.egg-info/top_level.txt
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.881859 timevery-0.0.2/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-13 10:37:19.000000 timevery-0.0.2/LICENSE
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     6185 2024-05-28 02:57:53.877859 timevery-0.0.2/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     4516 2024-05-28 02:57:14.000000 timevery-0.0.2/README.md
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      540 2024-05-28 02:29:51.000000 timevery-0.0.2/pyproject.toml
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-28 02:57:53.881859 timevery-0.0.2/setup.cfg
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:18:30.000000 timevery-0.0.2/setup.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/timevery/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      921 2024-05-28 02:41:39.000000 timevery-0.0.2/src/timevery/__init__.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     5236 2024-05-28 02:53:26.000000 timevery-0.0.2/src/timevery/timer.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/timevery.egg-info/
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     6185 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      267 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        5 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/requires.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/top_level.txt
```

### Comparing `timevery-0.0.1/LICENSE` & `timevery-0.0.2/LICENSE`

 * *Files identical despite different names*

