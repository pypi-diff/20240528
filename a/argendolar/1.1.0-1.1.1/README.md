# Comparing `tmp/argendolar-1.1.0.tar.gz` & `tmp/argendolar-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-1.1.0.tar", last modified: Tue May 28 14:29:39 2024, max compression
+gzip compressed data, was "argendolar-1.1.1.tar", last modified: Tue May 28 15:09:44 2024, max compression
```

## Comparing `argendolar-1.1.0.tar` & `argendolar-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 14:29:39.054025 argendolar-1.1.0/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-1.1.0/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 14:29:39.053758 argendolar-1.1.0/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     3936 2024-05-28 13:44:59.000000 argendolar-1.1.0/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 14:29:39.051956 argendolar-1.1.0/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-1.1.0/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492     6350 2024-05-28 13:30:31.000000 argendolar-1.1.0/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-1.1.0/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 14:29:39.053361 argendolar-1.1.0/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 14:29:39.000000 argendolar-1.1.0/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-28 14:29:39.000000 argendolar-1.1.0/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-28 14:29:39.000000 argendolar-1.1.0/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-28 14:29:39.000000 argendolar-1.1.0/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-28 14:29:39.000000 argendolar-1.1.0/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-28 14:29:39.054084 argendolar-1.1.0/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-28 14:29:31.000000 argendolar-1.1.0/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.893748 argendolar-1.1.1/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-1.1.1/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 15:09:44.893494 argendolar-1.1.1/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     3936 2024-05-28 13:44:59.000000 argendolar-1.1.1/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.891331 argendolar-1.1.1/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-1.1.1/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     6351 2024-05-28 14:58:58.000000 argendolar-1.1.1/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-1.1.1/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 15:09:44.893121 argendolar-1.1.1/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4620 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-28 15:09:44.000000 argendolar-1.1.1/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-28 15:09:44.893810 argendolar-1.1.1/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-28 15:09:41.000000 argendolar-1.1.1/setup.py
```

### Comparing `argendolar-1.1.0/LICENSE` & `argendolar-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.0/PKG-INFO` & `argendolar-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-1.1.0/README.md` & `argendolar-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.0/argendolar/argendolar.py` & `argendolar-1.1.1/argendolar/argendolar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 
 import pandas as pd
 
-from tipo_dolares import TipoDivisas
+from .tipo_dolares import TipoDivisas
 
 
 class Argendolar:
     def __init__(self):
         """
         Initialize the Argendolar class.
         """
```

### Comparing `argendolar-1.1.0/argendolar.egg-info/PKG-INFO` & `argendolar-1.1.1/argendolar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-1.1.0/setup.py` & `argendolar-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='1.1.0',
+    version='1.1.1',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

