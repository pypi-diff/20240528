# Comparing `tmp/geo_inference-2.0.3.tar.gz` & `tmp/geo_inference-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_inference-2.0.3.tar", last modified: Fri May 24 16:32:21 2024, max compression
+gzip compressed data, was "geo_inference-2.0.4.tar", last modified: Tue May 28 13:20:28 2024, max compression
```

## Comparing `geo_inference-2.0.3.tar` & `geo_inference-2.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.3/LICENSE
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.3/MANIFEST.in
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-24 16:32:21.656823 geo_inference-2.0.3/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3505 2024-04-17 02:45:20.000000 geo_inference-2.0.3/README.md
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-05-24 16:32:10.000000 geo_inference-2.0.3/geo_inference/__init__.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/config/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/config/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/config/log_config.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.3/geo_inference/config/logging_config.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.3/geo_inference/config/sample.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    16178 2024-05-24 15:05:14.000000 geo_inference-2.0.3/geo_inference/geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     5657 2024-05-14 16:59:04.000000 geo_inference-2.0.3/geo_inference/geo_inference.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/utils/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/utils/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.3/geo_inference/utils/geo.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.3/geo_inference/utils/geo_transforms.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.3/geo_inference/utils/helpers.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.3/geo_inference/utils/polygon.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference.egg-info/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/SOURCES.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/dependency_links.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/entry_points.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/requires.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/top_level.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1832 2024-05-24 16:32:10.000000 geo_inference-2.0.3/pyproject.toml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-05-24 16:32:21.656823 geo_inference-2.0.3/setup.cfg
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/tests/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.3/tests/test_geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.3/tests/test_geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.744493 geo_inference-2.0.4/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.4/LICENSE
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.4/MANIFEST.in
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-28 13:20:28.744493 geo_inference-2.0.4/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3505 2024-04-17 02:45:20.000000 geo_inference-2.0.4/README.md
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.740493 geo_inference-2.0.4/geo_inference/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-05-28 13:20:12.000000 geo_inference-2.0.4/geo_inference/__init__.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.740493 geo_inference-2.0.4/geo_inference/config/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.4/geo_inference/config/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.4/geo_inference/config/log_config.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.4/geo_inference/config/logging_config.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.4/geo_inference/config/sample.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    16020 2024-05-27 19:16:15.000000 geo_inference-2.0.4/geo_inference/geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     5457 2024-05-27 19:16:55.000000 geo_inference-2.0.4/geo_inference/geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.744493 geo_inference-2.0.4/geo_inference/utils/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.4/geo_inference/utils/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.4/geo_inference/utils/geo.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.4/geo_inference/utils/geo_transforms.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.4/geo_inference/utils/helpers.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.4/geo_inference/utils/polygon.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.744493 geo_inference-2.0.4/geo_inference.egg-info/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/entry_points.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/requires.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-05-28 13:20:28.000000 geo_inference-2.0.4/geo_inference.egg-info/top_level.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1832 2024-05-28 13:20:12.000000 geo_inference-2.0.4/pyproject.toml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-05-28 13:20:28.744493 geo_inference-2.0.4/setup.cfg
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-28 13:20:28.744493 geo_inference-2.0.4/tests/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.4/tests/test_geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.4/tests/test_geo_inference.py
```

### Comparing `geo_inference-2.0.3/LICENSE` & `geo_inference-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/PKG-INFO` & `geo_inference-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.3
+Version: 2.0.4
 Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geo_inference-2.0.3/README.md` & `geo_inference-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/config/log_config.yaml` & `geo_inference-2.0.4/geo_inference/config/log_config.yaml`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/config/logging_config.py` & `geo_inference-2.0.4/geo_inference/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/geo_blocks.py` & `geo_inference-2.0.4/geo_inference/geo_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,37 +306,33 @@
 class InferenceMerge:
     """
     A class for merging inference results.
     
     Attributes:
         height (int): The padded height of roi.
         width (int): The padded width of roi.
-        classes (int): The number of classes.
         device (torch.device): The device to use for computation.
         image (np.ndarray): The merged image.
         norm_mask (np.ndarray): The normalization mask.
     
     """
     def __init__(self, 
                  height: int, 
-                 width: int, 
-                 classes: int, 
+                 width: int,  
                  device: torch.device) -> None:
         """
         Initializes a new instance of the InferenceMerge class.
 
         Args:
             height (int): The padded height of roi.
             width (int): The padded width of roi.
-            classes (int): The number of classes.
             device (torch.device): The device to use for computation.
         """
         self.height = height
         self.width = width
-        self.classes = classes
         self.device = device
         self.image = np.zeros((self.classes, self.height, self.width), dtype=np.float16)
         self.norm_mask = np.ones((1, self.height, self.width), dtype=np.float16)
         # self.image = torch.zeros((self.classes, self.height, self.width), dtype=torch.float16, device=self.device)
         # self.norm_mask = torch.ones((1, self.height, self.width), dtype=torch.float16, device=self.device)
     
     @torch.no_grad()
```

