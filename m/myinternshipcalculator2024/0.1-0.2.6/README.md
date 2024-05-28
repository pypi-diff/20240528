# Comparing `tmp/myinternshipcalculator2024-0.1.tar.gz` & `tmp/myinternshipcalculator2024-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myinternshipcalculator2024-0.1.tar", last modified: Tue May 28 07:34:42 2024, max compression
+gzip compressed data, was "myinternshipcalculator2024-0.2.6.tar", last modified: Tue May 28 11:02:52 2024, max compression
```

## Comparing `myinternshipcalculator2024-0.1.tar` & `myinternshipcalculator2024-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 07:34:42.708194 myinternshipcalculator2024-0.1/
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 07:32:15.000000 myinternshipcalculator2024-0.1/LICENSE
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      622 2024-05-28 07:34:42.707995 myinternshipcalculator2024-0.1/PKG-INFO
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      137 2024-05-28 07:33:39.000000 myinternshipcalculator2024-0.1/README.md
-drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 07:34:42.707142 myinternshipcalculator2024-0.1/myinternshipcalculator2024/
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       72 2024-05-28 07:32:36.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024/__init__.py
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      523 2024-05-28 07:32:36.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024/calculator.py
-drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 07:34:42.707821 myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      622 2024-05-28 07:34:42.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/PKG-INFO
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      306 2024-05-28 07:34:42.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/SOURCES.txt
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)        1 2024-05-28 07:34:42.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/dependency_links.txt
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       27 2024-05-28 07:34:42.000000 myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/top_level.txt
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       38 2024-05-28 07:34:42.708232 myinternshipcalculator2024-0.1/setup.cfg
--rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      669 2024-05-28 07:33:24.000000 myinternshipcalculator2024-0.1/setup.py
+drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 11:02:52.798192 myinternshipcalculator2024-0.2.6/
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)     1065 2024-05-28 07:51:12.000000 myinternshipcalculator2024-0.2.6/LICENSE
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      624 2024-05-28 11:02:52.797998 myinternshipcalculator2024-0.2.6/PKG-INFO
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      137 2024-05-28 07:33:39.000000 myinternshipcalculator2024-0.2.6/README.md
+drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 11:02:52.796573 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024/
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       72 2024-05-28 07:32:36.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024/__init__.py
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      523 2024-05-28 07:32:36.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024/calculator.py
+drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 11:02:52.797785 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      624 2024-05-28 11:02:52.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/PKG-INFO
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      361 2024-05-28 11:02:52.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/SOURCES.txt
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)        1 2024-05-28 11:02:52.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/dependency_links.txt
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       33 2024-05-28 11:02:52.000000 myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/top_level.txt
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)       38 2024-05-28 11:02:52.798241 myinternshipcalculator2024-0.2.6/setup.cfg
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      671 2024-05-28 10:33:08.000000 myinternshipcalculator2024-0.2.6/setup.py
+drwxr-xr-x   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 11:02:52.797401 myinternshipcalculator2024-0.2.6/tests/
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)        0 2024-05-28 08:00:20.000000 myinternshipcalculator2024-0.2.6/tests/__init__.py
+-rw-r--r--   0 abdallahabdelsameia   (501) staff       (20)      441 2024-05-28 08:05:05.000000 myinternshipcalculator2024-0.2.6/tests/test_calculate_weekly_hours.py
```

### Comparing `myinternshipcalculator2024-0.1/PKG-INFO` & `myinternshipcalculator2024-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myinternshipcalculator2024
-Version: 0.1
+Version: 0.2.6
 Summary: A simple internship hours calculator.
 Home-page: https://github.com/aabdelsameia1/myinternshipcalculator2024
 Author: Abdallah Abdelsameia
 Author-email: aabdelsameia1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `myinternshipcalculator2024-0.1/myinternshipcalculator2024/calculator.py` & `myinternshipcalculator2024-0.2.6/myinternshipcalculator2024/calculator.py`

 * *Files identical despite different names*

### Comparing `myinternshipcalculator2024-0.1/myinternshipcalculator2024.egg-info/PKG-INFO` & `myinternshipcalculator2024-0.2.6/myinternshipcalculator2024.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myinternshipcalculator2024
-Version: 0.1
+Version: 0.2.6
 Summary: A simple internship hours calculator.
 Home-page: https://github.com/aabdelsameia1/myinternshipcalculator2024
 Author: Abdallah Abdelsameia
 Author-email: aabdelsameia1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `myinternshipcalculator2024-0.1/setup.py` & `myinternshipcalculator2024-0.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myinternshipcalculator2024',
-    version='0.1',
+    version='0.2.6',
     packages=find_packages(),
     install_requires=[],
     author='Abdallah Abdelsameia',
     author_email='aabdelsameia1@gmail.com',
     description='A simple internship hours calculator.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

