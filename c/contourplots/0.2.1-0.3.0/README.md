# Comparing `tmp/contourplots-0.2.1.tar.gz` & `tmp/contourplots-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contourplots-0.2.1.tar", last modified: Wed Apr 12 02:18:52 2023, max compression
+gzip compressed data, was "contourplots-0.3.0.tar", last modified: Tue May 28 01:41:09 2024, max compression
```

## Comparing `contourplots-0.2.1.tar` & `contourplots-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.910452 contourplots-0.2.1/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      608 2023-04-12 02:18:52.909453 contourplots-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.900478 contourplots-0.2.1/contourplots/
--rw-rw-rw-   0        0        0      732 2023-04-12 02:18:07.000000 contourplots-0.2.1/contourplots/__init__.py
--rw-rw-rw-   0        0        0    25746 2023-04-12 02:17:52.000000 contourplots-0.2.1/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.908457 contourplots-0.2.1/contourplots.egg-info/
--rw-rw-rw-   0        0        0      608 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 02:18:52.910452 contourplots-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-12 02:18:15.000000 contourplots-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.729453 contourplots-0.3.0/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      704 2024-05-28 01:41:09.727484 contourplots-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.717850 contourplots-0.3.0/contourplots/
+-rw-rw-rw-   0        0        0      892 2024-05-28 01:35:27.000000 contourplots-0.3.0/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    64395 2024-05-15 05:16:55.000000 contourplots-0.3.0/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.726473 contourplots-0.3.0/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 01:41:09.730449 contourplots-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-28 01:35:18.000000 contourplots-0.3.0/setup.py
```

### Comparing `contourplots-0.2.1/LICENSE.txt` & `contourplots-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.2.1/setup.py` & `contourplots-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.2.1',    
+    version='0.3.0',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

