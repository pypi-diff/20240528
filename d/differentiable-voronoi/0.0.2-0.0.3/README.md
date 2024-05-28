# Comparing `tmp/differentiable-voronoi-0.0.2.tar.gz` & `tmp/differentiable-voronoi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "differentiable-voronoi-0.0.2.tar", last modified: Tue May 28 15:50:36 2024, max compression
+gzip compressed data, was "differentiable-voronoi-0.0.3.tar", last modified: Tue May 28 16:04:12 2024, max compression
```

## Comparing `differentiable-voronoi-0.0.2.tar` & `differentiable-voronoi-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.414655 differentiable-voronoi-0.0.2/
--rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 15:50:36.414459 differentiable-voronoi-0.0.2/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)     3001 2024-05-28 14:28:32.000000 differentiable-voronoi-0.0.2/README.md
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.413353 differentiable-voronoi-0.0.2/differentiable_voronoi/
--rw-r--r--   0 sergei     (501) staff       (20)       58 2024-05-28 11:52:33.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/__init__.py
--rw-r--r--   0 sergei     (501) staff       (20)    20477 2024-05-27 19:59:42.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/differentiable_voronoi.py
--rw-r--r--   0 sergei     (501) staff       (20)     1711 2024-05-28 14:01:54.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/main.py
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.414232 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/
--rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)      362 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/SOURCES.txt
--rw-r--r--   0 sergei     (501) staff       (20)        1 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/dependency_links.txt
--rw-r--r--   0 sergei     (501) staff       (20)      433 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/requires.txt
--rw-r--r--   0 sergei     (501) staff       (20)       23 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/top_level.txt
--rw-r--r--   0 sergei     (501) staff       (20)       38 2024-05-28 15:50:36.414707 differentiable-voronoi-0.0.2/setup.cfg
--rw-r--r--   0 sergei     (501) staff       (20)     1427 2024-05-28 15:50:26.000000 differentiable-voronoi-0.0.2/setup.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 16:04:12.599676 differentiable-voronoi-0.0.3/
+-rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 16:04:12.599468 differentiable-voronoi-0.0.3/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)     3001 2024-05-28 14:28:32.000000 differentiable-voronoi-0.0.3/README.md
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 16:04:12.598450 differentiable-voronoi-0.0.3/differentiable_voronoi/
+-rw-r--r--   0 sergei     (501) staff       (20)       71 2024-05-28 16:02:59.000000 differentiable-voronoi-0.0.3/differentiable_voronoi/__init__.py
+-rw-r--r--   0 sergei     (501) staff       (20)    20477 2024-05-27 19:59:42.000000 differentiable-voronoi-0.0.3/differentiable_voronoi/differentiable_voronoi.py
+-rw-r--r--   0 sergei     (501) staff       (20)     1711 2024-05-28 14:01:54.000000 differentiable-voronoi-0.0.3/differentiable_voronoi/main.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 16:04:12.599221 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/
+-rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 16:04:12.000000 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)      362 2024-05-28 16:04:12.000000 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/SOURCES.txt
+-rw-r--r--   0 sergei     (501) staff       (20)        1 2024-05-28 16:04:12.000000 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/dependency_links.txt
+-rw-r--r--   0 sergei     (501) staff       (20)      433 2024-05-28 16:04:12.000000 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/requires.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       23 2024-05-28 16:04:12.000000 differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/top_level.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       38 2024-05-28 16:04:12.599722 differentiable-voronoi-0.0.3/setup.cfg
+-rw-r--r--   0 sergei     (501) staff       (20)     1427 2024-05-28 16:04:04.000000 differentiable-voronoi-0.0.3/setup.py
```

### Comparing `differentiable-voronoi-0.0.2/PKG-INFO` & `differentiable-voronoi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: differentiable-voronoi
-Version: 0.0.2
+Version: 0.0.3
 Summary: differentiable Voronoi tessellation
 Home-page: https://github.com/SergeiShumilin/differentiable-voronoi
 Author: Sergei Shumilin
 Author-email: ishumili@gmail.com
 Requires-Dist: contourpy==1.2.1
 Requires-Dist: cycler==0.12.1
 Requires-Dist: filelock==3.14.0
```

### Comparing `differentiable-voronoi-0.0.2/README.md` & `differentiable-voronoi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `differentiable-voronoi-0.0.2/differentiable_voronoi/differentiable_voronoi.py` & `differentiable-voronoi-0.0.3/differentiable_voronoi/differentiable_voronoi.py`

 * *Files identical despite different names*

### Comparing `differentiable-voronoi-0.0.2/differentiable_voronoi/main.py` & `differentiable-voronoi-0.0.3/differentiable_voronoi/main.py`

 * *Files identical despite different names*

### Comparing `differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/PKG-INFO` & `differentiable-voronoi-0.0.3/differentiable_voronoi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: differentiable-voronoi
-Version: 0.0.2
+Version: 0.0.3
 Summary: differentiable Voronoi tessellation
 Home-page: https://github.com/SergeiShumilin/differentiable-voronoi
 Author: Sergei Shumilin
 Author-email: ishumili@gmail.com
 Requires-Dist: contourpy==1.2.1
 Requires-Dist: cycler==0.12.1
 Requires-Dist: filelock==3.14.0
```

### Comparing `differentiable-voronoi-0.0.2/setup.py` & `differentiable-voronoi-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='differentiable-voronoi',
-    version='0.0.2',
+    version='0.0.3',
     packages=['differentiable_voronoi'],
     url='https://github.com/SergeiShumilin/differentiable-voronoi',
     license='',
     author='Sergei Shumilin',
     author_email='ishumili@gmail.com',
     description='differentiable Voronoi tessellation',
     install_requires=['contourpy==1.2.1',
```

