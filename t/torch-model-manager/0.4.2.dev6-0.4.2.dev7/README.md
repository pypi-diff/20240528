# Comparing `tmp/torch_model_manager-0.4.2.dev6.tar.gz` & `tmp/torch_model_manager-0.4.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.2.dev6.tar", last modified: Tue May 28 20:51:55 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.2.dev7.tar", last modified: Tue May 28 20:55:31 2024, max compression
```

## Comparing `torch_model_manager-0.4.2.dev6.tar` & `torch_model_manager-0.4.2.dev7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.914737 torch_model_manager-0.4.2.dev6/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:51:55.914737 torch_model_manager-0.4.2.dev6/PKG-INFO
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:51:55.914737 torch_model_manager-0.4.2.dev6/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:51:52.000000 torch_model_manager-0.4.2.dev6/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.894737 torch_model_manager-0.4.2.dev6/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.898737 torch_model_manager-0.4.2.dev6/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.898737 torch_model_manager-0.4.2.dev6/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.906737 torch_model_manager-0.4.2.dev6/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1763 2024-05-28 20:51:30.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24167 2024-05-28 20:35:03.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev6/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.910737 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:51:55.000000 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:51:55.000000 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:51:55.000000 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:51:55.000000 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:51:55.000000 torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:51:55.910737 torch_model_manager-0.4.2.dev6/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev6/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev6/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/PKG-INFO
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:55:27.000000 torch_model_manager-0.4.2.dev7/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.100793 torch_model_manager-0.4.2.dev7/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.104793 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.104793 torch_model_manager-0.4.2.dev7/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1627 2024-05-28 20:55:15.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24167 2024-05-28 20:35:03.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.2.dev6/PKG-INFO` & `torch_model_manager-0.4.2.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev6
+Version: 0.4.2.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev6/README.md` & `torch_model_manager-0.4.2.dev7/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/setup.py` & `torch_model_manager-0.4.2.dev7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.2.dev6',
+    version='0.4.2.dev7',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.2.dev6/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.2.dev7/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.2.dev7/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.2.dev7/torch_model_manager/notebook_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if change_dir:
         os.chdir(project)
 
 def install_dependencies(requirements_file="requirements.txt", script_file="requirements.sh", compiler="bash"):
     """
     Install the requirements from the requirements.txt file.
     """
-    assert os.path.exists(requirements_file) or os.path.exists(script_file), "Both requirements.txt and requirements.sh files are not found"
+    
     assert requirements_file is not None or script_file is not None, "Both requirements.txt and requirements.sh files are not found"
     
     if requirements_file is not None:
         os.system(f"pip install -r {requirements_file}")
     
     if script_file is not None:
         os.system(f"{compiler} {script_file}")
```

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.2.dev7/torch_model_manager/segmentation_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.2.dev7/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.2.dev7/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev6
+Version: 0.4.2.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev6/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev6/utils/helpers.py` & `torch_model_manager-0.4.2.dev7/utils/helpers.py`

 * *Files identical despite different names*

