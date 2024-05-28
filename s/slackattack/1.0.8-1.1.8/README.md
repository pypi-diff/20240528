# Comparing `tmp/slackattack-1.0.8.tar.gz` & `tmp/slackattack-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackattack-1.0.8.tar", last modified: Mon May 27 22:29:41 2024, max compression
+gzip compressed data, was "slackattack-1.1.8.tar", last modified: Tue May 28 01:29:17 2024, max compression
```

## Comparing `slackattack-1.0.8.tar` & `slackattack-1.1.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:29:41.381497 slackattack-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 22:29:38.000000 slackattack-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-27 22:29:41.381497 slackattack-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-27 22:29:38.000000 slackattack-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:29:41.381497 slackattack-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-27 22:29:38.000000 slackattack-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:29:41.381497 slackattack-1.0.8/slackattack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-27 22:29:41.000000 slackattack-1.0.8/slackattack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 22:29:41.000000 slackattack-1.0.8/slackattack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:29:41.000000 slackattack-1.0.8/slackattack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 22:29:41.000000 slackattack-1.0.8/slackattack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:29:41.000000 slackattack-1.0.8/slackattack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:29:17.209452 slackattack-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:29:08.000000 slackattack-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-28 01:29:17.205452 slackattack-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:29:08.000000 slackattack-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:29:08.000000 slackattack-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:29:17.209452 slackattack-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-28 01:29:08.000000 slackattack-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:29:17.205452 slackattack-1.1.8/slackattack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-28 01:29:17.000000 slackattack-1.1.8/slackattack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 01:29:17.000000 slackattack-1.1.8/slackattack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:29:17.000000 slackattack-1.1.8/slackattack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:29:17.000000 slackattack-1.1.8/slackattack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:29:17.000000 slackattack-1.1.8/slackattack.egg-info/top_level.txt
```

### Comparing `slackattack-1.0.8/LICENSE` & `slackattack-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slackattack-1.0.8/PKG-INFO` & `slackattack-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.0.8
+Version: 1.1.8
 Summary: Description of your tool
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Slackattack
 
 ## Background
```

### Comparing `slackattack-1.0.8/README.md` & `slackattack-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `slackattack-1.0.8/setup.py` & `slackattack-1.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,21 @@
         requirements = f.read().splitlines() if os.path.exists('requirements.txt') else []
 
 except FileNotFoundError:
     requirements = []
 
 setup(
     name='slackattack',
-    version='1.0.8',
+    version='1.1.8',
     author='Jonathan Stines',
     description='Description of your tool',
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
-    python_requires='>=3.6',
 )
```

### Comparing `slackattack-1.0.8/slackattack.egg-info/PKG-INFO` & `slackattack-1.1.8/slackattack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.0.8
+Version: 1.1.8
 Summary: Description of your tool
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Slackattack
 
 ## Background
```

