# Comparing `tmp/sc2spa-1.2.4.tar.gz` & `tmp/sc2spa-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc2spa-1.2.4.tar", last modified: Tue May 28 00:48:18 2024, max compression
+gzip compressed data, was "sc2spa-1.2.5.tar", last modified: Tue May 28 01:19:33 2024, max compression
```

## Comparing `sc2spa-1.2.4.tar` & `sc2spa-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1525 2024-05-28 00:26:30.000000 sc2spa-1.2.4/LICENSE
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 00:48:18.503921 sc2spa-1.2.4/PKG-INFO
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1229 2024-05-28 00:26:30.000000 sc2spa-1.2.4/README.md
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/SC2Spa/
--rw-r--r--   0 linbu     (1000) linbu     (1000)      211 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/__init__.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)      460 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/__metadata__.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    20205 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/bm.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     8248 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/me.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    23478 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/pl.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3062 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/pp.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     4381 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/sva.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    51301 2024-05-28 00:46:44.000000 sc2spa-1.2.4/SC2Spa/tl.py
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/SC2Spa.egg-info/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/PKG-INFO
--rw-r--r--   0 linbu     (1000) linbu     (1000)      317 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/SOURCES.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)        1 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/dependency_links.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)        7 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/top_level.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)      691 2024-05-28 00:37:12.000000 sc2spa-1.2.4/pyproject.toml
--rw-r--r--   0 linbu     (1000) linbu     (1000)       38 2024-05-28 00:48:18.503921 sc2spa-1.2.4/setup.cfg
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/tests/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3122 2024-05-28 00:26:31.000000 sc2spa-1.2.4/tests/test_loading.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3545 2024-05-28 00:26:31.000000 sc2spa-1.2.4/tests/test_mapping.py
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 01:19:33.203922 sc2spa-1.2.5/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1525 2024-05-28 00:26:30.000000 sc2spa-1.2.5/LICENSE
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 01:19:33.203922 sc2spa-1.2.5/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1229 2024-05-28 00:26:30.000000 sc2spa-1.2.5/README.md
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 01:19:33.203922 sc2spa-1.2.5/SC2Spa/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      211 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/__init__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      461 2024-05-28 01:18:22.000000 sc2spa-1.2.5/SC2Spa/__metadata__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    20205 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/bm.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     8248 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/me.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    23478 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/pl.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3062 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/pp.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     4381 2024-05-28 00:26:30.000000 sc2spa-1.2.5/SC2Spa/sva.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    51301 2024-05-28 00:46:44.000000 sc2spa-1.2.5/SC2Spa/tl.py
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 01:19:33.203922 sc2spa-1.2.5/SC2Spa.egg-info/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 01:19:33.000000 sc2spa-1.2.5/SC2Spa.egg-info/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      317 2024-05-28 01:19:33.000000 sc2spa-1.2.5/SC2Spa.egg-info/SOURCES.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        1 2024-05-28 01:19:33.000000 sc2spa-1.2.5/SC2Spa.egg-info/dependency_links.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        7 2024-05-28 01:19:33.000000 sc2spa-1.2.5/SC2Spa.egg-info/top_level.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      691 2024-05-28 01:18:52.000000 sc2spa-1.2.5/pyproject.toml
+-rw-r--r--   0 linbu     (1000) linbu     (1000)       38 2024-05-28 01:19:33.203922 sc2spa-1.2.5/setup.cfg
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 01:19:33.203922 sc2spa-1.2.5/tests/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3122 2024-05-28 00:26:31.000000 sc2spa-1.2.5/tests/test_loading.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3545 2024-05-28 00:26:31.000000 sc2spa-1.2.5/tests/test_mapping.py
```

### Comparing `sc2spa-1.2.4/LICENSE` & `sc2spa-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/PKG-INFO` & `sc2spa-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.4
+Version: 1.2.5
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `sc2spa-1.2.4/README.md` & `sc2spa-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/bm.py` & `sc2spa-1.2.5/SC2Spa/bm.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/me.py` & `sc2spa-1.2.5/SC2Spa/me.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/pl.py` & `sc2spa-1.2.5/SC2Spa/pl.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/pp.py` & `sc2spa-1.2.5/SC2Spa/pp.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/sva.py` & `sc2spa-1.2.5/SC2Spa/sva.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa/tl.py` & `sc2spa-1.2.5/SC2Spa/tl.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/SC2Spa.egg-info/PKG-INFO` & `sc2spa-1.2.5/SC2Spa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.4
+Version: 1.2.5
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `sc2spa-1.2.4/pyproject.toml` & `sc2spa-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sc2spa-1.2.4/tests/test_loading.py` & `sc2spa-1.2.5/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.4/tests/test_mapping.py` & `sc2spa-1.2.5/tests/test_mapping.py`

 * *Files identical despite different names*

