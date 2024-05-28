# Comparing `tmp/comseg-0.0.7.tar.gz` & `tmp/comseg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comseg-0.0.7.tar", last modified: Tue May  7 17:02:50 2024, max compression
+gzip compressed data, was "comseg-0.0.8.tar", last modified: Tue May 28 19:17:20 2024, max compression
```

## Comparing `comseg-0.0.7.tar` & `comseg-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.0.7/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1191 2024-05-07 17:02:50.462541 comseg-0.0.7/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      756 2024-01-04 19:49:48.000000 comseg-0.0.7/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      513 2024-05-07 17:02:43.000000 comseg-0.0.7/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)      356 2024-01-04 17:54:13.000000 comseg-0.0.7/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-07 17:02:50.462541 comseg-0.0.7/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.458541 comseg-0.0.7/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/ComSeg.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1191 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-07 17:02:50.000000 comseg-0.0.7/src/ComSeg.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.0.7/src/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/comseg/
--rw-rw-r--   0 tom       (1000) tom       (1000)      405 2024-05-07 15:28:06.000000 comseg-0.0.7/src/comseg/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18309 2024-03-19 13:32:23.000000 comseg-0.0.7/src/comseg/clustering.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18590 2024-05-07 15:22:51.000000 comseg-0.0.7/src/comseg/dataset.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18478 2024-05-07 16:26:44.000000 comseg-0.0.7/src/comseg/dictionary.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    35878 2024-05-07 15:33:03.000000 comseg-0.0.7/src/comseg/model.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-07 17:02:50.462541 comseg-0.0.7/src/comseg/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.0.7/src/comseg/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18790 2024-05-07 15:31:41.000000 comseg-0.0.7/src/comseg/utils/custom_louvain.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.0.7/src/comseg/utils/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.0.7/src/comseg/utils/preprocessing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.0.7/src/comseg/utils/utils_graph.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.0.8/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1235 2024-05-28 19:17:20.677910 comseg-0.0.8/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      800 2024-05-28 17:16:59.000000 comseg-0.0.8/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      513 2024-05-28 17:10:57.000000 comseg-0.0.8/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      374 2024-05-28 17:08:31.000000 comseg-0.0.8/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-28 19:17:20.677910 comseg-0.0.8/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.673910 comseg-0.0.8/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/ComSeg.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1235 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.0.8/src/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/comseg/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      405 2024-05-15 12:21:09.000000 comseg-0.0.8/src/comseg/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18288 2024-05-15 12:06:26.000000 comseg-0.0.8/src/comseg/clustering.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18324 2024-05-28 17:22:36.000000 comseg-0.0.8/src/comseg/dataset.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23616 2024-05-28 18:07:40.000000 comseg-0.0.8/src/comseg/dictionary.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    40561 2024-05-28 19:11:45.000000 comseg-0.0.8/src/comseg/model.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/comseg/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.0.8/src/comseg/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18897 2024-05-27 07:57:03.000000 comseg-0.0.8/src/comseg/utils/custom_louvain.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.0.8/src/comseg/utils/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.0.8/src/comseg/utils/preprocessing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.0.8/src/comseg/utils/utils_graph.py
```

### Comparing `comseg-0.0.7/LICENSE` & `comseg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `comseg-0.0.7/PKG-INFO` & `comseg-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.0.7
+Version: 0.0.8
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+<img src="./comseg.png" width="650" height="263">
+
+# News
+
+Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
+
+# Support
+
+If you have any questions relative to the package or bug, please open an issue in this repository.
+
+
 # ComSeg framework
 
-A detail documentation is available Here https://comseg.readthedocs.io/en/latest/userguide.html
+A detail documentation is available at https://comseg.readthedocs.io/
 
 
 # Single cell spatial RNA profiling 
 
 ComSeg is an algorithm for single cell spatial RNA profiling in image-based transcriptomic data.
 
 It takes as input a csv with the spot coordinates and output an anndata 
 object with the  genes expression and coordinates of each cell.
 
 ### Citation 
- A point cloud segmentation framework for image-based spatial transcriptomics
-Thomas Defard, Hugo Laporte, Mallick Ayan, Soulier Juliette, Sandra Curras-Alonso, Christian Weber, Florian Massip, José-Arturo Londoño-Vallejo, Charles Fouillade, Florian Mueller, Thomas Walter
-bioRxiv 2023.12.01.569528; doi: https://doi.org/10.1101/2023.12.01.569528 
+
+A point cloud segmentation framework for image-based spatial transcriptomic, Defard et al bioRxiv 2023.12.01.569528; doi: https://doi.org/10.1101/2023.12.01.569528
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `comseg-0.0.7/pyproject.toml` & `comseg-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ComSeg"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Thomas Defard", email="thomas.defard@mines-paristech.fr" },
 ]
 description = "single cell RNA profiling analysis of imaging-based spatial transcriptomics data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `comseg-0.0.7/src/ComSeg.egg-info/PKG-INFO` & `comseg-0.0.8/src/ComSeg.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.0.7
+Version: 0.0.8
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+<img src="./comseg.png" width="650" height="263">
+
+# News
+
+Update with comseg 0.0.7. Computation of the co-expression matrix is now faster.
+
+# Support
+
+If you have any questions relative to the package or bug, please open an issue in this repository.
+
+
 # ComSeg framework
 
-A detail documentation is available Here https://comseg.readthedocs.io/en/latest/userguide.html
+A detail documentation is available at https://comseg.readthedocs.io/
 
 
 # Single cell spatial RNA profiling 
 
 ComSeg is an algorithm for single cell spatial RNA profiling in image-based transcriptomic data.
 
 It takes as input a csv with the spot coordinates and output an anndata 
 object with the  genes expression and coordinates of each cell.
 
 ### Citation 
- A point cloud segmentation framework for image-based spatial transcriptomics
-Thomas Defard, Hugo Laporte, Mallick Ayan, Soulier Juliette, Sandra Curras-Alonso, Christian Weber, Florian Massip, José-Arturo Londoño-Vallejo, Charles Fouillade, Florian Mueller, Thomas Walter
-bioRxiv 2023.12.01.569528; doi: https://doi.org/10.1101/2023.12.01.569528 
+
+A point cloud segmentation framework for image-based spatial transcriptomic, Defard et al bioRxiv 2023.12.01.569528; doi: https://doi.org/10.1101/2023.12.01.569528
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `comseg-0.0.7/src/comseg/clustering.py` & `comseg-0.0.8/src/comseg/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,22 +419,22 @@
                     array_of_vect = unclassified_vector,
                     pca_model = pca_model,
                     kn_neighb =     kn_neighb,
                     min_proba=min_proba_small_commu,
                     param_sctransform=self.param_sctransform
                 )
 
-                list_pred_rna = np.array(self.anndata.obs['leiden_merged'])
+                list_pred_rna = np.array(self.anndata.obs[key_pred])
                 list_pred_rna[index_unclassified] = list_pred_rna_seq
-                self.anndata.obs['leiden_merged'] = list_pred_rna
+                self.anndata.obs[key_pred] = list_pred_rna
             else:
                 print("no small vector to classify")
 
 
-            return self.anndata.obs['leiden_merged']
+            return self.anndata.obs[key_pred]
```

