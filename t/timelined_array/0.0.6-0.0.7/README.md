# Comparing `tmp/timelined_array-0.0.6.tar.gz` & `tmp/timelined_array-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelined_array-0.0.6.tar", last modified: Tue May 28 14:29:52 2024, max compression
+gzip compressed data, was "timelined_array-0.0.7.tar", last modified: Tue May 28 14:51:08 2024, max compression
```

## Comparing `timelined_array-0.0.6.tar` & `timelined_array-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-28 14:29:37.323919 timelined_array-0.0.6/LICENSE
--rw-r--r--   0        0        0     2859 2024-05-28 14:29:37.323919 timelined_array-0.0.6/README.md
--rw-r--r--   0        0        0      613 2024-05-28 14:29:52.311951 timelined_array-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       97 2024-05-28 14:29:37.323919 timelined_array-0.0.6/src/timelined_array/__init__.py
--rw-r--r--   0        0        0    52532 2024-05-28 14:29:37.323919 timelined_array-0.0.6/src/timelined_array/time.py
--rw-r--r--   0        0        0        0 2024-05-28 14:29:37.323919 timelined_array-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 timelined_array-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 14:50:56.202655 timelined_array-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2859 2024-05-28 14:50:56.202655 timelined_array-0.0.7/README.md
+-rw-r--r--   0        0        0      613 2024-05-28 14:51:08.146571 timelined_array-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-28 14:50:56.202655 timelined_array-0.0.7/src/timelined_array/__init__.py
+-rw-r--r--   0        0        0    52649 2024-05-28 14:50:56.202655 timelined_array-0.0.7/src/timelined_array/time.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:50:56.202655 timelined_array-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 timelined_array-0.0.7/PKG-INFO
```

### Comparing `timelined_array-0.0.6/LICENSE` & `timelined_array-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.6/README.md` & `timelined_array-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.6/pyproject.toml` & `timelined_array-0.0.7/pyproject.toml`

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
-version = "0.0.6"
+version = "0.0.7"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `timelined_array-0.0.6/src/timelined_array/time.py` & `timelined_array-0.0.7/src/timelined_array/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,18 @@
             # if arguments are an uniform list of timelined array
             # (often use to make mean and std of synchonized timelines), we pick up the first one.
             # but it also means default numpy packing will set the new dimension as dimension 0.
             # As such, the current time dimension will have to be the time dimension of the listed elements,
             # +1 (a.k.a. shifted one dimension deeper)
 
             for element in data:
-                time_dimension = getattr(element, "time_dimension", None) + 1
+                time_dimension = getattr(element, "time_dimension", None)
+                if time_dimension is None:
+                    break
+                time_dimension = time_dimension + 1
                 _unpacking = True
                 break
             else:
                 time_dimension = 0
 
         if time_dimension is None:
             time_dimension = 0
```

### Comparing `timelined_array-0.0.6/PKG-INFO` & `timelined_array-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelined_array
-Version: 0.0.6
+Version: 0.0.7
 Summary: Manage easily 1 or multidimensionnal samples numpy arrays that are time related. Extends numpy without removing any of it's abilities on such arrays.
 Author-Email: Timothe Jost <timothe.jost@wanadoo.fr>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
```

