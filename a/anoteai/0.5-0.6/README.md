# Comparing `tmp/anoteai-0.5.tar.gz` & `tmp/anoteai-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoteai-0.5.tar", last modified: Thu Feb 29 21:25:11 2024, max compression
+gzip compressed data, was "anoteai-0.6.tar", last modified: Tue May 28 15:52:22 2024, max compression
```

## Comparing `anoteai-0.5.tar` & `anoteai-0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-02-29 21:25:11.721331 anoteai-0.5/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-02-29 21:25:11.721214 anoteai-0.5/PKG-INFO
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-02-29 21:25:11.720484 anoteai-0.5/anoteai/
--rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.5/anoteai/__init__.py
--rw-r--r--   0 natanvidra   (501) staff       (20)     3797 2024-02-29 21:23:26.000000 anoteai-0.5/anoteai/core.py
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-02-29 21:25:11.721070 anoteai-0.5/anoteai.egg-info/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-02-29 21:25:11.000000 anoteai-0.5/anoteai.egg-info/PKG-INFO
--rw-r--r--   0 natanvidra   (501) staff       (20)      198 2024-02-29 21:25:11.000000 anoteai-0.5/anoteai.egg-info/SOURCES.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-02-29 21:25:11.000000 anoteai-0.5/anoteai.egg-info/dependency_links.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        9 2024-02-29 21:25:11.000000 anoteai-0.5/anoteai.egg-info/requires.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-02-29 21:25:11.000000 anoteai-0.5/anoteai.egg-info/top_level.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-02-29 21:25:11.721369 anoteai-0.5/setup.cfg
--rw-r--r--   0 natanvidra   (501) staff       (20)      340 2024-02-29 21:23:36.000000 anoteai-0.5/setup.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.381186 anoteai-0.6/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 15:52:22.381071 anoteai-0.6/PKG-INFO
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.380156 anoteai-0.6/anoteai/
+-rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.6/anoteai/__init__.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)    15495 2024-05-28 15:51:11.000000 anoteai-0.6/anoteai/core.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)     2328 2024-05-28 15:44:20.000000 anoteai-0.6/anoteai/testing.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.380798 anoteai-0.6/anoteai.egg-info/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/PKG-INFO
+-rw-r--r--   0 natanvidra   (501) staff       (20)      217 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/SOURCES.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/dependency_links.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        9 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/requires.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/top_level.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-05-28 15:52:22.381224 anoteai-0.6/setup.cfg
+-rw-r--r--   0 natanvidra   (501) staff       (20)      340 2024-05-28 15:52:19.000000 anoteai-0.6/setup.py
```

