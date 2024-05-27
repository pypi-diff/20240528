# Comparing `tmp/timelined_array-0.0.3.tar.gz` & `tmp/timelined_array-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelined_array-0.0.3.tar", last modified: Mon May 27 20:16:03 2024, max compression
+gzip compressed data, was "timelined_array-0.0.4.tar", last modified: Mon May 27 23:29:50 2024, max compression
```

## Comparing `timelined_array-0.0.3.tar` & `timelined_array-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-27 20:15:51.409943 timelined_array-0.0.3/LICENSE
--rw-r--r--   0        0        0       18 2024-05-27 20:15:51.409943 timelined_array-0.0.3/README.md
--rw-r--r--   0        0        0      613 2024-05-27 20:16:03.761940 timelined_array-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-27 20:15:51.409943 timelined_array-0.0.3/src/timelined_array/__init__.py
--rw-r--r--   0        0        0    31210 2024-05-27 20:15:51.409943 timelined_array-0.0.3/src/timelined_array/time.py
--rw-r--r--   0        0        0        0 2024-05-27 20:15:51.409943 timelined_array-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 timelined_array-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-27 23:29:37.717195 timelined_array-0.0.4/LICENSE
+-rw-r--r--   0        0        0       18 2024-05-27 23:29:37.717195 timelined_array-0.0.4/README.md
+-rw-r--r--   0        0        0      613 2024-05-27 23:29:50.913127 timelined_array-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-27 23:29:37.717195 timelined_array-0.0.4/src/timelined_array/__init__.py
+-rw-r--r--   0        0        0    50908 2024-05-27 23:29:37.717195 timelined_array-0.0.4/src/timelined_array/time.py
+-rw-r--r--   0        0        0        0 2024-05-27 23:29:37.717195 timelined_array-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 timelined_array-0.0.4/PKG-INFO
```

### Comparing `timelined_array-0.0.3/LICENSE` & `timelined_array-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.3/pyproject.toml` & `timelined_array-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "numpy",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

