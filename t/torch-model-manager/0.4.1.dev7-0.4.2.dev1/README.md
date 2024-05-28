# Comparing `tmp/torch_model_manager-0.4.1.dev7.tar.gz` & `tmp/torch_model_manager-0.4.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.1.dev7.tar", last modified: Fri May 24 12:06:21 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.2.dev1.tar", last modified: Tue May 28 14:09:21 2024, max compression
```

## Comparing `torch_model_manager-0.4.1.dev7.tar` & `torch_model_manager-0.4.2.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.648494 torch_model_manager-0.4.1.dev7/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-24 12:06:21.648494 torch_model_manager-0.4.1.dev7/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-24 12:06:21.648494 torch_model_manager-0.4.1.dev7/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-24 12:06:19.000000 torch_model_manager-0.4.1.dev7/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.640494 torch_model_manager-0.4.1.dev7/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.640494 torch_model_manager-0.4.1.dev7/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.644494 torch_model_manager-0.4.1.dev7/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.644494 torch_model_manager-0.4.1.dev7/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    21686 2024-05-24 12:05:37.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev7/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.648494 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-24 12:06:21.000000 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-24 12:06:21.000000 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-24 12:06:21.000000 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-24 12:06:21.000000 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-24 12:06:21.000000 torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 12:06:21.648494 torch_model_manager-0.4.1.dev7/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev7/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev7/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-28 14:09:19.000000 torch_model_manager-0.4.2.dev1/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    23728 2024-05-28 14:05:47.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.2.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-28 14:09:21.000000 torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-28 14:09:21.753899 torch_model_manager-0.4.2.dev1/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.2.dev1/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.2.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.1.dev7/PKG-INFO` & `torch_model_manager-0.4.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev7
+Version: 0.4.2.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev7/README.md` & `torch_model_manager-0.4.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/setup.py` & `torch_model_manager-0.4.2.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.1.dev7',
+    version='0.4.2.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.1.dev7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.2.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.2.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.2.dev1/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.2.dev1/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.2.dev1/torch_model_manager/segmentation_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import supervision as sv
 
 import sys
 import os
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 from groundingdino.util.inference import Model
 from utils import helpers
-from segment_anything import sam_model_registry, SamPredictor
+from segment_anything import sam_model_registry, SamPredictor, SamAutomaticMaskGenerator
 from scipy.stats import hmean
 import pandas as pd
 from tqdm import tqdm
 from PIL import Image
 import matplotlib.pyplot as plt
 from torchvision import transforms
 from sklearn.preprocessing import LabelEncoder
@@ -164,22 +164,24 @@
                 os.system(f"mv groundingdino_swint_ogc.pth {g_dino_checkpoint_path}")
 
         # Initialize models
         self.grounding_dino_model = Model(model_config_path=g_dino_model_config_path, 
                                           model_checkpoint_path=g_dino_checkpoint_path,
                                           device = self.device)
 
-        sam = sam_model_registry[sam_type](checkpoint=sam_checkpoint_path)
-        sam.to(device=self.device)
-        self.sam_predictor = SamPredictor(sam)
+        self.sam = sam_model_registry[sam_type](checkpoint=sam_checkpoint_path)
+        self.sam.to(device=self.device)
+        self.sam_predictor = SamPredictor(self.sam)
+        self.mask_generator = SamAutomaticMaskGenerator(self.sam)
 
     def load_image(self, image_path):
         return cv2.imread(image_path)
 
-
+    def set_mask_generator_(self, **kwargs):
+        self.mask_generator = SamAutomaticMaskGenerator(self.sam, **kwargs)
 
     def detect_objects(self, image, classes, box_threshold=0.25, text_threshold=0.25):
         detections = self.grounding_dino_model.predict_with_classes(
             image=image,
             classes=classes,
             box_threshold=box_threshold,
             text_threshold=text_threshold
@@ -293,15 +295,14 @@
         # Remove None values
         class_ids = np.delete(class_ids, none_indices)
         confidences = np.delete(confidences, none_indices)
         detections.xyxy = np.delete(detections.xyxy, none_indices, axis=0)
         detections.mask = np.delete(detections.mask, none_indices, axis=0)
         detections.class_id = class_ids
         detections.confidence = confidences
-        print(detections)
 
         labels = [f"{classes[class_id]} {confidence:0.2f}" for class_id, confidence in zip(class_ids, confidences)]
 
         annotated_image = mask_annotator.annotate(scene=image.copy(), detections=detections)
         annotated_image = box_annotator.annotate(scene=annotated_image, detections=detections, labels=labels)
         return annotated_image
 
@@ -441,14 +442,56 @@
         if run is not None and output_namespaces["adjacency_tensor"] is not None:
             run.log_files(data=tensor, namespace=output_namespaces["adjacency_tensor"], extension="pkl", wait=True)
 
         return {"adjacency_tensor" : tensor, "index": matrix.index, "columns": classes, "annotation_matrix": matrix}
 
     def save_image(self, image, path):
         cv2.imwrite(path, image)
+
+    def auto_segmentation(self, img_path, img_size=(1024, 1024), run=None, output_namespaces=None, **kwargs):
+        def show_anns(anns):
+            if len(anns) == 0:
+                return
+            sorted_anns = sorted(anns, key=(lambda x: x['area']), reverse=True)
+
+            img = np.ones((sorted_anns[0]['segmentation'].shape[0], sorted_anns[0]['segmentation'].shape[1], 4))
+            img[:,:,3] = 0
+            for ann in sorted_anns:
+                m = ann['segmentation']
+                color_mask = np.concatenate([np.random.random(3), [0.35]])
+                img[m] = color_mask
+            return img
+            
+        # Read the image
+        image = cv2.imread(img_path)
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        image = cv2.resize(image, img_size)
+
+        if kwargs != {}:
+            self.set_mask_generator_(**kwargs)
+
+        masks = self.mask_generator.generate(image)
+        annot_img = show_anns(masks)
+
+        if run is not None:
+            if output_namespaces["annotated_images"] is not None:
+                # Define a transform to convert the image to tensor
+                transform = transforms.ToTensor()
+
+                # Convert the image to PyTorch tensor
+                rgb_image = transform(image)
+                rgb_image = rgb_image[[2, 1, 0], :, :]
+                run.log_tensors(tensors=[rgb_image], paths=[os.path.join(output_namespaces["annotated_images"], img_path.split("/")[-1])], on_series=False)
+            
+            if output_namespaces["detections"] is not None:
+                image_name = img_path.split("/")[-1]
+                image_name = image_name.split(".")[0]
+                run.log_files(data = masks, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
+
+        return masks, annot_img
         
 # # # Example usage
 # if __name__ == "__main__":
 #     SOURCE_IMAGE_PATH = "G0041951.JPG"
 #     CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
 #     BOX_THRESHOLD = 0.3
 #     TEXT_THRESHOLD = 0.25
```

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.2.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.2.dev1/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev7
+Version: 0.4.2.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.2.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev7/utils/helpers.py` & `torch_model_manager-0.4.2.dev1/utils/helpers.py`

 * *Files identical despite different names*

