# Comparing `tmp/torch_model_manager-0.4.2.dev4.tar.gz` & `tmp/torch_model_manager-0.4.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.2.dev4.tar", last modified: Tue May 28 20:04:35 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.2.dev5.tar", last modified: Tue May 28 20:35:20 2024, max compression
```

## Comparing `torch_model_manager-0.4.2.dev4.tar` & `torch_model_manager-0.4.2.dev5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/PKG-INFO
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:04:11.000000 torch_model_manager-0.4.2.dev4/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.800153 torch_model_manager-0.4.2.dev4/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.800153 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.812153 torch_model_manager-0.4.2.dev4/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24121 2024-05-28 19:37:06.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:04:35.000000 torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:04:35.840154 torch_model_manager-0.4.2.dev4/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev4/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev4/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.477378 torch_model_manager-0.4.2.dev5/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:35:20.477378 torch_model_manager-0.4.2.dev5/PKG-INFO
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 20:35:20.477378 torch_model_manager-0.4.2.dev5/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 20:35:16.000000 torch_model_manager-0.4.2.dev5/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.457378 torch_model_manager-0.4.2.dev5/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.461378 torch_model_manager-0.4.2.dev5/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.465378 torch_model_manager-0.4.2.dev5/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.473378 torch_model_manager-0.4.2.dev5/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24167 2024-05-28 20:35:03.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.473378 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 20:35:20.000000 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 20:35:20.000000 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 20:35:20.000000 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 20:35:20.000000 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 20:35:20.000000 torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 20:35:20.473378 torch_model_manager-0.4.2.dev5/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev5/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev5/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.2.dev4/PKG-INFO` & `torch_model_manager-0.4.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev4
+Version: 0.4.2.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev4/README.md` & `torch_model_manager-0.4.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/setup.py` & `torch_model_manager-0.4.2.dev5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.2.dev4',
+    version='0.4.2.dev5',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.2.dev4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.2.dev5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.2.dev5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.2.dev5/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.2.dev5/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.2.dev5/torch_model_manager/segmentation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,15 @@
                 image_name = image_name.split(".")[0]
                 run.log_files(data = masks, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
 
         return masks, annot_img
     
     def auto_seg_images(self, image_folder_path, image_size=None, run=None, output_namespaces=None, **kwargs):
         image_paths = sorted([os.path.join(image_folder_path, img) for img in os.listdir(image_folder_path)])
-        for img_path in image_paths:
+        for img_path in tqdm(image_paths, desc="Segmenting images", unit="image"):
             self.auto_segmentation(img_path, image_size, run, output_namespaces, **kwargs)
     
     
         
 # # # Example usage
 # if __name__ == "__main__":
 #     SOURCE_IMAGE_PATH = "G0041951.JPG"
```

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.2.dev5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.2.dev5/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev4
+Version: 0.4.2.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev4/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.2.dev5/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev4/utils/helpers.py` & `torch_model_manager-0.4.2.dev5/utils/helpers.py`

 * *Files identical despite different names*