### Comparing `comseg-0.0.7/src/comseg/dataset.py` & `comseg-0.0.8/src/comseg/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,19 +31,20 @@
     3) add prior knowledge if available
 
     The dataset class can be used like a dictionary of where the keys are the csv file names and the values are the csv
 
     """
 
     def __init__(self,
-        path_dataset_folder = None,
+        path_dataset_folder,
         path_to_mask_prior = None,
         mask_file_extension = ".tiff",
         dict_scale={"x": 0.103, 'y': 0.103, "z": 0.3},
-        mean_cell_diameter = 15):
+        mean_cell_diameter = 15,
+       gene_column = "gene"):
 
         """
         :param path_dataset_folder: path to the folder containing the csv files
         :type path_dataset_folder: str
         :param path_to_mask_prior: path to the folder containing the mask priors. They must have the same name as the corresponding csv files
         :type path_to_mask_prior:  str
         :param mask_file_extension: file extension of the mask priors
@@ -51,28 +52,33 @@
         :param dict_scale: dictionary containing the pixel/voxel size of the images in µm default is {"x": 0.103, 'y': 0.103, "z": 0.3}
         :type dict_scale: dict
         :param mean_cell_diameter: the expected mean cell diameter in µm default is 15µm
         :type mean_cell_diameter: float
         """
 
         self.path_dataset_folder = Path(path_dataset_folder)
-        self.path_to_mask_prior = Path(path_to_mask_prior)
+        if path_to_mask_prior is not None:
+            self.path_to_mask_prior = Path(path_to_mask_prior)
+        else:
+            self.path_to_mask_prior = None
         self.mask_file_extension = mask_file_extension
         self.path_image_dict = {}
+        self.gene_column = gene_column
+
         unique_gene = []
         for image_path_df in self.path_dataset_folder.glob(f'*.csv'):
             print(f"add {image_path_df.stem}")
             self.path_image_dict[image_path_df.stem] = image_path_df
-            unique_gene += list(pd.read_csv(self.path_image_dict[image_path_df.stem]).gene.unique())
+            unique_gene += list(pd.read_csv(self.path_image_dict[image_path_df.stem])[self.gene_column].unique())
         if len(self.path_image_dict) == 0:
             raise ValueError(f"no csv file found in the dataset folder {self.path_dataset_folder}")
         self.list_index = list(self.path_image_dict.keys())
         self.selected_genes = np.unique(unique_gene)
         self.dict_scale = dict_scale
-        self.dict_centroid = {}
+        self.dict_centroid = None
         self.mean_cell_diameter = mean_cell_diameter
 
     def __getitem__(self, key):
         if isinstance(key, int):
             return pd.read_csv(self.path_image_dict[self.list_index[key]])
         elif isinstance(key, str):
             return pd.read_csv(self.path_image_dict[key])
@@ -87,22 +93,45 @@
 
     def __repr__(self):
         return repr(f'dataset comseg  {self.list_index}')
 
     def keys(self):
         return self.list_index
 
+    def convert_spots_coord_in_pixel(self, overwrite = True):
+        """
+        convert the coordinates of the spots in the csv files from µm to pixels using the dict_scale attribute of the dataset object
+
+        :param overwrite: if True, overwrite the csv files with the new coordinates in pixels else save the new csv files with the suffix "_pixel"
+        :type bool
+        :return:
+        """
+        for image_path_df in self.path_dataset_folder.glob('*.csv'):
+            print(f"to pixel coordinates {image_path_df.stem}")
+            df_spots = pd.read_csv(image_path_df)
+
+            df_spots["y"] = (df_spots["y"] / self.dict_scale["y"]).astype(int)
+            df_spots["x"] = (df_spots["x"] / self.dict_scale["x"]).astype(int)
+            if "z" in df_spots.columns:
+                df_spots["z"] = (df_spots["z"] / self.dict_scale["z"]).astype(int)
+            if overwrite:
+                df_spots.to_csv(image_path_df, index=False)
+            else:
+                print(f"nex csv save as {image_path_df.parent /(image_path_df.stem+'_pixel.csv')}")
+                df_spots.to_csv(image_path_df.parent /(image_path_df.stem+'_pixel.csv'), index=False)
+
 
 
     #### fct adding prior
 
     def add_prior_from_mask(self,
                             prior_keys_name = 'in_nucleus',
                             overwrite = False,
                             compute_centroid = False,
+                            regex_df = "*.csv"
                             ):
 
         """
 
         This function add prior knowledge to the dataset. It adds a column in the csv files indicating prior label of each spot.
         It takes the positition of each spot and add the corresponding value of the mask prior at this position.
 
