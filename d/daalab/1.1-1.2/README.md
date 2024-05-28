# Comparing `tmp/daalab-1.1.tar.gz` & `tmp/daalab-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-1.1.tar", last modified: Mon May 27 03:37:12 2024, max compression
+gzip compressed data, was "daalab-1.2.tar", last modified: Mon May 27 03:46:57 2024, max compression
```

## Comparing `daalab-1.1.tar` & `daalab-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.597422 daalab-1.1/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:37:12.597292 daalab-1.1/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-1.1/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.596366 daalab-1.1/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    31731 2024-05-27 03:01:50.000000 daalab-1.1/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    40506 2024-05-27 03:13:22.000000 daalab-1.1/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1363 2024-05-24 02:29:40.000000 daalab-1.1/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.597116 daalab-1.1/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-27 03:37:12.597469 daalab-1.1/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-27 02:33:32.000000 daalab-1.1/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:46:57.687966 daalab-1.2/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:46:57.687841 daalab-1.2/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-1.2/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:46:57.687033 daalab-1.2/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1119 2024-05-27 03:46:48.000000 daalab-1.2/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    40506 2024-05-27 03:13:22.000000 daalab-1.2/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1363 2024-05-24 02:29:40.000000 daalab-1.2/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:46:57.687681 daalab-1.2/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:46:57.000000 daalab-1.2/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-27 03:46:57.000000 daalab-1.2/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-27 03:46:57.000000 daalab-1.2/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-27 03:46:57.000000 daalab-1.2/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-27 03:46:57.688013 daalab-1.2/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-27 03:46:53.000000 daalab-1.2/setup.py
```

### Comparing `daalab-1.1/README.md` & `daalab-1.2/README.md`

 * *Files identical despite different names*

### Comparing `daalab-1.1/daalab/codes.py` & `daalab-1.2/daalab/codes.py`

 * *Files identical despite different names*

### Comparing `daalab-1.1/daalab/testing.py` & `daalab-1.2/daalab/testing.py`

 * *Files identical despite different names*

