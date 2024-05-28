# Comparing `tmp/tf_idf_cosimm-0.0.1.tar.gz` & `tmp/tf_idf_cosimm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_idf_cosimm-0.0.1.tar", last modified: Thu May 23 20:20:07 2024, max compression
+gzip compressed data, was "tf_idf_cosimm-0.0.2.tar", last modified: Tue May 28 18:03:16 2024, max compression
```

## Comparing `tf_idf_cosimm-0.0.1.tar` & `tf_idf_cosimm-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-23 20:20:07.144382 tf_idf_cosimm-0.0.1/
--rw-r--r--   0 ryan      (1000) ryan      (1000)    11337 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.1/LICENSE
--rw-r--r--   0 ryan      (1000) ryan      (1000)      111 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.1/MANIFEST.in
--rw-r--r--   0 ryan      (1000) ryan      (1000)    11629 2024-05-23 20:20:07.144382 tf_idf_cosimm-0.0.1/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)    10697 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.1/README.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1062 2024-05-23 20:19:41.000000 tf_idf_cosimm-0.0.1/settings.ini
--rw-r--r--   0 ryan      (1000) ryan      (1000)       38 2024-05-23 20:20:07.144382 tf_idf_cosimm-0.0.1/setup.cfg
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2596 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.1/setup.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-23 20:20:07.141049 tf_idf_cosimm-0.0.1/tf_idf/
--rw-r--r--   0 ryan      (1000) ryan      (1000)       22 2024-05-23 20:20:01.000000 tf_idf_cosimm-0.0.1/tf_idf/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)      613 2024-05-23 20:20:01.000000 tf_idf_cosimm-0.0.1/tf_idf/_modidx.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3344 2024-05-23 20:20:01.000000 tf_idf_cosimm-0.0.1/tf_idf/core.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-23 20:20:07.144382 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)    11629 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)      363 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/SOURCES.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/dependency_links.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       34 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/entry_points.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/not-zip-safe
--rw-r--r--   0 ryan      (1000) ryan      (1000)       38 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/requires.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)        7 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/top_level.txt
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-28 18:03:16.007412 tf_idf_cosimm-0.0.2/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    11337 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.2/LICENSE
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      111 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.2/MANIFEST.in
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    11629 2024-05-28 18:03:16.007412 tf_idf_cosimm-0.0.2/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    10697 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.2/README.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      920 2024-05-28 18:01:51.000000 tf_idf_cosimm-0.0.2/settings.ini
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       38 2024-05-28 18:03:16.007412 tf_idf_cosimm-0.0.2/setup.cfg
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     2596 2024-05-22 15:10:42.000000 tf_idf_cosimm-0.0.2/setup.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-28 18:03:16.007412 tf_idf_cosimm-0.0.2/tf_idf/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       22 2024-05-28 18:01:51.000000 tf_idf_cosimm-0.0.2/tf_idf/__init__.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      613 2024-05-28 18:01:51.000000 tf_idf_cosimm-0.0.2/tf_idf/_modidx.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3448 2024-05-28 18:01:51.000000 tf_idf_cosimm-0.0.2/tf_idf/core.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2024-05-28 18:03:16.007412 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    11629 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      363 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       34 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/entry_points.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2024-05-23 20:20:07.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/not-zip-safe
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       38 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/requires.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        7 2024-05-28 18:03:15.000000 tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/top_level.txt
```

### Comparing `tf_idf_cosimm-0.0.1/LICENSE` & `tf_idf_cosimm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tf_idf_cosimm-0.0.1/PKG-INFO` & `tf_idf_cosimm-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf_idf_cosimm
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a short set of functions meant to help analyze cosine similarity between texts
 Home-page: https://github.com/cooperrc/tf_idf_cosimm
 Author: Ryan C. Cooper
 Author-email: ryan.c.cooper@uconn.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tf_idf_cosimm Version: 0.0.1 Summary: This is a
+Metadata-Version: 2.1 Name: tf_idf_cosimm Version: 0.0.2 Summary: This is a
 short set of functions meant to help analyze cosine similarity between texts
 Home-page: https://github.com/cooperrc/tf_idf_cosimm Author: Ryan C. Cooper
 Author-email: ryan.c.cooper@uconn.edu License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `tf_idf_cosimm-0.0.1/README.md` & `tf_idf_cosimm-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tf_idf_cosimm-0.0.1/settings.ini` & `tf_idf_cosimm-0.0.2/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = tf_idf_cosimm
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = tf_idf_cosimm
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
-
-### nbdev ###
 doc_path = _docs
 lib_path = tf_idf
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://cooperrc.github.io
+doc_baseurl = /tf_idf_cosimm
+git_url = https://github.com/cooperrc/tf_idf_cosimm
+title = tf_idf_cosimm
 audience = Developers
 author = Ryan C. Cooper
 author_email = ryan.c.cooper@uconn.edu
-copyright = 2024 onwards, %(author)s
+copyright = 2024 onwards, Ryan C. Cooper
 description = This is a short set of functions meant to help analyze cosine similarity between texts
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = cooperrc
-
-### Optional ###
 requirements = numpy pandas nltk scikit-learn
-# dev_requirements = 
-# console_scripts =
-# conda_user = 
-# package_data =
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = False
+clean_ids = True
+clear_all = False
+
```

### Comparing `tf_idf_cosimm-0.0.1/setup.py` & `tf_idf_cosimm-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tf_idf_cosimm-0.0.1/tf_idf/_modidx.py` & `tf_idf_cosimm-0.0.2/tf_idf/_modidx.py`

 * *Files identical despite different names*

### Comparing `tf_idf_cosimm-0.0.1/tf_idf/core.py` & `tf_idf_cosimm-0.0.2/tf_idf/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,15 +64,19 @@
     
     # Count TF-IDF
     from sklearn.feature_extraction.text import TfidfVectorizer
     vectorizer = TfidfVectorizer()
     tfidf_matrix = vectorizer.fit_transform(stemming)
     
     # Get words from stopwords array to use as headers
-    feature_names = vectorizer.get_feature_names_out()
+    try:
+        feature_names = vectorizer.get_feature_names_out()
+    except AttributeError:
+        feature_names = vectorizer.get_feature_names()
+        
 
     # Combine header titles and weights
     df_tfidf = pd.DataFrame(tfidf_matrix.toarray(), columns=feature_names)
     df_tfidf = pd.concat([df, df_tfidf], axis=1)
 
     return df_tfidf
```

### Comparing `tf_idf_cosimm-0.0.1/tf_idf_cosimm.egg-info/PKG-INFO` & `tf_idf_cosimm-0.0.2/tf_idf_cosimm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf_idf_cosimm
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a short set of functions meant to help analyze cosine similarity between texts
 Home-page: https://github.com/cooperrc/tf_idf_cosimm
 Author: Ryan C. Cooper
 Author-email: ryan.c.cooper@uconn.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tf_idf_cosimm Version: 0.0.1 Summary: This is a
+Metadata-Version: 2.1 Name: tf_idf_cosimm Version: 0.0.2 Summary: This is a
 short set of functions meant to help analyze cosine similarity between texts
 Home-page: https://github.com/cooperrc/tf_idf_cosimm Author: Ryan C. Cooper
 Author-email: ryan.c.cooper@uconn.edu License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

