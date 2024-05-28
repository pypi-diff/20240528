# Comparing `tmp/SC2Spa-1.2.3.tar.gz` & `tmp/sc2spa-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.2.3.tar", last modified: Mon Jul 31 16:11:30 2023, max compression
+gzip compressed data, was "sc2spa-1.2.4.tar", last modified: Tue May 28 00:48:18 2024, max compression
```

## Comparing `SC2Spa-1.2.3.tar` & `sc2spa-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 16:11:30.172350 SC2Spa-1.2.3/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 16:11:30.171897 SC2Spa-1.2.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 16:11:30.166515 SC2Spa-1.2.3/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.3/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-31 15:59:27.000000 SC2Spa-1.2.3/SC2Spa/__metadata__.py
--rwxrwxrwx   0 root         (0) root         (0)    20204 2023-07-31 16:09:26.000000 SC2Spa-1.2.3/SC2Spa/bm.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.3/SC2Spa/me.py
--rwxrwxrwx   0 root         (0) root         (0)    23478 2023-07-31 15:48:59.000000 SC2Spa-1.2.3/SC2Spa/pl.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.3/SC2Spa/pp.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-07-31 15:59:25.000000 SC2Spa-1.2.3/SC2Spa/sva.py
--rwxrwxrwx   0 root         (0) root         (0)    51128 2023-07-31 16:09:26.000000 SC2Spa-1.2.3/SC2Spa/tl.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 16:11:30.170931 SC2Spa-1.2.3/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 16:11:30.000000 SC2Spa-1.2.3/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      273 2023-07-31 16:11:30.000000 SC2Spa-1.2.3/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-31 16:11:30.000000 SC2Spa-1.2.3/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-31 16:11:30.000000 SC2Spa-1.2.3/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-31 16:10:29.000000 SC2Spa-1.2.3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-31 16:11:30.172542 SC2Spa-1.2.3/setup.cfg
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1525 2024-05-28 00:26:30.000000 sc2spa-1.2.4/LICENSE
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 00:48:18.503921 sc2spa-1.2.4/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1229 2024-05-28 00:26:30.000000 sc2spa-1.2.4/README.md
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/SC2Spa/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      211 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/__init__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      460 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/__metadata__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    20205 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/bm.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     8248 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/me.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    23478 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/pl.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3062 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/pp.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     4381 2024-05-28 00:26:30.000000 sc2spa-1.2.4/SC2Spa/sva.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    51301 2024-05-28 00:46:44.000000 sc2spa-1.2.4/SC2Spa/tl.py
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/SC2Spa.egg-info/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      317 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/SOURCES.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        1 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/dependency_links.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        7 2024-05-28 00:48:18.000000 sc2spa-1.2.4/SC2Spa.egg-info/top_level.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      691 2024-05-28 00:37:12.000000 sc2spa-1.2.4/pyproject.toml
+-rw-r--r--   0 linbu     (1000) linbu     (1000)       38 2024-05-28 00:48:18.503921 sc2spa-1.2.4/setup.cfg
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 00:48:18.503921 sc2spa-1.2.4/tests/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3122 2024-05-28 00:26:31.000000 sc2spa-1.2.4/tests/test_loading.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3545 2024-05-28 00:26:31.000000 sc2spa-1.2.4/tests/test_mapping.py
```

### Comparing `SC2Spa-1.2.3/LICENSE` & `sc2spa-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.3/PKG-INFO` & `sc2spa-1.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.3
+Version: 1.2.4
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -19,18 +19,27 @@
 ====================================================================================
 
 <p align="center">
   <img src="./SC2Spa.png" alt="SC2Spa Overview" width="600"/>
 </p>
 
 ## Install
-Install SC2Spa via PyPI by running:
+Install SC2Spa:
 ```
+conda create -n SC2Spa python=3.9
+conda activate SC2Spa
 pip install SC2Spa
 ```
 
 ## Analysis for the SC2Spa manuscript
