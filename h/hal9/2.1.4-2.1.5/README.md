# Comparing `tmp/hal9-2.1.4.tar.gz` & `tmp/hal9-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.1.4.tar", max compression
+gzip compressed data, was "hal9-2.1.5.tar", max compression
```

## Comparing `hal9-2.1.4.tar` & `hal9-2.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2948 2024-05-18 19:36:24.912012 hal9-2.1.4/README.md
--rw-r--r--   0        0        0       86 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/create.py
--rw-r--r--   0        0        0      574 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/run.py
--rw-r--r--   0        0        0      352 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/targets/docker.py
--rw-r--r--   0        0        0     2021 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       38 2024-05-18 19:36:24.840013 hal9-2.1.4/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-18 19:36:24.840013 hal9-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 hal9-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-05-28 20:23:05.052425 hal9-2.1.5/README.md
+-rw-r--r--   0        0        0       86 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2021 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-28 20:23:04.592424 hal9-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 hal9-2.1.5/PKG-INFO
```

### Comparing `hal9-2.1.4/README.md` & `hal9-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/hal9/cli.py` & `hal9-2.1.5/hal9/cli.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/hal9/create.py` & `hal9-2.1.5/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/hal9/deploy.py` & `hal9-2.1.5/hal9/deploy.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/hal9/run.py` & `hal9-2.1.5/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/hal9/targets/hal9.py` & `hal9-2.1.5/hal9/targets/hal9.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.4/PKG-INFO` & `hal9-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.1.4
+Version: 2.1.5
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

