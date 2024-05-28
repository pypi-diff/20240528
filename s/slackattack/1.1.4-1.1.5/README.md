# Comparing `tmp/slackattack-1.1.4.tar.gz` & `tmp/slackattack-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackattack-1.1.4.tar", last modified: Tue May 28 01:41:10 2024, max compression
+gzip compressed data, was "slackattack-1.1.5.tar", last modified: Tue May 28 01:56:10 2024, max compression
```

## Comparing `slackattack-1.1.4.tar` & `slackattack-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:10.078549 slackattack-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:41:04.000000 slackattack-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:41:10.078549 slackattack-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:41:04.000000 slackattack-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:41:04.000000 slackattack-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:41:10.078549 slackattack-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 01:41:04.000000 slackattack-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:10.078549 slackattack-1.1.4/slackattack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:41:10.000000 slackattack-1.1.4/slackattack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 01:41:10.000000 slackattack-1.1.4/slackattack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:41:10.000000 slackattack-1.1.4/slackattack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:41:10.000000 slackattack-1.1.4/slackattack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:41:10.000000 slackattack-1.1.4/slackattack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:56:10.352348 slackattack-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:56:06.000000 slackattack-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:56:10.352348 slackattack-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:56:06.000000 slackattack-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:56:06.000000 slackattack-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:56:10.352348 slackattack-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 01:56:06.000000 slackattack-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:56:10.352348 slackattack-1.1.5/slackattack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34078 2024-05-28 01:56:06.000000 slackattack-1.1.5/slackattack.py
```

### Comparing `slackattack-1.1.4/LICENSE` & `slackattack-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.4/PKG-INFO` & `slackattack-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.4
+Version: 1.1.5
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `slackattack-1.1.4/README.md` & `slackattack-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.4/pyproject.toml` & `slackattack-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slackattack"
-version = "1.1.4"
+version = "1.1.5"
 description = "Slack post-exploitation script for leaked bot tokens and xoxd cookies"
 authors = [
   { name = "Jonathan Stines", email = "jonathan.stines@gmail.com" }
 ]
 readme = "README.md"
 license = { text = "UNKNOWN" }
 classifiers = [
```

### Comparing `slackattack-1.1.4/setup.py` & `slackattack-1.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,22 @@
         requirements = f.read().splitlines() if os.path.exists('requirements.txt') else []
 
 except FileNotFoundError:
     requirements = []
 
 setup(
     name='slackattack',
-    version='1.1.4',
+    version='1.1.5',
     author='Jonathan Stines',
     description='Slack post-exploitation script for leaked bot tokens and "d" cookies',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fr4nk3nst1ner/slackattack',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-)
+    scripts=['slackattack.py'],  
+)
```

### Comparing `slackattack-1.1.4/slackattack.egg-info/PKG-INFO` & `slackattack-1.1.5/slackattack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.4
+Version: 1.1.5
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

