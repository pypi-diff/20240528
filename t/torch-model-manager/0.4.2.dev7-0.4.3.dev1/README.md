# Comparing `tmp/torch_model_manager-0.4.2.dev7.tar.gz` & `tmp/torch_model_manager-0.4.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.2.dev7.tar", last modified: Tue May 28 20:55:31 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.3.dev1.tar", last modified: Tue May 28 21:01:41 2024, max compression
```

## Comparing `torch_model_manager-0.4.2.dev7.tar` & `torch_model_manager-0.4.3.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/PKG-INFO
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:55:31.112793 torch_model_manager-0.4.2.dev7/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:55:27.000000 torch_model_manager-0.4.2.dev7/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.100793 torch_model_manager-0.4.2.dev7/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.104793 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.104793 torch_model_manager-0.4.2.dev7/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1627 2024-05-28 20:55:15.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24167 2024-05-28 20:35:03.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:55:31.000000 torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:55:31.108793 torch_model_manager-0.4.2.dev7/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev7/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev7/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.116384 torch_model_manager-0.4.3.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 21:01:41.116384 torch_model_manager-0.4.3.dev1/PKG-INFO
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 21:01:41.116384 torch_model_manager-0.4.3.dev1/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 21:01:38.000000 torch_model_manager-0.4.3.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.108384 torch_model_manager-0.4.3.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.112384 torch_model_manager-0.4.3.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.112384 torch_model_manager-0.4.3.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.112384 torch_model_manager-0.4.3.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1627 2024-05-28 20:55:15.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24173 2024-05-28 21:01:03.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.116384 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 21:01:41.000000 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 21:01:41.000000 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 21:01:41.000000 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 21:01:41.000000 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 21:01:41.000000 torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 21:01:41.116384 torch_model_manager-0.4.3.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.3.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.3.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.2.dev7/PKG-INFO` & `torch_model_manager-0.4.3.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev7
+Version: 0.4.3.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev7/README.md` & `torch_model_manager-0.4.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/setup.py` & `torch_model_manager-0.4.3.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.2.dev7',
+    version='0.4.3.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.2.dev7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.3.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.3.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.3.dev1/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.3.dev1/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.3.dev1/torch_model_manager/segmentation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,16 +475,16 @@
 
         if run is not None:
             if output_namespaces["annotated_images"] is not None:
                 # Define a transform to convert the image to tensor
                 transform = transforms.ToTensor()
 
                 # Convert the image to PyTorch tensor
-                rgb_image = transform(image)
-                rgb_image = rgb_image[[2, 1, 0], :, :]
+                rgb_image = transform(annot_img)
+                # rgb_image = rgb_image[[2, 1, 0], :, :]
                 run.log_tensors(tensors=[rgb_image], paths=[os.path.join(output_namespaces["annotated_images"], img_path.split("/")[-1])], on_series=False)
             
             if output_namespaces["detections"] is not None:
                 image_name = img_path.split("/")[-1]
                 image_name = image_name.split(".")[0]
                 run.log_files(data = masks, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
```

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.3.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.3.dev1/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev7
+Version: 0.4.3.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.3.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev7/utils/helpers.py` & `torch_model_manager-0.4.3.dev1/utils/helpers.py`

 * *Files identical despite different names*