@@ -110,48 +139,52 @@
         :type str
         :param overwrite: if True, overwrite the prior_keys_name column if it already exists
         :type bool
         :param compute_centroid : if True, compute the centroid of each cell/nucleus in segmentation mask for to use it for RNA-cell association
         :type bool
         :return: None
         """
-        for image_path_df in self.path_dataset_folder.glob('*.csv'):
+        if compute_centroid:
+            self.dict_centroid = {}
+        for image_path_df in self.path_dataset_folder.glob(regex_df):
             print(f"add prior to {image_path_df.stem}")
             df_spots = pd.read_csv(image_path_df)
 
             assert (self.path_to_mask_prior / (image_path_df.stem + self.mask_file_extension)  ).exists(), f"no mask prior found for {image_path_df.stem}"
 
             if 'tif' in self.mask_file_extension[-4:] :
                 mask = tifffile.imread(self.path_to_mask_prior / (image_path_df.stem + self.mask_file_extension) )
             elif 'npy' in self.mask_file_extension[-4:]:
                 mask = np.load(self.path_to_mask_prior / (image_path_df.stem + self.mask_file_extension) )
             else:
                 raise ValueError("mask file extension not supported please use image_name.npy or image_name.tif(f)")
-            x_list = list(df_spots.x)
-            y_list = list(df_spots.y)
-            z_list = list(df_spots.z)
-            prior_list = []
-
-            for ix in range(len(z_list)):
-                nuc_index_prior = mask[int(z_list[ix]), int(y_list[ix]), int(x_list[ix])]
-                prior_list.append(nuc_index_prior)
+
+
+            if "z" in df_spots.columns and len(mask.shape) == 3:
+                pixel_coordinates = (df_spots[["z", "y", "x"]]).astype(int).values
+                prior_list = [mask[z, y, x] for (z, y, x) in pixel_coordinates]
+
+            else:
+                pixel_coordinates = (df_spots[["y",  "x"]]).astype(int).values
+                prior_list = [mask[y, x] for (y, x) in pixel_coordinates]
+
+
             if prior_keys_name in df_spots.columns and overwrite == False:
                 raise Exception(f"prior_keys_name {prior_keys_name} already in df_spots and overwrite is False")
             df_spots[prior_keys_name] = prior_list
             df_spots.to_csv(image_path_df,  index=False)
-            print(f"prior added to {image_path_df.stem} and save in csv file")
+            print(f"prior added to {image_path_df.stem} and saved in csv file")
 
-            from skimage import measure
 
             if compute_centroid:
                 dict_centroid = compute_dict_centroid(mask_nuclei = mask,
                                                       background=0)
 
                 self.dict_centroid[image_path_df.stem] = dict_centroid
-
+                print(f"dict_centroid added for {image_path_df.stem} ")
 
     ### compute the co-expression matrix
 
     def count_matrix_in_situ_from_knn(self,
                                       df_spots_label,
                                       n_neighbors=5,
                                       radius=None,
@@ -190,21 +223,21 @@
             list_coordo_order = list_coordo_order_no_scaling * np.array(
                 [self.dict_scale['z'], self.dict_scale['y'], self.dict_scale["x"]])
         else:
             list_coordo_order_no_scaling = np.array([df_spots_label.y, df_spots_label.x]).T
             list_coordo_order = list_coordo_order_no_scaling * np.array([self.dict_scale['y'], self.dict_scale['x']])
 
         dico_list_features = {}
-        assert 'gene' in df_spots_label.columns
+        assert self.gene_column in df_spots_label.columns
         for feature in df_spots_label.columns:
             dico_list_features[feature] = list(df_spots_label[feature])
         list_features = list(dico_list_features.keys())
         list_features_order = [(i, {feature: dico_list_features[feature][i] for feature in list_features}) for i in
                                range(len(df_spots_label))]
-        array_gene_indexed = np.array([dico_list_features['gene'][i] for i in range(len(df_spots_label))])
+        array_gene_indexed = np.array([dico_list_features[self.gene_column][i] for i in range(len(df_spots_label))])
 
 
         nbrs = NearestNeighbors(n_neighbors=n_neighbors, algorithm='ball_tree').fit(list_coordo_order)
         ad = nbrs.kneighbors_graph(list_coordo_order)  ## can be optimize here
         distance = nbrs.kneighbors_graph(list_coordo_order, mode='distance')
         ad[distance > radius] = 0
         ad.eliminate_zeros()
@@ -365,61 +398,14 @@
 
         dict_co_expression = self.get_dict_proba_edge_in_situ(count_matrix=count_matrix,
                                                           distance=distance,
                                                           )
         self.dict_co_expression = dict_co_expression
         return dico_proba_edge, count_matrix
 
-    def _compute_dico_centroid(mask_nuclei, dico_simu=None):
-        dico_nuclei_centroid = {}
-        nuclei_labels = measure.label(mask_nuclei, background=0)
-        for lb in measure.regionprops(nuclei_labels):
-            dico_nuclei_centroid[lb.label] = {}
-            dico_nuclei_centroid[lb.label]['centroid'] = lb.centroid
-            # print(lb.centroid)
-        return dico_nuclei_centroid
 
 
 
 
 
-    ### fct adding co-expression matrix
-
-
-if __name__ == "__main__":
-    list_marker_ns =  ['Atp6v0d2', 'Abcg1',# AM
-             'Rtkn2',  'Igfbp2', #AT1
-             'Sftpc','Cxcl15', #AT2,
-            'Cd79a', #B_cells
-             'Ms4a2', 'Fcer1a', #Basophils
-             'Ccdc153', #Ciliated
-             'Scgb3a2', 'Scgb1a1',#Club
-             'Cst3',#DC
-             'Cdh5', 'Clec14a',  #EC
-             'Inmt', 'Pcolce2', # Fibroblasts
-             'C1qc', 'C1qa', 'C1qb', # 'C3ar1', #IM
-             'Upk3b',# Mesotheliocytes
-             'Ifitm6','Plac8',# Monocytes
-            'Ms4a4b', 'Ccl5', 'Hcst', # NK_T_cells
-             'Gzma', 'Ncr1',# NK_cells
-             'S100a9',# Neutrophils
-             'Mmrn1',#Platelets
-           'Acta2','Myh11', # SMC
-             'Cd3g', 'Cd3d' #T_cells
-             ]
-
-    dataset = ComSegDataset(selected_genes = list_marker_ns,
-        path_dataset_folder = "/media/tom/T7/simulation/test_set/dataframes",
-                    path_to_mask_prior = "/media/tom/T7/simulation/test_set/mask",
-                    )
-    dataset.add_prior_from_mask()
 
-    dataset.compute_in_situ_edge(#dict_scale={"x": 0.103, 'y': 0.103, "z": 0.3},  # in micrometer
-            selected_genes=list_marker_ns,
-            images_subset = None,
-            mode="nearest_nn_radius",
-            n_neighbors=25,
-            radius=1,  # in micormeter
-            distance="pearson",
-            per_images=False,
-            sampling=False,
-            sampling_size=100000)
+    ### fct adding co-expression matrix
```

### Comparing `comseg-0.0.7/src/comseg/dictionary.py` & `comseg-0.0.8/src/comseg/dictionary.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 # update tutorial
 
 
 #%%
 
 
 
-
+import pandas as pd
 import os
 import sys
-
 from tqdm import tqdm
-
 import anndata as ad
 #from model import ComSegGraph
 #import clustering
 #from . import clustering ## for dev mode
 #import model
 #import clustering
 import pickle
@@ -60,16 +58,16 @@
                 detection method taking into account prior knowledge
         :type community_detection: str
         :param seed: (optional) seed for the graph partioning initialization
         :type seed: int
         :param prior_name: (optional) Name of the prior cell assignment column the input CSV file. Node with the same prior label will be merged into a super node.
         node with different prior label can not be merged during the modularity optimization.
         :type prior_name: str
-
         """
+
         #:param confidence_level: (experimental) confidence level for the prior knowledge (prior_name) in the range [0,1]. 1 means that the prior knowledge is certain.
         #:type confidence_level: float
         self.dataset = dataset
         self.mean_cell_diameter = mean_cell_diameter
         self.community_detection = community_detection
         self.seed = seed
         self.prior_name = prior_name
@@ -173,21 +171,24 @@
         :param self:
         :param k_nearest_neighbors: number of nearest neighbors to consider for the graph creation
         :type k_nearest_neighbors: int
         :return:
         """
         for img_name in tqdm(list(self.dataset)):
             #### GRAPH CREATION
-            comseg_m = ComSegGraph(selected_genes=self.dataset.selected_genes,
-                                         df_spots_label=self.dataset[img_name],
-                                         dict_scale=self.dataset.dict_scale,
-                                         mean_cell_diameter=self.mean_cell_diameter,  # in micrometer
-                                         dict_co_expression=self.dataset.dict_co_expression,
-                                         k_nearest_neighbors=k_nearest_neighbors,
-                                         )
+            comseg_m = ComSegGraph(
+                    selected_genes=self.dataset.selected_genes,
+                    df_spots_label=self.dataset[img_name],
+                    dict_scale=self.dataset.dict_scale,
+                    mean_cell_diameter=self.mean_cell_diameter,  # in micrometer
+                    dict_co_expression=self.dataset.dict_co_expression,
+                    k_nearest_neighbors=k_nearest_neighbors,
+                    gene_column= self.dataset.gene_column,
+                    prior_name=self.prior_name,
+                                   )
             comseg_m.create_graph()
             self[img_name] = comseg_m
 
             #### COMMÛTE COMMUNITY OF RNA
             comseg_m.community_vector(
                 clustering_method=self.community_detection,
                 seed=self.seed,
@@ -272,15 +273,15 @@
                                                           n_pcs=n_pcs,
                                                           n_comps=n_comps,
                                                           clustering_method=clustering_method,
                                                           n_neighbors=n_neighbors,
                                                           resolution=resolution,
                                                           n_clusters_kmeans=n_clusters_kmeans,
                                                           palette=palette
-                                                        )
+                                                          )
         self.in_situ_clustering.get_cluster_centroid(
             cluster_column_name=clustering_method,
             aggregation_mode="mean")
 
         if merge_cluster:
             self.in_situ_clustering.merge_cluster(nb_min_cluster=nb_min_cluster,
                                             min_merge_correlation=min_merge_correlation,
@@ -348,51 +349,74 @@
 
         return self
 
 
     ### Add and classify centroid
 
     def classify_centroid(self,
-                      path_dict_cell_centroid = None,
+                      path_cell_centroid = None,
                       n_neighbors=15,
                       dict_in_pixel=True,
                       max_dist_centroid=None,
                       key_pred="leiden_merged",
                       distance="ngb_distance_weights",
-                        file_extension = "tiff.npy"
-                      ):
+                      file_extension = "tiff.npy",
+                      centroid_csv_key = {"x": "x", "y": "y", "z": "z", "cell_index" : "cell"}
+                          ):
 
         """
         Classify cell centroids based on their  centroid neighbors RNA
         label from ``add_cluster_id_to_graph()``
 
 
