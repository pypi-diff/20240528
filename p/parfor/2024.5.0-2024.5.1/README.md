# Comparing `tmp/parfor-2024.5.0.tar.gz` & `tmp/parfor-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parfor-2024.5.0.tar", max compression
+gzip compressed data, was "parfor-2024.5.1.tar", max compression
```

## Comparing `parfor-2024.5.0.tar` & `parfor-2024.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.5.0/LICENSE
--rw-r--r--   0        0        0     5711 2024-05-24 14:54:49.226658 parfor-2024.5.0/README.md
--rw-r--r--   0        0        0    28025 2024-05-24 14:54:50.062661 parfor-2024.5.0/parfor/__init__.py
--rw-r--r--   0        0        0     4283 2024-04-15 13:16:29.130534 parfor-2024.5.0/parfor/pickler.py
--rw-r--r--   0        0        0      603 2024-05-24 14:41:51.587735 parfor-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 parfor-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     5711 2024-05-24 14:54:49.226658 parfor-2024.5.1/README.md
+-rw-r--r--   0        0        0    28062 2024-05-28 14:33:21.870805 parfor-2024.5.1/parfor/__init__.py
+-rw-r--r--   0        0        0     4283 2024-04-15 13:16:29.130534 parfor-2024.5.1/parfor/pickler.py
+-rw-r--r--   0        0        0      603 2024-05-28 14:34:13.130996 parfor-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 parfor-2024.5.1/PKG-INFO
```

### Comparing `parfor-2024.5.0/LICENSE` & `parfor-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parfor-2024.5.0/README.md` & `parfor-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `parfor-2024.5.0/parfor/__init__.py` & `parfor-2024.5.1/parfor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,16 @@
         new pool. The pool will close itself after 10 minutes of idle time. """
 
     instance = None
 
     def __new__(cls, n_processes: int = None, *args: Any, **kwargs: Any) -> PoolSingleton:
         # restart if any workers have shut down or if we want to have a different number of processes
         if cls.instance is not None:
-            if cls.instance.n_workers.value < cls.instance.n_processes or cls.instance.n_processes != n_processes:
+            if (cls.instance.n_workers.value < cls.instance.n_processes or
+                    cls.instance.n_processes != (n_processes or cpu_count)):
                 cls.instance.close()
         if cls.instance is None or not cls.instance.is_alive:
             new = super().__new__(cls)
             new.n_processes = n_processes or cpu_count
             new.instance = new
             new.is_started = False
             ctx = Context()
```

### Comparing `parfor-2024.5.0/parfor/pickler.py` & `parfor-2024.5.1/parfor/pickler.py`

 * *Files identical despite different names*

### Comparing `parfor-2024.5.0/pyproject.toml` & `parfor-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parfor"
-version = "2024.5.0"
+version = "2024.5.1"
 description = "A package to mimic the use of parfor as done in Matlab."
 authors = ["Wim Pomp <wimpomp@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["parfor", "concurrency", "multiprocessing", "parallel"]
 repository = "https://github.com/wimpomp/parfor"
```

### Comparing `parfor-2024.5.0/PKG-INFO` & `parfor-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parfor
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: A package to mimic the use of parfor as done in Matlab.
 Home-page: https://github.com/wimpomp/parfor
 License: GPLv3
 Keywords: parfor,concurrency,multiprocessing,parallel
 Author: Wim Pomp
 Author-email: wimpomp@gmail.com
 Requires-Python: >=3.10,<4.0
```

