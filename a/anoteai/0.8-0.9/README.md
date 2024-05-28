# Comparing `tmp/anoteai-0.8.tar.gz` & `tmp/anoteai-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoteai-0.8.tar", last modified: Tue May 28 16:42:12 2024, max compression
+gzip compressed data, was "anoteai-0.9.tar", last modified: Tue May 28 16:51:20 2024, max compression
```

## Comparing `anoteai-0.8.tar` & `anoteai-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:42:12.948068 anoteai-0.8/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:42:12.947911 anoteai-0.8/PKG-INFO
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:42:12.947003 anoteai-0.8/anoteai/
--rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.8/anoteai/__init__.py
--rw-r--r--   0 natanvidra   (501) staff       (20)    34331 2024-05-28 16:41:51.000000 anoteai-0.8/anoteai/core.py
--rw-r--r--   0 natanvidra   (501) staff       (20)      610 2024-05-28 16:27:12.000000 anoteai-0.8/anoteai/pop_quiz.py
--rw-r--r--   0 natanvidra   (501) staff       (20)     2384 2024-05-28 16:32:52.000000 anoteai-0.8/anoteai/testing.py
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:42:12.947726 anoteai-0.8/anoteai.egg-info/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:42:12.000000 anoteai-0.8/anoteai.egg-info/PKG-INFO
--rw-r--r--   0 natanvidra   (501) staff       (20)      237 2024-05-28 16:42:12.000000 anoteai-0.8/anoteai.egg-info/SOURCES.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-05-28 16:42:12.000000 anoteai-0.8/anoteai.egg-info/dependency_links.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        9 2024-05-28 16:42:12.000000 anoteai-0.8/anoteai.egg-info/requires.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-05-28 16:42:12.000000 anoteai-0.8/anoteai.egg-info/top_level.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-05-28 16:42:12.948117 anoteai-0.8/setup.cfg
--rw-r--r--   0 natanvidra   (501) staff       (20)      340 2024-05-28 16:42:08.000000 anoteai-0.8/setup.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:51:20.830263 anoteai-0.9/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:51:20.830148 anoteai-0.9/PKG-INFO
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:51:20.829398 anoteai-0.9/anoteai/
+-rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.9/anoteai/__init__.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)    34331 2024-05-28 16:41:51.000000 anoteai-0.9/anoteai/core.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)      610 2024-05-28 16:27:12.000000 anoteai-0.9/anoteai/pop_quiz.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)     2384 2024-05-28 16:32:52.000000 anoteai-0.9/anoteai/testing.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:51:20.830007 anoteai-0.9/anoteai.egg-info/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:51:20.000000 anoteai-0.9/anoteai.egg-info/PKG-INFO
+-rw-r--r--   0 natanvidra   (501) staff       (20)      237 2024-05-28 16:51:20.000000 anoteai-0.9/anoteai.egg-info/SOURCES.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-05-28 16:51:20.000000 anoteai-0.9/anoteai.egg-info/dependency_links.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)      758 2024-05-28 16:51:20.000000 anoteai-0.9/anoteai.egg-info/requires.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-05-28 16:51:20.000000 anoteai-0.9/anoteai.egg-info/top_level.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-05-28 16:51:20.830302 anoteai-0.9/setup.cfg
+-rw-r--r--   0 natanvidra   (501) staff       (20)      544 2024-05-28 16:50:15.000000 anoteai-0.9/setup.py
```

### Comparing `anoteai-0.8/anoteai/core.py` & `anoteai-0.9/anoteai/core.py`

 * *Files identical despite different names*

### Comparing `anoteai-0.8/anoteai/pop_quiz.py` & `anoteai-0.9/anoteai/pop_quiz.py`

 * *Files identical despite different names*

### Comparing `anoteai-0.8/anoteai/testing.py` & `anoteai-0.9/anoteai/testing.py`

 * *Files identical despite different names*

