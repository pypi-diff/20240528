# Comparing `tmp/torch_model_manager-0.4.2.dev1.tar.gz` & `tmp/torch_model_manager-0.4.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.2.dev1.tar", last modified: Tue May 28 14:09:21 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.2.dev2.tar", last modified: Tue May 28 19:09:12 2024, max compression
```

## Comparing `torch_model_manager-0.4.2.dev1.tar` & `torch_model_manager-0.4.2.dev2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-28 14:09:19.000000 torch_model_manager-0.4.2.dev1/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    23728 2024-05-28 14:05:47.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.2.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.128854 torch_model_manager-0.4.2.dev2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 19:09:12.128854 torch_model_manager-0.4.2.dev2/PKG-INFO
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-28 19:09:12.128854 torch_model_manager-0.4.2.dev2/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     2243 2024-05-28 19:09:09.000000 torch_model_manager-0.4.2.dev2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.120854 torch_model_manager-0.4.2.dev2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.120854 torch_model_manager-0.4.2.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.120854 torch_model_manager-0.4.2.dev2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.124854 torch_model_manager-0.4.2.dev2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      148 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    32763 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    24117 2024-05-28 19:05:35.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.128854 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9225 2024-05-28 19:09:12.000000 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      666 2024-05-28 19:09:12.000000 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-28 19:09:12.000000 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      241 2024-05-28 19:09:12.000000 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-28 19:09:12.000000 torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 19:09:12.124854 torch_model_manager-0.4.2.dev2/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-28 18:57:27.000000 torch_model_manager-0.4.2.dev2/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     9031 2024-05-28 18:57:50.000000 torch_model_manager-0.4.2.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.2.dev1/PKG-INFO` & `torch_model_manager-0.4.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev1
+Version: 0.4.2.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev1/README.md` & `torch_model_manager-0.4.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/setup.py` & `torch_model_manager-0.4.2.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.2.dev1',
+    version='0.4.2.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.2.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.2.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.2.dev2/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.2.dev2/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.2.dev2/torch_model_manager/segmentation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
             run.log_files(data=tensor, namespace=output_namespaces["adjacency_tensor"], extension="pkl", wait=True)
 
         return {"adjacency_tensor" : tensor, "index": matrix.index, "columns": classes, "annotation_matrix": matrix}
 
     def save_image(self, image, path):
         cv2.imwrite(path, image)
 
-    def auto_segmentation(self, img_path, img_size=(1024, 1024), run=None, output_namespaces=None, **kwargs):
+    def auto_segmentation(self, img_path, img_size=None, run=None, output_namespaces=None, **kwargs):
         def show_anns(anns):
             if len(anns) == 0:
                 return
             sorted_anns = sorted(anns, key=(lambda x: x['area']), reverse=True)
 
             img = np.ones((sorted_anns[0]['segmentation'].shape[0], sorted_anns[0]['segmentation'].shape[1], 4))
             img[:,:,3] = 0
@@ -460,15 +460,16 @@
                 color_mask = np.concatenate([np.random.random(3), [0.35]])
                 img[m] = color_mask
             return img
             
         # Read the image
         image = cv2.imread(img_path)
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        image = cv2.resize(image, img_size)
+        if img_size is not None:
+            image = cv2.resize(image, img_size)
 
         if kwargs != {}:
             self.set_mask_generator_(**kwargs)
 
         masks = self.mask_generator.generate(image)
         annot_img = show_anns(masks)
 
@@ -484,14 +485,21 @@
             
             if output_namespaces["detections"] is not None:
                 image_name = img_path.split("/")[-1]
                 image_name = image_name.split(".")[0]
                 run.log_files(data = masks, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
 
         return masks, annot_img
+    
+    def auto_seg_images(self, image_folder_path, img_size=None, run=None, output_namespaces=None, **kwargs):
+        image_paths = sorted([os.path.join(image_folder_path, img) for img in os.listdir(image_folder_path)])
+        for img_path in image_paths:
+            self.auto_segmentation(img_path, img_size, run, output_namespaces, **kwargs)
+    
+    
         
 # # # Example usage
 # if __name__ == "__main__":
 #     SOURCE_IMAGE_PATH = "G0041951.JPG"
 #     CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
 #     BOX_THRESHOLD = 0.3
 #     TEXT_THRESHOLD = 0.25
```

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.2.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.2.dev2/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.2.dev1
+Version: 0.4.2.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.2.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.2.dev1/utils/helpers.py` & `torch_model_manager-0.4.2.dev2/utils/helpers.py`

 * *Files identical despite different names*

