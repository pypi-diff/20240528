# Comparing `tmp/pyerualjetwork-1.2.9.tar.gz` & `tmp/pyerualjetwork-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.9.tar", last modified: Tue May 28 20:35:49 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.0.tar", last modified: Tue May 28 20:46:11 2024, max compression
```

## Comparing `pyerualjetwork-1.2.9.tar` & `pyerualjetwork-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.753892 pyerualjetwork-1.2.9/
--rw-rw-rw-   0        0        0      452 2024-05-28 20:35:49.752888 pyerualjetwork-1.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.698391 pyerualjetwork-1.2.9/plan/
--rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.2.9/plan/__init__.py
--rw-rw-rw-   0        0        0    42347 2024-05-28 20:20:20.000000 pyerualjetwork-1.2.9/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.748899 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-28 20:35:49.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 20:35:49.754880 pyerualjetwork-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      864 2024-05-28 20:35:41.000000 pyerualjetwork-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.074909 pyerualjetwork-1.3.0/
+-rw-rw-rw-   0        0        0      421 2024-05-28 20:46:11.073909 pyerualjetwork-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.051211 pyerualjetwork-1.3.0/plan/
+-rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.3.0/plan/__init__.py
+-rw-rw-rw-   0        0        0    42347 2024-05-28 20:20:20.000000 pyerualjetwork-1.3.0/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:46:11.071905 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      421 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-28 20:46:10.000000 pyerualjetwork-1.3.0/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 20:46:11.075904 pyerualjetwork-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-28 20:46:04.000000 pyerualjetwork-1.3.0/setup.py
```

### Comparing `pyerualjetwork-1.2.9/plan/plan.py` & `pyerualjetwork-1.3.0/plan/plan.py`

 * *Files identical despite different names*

### Comparing `pyerualjetwork-1.2.9/setup.py` & `pyerualjetwork-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.2.9",
+      version = "1.3.0",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
-      description= "Advanced python deep learning library. New Visualize parameter added ('y' or 'n') for TrainPlan and TestPLAN funcs. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
+      description= "Advanced python deep learning library. New Visualize parameter added ('y' or 'n') for TrainPLAN and TestPLAN funcs. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
-      install_requires=[
-          'numpy',
-          'scipy',
-            'time',
-            'math',
-            'colorama',
-            'typing'
-            ],
-      
-       extras_require={
-          'visualization': ['matplotlib','seaborn']
-      }
+
       
       )
```

