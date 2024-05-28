# Comparing `tmp/dilcher-configuration-0.6.4.tar.gz` & `tmp/dilcher_configuration-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dilcher-configuration-0.6.4.tar", last modified: Fri Nov  5 10:26:53 2021, max compression
+gzip compressed data, was "dilcher_configuration-0.6.5.tar", last modified: Tue May 28 11:03:48 2024, max compression
```

## Comparing `dilcher-configuration-0.6.4.tar` & `dilcher_configuration-0.6.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 10:26:53.942095 dilcher-configuration-0.6.4/
--rw-r--r--   0 root         (0) root         (0)    11356 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1187 2021-11-05 10:26:53.942095 dilcher-configuration-0.6.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 10:26:53.938095 dilcher-configuration-0.6.4/dilcher_configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      773 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration/apps.py
--rw-r--r--   0 root         (0) root         (0)     2804 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration/mixins.py
--rw-r--r--   0 root         (0) root         (0)     6920 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration/models.py
--rw-r--r--   0 root         (0) root         (0)    22822 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration/test_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 10:26:53.942095 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1187 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/dilcher_configuration.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-05 10:26:53.942095 dilcher-configuration-0.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      811 2021-11-05 10:26:53.000000 dilcher-configuration-0.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:03:48.374925 dilcher_configuration-0.6.5/
+-rw-r--r--   0 root         (0) root         (0)    11356 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-28 11:03:48.374925 dilcher_configuration-0.6.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:03:48.370925 dilcher_configuration-0.6.5/dilcher_configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      773 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     6920 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration/models.py
+-rw-r--r--   0 root         (0) root         (0)    22822 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration/test_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:03:48.370925 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/dilcher_configuration.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:03:48.374925 dilcher_configuration-0.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      811 2024-05-28 11:03:48.000000 dilcher_configuration-0.6.5/setup.py
```

### Comparing `dilcher-configuration-0.6.4/LICENSE` & `dilcher_configuration-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dilcher-configuration-0.6.4/PKG-INFO` & `dilcher_configuration-0.6.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dilcher-configuration
-Version: 0.6.4
+Version: 0.6.5
 Summary: The dilcher-configuration Django app is used to provide easily manageable settings for Django projects.
 Home-page: https://github.com/cdilcher/dilcher-configuration
 Author: Philipp Freyer
 Author-email: philipp.freyer@dilcher.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=3.0.0
 
 #### Dilcher-configuration
 
 The dilcher-configuration Django app is used to provide easily manageable settings
 for Django projects.
 
 It does not define any data model on its won. Instead, it provides an abstract
@@ -25,9 +24,7 @@
 
 When such a class is saved, then `pre_save` and `post_save` signals
 will take care of ensuring that timestamps are
 updated and only one set of Settings is active at a time.
 
 This module does not define any Django Admin views, you will need to do that
 in your own app.
-
-
```

### Comparing `dilcher-configuration-0.6.4/dilcher_configuration/apps.py` & `dilcher_configuration-0.6.5/dilcher_configuration/apps.py`

 * *Files identical despite different names*

### Comparing `dilcher-configuration-0.6.4/dilcher_configuration/mixins.py` & `dilcher_configuration-0.6.5/dilcher_configuration/mixins.py`

 * *Files identical despite different names*

### Comparing `dilcher-configuration-0.6.4/dilcher_configuration/models.py` & `dilcher_configuration-0.6.5/dilcher_configuration/models.py`

 * *Files identical despite different names*

### Comparing `dilcher-configuration-0.6.4/dilcher_configuration/test_models.py` & `dilcher_configuration-0.6.5/dilcher_configuration/test_models.py`

 * *Files identical despite different names*

### Comparing `dilcher-configuration-0.6.4/dilcher_configuration.egg-info/PKG-INFO` & `dilcher_configuration-0.6.5/dilcher_configuration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dilcher-configuration
-Version: 0.6.4
+Version: 0.6.5
 Summary: The dilcher-configuration Django app is used to provide easily manageable settings for Django projects.
 Home-page: https://github.com/cdilcher/dilcher-configuration
 Author: Philipp Freyer
 Author-email: philipp.freyer@dilcher.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=3.0.0
 
 #### Dilcher-configuration
 
 The dilcher-configuration Django app is used to provide easily manageable settings
 for Django projects.
 
 It does not define any data model on its won. Instead, it provides an abstract
@@ -25,9 +24,7 @@
 
 When such a class is saved, then `pre_save` and `post_save` signals
 will take care of ensuring that timestamps are
 updated and only one set of Settings is active at a time.
 
 This module does not define any Django Admin views, you will need to do that
 in your own app.
-
-
```

### Comparing `dilcher-configuration-0.6.4/setup.py` & `dilcher_configuration-0.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("Readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name="dilcher-configuration",       # Replace with your own username
-  version="0.6.4",
+  version="0.6.5",
   author="Philipp Freyer",
   author_email="philipp.freyer@dilcher.de",
   description="The dilcher-configuration Django app is used to provide easily manageable settings for Django projects.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/cdilcher/dilcher-configuration",
   packages=setuptools.find_packages(),
```

