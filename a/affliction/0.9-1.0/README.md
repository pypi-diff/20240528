# Comparing `tmp/affliction-0.9.tar.gz` & `tmp/affliction-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affliction-0.9.tar", last modified: Fri May 24 15:07:18 2024, max compression
+gzip compressed data, was "affliction-1.0.tar", last modified: Tue May 28 04:46:57 2024, max compression
```

## Comparing `affliction-0.9.tar` & `affliction-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 15:07:18.297356 affliction-0.9/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       85 2024-05-24 04:04:14.000000 affliction-0.9/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-24 15:07:18.297356 affliction-0.9/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2377 2024-05-24 04:04:14.000000 affliction-0.9/README.md
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 15:07:18.297356 affliction-0.9/affliction/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:04:14.000000 affliction-0.9/affliction/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4984 2024-05-24 04:43:51.000000 affliction-0.9/affliction/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      902 2024-05-24 04:04:14.000000 affliction-0.9/affliction/exchange_client.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    20188 2024-05-24 14:47:52.000000 affliction-0.9/affliction/graph_client.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       37 2024-05-24 15:07:16.000000 affliction-0.9/affliction/version_info.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 15:07:18.297356 affliction-0.9/affliction.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-24 15:07:18.000000 affliction-0.9/affliction.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      333 2024-05-24 15:07:18.000000 affliction-0.9/affliction.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-05-24 15:07:18.000000 affliction-0.9/affliction.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      143 2024-05-24 15:07:18.000000 affliction-0.9/affliction.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2024-05-24 15:07:18.000000 affliction-0.9/affliction.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      105 2024-05-24 04:04:14.000000 affliction-0.9/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-05-24 15:07:18.297356 affliction-0.9/setup.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2380 2024-05-24 15:07:16.000000 affliction-0.9/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-28 04:46:57.615617 affliction-1.0/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       85 2024-05-24 04:04:14.000000 affliction-1.0/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-28 04:46:57.615617 affliction-1.0/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2377 2024-05-24 04:04:14.000000 affliction-1.0/README.md
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-28 04:46:57.615617 affliction-1.0/affliction/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:04:14.000000 affliction-1.0/affliction/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4984 2024-05-24 04:43:51.000000 affliction-1.0/affliction/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      902 2024-05-24 04:04:14.000000 affliction-1.0/affliction/exchange_client.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    20233 2024-05-28 04:45:08.000000 affliction-1.0/affliction/graph_client.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       37 2024-05-28 04:46:55.000000 affliction-1.0/affliction/version_info.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-28 04:46:57.615617 affliction-1.0/affliction.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-28 04:46:57.000000 affliction-1.0/affliction.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      333 2024-05-28 04:46:57.000000 affliction-1.0/affliction.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-05-28 04:46:57.000000 affliction-1.0/affliction.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      143 2024-05-28 04:46:57.000000 affliction-1.0/affliction.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2024-05-28 04:46:57.000000 affliction-1.0/affliction.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      105 2024-05-24 04:04:14.000000 affliction-1.0/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-05-28 04:46:57.615617 affliction-1.0/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2380 2024-05-28 04:46:55.000000 affliction-1.0/setup.py
```

### Comparing `affliction-0.9/PKG-INFO` & `affliction-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affliction
-Version: 0.9
+Version: 1.0
 Summary: affliction
 Home-page: https://bitbucket.org/dbuy/affliction
 Author: dev
 Author-email: unknown@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `affliction-0.9/README.md` & `affliction-1.0/README.md`

 * *Files identical despite different names*

### Comparing `affliction-0.9/affliction/base.py` & `affliction-1.0/affliction/base.py`

 * *Files identical despite different names*

### Comparing `affliction-0.9/affliction/exchange_client.py` & `affliction-1.0/affliction/exchange_client.py`

 * *Files identical despite different names*

### Comparing `affliction-0.9/affliction/graph_client.py` & `affliction-1.0/affliction/graph_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,14 +486,16 @@
         )
         return self.get(url)
 
     def provision_on_demand(self, subjects, app_name, rule_name=None, **kwargs):
         service_principal = self.get_service_principal(name=app_name)
         service_principal_id = service_principal['id']
         jobs = self.get_app_jobs(service_principal_id=service_principal_id)
+        if not jobs:
+            return None
         job = jobs[0]
         job_id = job['id']
         schema = self.get_app_job_schema(job_id, service_principal_id)
         rules = schema['synchronizationRules']
         rule_id = 'sesame_meow_cat'
         if rule_name:
             for rule in rules:
```

### Comparing `affliction-0.9/affliction.egg-info/PKG-INFO` & `affliction-1.0/affliction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affliction
-Version: 0.9
+Version: 1.0
 Summary: affliction
 Home-page: https://bitbucket.org/dbuy/affliction
 Author: dev
 Author-email: unknown@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `affliction-0.9/setup.py` & `affliction-1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     all_extras = list(all_extras)
     all_extras.sort()
     extras['all'] = all_extras
 
 
 setup(
     name='affliction',
-    version='0.9',
+    version='1.0',
     description='affliction',
     license='BSD',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='dev',
     author_email='unknown@yahoo.com',
     url='https://bitbucket.org/dbuy/affliction',
```