-        :param path_dict_cell_centroid: If computed already by the ``ComSegDataset`` class from prior Maks leave it None. Otherwise :  Path to the folder containing the centroid dictionary {cell : {z:,y:,x:}}
-                        with each centroid dictionary in a file named as the image name and store in a npy format
+        :param path_dict_cell_centroid: If computed already by the ``ComSegDataset`` class from prior Maks leave it None.
+        Otherwise : path_dict_cell_centroid is a  Path to the folder containing the centroid dictionary {cell : {z:,y:,x:}} for each image.
+                         Each centroid dictionary has to be stored in a file in a npy format,  named as the image name.
         :type path_dict_cell_centroid: str
         :param n_neighbors: number of neighbors to consider for the classification of the centroid (default 15)
         :type n_neighbors: int
         :param dict_in_pixel: if True the centroid are in pixel and rescal if False the centroid are in um (default True)
         :type dict_in_pixel: bool
         :param max_dist_centroid: maximum distance to consider for the centroid (default None)
         :type max_dist_centroid: int
         :param key_pred: key of the node attribute containing the cluster id (default "leiden_merged")
         :type key_pred: str
         :param convex_hull_centroid: check that cell centroid is in the convex hull of its RNA neighbors (default True). If not the cell centroid is not classify to avoid artefact misclassification
         :type convex_hull_centroid: bool
         :param file_extension: file extension of the centroid dictionary
+        :type file_extension: str
+        :param centroid_csv_key: column name  of the centroid csv file
+        :type centroid_csv_key: dict
         :return:
         """
 
 
         for img_name in tqdm(self):
 
-            if path_dict_cell_centroid is not None:
-                dict_cell_centroid = np.load(Path(path_dict_cell_centroid) / (img_name + file_extension), allow_pickle=True).item()
+            if path_cell_centroid is not None:
+                assert self.dataset.dict_centroid is None, "The dict_centroid attribute of the dataset is not None. Please remove it or set it to None."
+                if str(file_extension)[-4:] == ".npy":
+                    dict_cell_centroid = np.load(Path(path_cell_centroid) / (img_name + file_extension), allow_pickle=True).item()
+                elif str(file_extension)[-4:] == ".csv":
+                    df_centroid = pd.read_csv(Path(path_cell_centroid) / (img_name + file_extension))
+                    x_list = list(df_centroid[centroid_csv_key["x"]])
+                    y_list = list(df_centroid["y"])
+                    if "z" in df_centroid.columns:
+                        z_list = list(df_centroid["z"])
+                    cell_list = list(df_centroid[centroid_csv_key["cell_index"]])
+                    if "z" in df_centroid.columns:
+                        dict_cell_centroid = {cell_list[i]:  np.array([ z_list[i], y_list[i], x_list[i]])
+                                                                      for i in range(len(cell_list))}
+                    else:
+                        dict_cell_centroid = {cell_list[i]: {"x": x_list[i], "y": y_list[i]} for i in range(len(cell_list))}
+                else:
+                    raise ValueError("The file extension of path_cell_centroid is not recognized. Please provide a .npy or .csv file")
             else:
+                if self.dataset.dict_centroid is None:
+                    raise ValueError("The dict_centroid attribute of the dataset is None.  Compute the centroid of the cells first. or provide a path to the centroid dataframe or dictionary {cell_index: {z:,y:,x:}} for each image.")
                 dict_cell_centroid = self.dataset.dict_centroid[img_name]
 
             self[img_name].classify_centroid(dict_cell_centroid,
                                              n_neighbors=n_neighbors,
                                              dict_in_pixel=dict_in_pixel,
                                              max_dist_centroid=max_dist_centroid,
                                              key_pred=key_pred,
@@ -401,15 +425,14 @@
 
 
     #### Apply diskjtra
 
 
     def associate_rna2landmark(self,
         key_pred="leiden_merged",
-        prior_name='in_nucleus',
         distance='distance',
         max_cell_radius=100):
         """
         Associate RNAs to landmarks based on the both transcriptomic landscape and the
         distance between the RNAs and the centroids of the landmark
 
 
@@ -423,45 +446,136 @@
 
         """
 
         for img_name in tqdm(self):
             print(img_name)
             self[img_name].associate_rna2landmark(
                 key_pred=key_pred,
-                prior_name=prior_name,
+                prior_name=self.prior_name,
                 distance=distance,
                 max_cell_radius=max_cell_radius)
 
     def anndata_from_comseg_result(self,
                                    key_cell_pred='cell_index_pred',
+                                   return_polygon=False,
+                                   alpha=0.5,
+                                   min_rna_per_cell=5
                                    ):
 
         """
         Return an anndata with the estimated expression vector of each cell in the dataset plus the spot positions.
 
         :param self:
         :param key_cell_pred: leave it to default