### Comparing `geo_inference-2.0.3/geo_inference/geo_inference.py` & `geo_inference-2.0.4/geo_inference/geo_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,14 @@
         self.work_dir: Path = get_directory(work_dir)
         self.device = get_device(device=device, 
                                  gpu_id=self.gpu_id)
         model_path: Path = get_model(model_path_or_url=model, 
                                      work_dir=self.work_dir)
         self.mask_to_vec = mask_to_vec
         self.model = torch.jit.load(model_path, map_location=self.device)
-        dummy_input = torch.ones((1, 3, 32, 32), device=self.device, dtype=torch.float)
-        with torch.no_grad():
-            self.classes = self.model(dummy_input).shape[1]
     
     @torch.no_grad() 
     def __call__(self, tiff_image: str, bbox: str = None, patch_size: int = 512, stride_size: str = None) -> None:
         """
         Perform geo inference on geospatial imagery.
 
         Args:
@@ -79,15 +76,15 @@
         
         dataset = RasterDataset(tiff_image, bbox=bbox)
         sampler = InferenceSampler(dataset, size=patch_size, stride=patch_size >> 1 if stride_size is None else stride_size, roi=dataset.bbox)
         roi_height = sampler.im_height 
         roi_width = sampler.im_width
         h_padded, w_padded = roi_height + patch_size, roi_width + patch_size
         output_meta = dataset.src.meta
-        merge_patches = InferenceMerge(height=h_padded, width=w_padded, classes=self.classes, device=self.device)
+        merge_patches = InferenceMerge(height=h_padded, width=w_padded, device=self.device)
         dataloader = DataLoader(dataset, batch_size=self.batch_size, sampler=sampler, collate_fn=stack_samples)
         
         start_time = time.time()
         
         for batch in tqdm(dataloader, desc='extracting features', unit='batch', total=len(dataloader)):
             image_tensor = batch["image"].to(self.device)
             window_tensor = batch["window"].unsqueeze(1).to(self.device)
```

### Comparing `geo_inference-2.0.3/geo_inference/utils/geo.py` & `geo_inference-2.0.4/geo_inference/utils/geo.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/utils/geo_transforms.py` & `geo_inference-2.0.4/geo_inference/utils/geo_transforms.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/utils/helpers.py` & `geo_inference-2.0.4/geo_inference/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference/utils/polygon.py` & `geo_inference-2.0.4/geo_inference/utils/polygon.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/geo_inference.egg-info/PKG-INFO` & `geo_inference-2.0.4/geo_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.3
+Version: 2.0.4
 Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geo_inference-2.0.3/geo_inference.egg-info/SOURCES.txt` & `geo_inference-2.0.4/geo_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/pyproject.toml` & `geo_inference-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geo-inference"
-version = "2.0.3"
+version = "2.0.4"
 description = "Extract features from geospatial imagery using deep learning models"
 readme = "README.md"
 authors = [{ name = "Victor Alhassan", email = "victor.alhassan@nrcan-rncan.gc.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
@@ -47,15 +47,15 @@
 [project.scripts]
 geo_inference = "geo_inference.geo_inference:main"
 
 [tool.setuptools.packages.find]
 include = ["geo_inference*"]
 
 [tool.bumpver]
-current_version = "2.0.3"
+current_version = "2.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `geo_inference-2.0.3/tests/test_geo_blocks.py` & `geo_inference-2.0.4/tests/test_geo_blocks.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.3/tests/test_geo_inference.py` & `geo_inference-2.0.4/tests/test_geo_inference.py`

 * *Files identical despite different names*

