# Comparing `tmp/aistrainer-0.0.1.tar.gz` & `tmp/aistrainer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistrainer-0.0.1.tar", last modified: Tue May 28 09:18:45 2024, max compression
+gzip compressed data, was "aistrainer-0.0.2.tar", last modified: Tue May 28 09:22:57 2024, max compression
```

## Comparing `aistrainer-0.0.1.tar` & `aistrainer-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:18:45.575739 aistrainer-0.0.1/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.1/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6535 2024-05-28 09:18:45.575739 aistrainer-0.0.1/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     5826 2024-05-28 09:16:12.000000 aistrainer-0.0.1/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      740 2024-05-27 16:03:10.000000 aistrainer-0.0.1/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-28 09:18:45.575739 aistrainer-0.0.1/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:18:45.575739 aistrainer-0.0.1/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:18:45.575739 aistrainer-0.0.1/src/aistrainer/
--rw-r--r--   0 man4j     (1000) man4j     (1000)    10454 2024-05-27 15:26:56.000000 aistrainer-0.0.1/src/aistrainer/aistrainer.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.1/src/aistrainer/models.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:18:45.575739 aistrainer-0.0.1/src/aistrainer.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6535 2024-05-28 09:18:45.000000 aistrainer-0.0.1/src/aistrainer.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-05-28 09:18:45.000000 aistrainer-0.0.1/src/aistrainer.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-28 09:18:45.000000 aistrainer-0.0.1/src/aistrainer.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-05-28 09:18:45.000000 aistrainer-0.0.1/src/aistrainer.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-05-28 09:18:45.000000 aistrainer-0.0.1/src/aistrainer.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:22:57.807016 aistrainer-0.0.2/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.2/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6536 2024-05-28 09:22:57.807016 aistrainer-0.0.2/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     5826 2024-05-28 09:16:12.000000 aistrainer-0.0.2/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      741 2024-05-28 09:20:55.000000 aistrainer-0.0.2/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-28 09:22:57.807016 aistrainer-0.0.2/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:22:57.807016 aistrainer-0.0.2/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:22:57.807016 aistrainer-0.0.2/src/aistrainer/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)    10454 2024-05-27 15:26:56.000000 aistrainer-0.0.2/src/aistrainer/aistrainer.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.2/src/aistrainer/models.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 09:22:57.807016 aistrainer-0.0.2/src/aistrainer.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6536 2024-05-28 09:22:57.000000 aistrainer-0.0.2/src/aistrainer.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-05-28 09:22:57.000000 aistrainer-0.0.2/src/aistrainer.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-28 09:22:57.000000 aistrainer-0.0.2/src/aistrainer.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-05-28 09:22:57.000000 aistrainer-0.0.2/src/aistrainer.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-05-28 09:22:57.000000 aistrainer-0.0.2/src/aistrainer.egg-info/top_level.txt
```

### Comparing `aistrainer-0.0.1/LICENSE` & `aistrainer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.1/PKG-INFO` & `aistrainer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aistrainer
-Version: 0.0.1
-Summary: AI Specialization Trainer for LLM model
+Version: 0.0.2
+Summary: AI Specialization Trainer for LLM models
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aistrainer-0.0.1/README.md` & `aistrainer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.1/pyproject.toml` & `aistrainer-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aistrainer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
-description = "AI Specialization Trainer for LLM model"
+description = "AI Specialization Trainer for LLM models"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `aistrainer-0.0.1/src/aistrainer/aistrainer.py` & `aistrainer-0.0.2/src/aistrainer/aistrainer.py`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.1/src/aistrainer/models.py` & `aistrainer-0.0.2/src/aistrainer/models.py`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.1/src/aistrainer.egg-info/PKG-INFO` & `aistrainer-0.0.2/src/aistrainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aistrainer
-Version: 0.0.1
-Summary: AI Specialization Trainer for LLM model
+Version: 0.0.2
+Summary: AI Specialization Trainer for LLM models
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

