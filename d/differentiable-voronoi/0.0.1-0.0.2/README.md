# Comparing `tmp/differentiable-voronoi-0.0.1.tar.gz` & `tmp/differentiable-voronoi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "differentiable-voronoi-0.0.1.tar", last modified: Tue May 28 15:22:21 2024, max compression
+gzip compressed data, was "differentiable-voronoi-0.0.2.tar", last modified: Tue May 28 15:50:36 2024, max compression
```

## Comparing `differentiable-voronoi-0.0.1.tar` & `differentiable-voronoi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:22:21.652502 differentiable-voronoi-0.0.1/
--rw-r--r--   0 sergei     (501) staff       (20)      236 2024-05-28 15:22:21.651833 differentiable-voronoi-0.0.1/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)     3001 2024-05-28 14:28:32.000000 differentiable-voronoi-0.0.1/README.md
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:22:21.649706 differentiable-voronoi-0.0.1/differentiable_voronoi/
--rw-r--r--   0 sergei     (501) staff       (20)       58 2024-05-28 11:52:33.000000 differentiable-voronoi-0.0.1/differentiable_voronoi/__init__.py
--rw-r--r--   0 sergei     (501) staff       (20)    20477 2024-05-27 19:59:42.000000 differentiable-voronoi-0.0.1/differentiable_voronoi/differentiable_voronoi.py
--rw-r--r--   0 sergei     (501) staff       (20)     1711 2024-05-28 14:01:54.000000 differentiable-voronoi-0.0.1/differentiable_voronoi/main.py
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:22:21.651374 differentiable-voronoi-0.0.1/differentiable_voronoi.egg-info/
--rw-r--r--   0 sergei     (501) staff       (20)      236 2024-05-28 15:22:21.000000 differentiable-voronoi-0.0.1/differentiable_voronoi.egg-info/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)      317 2024-05-28 15:22:21.000000 differentiable-voronoi-0.0.1/differentiable_voronoi.egg-info/SOURCES.txt
--rw-r--r--   0 sergei     (501) staff       (20)        1 2024-05-28 15:22:21.000000 differentiable-voronoi-0.0.1/differentiable_voronoi.egg-info/dependency_links.txt
--rw-r--r--   0 sergei     (501) staff       (20)       23 2024-05-28 15:22:21.000000 differentiable-voronoi-0.0.1/differentiable_voronoi.egg-info/top_level.txt
--rw-r--r--   0 sergei     (501) staff       (20)       38 2024-05-28 15:22:21.652768 differentiable-voronoi-0.0.1/setup.cfg
--rw-r--r--   0 sergei     (501) staff       (20)      343 2024-05-28 15:16:22.000000 differentiable-voronoi-0.0.1/setup.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.414655 differentiable-voronoi-0.0.2/
+-rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 15:50:36.414459 differentiable-voronoi-0.0.2/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)     3001 2024-05-28 14:28:32.000000 differentiable-voronoi-0.0.2/README.md
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.413353 differentiable-voronoi-0.0.2/differentiable_voronoi/
+-rw-r--r--   0 sergei     (501) staff       (20)       58 2024-05-28 11:52:33.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/__init__.py
+-rw-r--r--   0 sergei     (501) staff       (20)    20477 2024-05-27 19:59:42.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/differentiable_voronoi.py
+-rw-r--r--   0 sergei     (501) staff       (20)     1711 2024-05-28 14:01:54.000000 differentiable-voronoi-0.0.2/differentiable_voronoi/main.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2024-05-28 15:50:36.414232 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/
+-rw-r--r--   0 sergei     (501) staff       (20)     1059 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)      362 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/SOURCES.txt
+-rw-r--r--   0 sergei     (501) staff       (20)        1 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/dependency_links.txt
+-rw-r--r--   0 sergei     (501) staff       (20)      433 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/requires.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       23 2024-05-28 15:50:36.000000 differentiable-voronoi-0.0.2/differentiable_voronoi.egg-info/top_level.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       38 2024-05-28 15:50:36.414707 differentiable-voronoi-0.0.2/setup.cfg
+-rw-r--r--   0 sergei     (501) staff       (20)     1427 2024-05-28 15:50:26.000000 differentiable-voronoi-0.0.2/setup.py
```

### Comparing `differentiable-voronoi-0.0.1/README.md` & `differentiable-voronoi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `differentiable-voronoi-0.0.1/differentiable_voronoi/differentiable_voronoi.py` & `differentiable-voronoi-0.0.2/differentiable_voronoi/differentiable_voronoi.py`

 * *Files identical despite different names*

### Comparing `differentiable-voronoi-0.0.1/differentiable_voronoi/main.py` & `differentiable-voronoi-0.0.2/differentiable_voronoi/main.py`

 * *Files identical despite different names*

