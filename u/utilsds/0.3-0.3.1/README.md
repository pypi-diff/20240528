# Comparing `tmp/utilsds-0.3.tar.gz` & `tmp/utilsds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsds-0.3.tar", last modified: Tue May 28 10:24:13 2024, max compression
+gzip compressed data, was "utilsds-0.3.1.tar", last modified: Tue May 28 11:40:57 2024, max compression
```

## Comparing `utilsds-0.3.tar` & `utilsds-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 10:24:13.978445 utilsds-0.3/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     5828 2024-05-28 10:24:13.976601 utilsds-0.3/PKG-INFO
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)       67 2024-05-28 09:39:30.000000 utilsds-0.3/README.md
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)       38 2024-05-28 10:24:13.978501 utilsds-0.3/setup.cfg
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     5307 2024-05-28 10:22:08.000000 utilsds-0.3/setup.py
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 10:24:13.970260 utilsds-0.3/utilsds/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 09:41:40.000000 utilsds-0.3/utilsds/__init__.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2789 2024-05-28 09:39:31.000000 utilsds-0.3/utilsds/data_split.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     1174 2024-05-28 09:39:30.000000 utilsds-0.3/utilsds/ds_statistics.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)    14396 2024-05-28 09:39:30.000000 utilsds-0.3/utilsds/model_experiments.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     4659 2024-05-28 09:39:31.000000 utilsds-0.3/utilsds/transform_data.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)    12367 2024-05-28 09:39:31.000000 utilsds-0.3/utilsds/visualization.py
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 10:24:13.972768 utilsds-0.3/utilsds.egg-info/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     5828 2024-05-28 10:24:13.000000 utilsds-0.3/utilsds.egg-info/PKG-INFO
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)      319 2024-05-28 10:24:13.000000 utilsds-0.3/utilsds.egg-info/SOURCES.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        1 2024-05-28 10:24:13.000000 utilsds-0.3/utilsds.egg-info/dependency_links.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2940 2024-05-28 10:24:13.000000 utilsds-0.3/utilsds.egg-info/requires.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        8 2024-05-28 10:24:13.000000 utilsds-0.3/utilsds.egg-info/top_level.txt
+drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:40:57.040486 utilsds-0.3.1/
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     6225 2024-05-28 11:40:57.038548 utilsds-0.3.1/PKG-INFO
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)       67 2024-05-28 11:30:15.000000 utilsds-0.3.1/README.md
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)       38 2024-05-28 11:40:57.040597 utilsds-0.3.1/setup.cfg
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     5405 2024-05-28 11:37:34.000000 utilsds-0.3.1/setup.py
+drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:40:57.026034 utilsds-0.3.1/utilsds/
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 09:41:40.000000 utilsds-0.3.1/utilsds/__init__.py
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2789 2024-05-28 09:39:31.000000 utilsds-0.3.1/utilsds/data_split.py
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     1174 2024-05-28 09:39:30.000000 utilsds-0.3.1/utilsds/ds_statistics.py
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)    14396 2024-05-28 09:39:30.000000 utilsds-0.3.1/utilsds/model_experiments.py
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     4659 2024-05-28 09:39:31.000000 utilsds-0.3.1/utilsds/transform_data.py
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)    12367 2024-05-28 09:39:31.000000 utilsds-0.3.1/utilsds/visualization.py
+drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:40:57.033727 utilsds-0.3.1/utilsds.egg-info/
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     6225 2024-05-28 11:40:56.000000 utilsds-0.3.1/utilsds.egg-info/PKG-INFO
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)      319 2024-05-28 11:40:56.000000 utilsds-0.3.1/utilsds.egg-info/SOURCES.txt
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)        1 2024-05-28 11:40:56.000000 utilsds-0.3.1/utilsds.egg-info/dependency_links.txt
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2940 2024-05-28 11:40:56.000000 utilsds-0.3.1/utilsds.egg-info/requires.txt
+-rw-r--r--   0 patryk.kotulak   (502) staff       (20)        8 2024-05-28 11:40:56.000000 utilsds-0.3.1/utilsds.egg-info/top_level.txt
```

### Comparing `utilsds-0.3/PKG-INFO` & `utilsds-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsds
-Version: 0.3
+Version: 0.3.1
 Summary: Solution for DS Team
 Author: DS Team
 Author-email: ds@sts.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -172,10 +172,29 @@
 Requires-Dist: vine==5.1.0
 Requires-Dist: voluptuous==0.14.2
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yellowbrick==1.5
 Requires-Dist: zc.lockfile==3.0.post1
 
-# utils
+# utilsds
+
+Utilsds is a library includes classes and function used in ds project such as:
+- data_split: 
+    - train_validation_test_split
+- ds_statistics: 
+    - test_kruskal_wallis
+- model_experiments: 
+    - Modeling
+- transform_data: 
+    - PreprocesingData
+- visualization: 
+    - MetricsPlot,
+    - Radar,
+    - cluster_characteristics,
+    - comparison_density,
+    - feature_distribution_box,
+    - elbow_visualisation,
+    - describe_clusters_metrics
+
+
 
-Solution includes classes and function used in ds project.
```

### Comparing `utilsds-0.3/setup.py` & `utilsds-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
+with open('docs/ALTERNATIVE_README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name='utilsds',
-    version='0.3',
+    version='0.3.1',
     packages=find_packages(),
     install_requires=[
         'aiohttp==3.9.5',
         'aiohttp-retry==2.8.3',
         'aiosignal==1.3.1',
         'amqp==5.2.0',
         'annotated-types==0.6.0',
@@ -171,15 +174,15 @@
         'yarl==1.9.4',
         'yellowbrick==1.5',
         'zc.lockfile==3.0.post1',
     ],
     author='DS Team',
     author_email='ds@sts.pl',
     description='Solution for DS Team',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.11',
```

### Comparing `utilsds-0.3/utilsds/data_split.py` & `utilsds-0.3.1/utilsds/data_split.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3/utilsds/ds_statistics.py` & `utilsds-0.3.1/utilsds/ds_statistics.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3/utilsds/model_experiments.py` & `utilsds-0.3.1/utilsds/model_experiments.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3/utilsds/transform_data.py` & `utilsds-0.3.1/utilsds/transform_data.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3/utilsds/visualization.py` & `utilsds-0.3.1/utilsds/visualization.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3/utilsds.egg-info/PKG-INFO` & `utilsds-0.3.1/utilsds.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsds
-Version: 0.3
+Version: 0.3.1
 Summary: Solution for DS Team
 Author: DS Team
 Author-email: ds@sts.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -172,10 +172,29 @@
 Requires-Dist: vine==5.1.0
 Requires-Dist: voluptuous==0.14.2
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yellowbrick==1.5
 Requires-Dist: zc.lockfile==3.0.post1
 
-# utils
+# utilsds
+
+Utilsds is a library includes classes and function used in ds project such as:
+- data_split: 
+    - train_validation_test_split
+- ds_statistics: 
+    - test_kruskal_wallis
+- model_experiments: 
+    - Modeling
+- transform_data: 
+    - PreprocesingData
+- visualization: 
+    - MetricsPlot,
+    - Radar,
+    - cluster_characteristics,
+    - comparison_density,
+    - feature_distribution_box,
+    - elbow_visualisation,
+    - describe_clusters_metrics
+
+
 
-Solution includes classes and function used in ds project.
```

### Comparing `utilsds-0.3/utilsds.egg-info/requires.txt` & `utilsds-0.3.1/utilsds.egg-info/requires.txt`

 * *Files identical despite different names*

