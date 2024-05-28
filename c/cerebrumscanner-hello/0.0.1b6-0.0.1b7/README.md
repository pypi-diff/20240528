# Comparing `tmp/cerebrumscanner_hello-0.0.1b6.tar.gz` & `tmp/cerebrumscanner_hello-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner_hello-0.0.1b6.tar", last modified: Tue May 28 06:47:04 2024, max compression
+gzip compressed data, was "cerebrumscanner_hello-0.0.1b7.tar", last modified: Tue May 28 06:52:20 2024, max compression
```

## Comparing `cerebrumscanner_hello-0.0.1b6.tar` & `cerebrumscanner_hello-0.0.1b7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:47:04.481324 cerebrumscanner_hello-0.0.1b6/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 06:47:04.481324 cerebrumscanner_hello-0.0.1b6/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b6/README.md
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:47:04.481324 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:39:35.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello/__init__.py
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello/main.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:47:04.481324 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello.egg-info/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 06:47:04.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello.egg-info/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      262 2024-05-28 06:47:04.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello.egg-info/SOURCES.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:47:04.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello.egg-info/dependency_links.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       22 2024-05-28 06:47:04.000000 cerebrumscanner_hello-0.0.1b6/cerebrumscanner_hello.egg-info/top_level.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:47:04.481324 cerebrumscanner_hello-0.0.1b6/setup.cfg
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      167 2024-05-28 06:45:02.000000 cerebrumscanner_hello-0.0.1b6/setup.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:52:20.983335 cerebrumscanner_hello-0.0.1b7/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 06:52:20.983335 cerebrumscanner_hello-0.0.1b7/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b7/README.md
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:52:20.983335 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       31 2024-05-28 06:51:31.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello/__init__.py
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-28 06:36:11.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello/main.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:52:20.983335 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello.egg-info/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)       67 2024-05-28 06:52:20.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello.egg-info/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      262 2024-05-28 06:52:20.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:52:20.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       22 2024-05-28 06:52:20.000000 cerebrumscanner_hello-0.0.1b7/cerebrumscanner_hello.egg-info/top_level.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:52:20.983335 cerebrumscanner_hello-0.0.1b7/setup.cfg
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      167 2024-05-28 06:52:06.000000 cerebrumscanner_hello-0.0.1b7/setup.py
```

### Comparing `cerebrumscanner_hello-0.0.1b6/README.md` & `cerebrumscanner_hello-0.0.1b7/README.md`

 * *Files identical despite different names*

