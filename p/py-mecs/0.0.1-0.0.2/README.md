# Comparing `tmp/py_mecs-0.0.1.tar.gz` & `tmp/py_mecs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_mecs-0.0.1.tar", last modified: Tue May 28 18:30:48 2024, max compression
+gzip compressed data, was "py_mecs-0.0.2.tar", last modified: Tue May 28 19:10:03 2024, max compression
```

## Comparing `py_mecs-0.0.1.tar` & `py_mecs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 18:30:48.947302 py_mecs-0.0.1/
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     1068 2024-05-28 11:50:45.000000 py_mecs-0.0.1/LICENSE
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      574 2024-05-28 18:30:48.947302 py_mecs-0.0.1/PKG-INFO
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       52 2024-05-28 11:50:45.000000 py_mecs-0.0.1/README.md
-drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 18:30:48.943969 py_mecs-0.0.1/package/
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       27 2024-05-28 16:19:25.000000 py_mecs-0.0.1/package/__init__.py
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     2373 2024-05-28 15:59:42.000000 py_mecs-0.0.1/package/mecs.py
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     1468 2024-05-28 15:51:19.000000 py_mecs-0.0.1/package/mecs_short.py
-drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 18:30:48.947302 py_mecs-0.0.1/py_mecs.egg-info/
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      574 2024-05-28 18:30:48.000000 py_mecs-0.0.1/py_mecs.egg-info/PKG-INFO
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      214 2024-05-28 18:30:48.000000 py_mecs-0.0.1/py_mecs.egg-info/SOURCES.txt
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)        1 2024-05-28 18:30:48.000000 py_mecs-0.0.1/py_mecs.egg-info/dependency_links.txt
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)        8 2024-05-28 18:30:48.000000 py_mecs-0.0.1/py_mecs.egg-info/top_level.txt
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      592 2024-05-28 14:24:46.000000 py_mecs-0.0.1/pyproject.toml
--rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       38 2024-05-28 18:30:48.947302 py_mecs-0.0.1/setup.cfg
+drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 19:10:03.618642 py_mecs-0.0.2/
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     1068 2024-05-28 11:50:45.000000 py_mecs-0.0.2/LICENSE
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      574 2024-05-28 19:10:03.618642 py_mecs-0.0.2/PKG-INFO
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       52 2024-05-28 11:50:45.000000 py_mecs-0.0.2/README.md
+drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 19:10:03.618642 py_mecs-0.0.2/mecs/
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       27 2024-05-28 16:19:25.000000 py_mecs-0.0.2/mecs/__init__.py
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     2373 2024-05-28 15:59:42.000000 py_mecs-0.0.2/mecs/mecs.py
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)     1468 2024-05-28 15:51:19.000000 py_mecs-0.0.2/mecs/mecs_short.py
+drwxr-xr-x   0 arthurmaulii  (1000) arthurmaulii  (1001)        0 2024-05-28 19:10:03.618642 py_mecs-0.0.2/py_mecs.egg-info/
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      574 2024-05-28 19:10:03.000000 py_mecs-0.0.2/py_mecs.egg-info/PKG-INFO
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      205 2024-05-28 19:10:03.000000 py_mecs-0.0.2/py_mecs.egg-info/SOURCES.txt
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)        1 2024-05-28 19:10:03.000000 py_mecs-0.0.2/py_mecs.egg-info/dependency_links.txt
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)        5 2024-05-28 19:10:03.000000 py_mecs-0.0.2/py_mecs.egg-info/top_level.txt
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)      592 2024-05-28 19:06:35.000000 py_mecs-0.0.2/pyproject.toml
+-rw-r--r--   0 arthurmaulii  (1000) arthurmaulii  (1001)       38 2024-05-28 19:10:03.618642 py_mecs-0.0.2/setup.cfg
```

### Comparing `py_mecs-0.0.1/LICENSE` & `py_mecs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_mecs-0.0.1/PKG-INFO` & `py_mecs-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-mecs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple entity component system for python
 Author-email: Arthur Maul <arthurmiiengineering@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_mecs-0.0.1/package/mecs.py` & `py_mecs-0.0.2/mecs/mecs.py`

 * *Files identical despite different names*

### Comparing `py_mecs-0.0.1/package/mecs_short.py` & `py_mecs-0.0.2/mecs/mecs_short.py`

 * *Files identical despite different names*

### Comparing `py_mecs-0.0.1/py_mecs.egg-info/PKG-INFO` & `py_mecs-0.0.2/py_mecs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-mecs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple entity component system for python
 Author-email: Arthur Maul <arthurmiiengineering@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_mecs-0.0.1/pyproject.toml` & `py_mecs-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-mecs"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Arthur Maul", email="arthurmiiengineering@gmail.com" },
 ]
 description = "A simple entity component system for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