-The analysis for the SC2Spa manuscript can be found [here](https://github.com/linbuliao/SC2Spa_Notebooks)
-
+The analysis for the SC2Spa manuscript can be found in [this repository](https://github.com/linbuliao/SC2Spa_Notebooks).
+The analysis and related data were also uploaded to [Figshare](https://figshare.com/articles/dataset/Datasets_for_high_resolution_spatial_mapping_of_mouse_hippocampus_Slide-seqV2_for_SC2Spa/21829905/8) and [Zenodo](https://zenodo.org/records/8252715).
 
 ## Many more to come!
 We will update more on our [Read the Docs page](https://sc2spa.readthedocs.io/en/latest/)
+
+## News
+
+__2023/08/22__
+
+SC2Spa is now on BioRXiv!
+https://www.biorxiv.org/content/10.1101/2023.08.22.554277v1
```

### Comparing `SC2Spa-1.2.3/README.md` & `sc2spa-1.2.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,18 +5,27 @@
 ====================================================================================
 
 <p align="center">
   <img src="./SC2Spa.png" alt="SC2Spa Overview" width="600"/>
 </p>
 
 ## Install
-Install SC2Spa via PyPI by running:
+Install SC2Spa:
 ```
+conda create -n SC2Spa python=3.9
+conda activate SC2Spa
 pip install SC2Spa
 ```
 
 ## Analysis for the SC2Spa manuscript
-The analysis for the SC2Spa manuscript can be found [here](https://github.com/linbuliao/SC2Spa_Notebooks)
-
+The analysis for the SC2Spa manuscript can be found in [this repository](https://github.com/linbuliao/SC2Spa_Notebooks).
+The analysis and related data were also uploaded to [Figshare](https://figshare.com/articles/dataset/Datasets_for_high_resolution_spatial_mapping_of_mouse_hippocampus_Slide-seqV2_for_SC2Spa/21829905/8) and [Zenodo](https://zenodo.org/records/8252715).
 
 ## Many more to come!
 We will update more on our [Read the Docs page](https://sc2spa.readthedocs.io/en/latest/)
+
+## News
+
+__2023/08/22__
+
+SC2Spa is now on BioRXiv!
+https://www.biorxiv.org/content/10.1101/2023.08.22.554277v1
```

### Comparing `SC2Spa-1.2.3/SC2Spa/bm.py` & `sc2spa-1.2.4/SC2Spa/bm.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 n_col = 2
 
 
 def BVMI(adata1: anndata.AnnData, adata2: anndata.AnnData,
          GL: list, coords_name = 'spatial', n_neighbors=300, max_dis=1700):
 
     '''
-    Calculate bivariate Moran's I of the genes of two ST data
+    Calculate bivariate Moran's I of the genes of two ST data.
 
     The two ST datasets share some or all ST voxels/cells
 
     Parameters
     ---------
     adata1
         a anndata object.
```

### Comparing `SC2Spa-1.2.3/SC2Spa/me.py` & `sc2spa-1.2.4/SC2Spa/me.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.3/SC2Spa/pl.py` & `sc2spa-1.2.4/SC2Spa/pl.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.3/SC2Spa/pp.py` & `sc2spa-1.2.4/SC2Spa/pp.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.3/SC2Spa/sva.py` & `sc2spa-1.2.4/SC2Spa/sva.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.3/SC2Spa/tl.py` & `sc2spa-1.2.4/SC2Spa/tl.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 from sklearn.neighbors import NearestNeighbors
 from scipy.stats import wasserstein_distance
 
 import tensorflow as tf
 from keras.models import Model, load_model
 from keras.regularizers import l1_l2
-from keras.layers import Dense, Input, BatchNormalization, Dropout
+from keras.layers import Dense, Input, LayerNormalization, ReLU, Dropout
 from keras.callbacks import ReduceLROnPlateau, EarlyStopping
 
 from IPython.display import clear_output
 
 import keras.backend as K
 from . import pp
 
 def rmse(y_true, y_pred):
     return K.sqrt(K.mean(K.square(y_pred - y_true), axis=-1))
 def calc_rmse(y_true, y_pred):
     return np.sqrt(np.square(y_true - y_pred).mean())
 
-loss = rmse
-loss_name = 'rmse'
+#loss = rmse
+#loss_name = 'rmse'
 
 def FCNN(input_shape: tuple, out_shape: int,l1_reg = 1e-7, l2_reg = 0,
 	     dropout = 0, nodes = [4096, 1024, 256, 64, 16, 4], seed = None):
     '''
     Construct a fully connected neural network
 
     Parameters
@@ -52,16 +52,17 @@
     
     X_input = Input(input_shape)    
     X = X_input
     
     for node in nodes:
         X = Dropout(rate = dropout, seed = seed)(X)
         X = Dense(node, kernel_initializer = tf.keras.initializers.GlorotNormal(seed = seed),
-                  activation = 'relu', kernel_regularizer = l1_l2(l1_reg, l2_reg))(X)
-        X = BatchNormalization(axis = 1)(X)
+                  activation = None, kernel_regularizer = l1_l2(l1_reg, l2_reg))(X)
+        X = LayerNormalization(axis = 1)(X)
+        X = ReLU()(X)
     
     X = Dense(out_shape, kernel_initializer = tf.keras.initializers.GlorotNormal(seed = seed),
               activation = 'sigmoid')(X)
     
     model = Model(inputs = X_input, outputs = X, name = 'FCNN')
     
     return model
@@ -195,15 +196,15 @@
         gc.collect()
     
     return histories, train_preds, test_preds
 
 def Train(X, Y, root='Model_SI/', name = 'SI', 
 	      l1_reg = 1e-5, l2_reg = 0, dropout = 0.05,
           epoch = 500, batch_size = 4096,
-          nodes = [4096, 1024, 256, 64, 16, 4], lrr_patience = 20,
+          nodes = [4096, 1024, 256, 64, 16, 4], loss = 'mse', loss_name = 'mse', lrr_patience = 20,
           ES_patience = 50, min_lr = 1e-5, save = True, seed = None):
     '''
     Train a fully connected neural network.
     The model will be saved to `root+name+'.h5'`
 
     Parameters
     ----------
@@ -359,16 +360,16 @@
     Y_ref
         reference spatial coordinates
     '''
 
     # Select genes
     if(JGs == None):
         if (WD_cutoff == None):
-            adata_ref.var_names = adata_ref.var_names.str.upper()
-            adata_query.var_names = adata_query.var_names.str.upper()
+            #adata_ref.var_names = adata_ref.var_names.str.upper()
+            #adata_query.var_names = adata_query.var_names.str.upper()
 
             adata_ref.var_names_make_unique()
             adata_query.var_names_make_unique()
 
             JGs = sorted(list(set(adata_ref.var_names).intersection(set(adata_query.var_names))))
         else:
             JGs, WDs = WassersteinD(adata_ref, adata_query, WD_cutoff, sparse)
@@ -731,15 +732,16 @@
 
         adata_query.obs.loc[temp, 'Recon_scST'] = True
         adata_query.obs.loc[temp, 'Recon_scST_layer'] = layer
 
 def FineMapping(adata_ref, adata_query, sparse = True, model_path = None, WD_cutoff = None, JGs = None,
                 root = 'Model_SI/', name = 'SI', l1_reg = 1e-5, l2_reg = 0, dropout = 0.05, epoch = 500,
                 batch_size = 4096, nodes = [4096, 1024, 256, 64, 16, 4], lrr_patience = 20, ES_patience = 50,
-                min_lr = 1e-5, save = True, polar = True, FM = True, n_layer_cell = [1, 4],
+                min_lr = 1e-5, save = True, loss = 'mse', loss_name = 'mse', polar = True, FM = True,
+                n_layer_cell = [1, 4],
                 cell_radius = 5, n_neighbors = 1000, dis_cutoff = 15, seed = 2023):
 
     '''
     Finely map single cells to spatial locations and Reconstruct ST data at single cell resolution
 
     1. Finely map single cells to spatial locations.
     A model will be trained and saved to `root+name+'.h5'` if model_path is None and save is True.
@@ -815,15 +817,16 @@
     else:
         Y = pp.MinMaxNorm(Y_ref, Y_ref)
 
     if(model_path != None):
         model = load_model(model_path, compile=False)
     else:
         model = Train(X=X_ref, Y=Y, root = root, name = name, l1_reg = l1_reg, l2_reg = l2_reg,
-                      dropout = dropout, epoch = epoch, batch_size = batch_size, nodes = nodes,
+                      dropout = dropout, epoch = epoch, loss = loss, loss_name = loss_name,
+                      batch_size = batch_size, nodes = nodes,
                       lrr_patience = lrr_patience, ES_patience = ES_patience, min_lr = min_lr,
                       save = save, seed = seed)
     Query_pred_Y = BatchPredict(model, X_query)
     Ref_pred_Y = BatchPredict(model, X_ref)
     if(polar):
         Query_pred_Y = pp.RePolarTrans(pp.ReMMNorm(RTheta_ref, Query_pred_Y))
         Ref_pred_Y = pp.RePolarTrans(pp.ReMMNorm(RTheta_ref, Ref_pred_Y))
```

### Comparing `SC2Spa-1.2.3/SC2Spa.egg-info/PKG-INFO` & `sc2spa-1.2.4/SC2Spa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.3
+Version: 1.2.4
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -19,18 +19,27 @@
 ====================================================================================
 
 <p align="center">
   <img src="./SC2Spa.png" alt="SC2Spa Overview" width="600"/>
 </p>
 
 ## Install
-Install SC2Spa via PyPI by running:
+Install SC2Spa:
 ```
+conda create -n SC2Spa python=3.9
+conda activate SC2Spa
 pip install SC2Spa
 ```
 
 ## Analysis for the SC2Spa manuscript
-The analysis for the SC2Spa manuscript can be found [here](https://github.com/linbuliao/SC2Spa_Notebooks)
-
+The analysis for the SC2Spa manuscript can be found in [this repository](https://github.com/linbuliao/SC2Spa_Notebooks).
+The analysis and related data were also uploaded to [Figshare](https://figshare.com/articles/dataset/Datasets_for_high_resolution_spatial_mapping_of_mouse_hippocampus_Slide-seqV2_for_SC2Spa/21829905/8) and [Zenodo](https://zenodo.org/records/8252715).
 
 ## Many more to come!
 We will update more on our [Read the Docs page](https://sc2spa.readthedocs.io/en/latest/)
+
+## News
+
+__2023/08/22__
+
+SC2Spa is now on BioRXiv!
+https://www.biorxiv.org/content/10.1101/2023.08.22.554277v1
```

### Comparing `SC2Spa-1.2.3/pyproject.toml` & `sc2spa-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

