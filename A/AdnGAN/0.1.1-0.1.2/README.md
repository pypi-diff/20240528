# Comparing `tmp/AdnGAN-0.1.1.tar.gz` & `tmp/AdnGAN-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdnGAN-0.1.1.tar", last modified: Tue May 28 20:18:31 2024, max compression
+gzip compressed data, was "AdnGAN-0.1.2.tar", last modified: Tue May 28 20:21:13 2024, max compression
```

## Comparing `AdnGAN-0.1.1.tar` & `AdnGAN-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 20:18:31.560241 AdnGAN-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-28 20:18:31.556301 AdnGAN-0.1.1/AdnGAN/
--rw-rw-rw-   0        0        0     2129 2024-05-27 17:33:33.000000 AdnGAN-0.1.1/AdnGAN/Discriminator.py
--rw-rw-rw-   0        0        0     1187 2024-05-27 10:37:38.000000 AdnGAN-0.1.1/AdnGAN/Generator.py
--rw-rw-rw-   0        0        0     6842 2024-05-27 21:02:36.000000 AdnGAN-0.1.1/AdnGAN/ProGAN.py
--rw-rw-rw-   0        0        0      171 2024-05-27 18:08:46.000000 AdnGAN-0.1.1/AdnGAN/__init__.py
--rw-rw-rw-   0        0        0     1508 2024-05-28 20:12:05.000000 AdnGAN-0.1.1/AdnGAN/dataset.py
--rw-rw-rw-   0        0        0     3645 2024-05-27 18:08:21.000000 AdnGAN-0.1.1/AdnGAN/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-28 20:18:31.559209 AdnGAN-0.1.1/AdnGAN.egg-info/
--rw-rw-rw-   0        0        0      590 2024-05-28 20:18:31.000000 AdnGAN-0.1.1/AdnGAN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-28 20:18:31.000000 AdnGAN-0.1.1/AdnGAN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 20:18:31.000000 AdnGAN-0.1.1/AdnGAN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-28 20:18:31.000000 AdnGAN-0.1.1/AdnGAN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 20:18:31.000000 AdnGAN-0.1.1/AdnGAN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      590 2024-05-28 20:18:31.560241 AdnGAN-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-05-27 08:34:30.000000 AdnGAN-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 20:18:31.560241 AdnGAN-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      751 2024-05-28 20:18:16.000000 AdnGAN-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:21:13.515635 AdnGAN-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-28 20:21:13.511627 AdnGAN-0.1.2/AdnGAN/
+-rw-rw-rw-   0        0        0     2129 2024-05-27 17:33:33.000000 AdnGAN-0.1.2/AdnGAN/Discriminator.py
+-rw-rw-rw-   0        0        0     1187 2024-05-27 10:37:38.000000 AdnGAN-0.1.2/AdnGAN/Generator.py
+-rw-rw-rw-   0        0        0     6842 2024-05-27 21:02:36.000000 AdnGAN-0.1.2/AdnGAN/ProGAN.py
+-rw-rw-rw-   0        0        0      171 2024-05-27 18:08:46.000000 AdnGAN-0.1.2/AdnGAN/__init__.py
+-rw-rw-rw-   0        0        0     1504 2024-05-28 20:21:02.000000 AdnGAN-0.1.2/AdnGAN/dataset.py
+-rw-rw-rw-   0        0        0     3645 2024-05-27 18:08:21.000000 AdnGAN-0.1.2/AdnGAN/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:21:13.514633 AdnGAN-0.1.2/AdnGAN.egg-info/
+-rw-rw-rw-   0        0        0      590 2024-05-28 20:21:13.000000 AdnGAN-0.1.2/AdnGAN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-28 20:21:13.000000 AdnGAN-0.1.2/AdnGAN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 20:21:13.000000 AdnGAN-0.1.2/AdnGAN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-28 20:21:13.000000 AdnGAN-0.1.2/AdnGAN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 20:21:13.000000 AdnGAN-0.1.2/AdnGAN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      590 2024-05-28 20:21:13.514633 AdnGAN-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2024-05-27 08:34:30.000000 AdnGAN-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 20:21:13.515846 AdnGAN-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      751 2024-05-28 20:21:08.000000 AdnGAN-0.1.2/setup.py
```

### Comparing `AdnGAN-0.1.1/AdnGAN/Discriminator.py` & `AdnGAN-0.1.2/AdnGAN/Discriminator.py`

 * *Files identical despite different names*

### Comparing `AdnGAN-0.1.1/AdnGAN/Generator.py` & `AdnGAN-0.1.2/AdnGAN/Generator.py`

 * *Files identical despite different names*

### Comparing `AdnGAN-0.1.1/AdnGAN/ProGAN.py` & `AdnGAN-0.1.2/AdnGAN/ProGAN.py`

 * *Files identical despite different names*

### Comparing `AdnGAN-0.1.1/AdnGAN/dataset.py` & `AdnGAN-0.1.2/AdnGAN/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 
         def __getitem__(self, idx):
             idx = idx % len(self.image_folder)
             image, label = self.image_folder[idx]
             return image
         
 
-    custom_dataset = CustomDataset(root_dir=default_path, transform=transform)
+    custom_dataset = CustomDataset(root_dir=root_dir, transform=transform)
     dataloader = DataLoader(custom_dataset, batch_size=batch_size, shuffle=True)
 
 
     return dataloader,custom_dataset
```

### Comparing `AdnGAN-0.1.1/AdnGAN/tools.py` & `AdnGAN-0.1.2/AdnGAN/tools.py`

 * *Files identical despite different names*

### Comparing `AdnGAN-0.1.1/AdnGAN.egg-info/PKG-INFO` & `AdnGAN-0.1.2/AdnGAN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdnGAN
-Version: 0.1.1
+Version: 0.1.2
 Summary: AdnGAN is a Generative Adversarial Network (GAN) that generates images from random noise.
 Home-page: https://github.com/AdnaneMaj/AdnGAN/tree/main/AdnGAN
 Author: Adnane MAJDOUB
 Author-email: adnanemajdoub@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdnGAN-0.1.1/PKG-INFO` & `AdnGAN-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdnGAN
-Version: 0.1.1
+Version: 0.1.2
 Summary: AdnGAN is a Generative Adversarial Network (GAN) that generates images from random noise.
 Home-page: https://github.com/AdnaneMaj/AdnGAN/tree/main/AdnGAN
 Author: Adnane MAJDOUB
 Author-email: adnanemajdoub@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdnGAN-0.1.1/setup.py` & `AdnGAN-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AdnGAN',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'torch',
         'torchvision',
         'numpy',
         'matplotlib',
     ],
```

