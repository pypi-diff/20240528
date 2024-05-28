# Comparing `tmp/phones_local-0.0.28.tar.gz` & `tmp/phones_local-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.28.tar", last modified: Sun May 26 21:36:02 2024, max compression
+gzip compressed data, was "phones_local-0.0.29.tar", last modified: Mon May 27 19:31:44 2024, max compression
```

## Comparing `phones_local-0.0.28.tar` & `phones_local-0.0.29.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:36:02.676454 phones_local-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-26 21:35:37.000000 phones_local-0.0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.672454 phones_local-0.0.28/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-26 21:35:43.000000 phones_local-0.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:36:02.676454 phones_local-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 21:35:37.000000 phones_local-0.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 19:31:44.023930 phones_local-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-27 19:31:18.000000 phones_local-0.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.019930 phones_local-0.0.29/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 19:31:24.000000 phones_local-0.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:31:44.023930 phones_local-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-27 19:31:18.000000 phones_local-0.0.29/setup.py
```

### Comparing `phones_local-0.0.28/PKG-INFO` & `phones_local-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.28
+Version: 0.0.29
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.28/README.md` & `phones_local-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.28/phones_local/src/phone_local_constans.py` & `phones_local-0.0.29/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.28/phones_local/src/phones_local.py` & `phones_local-0.0.29/phones_local/src/phones_local.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.28/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.29/phones_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.28
+Version: 0.0.29
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.28/pyproject.toml` & `phones_local-0.0.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.28/setup.py` & `phones_local-0.0.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.28',  # https://pypi.org/project/phones-local/
+    version='0.0.29',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

