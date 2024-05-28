# Comparing `tmp/gbd_tools-4.8.6.tar.gz` & `tmp/gbd_tools-4.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.8.6.tar", last modified: Thu May  9 10:57:37 2024, max compression
+gzip compressed data, was "gbd_tools-4.8.7.tar", last modified: Tue May 28 19:00:25 2024, max compression
```

## Comparing `gbd_tools-4.8.6.tar` & `gbd_tools-4.8.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.8.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3589 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3123 2024-05-09 10:57:21.000000 gbd_tools-4.8.6/README.md
--rwxrwxr-x   0 root         (0) root         (0)    13399 2024-03-13 13:41:57.000000 gbd_tools-4.8.6/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.353085 gbd_tools-4.8.6/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.8.6/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11713 2024-05-09 10:57:21.000000 gbd_tools-4.8.6/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     2571 2023-10-11 12:15:20.000000 gbd_tools-4.8.6/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    12263 2024-02-26 13:09:27.000000 gbd_tools-4.8.6/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6981 2024-03-12 10:21:54.000000 gbd_tools-4.8.6/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5751 2024-03-13 14:26:05.000000 gbd_tools-4.8.6/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12527 2024-03-11 11:39:25.000000 gbd_tools-4.8.6/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-07-12 12:50:07.000000 gbd_tools-4.8.6/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3422 2024-03-12 16:33:18.000000 gbd_tools-4.8.6/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.353085 gbd_tools-4.8.6/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.8.6/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6560 2024-03-13 13:38:04.000000 gbd_tools-4.8.6/gbd_init/feature_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     2789 2023-10-11 12:15:20.000000 gbd_tools-4.8.6/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3088 2023-08-13 12:12:12.000000 gbd_tools-4.8.6/gbd_init/initializer.py
--rw-rw-r--   0 root         (0) root         (0)     4469 2024-03-13 13:38:12.000000 gbd_tools-4.8.6/gbd_init/instance_transformers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.353085 gbd_tools-4.8.6/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.8.6/gbd_server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9631 2024-03-11 17:35:42.000000 gbd_tools-4.8.6/gbd_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.353085 gbd_tools-4.8.6/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.8.6/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.8.6/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.8.6/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1855 2024-03-12 10:29:44.000000 gbd_tools-4.8.6/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.8.6/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     6788 2024-03-12 10:38:17.000000 gbd_tools-4.8.6/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3589 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 10:57:37.000000 gbd_tools-4.8.6/gbd_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 10:57:37.361085 gbd_tools-4.8.6/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      936 2024-05-09 10:57:21.000000 gbd_tools-4.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.991063 gbd_tools-4.8.7/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.8.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3589 2024-05-28 19:00:25.991063 gbd_tools-4.8.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3123 2024-05-09 10:57:21.000000 gbd_tools-4.8.7/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    13399 2024-03-13 13:41:57.000000 gbd_tools-4.8.7/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.983063 gbd_tools-4.8.7/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.8.7/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11713 2024-05-09 10:57:21.000000 gbd_tools-4.8.7/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2571 2023-10-11 12:15:20.000000 gbd_tools-4.8.7/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    12263 2024-02-26 13:09:27.000000 gbd_tools-4.8.7/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6914 2024-05-28 18:59:15.000000 gbd_tools-4.8.7/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5751 2024-03-13 14:26:05.000000 gbd_tools-4.8.7/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12527 2024-03-11 11:39:25.000000 gbd_tools-4.8.7/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-07-12 12:50:07.000000 gbd_tools-4.8.7/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-03-12 16:33:18.000000 gbd_tools-4.8.7/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.983063 gbd_tools-4.8.7/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.8.7/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6637 2024-05-28 07:59:23.000000 gbd_tools-4.8.7/gbd_init/feature_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     2789 2023-10-11 12:15:20.000000 gbd_tools-4.8.7/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3431 2024-05-28 08:06:28.000000 gbd_tools-4.8.7/gbd_init/initializer.py
+-rw-rw-r--   0 root         (0) root         (0)     4469 2024-03-13 13:38:12.000000 gbd_tools-4.8.7/gbd_init/instance_transformers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.983063 gbd_tools-4.8.7/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.8.7/gbd_server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9631 2024-03-11 17:35:42.000000 gbd_tools-4.8.7/gbd_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.983063 gbd_tools-4.8.7/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.987063 gbd_tools-4.8.7/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.8.7/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.8.7/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.8.7/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1855 2024-03-12 10:29:44.000000 gbd_tools-4.8.7/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.8.7/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.987063 gbd_tools-4.8.7/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     6788 2024-03-12 10:38:17.000000 gbd_tools-4.8.7/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:00:25.991063 gbd_tools-4.8.7/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3589 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 19:00:25.000000 gbd_tools-4.8.7/gbd_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 19:00:25.991063 gbd_tools-4.8.7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      936 2024-05-28 18:43:43.000000 gbd_tools-4.8.7/setup.py
```

### Comparing `gbd_tools-4.8.6/LICENSE` & `gbd_tools-4.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/PKG-INFO` & `gbd_tools-4.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.8.6
+Version: 4.8.7
 Summary: GBD Tools: Maintenance and Distribution of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.8.6/README.md` & `gbd_tools-4.8.7/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd.py` & `gbd_tools-4.8.7/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/api.py` & `gbd_tools-4.8.7/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/contexts.py` & `gbd_tools-4.8.7/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/database.py` & `gbd_tools-4.8.7/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/grammar.py` & `gbd_tools-4.8.7/gbd_core/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,23 @@
             | col:(dbname ":" column | column) cop:("=" | "!=" | "<=" | ">=" | "<" | ">" ) ter:termstart
             | col:(dbname ":" column | column) cop:("=" | "!=" | "<=" | ">=" | "<" | ">" ) str:string 
             | col:(dbname ":" column | column) cop:("like" | "unlike") ~ lik:(["%"] string ["%"])
             ;
 
         termstart 
             = 
