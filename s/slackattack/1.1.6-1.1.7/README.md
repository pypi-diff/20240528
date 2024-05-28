# Comparing `tmp/slackattack-1.1.6.tar.gz` & `tmp/slackattack-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackattack-1.1.6.tar", last modified: Tue May 28 01:59:42 2024, max compression
+gzip compressed data, was "slackattack-1.1.7.tar", last modified: Tue May 28 02:04:02 2024, max compression
```

## Comparing `slackattack-1.1.6.tar` & `slackattack-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:59:42.086888 slackattack-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:59:37.000000 slackattack-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:59:42.086888 slackattack-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:59:37.000000 slackattack-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:59:37.000000 slackattack-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:59:42.086888 slackattack-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 01:59:37.000000 slackattack-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:59:42.086888 slackattack-1.1.6/slackattack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    34024 2024-05-28 01:59:37.000000 slackattack-1.1.6/slackattack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:04:02.745367 slackattack-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 02:03:59.000000 slackattack-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 02:04:02.745367 slackattack-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 02:03:59.000000 slackattack-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 02:03:59.000000 slackattack-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:04:02.745367 slackattack-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 02:03:59.000000 slackattack-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:04:02.745367 slackattack-1.1.7/slackattack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 02:04:02.000000 slackattack-1.1.7/slackattack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 02:04:02.000000 slackattack-1.1.7/slackattack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:04:02.000000 slackattack-1.1.7/slackattack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 02:04:02.000000 slackattack-1.1.7/slackattack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:04:02.000000 slackattack-1.1.7/slackattack.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41129 2024-05-28 02:03:59.000000 slackattack-1.1.7/slackattack.py
```

### Comparing `slackattack-1.1.6/LICENSE` & `slackattack-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.6/PKG-INFO` & `slackattack-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.6
+Version: 1.1.7
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `slackattack-1.1.6/README.md` & `slackattack-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.6/pyproject.toml` & `slackattack-1.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slackattack"
-version = "1.1.6"
+version = "1.1.7"
 description = "Slack post-exploitation script for leaked bot tokens and xoxd cookies"
 authors = [
   { name = "Jonathan Stines", email = "jonathan.stines@gmail.com" }
 ]
 readme = "README.md"
 license = { text = "UNKNOWN" }
 classifiers = [
```

### Comparing `slackattack-1.1.6/setup.py` & `slackattack-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         requirements = f.read().splitlines() if os.path.exists('requirements.txt') else []
 
 except FileNotFoundError:
     requirements = []
 
 setup(
     name='slackattack',
-    version='1.1.6',
+    version='1.1.7',
     author='Jonathan Stines',
     description='Slack post-exploitation script for leaked bot tokens and "d" cookies',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fr4nk3nst1ner/slackattack',
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `slackattack-1.1.6/slackattack.egg-info/PKG-INFO` & `slackattack-1.1.7/slackattack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.6
+Version: 1.1.7
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