+        :type key_cell_pred: str
+        :param return_polygon: if True return the polygon of the cells
+        :type return_polygon: bool
+        :param alpha: alpha parameter to compute the alphashape polygone : https://pypi.org/project/alphashape/.
+         alpha is between 0 and 1, 1 correspond to the convex hull of the cell
+        :type alpha: float
+        :param min_rna_per_cell: minimum number of RNA to consider a cell
+        :type min_rna_per_cell: int
         :return:
         """
         list_image_name = []
         anndata_list = []
         dict_df_spots = {}
+        dict_json_img = {}
 
         for img_name in tqdm(self):
-            anndata = self[img_name].get_anndata_from_result(
-                key_cell_pred=key_cell_pred)
+            anndata, json_dict = self[img_name].get_anndata_from_result(
+                key_cell_pred=key_cell_pred,
+                return_polygon=return_polygon,
+                alpha=alpha,
+                min_rna_per_cell=min_rna_per_cell)
+            dict_json_img[img_name] = json_dict
 
             anndata_list.append(anndata)
             list_image_name += [img_name] * len(anndata)
             dict_df_spots[img_name] = anndata.uns["df_spots"]
 
             assert np.array_equal(anndata.var_names, self.dataset.selected_genes), "The anndata var names are not the same as the dataset selected genes"
 
 
 
         self.final_anndata = ad.concat(anndata_list)
         self.final_anndata.obs["image_name"] = list_image_name
         self.final_anndata.var["features"] = self.dataset.selected_genes
         self.final_anndata.var_names = self.dataset.selected_genes
         self.final_anndata.uns["df_spots"] = dict_df_spots
-        return self.final_anndata
+        return self.final_anndata, dict_json_img
+
+
+
+    def run_all(self,
+                max_cell_radius,
+                ## in situ clutering parameter
+                size_commu_min = 3,
+                norm_vector = False,
+                    ### parameter clustering
+                n_pcs = 3,
+                n_comps = 3,
+                clustering_method = "leiden",
+                n_neighbors = 20,
+                resolution = 1,
+                n_clusters_kmeans = 4,
+                palette = None,
+                nb_min_cluster = 0,
+                min_merge_correlation = 0.8,
+                ### classify centroid
+                path_dataset_folder_centroid=None,
+                file_extension=".csv"
+                ):
+        """
+        function running all the ComSeg steps: (compute_community_vector(),
+        compute_insitu_clustering(), add_cluster_id_to_graph(), classify_centroid(), associate_rna2landmark() )
+        :param max_cell_radius:
+        :param size_commu_min:
+        :param norm_vector:
+        :param n_pcs:
+        :param n_comps:
+        :param clustering_method:
+        :param n_neighbors:
+        :param resolution:
+        :param n_clusters_kmeans:
+        :param palette:
+        :param nb_min_cluster:
+        :param min_merge_correlation:
+        :param path_dataset_folder_centroid:
+        :param file_extension:
+        :return:
+        """
+
+        self.compute_community_vector()
+
+        self.compute_insitu_clustering(
+            size_commu_min=size_commu_min,
+            norm_vector=norm_vector,
+            ### parameter clustering
+            n_pcs=n_pcs,
+            n_comps=n_pcs,
+            clustering_method=clustering_method,
+            n_neighbors=n_neighbors,
+            resolution=resolution,
+            n_clusters_kmeans=n_clusters_kmeans,
+            palette=None,
+            nb_min_cluster=nb_min_cluster,
+            min_merge_correlation=min_merge_correlation,
+        )
+
+        self.add_cluster_id_to_graph(clustering_method="leiden_merged")
+
+        self.classify_centroid(
+            path_cell_centroid=path_dataset_folder_centroid,
+            n_neighbors=15,
+            dict_in_pixel=True,
+            max_dist_centroid=None,
+            key_pred="leiden_merged",
+            distance="ngb_distance_weights",
+            file_extension=file_extension
+        )
+
+        self.associate_rna2landmark(
+            key_pred="leiden_merged",
+            distance='distance',
+            max_cell_radius=max_cell_radius)
```

### Comparing `comseg-0.0.7/src/comseg/model.py` & `comseg-0.0.8/src/comseg/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 labeled community with the clustering classes
 add centroid from the dataset in the graph
 apply dikstra to compute the distance between the centroid and the other nodes
 return a count matrix of the image
 """
 
 
-
+import alphashape
 
 #%%
 
 from tqdm import tqdm
 import networkx as nx
 import scipy.sparse as sp
 
@@ -31,15 +31,15 @@
 from sklearn.utils.extmath import weighted_mode
 from scipy.spatial import ConvexHull, Delaunay
 from .utils import custom_louvain ## for dev mode
 
 
 __all__ = ["ComSegGraph"]
 
-
+import shapely
 def normal_dist(x , mean , sd):
     prob_density = (np.pi*sd) * np.exp(-0.5*((x-mean)/sd)**2)
     return prob_density
 
 
 class ComSegGraph():
 
@@ -60,14 +60,16 @@
                 df_spots_label,
                 selected_genes,
                  dict_co_expression,
                 dict_scale={"x": 0.103, 'y': 0.103, "z": 0.3},  # in micrometer
                 mean_cell_diameter=15,  # in micrometer
                 k_nearest_neighbors = 10,
                 edge_max_length = None,
+                gene_column = "gene",
+                 prior_name = "in_nucleus",
                  ):
 
 
 
         """
         :param df_spots_label: dataframe of the spots with column x,y,z, gene and optionally the prior label column
         :type df_spots_label: pd.DataFrame
@@ -96,14 +98,16 @@
         self.gene_index_dict = {}
         for gene_id in range(len(selected_genes)):
             self.gene_index_dict[selected_genes[gene_id]] = gene_id
         self.agg_sd =  1
         self.agg_max_dist = mean_cell_diameter/2
         self.dico_xyz_index = {"x": 2, "y":1, "z":0 }
         self.mean_cell_diameter = mean_cell_diameter
+        self.gene_column = gene_column
+        self.prior_name = prior_name
 
     ## create directed graph
 
     def create_graph(self):
         """
         create the graph of the RNA nodes, all the graph generation parameters are set in the __init__() function
 
@@ -121,15 +125,15 @@
             list_coordo_order = list_coordo_order_no_scaling * np.array([self.dict_scale['z'],
                                                                          self.dict_scale['y'],
                                                                          self.dict_scale["x"]])
         else:
             list_coordo_order_no_scaling = np.array([self.df_spots_label.x, self.df_spots_label.y]).T
             list_coordo_order = list_coordo_order_no_scaling * np.array([self.dict_scale['y'], self.dict_scale['x']])
         dico_list_features = {}
-        assert 'gene' in self.df_spots_label.columns, "the column gene is not in the dataframe"
+        assert self.gene_column in self.df_spots_label.columns, f"the column {self.gene_column} is not in the dataframe"
         for feature in self.df_spots_label.columns:
                 dico_list_features[feature] = list(self.df_spots_label[feature])
         list_features = list(dico_list_features.keys())
         list_features_order = [(i, {feature: dico_list_features[feature][i] for feature in list_features}) for i in range(len(self.df_spots_label))]
         dico_features_order = {}
         for node in range(len(list_features_order)):
             dico_features_order[node] = list_features_order[node][1]
@@ -149,16 +153,16 @@
         edges_list = list(zip(rows.tolist(), cols.tolist()))
         distance_list = [distance[rows[i], cols[i]] for i in range(len(cols))]
         G = nx.DiGraph()  # oriented graph
         list_features_order = [(k, dico_features_order[k]) for k in dico_features_order]
         G.add_nodes_from(list_features_order)
         for edges_index in range(len(edges_list)):
             edges = edges_list[edges_index]
-            gene_source = G.nodes[edges[0]]['gene']
-            gene_target = G.nodes[edges[1]]['gene']
+            gene_source = G.nodes[edges[0]][self.gene_column]
+            gene_target = G.nodes[edges[1]][self.gene_column]
             G.add_edge(edges[0], edges[1])
             weight = self.dict_co_expression[gene_source][gene_target]
             G[edges[0]][edges[1]]["weight"] = weight
             G[edges[0]][edges[1]]["distance"] = distance_list[edges_index]
             G[edges[0]][edges[1]]["gaussian"] = normal_dist(distance_list[edges_index], mean=0, sd =1)
 
         self.G = G
@@ -236,18 +240,18 @@
         list_coordinates = []
         list_node_index = []
         list_prior = []
 
 
         for index_commu in range(len(comm)):
             cluster_coordinate = []
