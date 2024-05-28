# Comparing `tmp/chess_transformer-0.1.7.tar.gz` & `tmp/chess_transformer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.7.tar", last modified: Tue May 28 08:45:00 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.8.tar", last modified: Tue May 28 08:55:09 2024, max compression
```

## Comparing `chess_transformer-0.1.7.tar` & `chess_transformer-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      307 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-05-27 14:59:07.000000 chess_transformer-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-05-28 08:44:50.000000 chess_transformer-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.022151 chess_transformer-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      125 2024-05-27 15:03:14.000000 chess_transformer-0.1.7/src/chess_transformer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      302 2024-05-27 18:53:00.000000 chess_transformer-0.1.7/src/chess_transformer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      341 2024-05-27 18:29:49.000000 chess_transformer-0.1.7/src/chess_transformer/_vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer/pytorch/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-27 15:05:21.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-27 19:07:13.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      250 2024-05-27 15:07:20.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/_loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1326 2024-05-27 19:13:32.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/data.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1166 2024-05-28 08:39:47.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/decode.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1375 2024-05-27 19:34:27.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/model.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      909 2024-05-27 19:32:53.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/pos_enc.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1484 2024-05-27 18:58:37.000000 chess_transformer-0.1.7/src/chess_transformer/samples.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      307 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-05-27 14:59:07.000000 chess_transformer-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-28 08:55:06.000000 chess_transformer-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.302162 chess_transformer-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.302162 chess_transformer-0.1.8/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      125 2024-05-27 15:03:14.000000 chess_transformer-0.1.8/src/chess_transformer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      302 2024-05-27 18:53:00.000000 chess_transformer-0.1.8/src/chess_transformer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      342 2024-05-28 08:55:02.000000 chess_transformer-0.1.8/src/chess_transformer/_vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/src/chess_transformer/pytorch/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-27 15:05:21.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-27 19:07:13.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      250 2024-05-27 15:07:20.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/_loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1326 2024-05-27 19:13:32.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/data.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1166 2024-05-28 08:39:47.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/decode.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1375 2024-05-27 19:34:27.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/model.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      909 2024-05-27 19:32:53.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/pos_enc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1484 2024-05-27 18:58:37.000000 chess_transformer-0.1.8/src/chess_transformer/samples.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      664 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.7/pyproject.toml` & `chess_transformer-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
-  
+  "chess", "jaxtyping", "haskellian", "chess-notation", "chess-utils"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `chess_transformer-0.1.7/src/chess_transformer/pytorch/data.py` & `chess_transformer-0.1.8/src/chess_transformer/pytorch/data.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.7/src/chess_transformer/pytorch/decode.py` & `chess_transformer-0.1.8/src/chess_transformer/pytorch/decode.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.7/src/chess_transformer/pytorch/model.py` & `chess_transformer-0.1.8/src/chess_transformer/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.7/src/chess_transformer/pytorch/pos_enc.py` & `chess_transformer-0.1.8/src/chess_transformer/pytorch/pos_enc.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.7/src/chess_transformer/samples.py` & `chess_transformer-0.1.8/src/chess_transformer/samples.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.7/src/chess_transformer.egg-info/SOURCES.txt` & `chess_transformer-0.1.8/src/chess_transformer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/chess_transformer/__init__.py
 src/chess_transformer/__init__.pyi
 src/chess_transformer/_vocab.py
 src/chess_transformer/samples.py
 src/chess_transformer.egg-info/PKG-INFO
 src/chess_transformer.egg-info/SOURCES.txt
 src/chess_transformer.egg-info/dependency_links.txt
+src/chess_transformer.egg-info/requires.txt
 src/chess_transformer.egg-info/top_level.txt
 src/chess_transformer/pytorch/__init__.py
 src/chess_transformer/pytorch/__init__.pyi
 src/chess_transformer/pytorch/_loss.py
 src/chess_transformer/pytorch/data.py
 src/chess_transformer/pytorch/decode.py
 src/chess_transformer/pytorch/model.py
```

