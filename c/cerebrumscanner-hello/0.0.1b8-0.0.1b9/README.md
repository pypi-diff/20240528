# Comparing `tmp/cerebrumscanner_hello-0.0.1b8.tar.gz` & `tmp/cerebrumscanner_hello-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner_hello-0.0.1b8.tar", last modified: Tue May 28 07:25:58 2024, max compression
+gzip compressed data, was "cerebrumscanner_hello-0.0.1b9.tar", last modified: Tue May 28 07:31:17 2024, max compression
```

## Comparing `cerebrumscanner_hello-0.0.1b8.tar` & `cerebrumscanner_hello-0.0.1b9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b8/README.md
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/setup.cfg
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      260 2024-05-28 07:25:48.000000 cerebrumscanner_hello-0.0.1b8/setup.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/src/
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:20:36.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello/__init__.py
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello/main.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:25:58.740472 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello.egg-info/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 07:25:58.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello.egg-info/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      286 2024-05-28 07:25:58.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello.egg-info/SOURCES.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 07:25:58.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello.egg-info/dependency_links.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       22 2024-05-28 07:25:58.000000 cerebrumscanner_hello-0.0.1b8/src/cerebrumscanner_hello.egg-info/top_level.txt
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:31:17.262545 cerebrumscanner_hello-0.0.1b9/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 07:31:17.262545 cerebrumscanner_hello-0.0.1b9/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b9/README.md
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 07:31:17.262545 cerebrumscanner_hello-0.0.1b9/setup.cfg
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      260 2024-05-28 07:30:20.000000 cerebrumscanner_hello-0.0.1b9/setup.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:31:17.258545 cerebrumscanner_hello-0.0.1b9/src/
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:31:17.258545 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:20:36.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello/__init__.py
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello/main.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 07:31:17.262545 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello.egg-info/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 07:31:17.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello.egg-info/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      286 2024-05-28 07:31:17.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 07:31:17.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       22 2024-05-28 07:31:17.000000 cerebrumscanner_hello-0.0.1b9/src/cerebrumscanner_hello.egg-info/top_level.txt
```

### Comparing `cerebrumscanner_hello-0.0.1b8/README.md` & `cerebrumscanner_hello-0.0.1b9/README.md`

 * *Files identical despite different names*