-            expression_vector = np.bincount([self.gene_index_dict[self.G.nodes[ind_node]["gene"]] for ind_node in comm[index_commu]],
+            expression_vector = np.bincount([self.gene_index_dict[self.G.nodes[ind_node][self.gene_column]] for ind_node in comm[index_commu]],
                                             minlength = len(self.gene_index_dict))
             for node in comm[index_commu]:
-                if self.G.nodes[node]['gene'] == "centroid":
+                if self.G.nodes[node][self.gene_column] == "centroid":
                         continue
                 self.G.nodes[node]["index_commu"] =  index_commu
                 if "z" in self.G.nodes[0]:
                     cluster_coordinate.append([self.G.nodes[node]['x'],
                                                self.G.nodes[node]['y'],
                                                self.G.nodes[node]['z']])
                 else:
@@ -302,15 +306,15 @@
 
         list_index_commu = list(self.community_anndata.obs['index_commu'])
         dico_commu_cluster = {}
         for index_commu in dict_cluster_id:
             dico_commu_cluster[list_index_commu[index_commu]] = dict_cluster_id[index_commu]
         G = self.G
         for node in tqdm(G.nodes()):
-            if G.nodes[node]['gene'] == 'centroid':
+            if G.nodes[node][self.gene_column] == 'centroid':
                 continue
             G.nodes[node][clustering_method] = str(dico_commu_cluster[G.nodes[node]['index_commu']])
         self.G = G
 
 
 
     def _estimation_density_vec(self,
@@ -332,18 +336,18 @@
         if distance_weight_mode == "exp":
             list_nn = point_tree.query_ball_point(self.list_coordo_order, self.agg_max_dist )
         if distance_weight_mode == "linear":
             list_nn = point_tree.query_ball_point(self.list_coordo_order,self.edge_max_length)
         for node_index, node_data in self.G.nodes(data=True): ## create a kernel density estimation for each node
             if distance_weight_mode == "None":
                 nn_expression_vector = np.zeros(len(self.selected_genes))
-                nn_expression_vector[self.gene_index_dict[self.G.nodes[node_index]["gene"]]] = 1
+                nn_expression_vector[self.gene_index_dict[self.G.nodes[node_index][self.gene_column]]] = 1
                 self.G.nodes[node_index][key_word] = np.ones(len(self.selected_genes))
                 continue
-            if node_data["gene"] == 'centroid':
+            if node_data[self.gene_column] == 'centroid':
                 continue
             if remove_self_node:
                 list_nn[node_index].remove(node_index)
             list_nn_node_index = list_nn[node_index]
             array_distance = spatial.distance.cdist([self.list_coordo_order[node_index]],
                                                     self.list_coordo_order[list_nn_node_index],
                                                     'euclidean')
@@ -352,15 +356,15 @@
                 distance_weights = normal_dist(array_distance[0],
                                                     mean=0,
                                                     sd=self.agg_sd,
                                                     norm_gauss = norm_gauss)
             if distance_weight_mode == "linear":
                 distance_weights = (self.edge_max_length - array_distance[0]) / self.edge_max_length
             ## add code to remove centroid but there is no centroid in list coordo ?
-            nn_expression_vector = np.bincount([self.gene_index_dict[self.G.nodes[node_nn]["gene"]] for node_nn in list_nn_node_index],
+            nn_expression_vector = np.bincount([self.gene_index_dict[self.G.nodes[node_nn][self.gene_column]] for node_nn in list_nn_node_index],
                                                weights=distance_weights,
                                                minlength=len(self.gene_index_dict))
             self.G.nodes[node_index][key_word] = nn_expression_vector
         ## to factorize with community_nn_message_passing_agg
         list_expression_vectors = []
         for comm_index in range(len(self.community_anndata.obs["index_commu"])):
             nn_expression_vector = np.zeros(len(self.gene_index_dict))
@@ -394,20 +398,21 @@
         """
         for cell, centroid in dict_cell_centroid.items():
             centroid  = np.array(centroid)
             if centroid.ndim == 2:
                 centroid = np.mean(centroid, axis=0)
             assert centroid.ndim == 1
             self.G.add_node(len(self.G) -1 + int(cell),
-                            gene = "centroid",
+                           # gene = "centroid",
                             cell = cell,
                             in_nucleus = cell,
                             z = centroid[self.dico_xyz_index["z"]],
                             y = centroid[self.dico_xyz_index["y"]],
                             x = centroid[self.dico_xyz_index["x"]])
+            self.G.nodes[len(self.G.nodes)-1][self.gene_column] = "centroid"
             self.dict_cell_centroid = dict_cell_centroid
         return self.G
 
 
 
 
     ### add classify it
@@ -441,15 +446,14 @@
 
         self.dict_cell_centroid = dict_cell_centroid
 
         if max_dist_centroid is None:
             max_dist_centroid = self.mean_cell_diameter / 2
         nbrs = NearestNeighbors(n_neighbors=n_neighbors,
                                 algorithm='ball_tree').fit(self.list_coordo_order)
-
         if dict_in_pixel:
             list_coordo_order_nuc_centroid_no_scaling = []
             list_coordo_order_nuc_centroid = []
             for nuc in self.dict_cell_centroid:
                 if len(self.dict_cell_centroid[nuc]) == 1:
                     centroid_pix = np.array(self.dict_cell_centroid[nuc][0]) ## to clean, in case of old version of dict
                 else:
@@ -488,15 +492,15 @@
 
             dico_nuclei_centroid[nuc]["type_list"] = []
             dico_nuclei_centroid[nuc]["gr_type_list"] = []
             dico_nuclei_centroid[nuc]["ngb_distance"] = []
             dico_nuclei_centroid[nuc]["ngb_gr_cell"] = []
             dico_nuclei_centroid[nuc]["ngb_distance_weights"] = []
             dico_nuclei_centroid[nuc]["gaussian"] = []
-            dico_nuclei_centroid[nuc]["gene"] = "centroid"
+            dico_nuclei_centroid[nuc][self.gene_column] = "centroid"
             dico_nuclei_centroid[nuc]["cell"] = nuc
             dico_nuclei_centroid[nuc]["in_nucleus"] = nuc
             dico_nuclei_centroid[nuc]["index_commu_in_nucleus"] = nuc
             type_list = []
             array_index_nn = np.nonzero(ad_nuc_centroid[nuc_index].toarray())[1]
             index_type_list = []
             for index_nn_centroid in array_index_nn:
@@ -522,15 +526,15 @@
 
         ### add new attribute to node centroid
 
             node_index = len(self.list_coordo_order) - 1 + nuc
             self.G.add_nodes_from([(node_index, dico_nuclei_centroid[nuc])])
             for ii in array_index_nn:
                 self.G.add_edge(node_index, ii)
-                if nuc == self.G.nodes[ii]['in_nucleus']:
+                if nuc == self.G.nodes[ii][self.prior_name]:
                     self.G.add_edge(node_index, ii, distance = 0)
                 else:
                     self.G.add_edge(node_index, ii, distance = distance_nuc_centroid[nuc_index, ii])
 
         return self.G
 
 
@@ -569,14 +573,15 @@
             distance=distance,
             max_cell_radius=max_cell_radius,
         )
         for super_node_index in G_merge.nodes():
             set_super_nodes = G_merge.nodes[super_node_index]['nodes']
             for simple_nodes in set_super_nodes:
                 self.G.nodes[simple_nodes]["cell_index_pred"] = G_merge.nodes[super_node_index]["cell_index_pred"]
+                self.G.nodes[simple_nodes]["distance2centroid"] = G_merge.nodes[super_node_index]["distance2centroid"]
         return self.G
 
     def _associate_rna2landmark(self,
             G,
             distance='distance',
             max_cell_radius=100,  ## in theunit of the graph distance ie um
     ):
@@ -619,15 +624,15 @@
                 if len(set(centroid_list).intersection(cc)) == 1:
                     nucleus_node = list(set(centroid_list).intersection(cc))[0]
                     length, path = nx.single_source_dijkstra(G.subgraph(cc).to_undirected(),
                                                              nucleus_node,
                                                              weight=distance,
                                                              cutoff=max_cell_radius)
 
-                    dico_expression_m[nucleus_node] = list(length.keys())
+                    dico_expression_m[nucleus_node] = [[node,length[node]] for node in length.keys()]
                     find += len(list(length.keys()))
                 if len(set(centroid_list).intersection(cc)) > 1:
                     # break
                     list_nuclei = list(set(centroid_list).intersection(cc))
                     dico_length = {}  # {centroid : length list}
                     dico_shortest_path = {}
                     # print(f'list_nuclei len  {len(list_nuclei)}')
@@ -648,30 +653,32 @@
                             if node in dico_length[nucleus_node]:
                                 dico_nodes_centroid_distance[node][nucleus_node] = dico_length[nucleus_node][node]
                     for node in cc:
                         try:
                             if len(dico_nodes_centroid_distance[node]) > 0:
                                 nearest_c = min(dico_nodes_centroid_distance[node],
                                                 key=dico_nodes_centroid_distance[node].get)
-                                dico_expression_m[nearest_c].append(node)
+                                distance2centroid = dico_nodes_centroid_distance[node][nearest_c]
+                                dico_expression_m[nearest_c].append((node, distance2centroid))
                                 find += 1
-                            # farest = list(set(list_nuclei) - set([nearest_c]))[0]
-                            # if node not in [nearest_c,farest ]:
-                            #    assert nx.shortest_path_length(G.subgraph(cc).to_undirected(), source=farest, target=node,weight =  "distance")
-                            #    >= nx.shortest_path_length(G.subgraph(cc).to_undirected(), source=nearest_c, target=node,weight =  "distance")
                         except ValueError as e:
                             print(e)
                             raise ValueError(f"node {node} not find in dikjtra")
         ## add new_label to the grpa
         for node_all in G.nodes():
             G.nodes[node_all]["cell_index_pred"] = 0
+            G.nodes[node_all]["distance2centroid"] = np.inf
         for centroid in dico_expression_m:
             nuc_index = G.nodes[centroid]["super_node_prior_key"]
-            for node in dico_expression_m[centroid]:
+            for value_exp in dico_expression_m[centroid]:
+                node = value_exp[0]
+                distance2centroid = value_exp[1]
                 G.nodes[node]["cell_index_pred"] = nuc_index
+                G.nodes[node]["distance2centroid"] = distance2centroid
+
         return G, dico_expression_m
 
 
 
     ##### generate an anndata from the graph
 
     #### return an anndata with expresion vector
@@ -679,91 +686,177 @@
     # list of rna spots coordinate |
     # list of the corresponding rna species
     #
 
     def get_anndata_from_result(
                 self,
                key_cell_pred =  'cell_index_pred',
+                return_polygon = False,
+                alpha = 0.5,
+                min_rna_per_cell = 5,
+                allow_disconnected_polygone = False
                ):
         """
         Generate an anndata storing the estimated expression vector and their spots coordinates
 
         :param key_cell_pred:  key of the cell prediction in the graph (default cell_index_pred)
         :type key_cell_pred: str
+        :param return_polygon: if True return the polygon of the cells
+        :type return_polygon: bool
+        :param alpha: alpha parameter to compute the alphashape polygone : https://pypi.org/project/alphashape/.
+         alpha is between 0 and 1, 1 correspond to the convex hull of the cell
+        :type alpha: float
+        :param min_rna_per_cell: minimum number of RNA to consider a cell
+        :type min_rna_per_cell: int
+        :param allow_disconnected_polygone: if True allow disconnected polygon
         :return:
         """
 
         dict_cell_genes = {}
         dict_cell_genes_coordinate = {}
         dict_cell_genes_name = {}
         dict_cell_genes_mol_index = {}
-        list_cell_centroid = []
+        dict_cell_dist2centroid= {}
+
         for cell in self.dict_cell_centroid:
             dict_cell_genes[cell] = []
             dict_cell_genes_coordinate[cell] = []
             dict_cell_genes_name[cell] = []
             dict_cell_genes_mol_index[cell] = []
-            centroid = self.dict_cell_centroid[cell]
-            centroid  = np.array(centroid)
-            if centroid.ndim == 2:
-                centroid = np.mean(centroid, axis=0)
-            list_cell_centroid += [tuple(centroid)]
+            dict_cell_dist2centroid[cell] = []
+
         for node_index, node_data in self.G.nodes(data = True):
-            if node_data['gene'] != 'centroid' and node_data[key_cell_pred] != 0:
-                dict_cell_genes[node_data[key_cell_pred]].append(node_data['gene'])
-                dict_cell_genes_coordinate[node_data[key_cell_pred]].append([node_data["z"],
-                                                         node_data['y'],
-                                                         node_data['x']])
+            if node_data[self.gene_column] != 'centroid' and node_data[key_cell_pred] != 0:
+                if node_data[key_cell_pred] in dict_cell_genes: ## check that the centroid is indeed in the crop and not only the prior
+                    dict_cell_genes[node_data[key_cell_pred]].append(node_data[self.gene_column])
+                    dict_cell_genes_coordinate[node_data[key_cell_pred]].append([node_data["z"],
+                                                             node_data['y'],
+                                                             node_data['x']])
+                    dict_cell_dist2centroid[node_data[key_cell_pred]].append(node_data["distance2centroid"])
+                    dict_cell_genes_mol_index[node_data[key_cell_pred]].append(node_data['index'])
 
-                dict_cell_genes_mol_index[node_data[key_cell_pred]].append(node_data['index'])
 
         list_expression_vectors = []
         list_cell_id = []
         list_cell_genes_coordinate = []
         list_genes_name = []
         list_gene_index  = []
+        list_cell_centroid = []
+        list_gene_dist2centroid = []
         for cell in dict_cell_genes:
             expression_vector = np.bincount(
                 [self.gene_index_dict[gene] for gene in dict_cell_genes[cell]]
                         , minlength=len(self.gene_index_dict))
+            if np.sum(expression_vector) < min_rna_per_cell:
+                continue
             list_expression_vectors.append(expression_vector)
             list_cell_id.append(cell)
             list_cell_genes_coordinate.append(
                 np.array(dict_cell_genes_coordinate[cell])
             )
             list_genes_name.append(dict_cell_genes[cell])
-
             list_gene_index.append(dict_cell_genes_mol_index[cell])
+            list_gene_dist2centroid.append(dict_cell_dist2centroid[cell])
+            centroid = self.dict_cell_centroid[cell]
+            centroid  = np.array(centroid)
+            if centroid.ndim == 2:
+                centroid = np.mean(centroid, axis=0)
+            list_cell_centroid += [tuple(centroid)]
 
         anndata = ad.AnnData(np.array(list_expression_vectors))
         anndata.var["features"] = self.selected_genes
         anndata.var_names = self.selected_genes
-        anndata.obs["cell_id"] = list_cell_id
-        anndata.obs["centroid"] = list_cell_centroid
+        anndata.var["Name"] = self.selected_genes
+        #
+        random_string = str(np.random.randint(0, 10000))
+
+        anndata.obs["CellID"] = list_cell_id
+        anndata.obs["Name"] = [random_string+ "_" + str(i) for i in list_cell_id]
+        anndata.obs.index = [random_string+ "_" + str(i) for i in list_cell_id]
+        anndata.obs_names = [random_string+ "_" + str(i) for i in list_cell_id]
+        if len(list_cell_centroid[0]) == 2:
+            x_list_centroid = [x[1] for x in list_cell_centroid]
+            y_list_centroid = [x[0] for x in list_cell_centroid]
+            anndata.obs["centroid_y"] = y_list_centroid
+            anndata.obs["centroid_x"] = x_list_centroid
+        else:
+            assert len(list_cell_centroid[0]) == 3
+            x_list_centroid = [x[2] for x in list_cell_centroid]
+            y_list_centroid = [x[1] for x in list_cell_centroid]
+            z_list_centroid = [x[0] for x in list_cell_centroid]
+            anndata.obs["centroid_z"] = z_list_centroid
+            anndata.obs["centroid_y"] = y_list_centroid
+            anndata.obs["centroid_x"] = x_list_centroid
+
         #anndata.obs["spots_coordinates"] = np.array(list_cell_genes_coordinate)
         #anndata.obs["genes"] = np.array(list_genes_name)
 
         ### create csv file
-        csv_list_z = []
-        csv_list_y = []
-        csv_list_x = []
-        csv_list_gene = []
-        csv_list_cell = []
-        csv_index_list = []
+        column_name = list(self.G.nodes[list(self.G.nodes)[0]].keys())
+        if "kernel_vector" in column_name:
+            column_name.remove("kernel_vector")
+        dict_dataframe = {}
+        for column in column_name:
+            dict_dataframe[column] = []
+        for node_index, node_data in self.G.nodes(data = True):
+            if node_data[self.gene_column] != 'centroid':
+                for column in column_name:
+                    dict_dataframe[column].append(node_data[column])
+        df_spots = pd.DataFrame(dict_dataframe)
+
+        ## rename colum index by original index node
+        df_spots.rename(columns = {"index" : "node_index"}, inplace = True)
+
+        anndata.uns["df_spots"] = df_spots
+        self.final_anndata = anndata
+
+        if not return_polygon:
+            return anndata, {}
+        assert min_rna_per_cell > 0, "min_rna_per_cell should be > 0"
+
+        list_polygon = []
+        dict_polygon = {}
         for cell_index in range(len(list_cell_id)):
-            if len(list_genes_name[cell_index]) > 0:
-                csv_list_z += list(np.array(list_cell_genes_coordinate[cell_index])[:, 0])
+            csv_list_y = []
+            csv_list_x = []
+            if len(list_genes_name[cell_index]) >= min_rna_per_cell:
                 csv_list_y += list(np.array(list_cell_genes_coordinate[cell_index])[:, 1])
                 csv_list_x += list(np.array(list_cell_genes_coordinate[cell_index])[:, 2])
-                csv_list_cell += [list_cell_id[cell_index]] * len(list_genes_name[cell_index])
-                csv_list_gene += list_genes_name[cell_index]
-                csv_index_list += list(dict_cell_genes_mol_index[list_cell_id[cell_index]])
-
-        df_spots = pd.DataFrame({"z": csv_list_z,
-                                 "y": csv_list_y,
-                                 "x": csv_list_x,
-                                 "gene": csv_list_gene,
-                                 "cell": csv_list_cell,
-                                 "original_index" : csv_index_list})
-
-        anndata.uns["df_spots"] = df_spots
-        return anndata
+                list_point = list(zip(csv_list_x, csv_list_y))
+                alpha_shape = alphashape.alphashape(list_point, alpha)
+                list_polygon.append(alpha_shape)
+                dict_polygon[list_cell_id[cell_index]] = alpha_shape
+
+        ### ensure that there is no overlap between the polygons of list_polygon
+        for i in tqdm(list(range(len(list_polygon)))):
+            for j in range(i+1, len(list_polygon)):
+                if list_polygon[i].intersects(list_polygon[j]):
+                    list_polygon[i] = list_polygon[i].difference(list_polygon[j])
+        list_keys = list(dict_polygon.keys())
+        for i in range(len(list_keys)):
+            dict_polygon[list_keys[i]] = list_polygon[i]
+        self.list_polygon = list_polygon
+        self.dict_polygon = dict_polygon
+
+        ## Create the json
+        json_dict = {"geometries": []}
+        for cell in dict_polygon:
+            geometry = dict_polygon[cell]
+            if isinstance(geometry, shapely.geometry.Polygon):
+                json_dict["geometries"].append({
+                    "type": "Polygon",
+                    "coordinates": [list(geometry.exterior.coords)],
+                    "cell": cell
+                })
+            elif isinstance(geometry, shapely.geometry.MultiPolygon):
+                for poly in list(geometry.geoms):
+                    if allow_disconnected_polygone:
+                        json_dict["geometries"].append({
+                            "type": "Polygon",
+                            "coordinates": [list(poly.exterior.coords)],
+                            "cell": cell
+                        })
+                    else:
+                        raise ValueError("disconnected polygon are not allowed change allow_disconnected_polygon=True")
+            else:
+                continue
+        return anndata, json_dict
```

### Comparing `comseg-0.0.7/src/comseg/utils/custom_louvain.py` & `comseg-0.0.8/src/comseg/utils/custom_louvain.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,31 +235,32 @@
     #print(len(partition))
     improvement = True
     while improvement:
         new_mod = modularity(
             graph, inner_partition, resolution=resolution, weight="weight"
         )
         graph = _gen_graph(graph, partition = inner_partition)
-        if new_mod - mod <= threshold:
-            print(f'stop because of threshold {new_mod - mod} inf to {threshold}')
-            return
-        print(f'improvement of modularity {new_mod - mod}')
-        mod = new_mod
         yield [s.copy() for s in partition], graph
 
-        partition, inner_partition, improvement = _one_level(
-            graph=graph,
-            m=m,
-            partition=partition,
-            resolution=resolution,
-            is_directed=is_directed,
-            seed=seed,
-            confidence_level=confidence_level,
-            prior_key="prior_index", ## harcoded prior key name from _gen_graph
-        )
+        if new_mod - mod <= threshold:
+            print(f'stop because of improvement of modularity {new_mod - mod}  below  the threshold  {threshold}')
+            improvement = False
+        else:
+            print(f'improvement of modularity {new_mod - mod}')
+            mod = new_mod
+            partition, inner_partition, improvement = _one_level(
+                graph=graph,
+                m=m,
+                partition=partition,
+                resolution=resolution,
+                is_directed=is_directed,
+                seed=seed,
+                confidence_level=confidence_level,
+                prior_key="prior_index", ## harcoded prior key name from _gen_graph
+            )
         #print(len(partition))
 
 
 def compute_prior_factor(source, ind_node, confidence_level = 0.99):
 
     if confidence_level is None:
         return 1
```

### Comparing `comseg-0.0.7/src/comseg/utils/plot.py` & `comseg-0.0.8/src/comseg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.7/src/comseg/utils/preprocessing.py` & `comseg-0.0.8/src/comseg/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.7/src/comseg/utils/utils_graph.py` & `comseg-0.0.8/src/comseg/utils/utils_graph.py`

 * *Files identical despite different names*