-            t:term
+            ("(") t:term (")")
             ;
 
         term 
             = 
-            | left:(term | termend) top:("+" | "-" | "*" | "/") right:(term | termend)
-            | ("(") t:(term | termend) (")")
+            | left:term top:("+" | "-" | "*" | "/") right:term
+            | ("(") t:term (")")
             | constant:number
-            ;
-
-        termend
-            =
-            col:(dbname ":" column | column)
+            | col:(dbname ":" column | column)
             ;
 
         string
             =
             | "'" @:singlequotedstring "'"
             | '"' @:doublequotedstring '"'
             | /[a-zA-Z0-9_\.\-\/\,\:\+\=\@]+/
```

### Comparing `gbd_tools-4.8.6/gbd_core/query.py` & `gbd_tools-4.8.7/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/schema.py` & `gbd_tools-4.8.7/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/util.py` & `gbd_tools-4.8.7/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_core/util_argparse.py` & `gbd_tools-4.8.7/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_init/feature_extractors.py` & `gbd_tools-4.8.7/gbd_init/feature_extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 generic_extractors = {
     "base" : {
         "description" : "Extract base features from CNF files. ",
         "contexts" : [ "cnf" ],
         "features" : [ (name, "empty") for name in base_feature_names() ],
         "compute" : compute_base_features,
+        "haspool" : True,
     },
     "gate" : {
         "description" : "Extract gate features from CNF files. ",
         "contexts" : [ "cnf" ],
         "features" : [ (name, "empty") for name in gate_feature_names() ],
         "compute" : compute_gate_features,
     },
@@ -129,15 +130,15 @@
 
 
 def init_features_generic(key: str, api: GBD, rlimits, df, target_db):
     einfo = generic_extractors[key]
     context = api.database.dcontext(target_db)
     if not context in einfo["contexts"]:
         raise InitializerException("Target database context must be in {}".format(einfo["contexts"]))
-    extractor = Initializer(api, rlimits, target_db, einfo["features"], einfo["compute"])
+    extractor = Initializer(api, rlimits, target_db, einfo["features"], einfo["compute"], einfo["haspool"] if "haspool" in einfo else False)
     extractor.create_features()
     extractor.run(df)
 
 
 def init_local(api: GBD, rlimits, root, target_db):
     context = api.database.dcontext(target_db)
```

### Comparing `gbd_tools-4.8.6/gbd_init/gbdhash.py` & `gbd_tools-4.8.7/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_init/initializer.py` & `gbd_tools-4.8.7/gbd_init/initializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from gbd_core import util
 
 class InitializerException(Exception):
     pass
 
 class Initializer:
 
-    def __init__(self, api: GBD, rlimits: dict, target_db: str, features: list, initfunc):
+    def __init__(self, api: GBD, rlimits: dict, target_db: str, features: list, initfunc, haspool=False):
         self.api = api
         self.api.database.set_auto_commit(False)
         self.target_db = target_db
         self.features = features
         self.initfunc = initfunc
         self.rlimits = rlimits
 
@@ -47,18 +47,27 @@
             self.api.database.set_values(name, value, [hashv], self.target_db)
         self.api.database.commit()
 
 
     def run(self, instances: pd.DataFrame):
         if self.rlimits['jobs'] == 1:
             self.init_sequential(instances)
+        elif self.haspool:
+            self.init_parallel2(instances)
         else:
             self.init_parallel(instances)
 
 
+    def init_parallel2(self, instances: pd.DataFrame):
+        handle = self.initfunc(instances, self.rlimits) # non-blocking call
+        while not handle.done():
+            result = handle.result() # blocking call
+            self.save_features(result)
+
+
     def init_sequential(self, instances: pd.DataFrame):
         for idx, row in instances.iterrows():
             result = self.initfunc(row['hash'], row['local'], self.rlimits)
             self.save_features(result)
 
 
     def init_parallel(self, instances: pd.DataFrame):
```

### Comparing `gbd_tools-4.8.6/gbd_init/instance_transformers.py` & `gbd_tools-4.8.7/gbd_init/instance_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/server.py` & `gbd_tools-4.8.7/gbd_server/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.8.7/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.8.7/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.8.7/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/static/main.css` & `gbd_tools-4.8.7/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/static/w3.js` & `gbd_tools-4.8.7/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_server/templates/index.html` & `gbd_tools-4.8.7/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.8.7/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.8.6
+Version: 4.8.7
 Summary: GBD Tools: Maintenance and Distribution of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.8.6/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.8.7/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.8.6/setup.py` & `gbd_tools-4.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.8.6',
+  version='4.8.7',
   description='GBD Tools: Maintenance and Distribution of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser',
   author_email='markus.iser@kit.edu',
   packages=[
```

