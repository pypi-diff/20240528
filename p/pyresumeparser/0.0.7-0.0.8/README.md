# Comparing `tmp/pyresumeparser-0.0.7.tar.gz` & `tmp/pyresumeparser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresumeparser-0.0.7.tar", last modified: Tue May 28 12:36:24 2024, max compression
+gzip compressed data, was "pyresumeparser-0.0.8.tar", last modified: Tue May 28 12:45:27 2024, max compression
```

## Comparing `pyresumeparser-0.0.7.tar` & `pyresumeparser-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.776125 pyresumeparser-0.0.7/
--rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:36:24.774981 pyresumeparser-0.0.7/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)     2435 2024-05-28 12:32:46.000000 pyresumeparser-0.0.7/README.md
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.767076 pyresumeparser-0.0.7/pyresumeparser/
--rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.7/pyresumeparser/__init__.py
--rw-r--r--   0 pluto      (501) staff       (20)     4734 2024-05-28 12:33:59.000000 pyresumeparser-0.0.7/pyresumeparser/main.py
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.772648 pyresumeparser-0.0.7/pyresumeparser.egg-info/
--rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/SOURCES.txt
--rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/dependency_links.txt
--rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/entry_points.txt
--rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/requires.txt
--rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/top_level.txt
--rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 12:36:24.776394 pyresumeparser-0.0.7/setup.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     1016 2024-05-28 12:34:54.000000 pyresumeparser-0.0.7/setup.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:45:27.705785 pyresumeparser-0.0.8/
+-rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:45:27.704624 pyresumeparser-0.0.8/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)     2435 2024-05-28 12:32:46.000000 pyresumeparser-0.0.8/README.md
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:45:27.696415 pyresumeparser-0.0.8/pyresumeparser/
+-rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.8/pyresumeparser/__init__.py
+-rw-r--r--   0 pluto      (501) staff       (20)     4734 2024-05-28 12:33:59.000000 pyresumeparser-0.0.8/pyresumeparser/main.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:45:27.702287 pyresumeparser-0.0.8/pyresumeparser.egg-info/
+-rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/SOURCES.txt
+-rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/dependency_links.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/entry_points.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/requires.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 12:45:27.000000 pyresumeparser-0.0.8/pyresumeparser.egg-info/top_level.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 12:45:27.706085 pyresumeparser-0.0.8/setup.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     1016 2024-05-28 12:41:51.000000 pyresumeparser-0.0.8/setup.py
```

### Comparing `pyresumeparser-0.0.7/PKG-INFO` & `pyresumeparser-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyresumeparser-0.0.7/README.md` & `pyresumeparser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.7/pyresumeparser/main.py` & `pyresumeparser-0.0.8/pyresumeparser/main.py`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.7/pyresumeparser.egg-info/PKG-INFO` & `pyresumeparser-0.0.8/pyresumeparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyresumeparser-0.0.7/setup.py` & `pyresumeparser-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyresumeparser',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[
         'pdfminer.six==20231228',
         'spacy==3.7.4',
         'spacy-transformers==1.3.5',
         'tqdm==4.66.4'
     ],
```

