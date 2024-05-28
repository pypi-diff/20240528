# Comparing `tmp/medium_article_py-0.1.7.tar.gz` & `tmp/medium_article_py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_article_py-0.1.7.tar", last modified: Tue May 28 12:05:31 2024, max compression
+gzip compressed data, was "medium_article_py-0.1.8.tar", last modified: Tue May 28 12:30:44 2024, max compression
```

## Comparing `medium_article_py-0.1.7.tar` & `medium_article_py-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:05:31.456769 medium_article_py-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 12:05:14.000000 medium_article_py-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:05:31.456769 medium_article_py-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-28 12:05:14.000000 medium_article_py-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:05:31.456769 medium_article_py-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 12:05:14.000000 medium_article_py-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:05:31.452769 medium_article_py-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:05:31.456769 medium_article_py-0.1.7/src/medium_article_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:05:31.000000 medium_article_py-0.1.7/src/medium_article_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 12:05:31.000000 medium_article_py-0.1.7/src/medium_article_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:05:31.000000 medium_article_py-0.1.7/src/medium_article_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:05:31.000000 medium_article_py-0.1.7/src/medium_article_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:05:31.000000 medium_article_py-0.1.7/src/medium_article_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:05:31.456769 medium_article_py-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 12:05:14.000000 medium_article_py-0.1.7/test/test_medium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/medium_article_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/src/medium_article_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/src/medium_article_py/medium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/medium_article_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/top_level.txt
```

### Comparing `medium_article_py-0.1.7/LICENSE` & `medium_article_py-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.7/PKG-INFO` & `medium_article_py-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medium_article_py-0.1.7/README.rst` & `medium_article_py-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.7/setup.py` & `medium_article_py-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='medium-article-py',
-    version='v0.1.7',
+    version='v0.1.8',
     description='A simple python library for Medium Articles APIs',
     long_description=long_description,
     author='Muhammad Usman',
     author_email='umuhammad202@yahoo.com',
     packages=setuptools.find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `medium_article_py-0.1.7/src/medium_article_py.egg-info/PKG-INFO` & `medium_article_py-0.1.8/src/medium_article_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

