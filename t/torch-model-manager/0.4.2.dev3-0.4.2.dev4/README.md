# Comparing `tmp/torch_model_manager-0.4.2.dev3.tar.gz` & `tmp/torch_model_manager-0.4.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.2.dev3.tar", last modified: Tue May 28 19:37:17 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.2.dev4.tar", last modified: Tue May 28 20:04:35 2024, max compression
```

## Comparing `torch_model_manager-0.4.2.dev3.tar` & `torch_model_manager-0.4.2.dev4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.628869 torch_model_manager-0.4.2.dev3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 19:37:17.628869 torch_model_manager-0.4.2.dev3/PKG-INFO
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 19:37:17.628869 torch_model_manager-0.4.2.dev3/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 19:37:13.000000 torch_model_manager-0.4.2.dev3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.608869 torch_model_manager-0.4.2.dev3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.616869 torch_model_manager-0.4.2.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.616869 torch_model_manager-0.4.2.dev3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.624869 torch_model_manager-0.4.2.dev3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24121 2024-05-28 19:37:06.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.628869 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 19:37:17.000000 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 19:37:17.000000 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 19:37:17.000000 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 19:37:17.000000 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 19:37:17.000000 torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:37:17.628869 torch_model_manager-0.4.2.dev3/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev3/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev3/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/PKG-INFO
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:04:11.000000 torch_model_manager-0.4.2.dev4/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.800153 torch_model_manager-0.4.2.dev4/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.800153 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.812153 torch_model_manager-0.4.2.dev4/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24121 2024-05-28 19:37:06.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.2.dev3/PKG-INFO` & `torch_model_manager-0.4.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev3
+Version: 0.4.2.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev3/README.md` & `torch_model_manager-0.4.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/setup.py` & `torch_model_manager-0.4.2.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.2.dev3',
+    version='0.4.2.dev4',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.2.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.2.dev4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.2.dev4/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.2.dev4/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.2.dev4/torch_model_manager/segmentation_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.2.dev4/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.2.dev4/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev3
+Version: 0.4.2.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev3/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev3/utils/helpers.py` & `torch_model_manager-0.4.2.dev4/utils/helpers.py`

 * *Files identical despite different names*

