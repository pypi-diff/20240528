# Comparing `tmp/dbSQL_connect-0.0.7.tar.gz` & `tmp/dbSQL_connect-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbSQL_connect-0.0.7.tar", last modified: Mon May 27 19:29:26 2024, max compression
+gzip compressed data, was "dbSQL_connect-0.0.8.tar", last modified: Mon May 27 21:07:35 2024, max compression
```

## Comparing `dbSQL_connect-0.0.7.tar` & `dbSQL_connect-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/
--rw-rw-rw-   0        0        0      398 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.807415 dbSQL_connect-0.0.7/dbSQL_connect/
--rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.7/dbSQL_connect/__init__.py
--rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.7/dbSQL_connect/_entry_points.py
--rw-rw-rw-   0        0        0    10277 2024-05-17 07:54:35.000000 dbSQL_connect-0.0.7/dbSQL_connect/_imp.py
--rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.7/dbSQL_connect/requires.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.812403 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/
--rw-rw-rw-   0        0        0      398 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      656 2024-05-27 19:29:24.000000 dbSQL_connect-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:07:35.499936 dbSQL_connect-0.0.8/
+-rw-rw-rw-   0        0        0      398 2024-05-27 21:07:35.499936 dbSQL_connect-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 21:07:35.494948 dbSQL_connect-0.0.8/dbSQL_connect/
+-rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.8/dbSQL_connect/__init__.py
+-rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.8/dbSQL_connect/_entry_points.py
+-rw-rw-rw-   0        0        0    10277 2024-05-17 07:54:35.000000 dbSQL_connect-0.0.8/dbSQL_connect/_imp.py
+-rw-rw-rw-   0        0        0    47478 2024-05-27 21:06:48.000000 dbSQL_connect-0.0.8/dbSQL_connect/importlib_metadata.py
+-rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.8/dbSQL_connect/requires.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:07:35.498939 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-05-27 21:07:35.000000 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-05-27 21:07:35.000000 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 21:07:35.000000 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 21:07:35.000000 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 21:07:35.000000 dbSQL_connect-0.0.8/dbSQL_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 21:07:35.500934 dbSQL_connect-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      656 2024-05-27 21:07:29.000000 dbSQL_connect-0.0.8/setup.py
```

### Comparing `dbSQL_connect-0.0.7/dbSQL_connect/_entry_points.py` & `dbSQL_connect-0.0.8/dbSQL_connect/_entry_points.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.7/dbSQL_connect/_imp.py` & `dbSQL_connect-0.0.8/dbSQL_connect/_imp.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.7/dbSQL_connect/requires.py` & `dbSQL_connect-0.0.8/dbSQL_connect/requires.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.7/setup.py` & `dbSQL_connect-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='dbSQL_connect',
-  version='0.0.7',
+  version='0.0.8',
   author='virginxlub',
   author_email='vzlomka927@yandex.ru',
   description='This is the simplest module for quick work with files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
```

