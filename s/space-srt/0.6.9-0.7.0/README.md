# Comparing `tmp/space-srt-0.6.9.tar.gz` & `tmp/space_srt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-srt-0.6.9.tar", last modified: Sun Oct 15 11:35:26 2023, max compression
+gzip compressed data, was "space_srt-0.7.0.tar", last modified: Tue May 28 08:23:19 2024, max compression
```

## Comparing `space-srt-0.6.9.tar` & `space_srt-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-10-15 11:35:26.829364 space-srt-0.6.9/
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     1065 2023-10-12 07:49:56.000000 space-srt-0.6.9/LICENSE
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     1697 2023-10-15 11:35:26.829364 space-srt-0.6.9/PKG-INFO
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)      696 2023-10-12 07:49:56.000000 space-srt-0.6.9/README.md
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     1002 2023-10-15 11:33:52.000000 space-srt-0.6.9/pyproject.toml
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)       38 2023-10-15 11:35:26.829364 space-srt-0.6.9/setup.cfg
-drwxr-xr-x   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-10-15 11:35:26.829364 space-srt-0.6.9/src/
-drwxr-xr-x   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-10-15 11:35:26.829364 space-srt-0.6.9/src/space/
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)      110 2023-10-15 11:33:24.000000 space-srt-0.6.9/src/space/__init__.py
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     7034 2023-10-12 07:50:10.000000 space-srt-0.6.9/src/space/function.py
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     3189 2023-10-12 07:50:10.000000 space-srt-0.6.9/src/space/layer.py
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     4839 2023-10-12 07:50:10.000000 space-srt-0.6.9/src/space/model.py
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     8604 2023-10-12 07:50:10.000000 space-srt-0.6.9/src/space/train.py
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)    11214 2023-10-15 11:33:16.000000 space-srt-0.6.9/src/space/utils.py
-drwxr-xr-x   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-10-15 11:35:26.829364 space-srt-0.6.9/src/space_srt.egg-info/
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)     1697 2023-10-15 11:35:26.000000 space-srt-0.6.9/src/space_srt.egg-info/PKG-INFO
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)      346 2023-10-15 11:35:26.000000 space-srt-0.6.9/src/space_srt.egg-info/SOURCES.txt
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)        1 2023-10-15 11:35:26.000000 space-srt-0.6.9/src/space_srt.egg-info/dependency_links.txt
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)      114 2023-10-15 11:35:26.000000 space-srt-0.6.9/src/space_srt.egg-info/requires.txt
--rw-r--r--   0 liyuzhe   (7189) zhangqflab  (9018)        6 2023-10-15 11:35:26.000000 space-srt-0.6.9/src/space_srt.egg-info/top_level.txt
+drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2024-05-28 08:23:19.475661 space_srt-0.7.0/
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     1065 2024-04-25 01:53:43.000000 space_srt-0.7.0/LICENSE
+-rw-r--r--   0 liyuzhe    (501) staff       (20)     2250 2024-05-28 08:23:19.475561 space_srt-0.7.0/PKG-INFO
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     1247 2024-04-25 01:53:43.000000 space_srt-0.7.0/README.md
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     1004 2024-05-28 08:13:18.000000 space_srt-0.7.0/pyproject.toml
+-rw-r--r--   0 liyuzhe    (501) staff       (20)       38 2024-05-28 08:23:19.475857 space_srt-0.7.0/setup.cfg
+drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2024-05-28 08:23:19.471956 space_srt-0.7.0/src/
+drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2024-05-28 08:23:19.474287 space_srt-0.7.0/src/space/
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)      110 2024-05-28 08:14:12.000000 space_srt-0.7.0/src/space/__init__.py
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     6306 2024-04-25 01:53:43.000000 space_srt-0.7.0/src/space/function.py
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     2241 2024-04-25 01:53:43.000000 space_srt-0.7.0/src/space/layer.py
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     2642 2024-04-25 01:53:43.000000 space_srt-0.7.0/src/space/model.py
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)     5781 2024-04-25 01:53:43.000000 space_srt-0.7.0/src/space/train.py
+-rw-rw-r--   0 liyuzhe    (501) staff       (20)    15123 2024-04-25 01:53:43.000000 space_srt-0.7.0/src/space/utils.py
+drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2024-05-28 08:23:19.475340 space_srt-0.7.0/src/space_srt.egg-info/
+-rw-r--r--   0 liyuzhe    (501) staff       (20)     2250 2024-05-28 08:23:19.000000 space_srt-0.7.0/src/space_srt.egg-info/PKG-INFO
+-rw-r--r--   0 liyuzhe    (501) staff       (20)      346 2024-05-28 08:23:19.000000 space_srt-0.7.0/src/space_srt.egg-info/SOURCES.txt
+-rw-r--r--   0 liyuzhe    (501) staff       (20)        1 2024-05-28 08:23:19.000000 space_srt-0.7.0/src/space_srt.egg-info/dependency_links.txt
+-rw-r--r--   0 liyuzhe    (501) staff       (20)      114 2024-05-28 08:23:19.000000 space_srt-0.7.0/src/space_srt.egg-info/requires.txt
+-rw-r--r--   0 liyuzhe    (501) staff       (20)        6 2024-05-28 08:23:19.000000 space_srt-0.7.0/src/space_srt.egg-info/top_level.txt
```

### Comparing `space-srt-0.6.9/LICENSE` & `space_srt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `space-srt-0.6.9/pyproject.toml` & `space_srt-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=42.0","wheel","build","packaging","tomli"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "space-srt"
-version = "0.6.9"
+version = "0.7.0"
 authors = [
   { name="Yuzhe Li", email="liyuzhezju@gmail.com" },
 ]
 description = "SPatial transcriptomics Analysis via Cell Embedding"
 readme = "README.md"
-requires-python = ">3.6.0"
+requires-python = ">3.7.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     'Development Status :: 4 - Beta',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
@@ -33,9 +33,9 @@
     "matplotlib",
     "leidenalg",
     "squidpy",
     "networkx"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/ericli0419/SPACE"
-"Bug Tracker" = "https://github.com/ericli0419/SPACE/issues"
+"Homepage" = "https://github.com/zhangqf-lab/SPACE"
+"Bug Tracker" = "https://github.com/zhangqf-lab/SPACE/issues"
```

### Comparing `space-srt-0.6.9/src/space/function.py` & `space_srt-0.7.0/src/space/function.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from sklearn.preprocessing import MaxAbsScaler
 
 import torch
 import torch_geometric
 import torch_geometric.transforms as T
 from torch_geometric.data import Data
 
-from .layer import GAT_Encoder, GCN_Encoder
-from .model import SPACE_Graph, SPACE_Graph_GCN
-from .train import train_SPACE, train_SPACE_GCN 
+from .layer import GAT_Encoder
+from .model import SPACE_Graph
+from .train import train_SPACE
 from .utils import graph_construction
 
 
 
-def SPACE(adata,k=20,graph_const_method='SPACE',encoder_type='GAT',alpha=0.5,beta=10,seed=42,GPU=0,epoch=5000,lr=0.005,patience=50,outdir='./',loss_type='MSE',save_attn=False,verbose=False,heads=6):
+def SPACE(adata,k=20,graph_const_method='SPACE',alpha=0.5,seed=42,GPU=0,epoch=5000,lr=0.005,patience=50,outdir='./',loss_type='MSE',save_attn=False,verbose=False,heads=6):
     """
     Single-Cell integrative Analysis via Latent feature Extraction
     
     Parameters
     ----------
     adata
         An AnnData Object with spot/cell x gene matrix stored.
@@ -114,58 +114,47 @@
 
     transform = T.RandomLinkSplit(num_val=0.0, num_test=0.0, is_undirected=True, 
                                   add_negative_train_samples=False, split_labels=True)
     train_data, _ , _ = transform(data_obj) 
     num_features = data_obj.num_features
     
     print('Load SPACE model')
-    if encoder_type=='GAT':
-        encoder = GAT_Encoder(
-            in_channels=num_features,
-            num_heads={'first':heads,'second':heads,'mean':heads},
-            hidden_dims=[128,128],
-            dropout=[0.3,0.3],
-            concat={'first': True, 'second': True})
-        model = SPACE_Graph(encoder= encoder,decoder=None,loss_type=loss_type)
-        print(model) 
-        print('Train SPACE model')
-        device=train_SPACE(model, train_data, epoch=epoch, lr=lr, patience=patience, GPU=GPU, seed=seed, a=alpha,b=beta,loss_type=loss_type, outdir= outdir, verbose=verbose)
-    elif encoder_type=='GCN':
-        encoder = GCN_Encoder(
-            in_channels=num_features,
-            hidden_dims=[128,32])
-        model = SPACE_Graph_GCN(encoder= encoder,decoder=None,loss_type=loss_type)
-        print(model) 
-        print('Train SPACE model')
-        device=train_SPACE_GCN(model, train_data, epoch=epoch, lr=lr, patience=patience, GPU=GPU, seed=seed, a=alpha,b=beta,loss_type=loss_type, outdir= outdir, verbose=verbose)
+    encoder = GAT_Encoder(
+        in_channels=num_features,
+        num_heads={'first':heads,'second':heads,'mean':heads},
+        hidden_dims=[128,128],
+        dropout=[0.3,0.3],
+        concat={'first': True, 'second': True})
+    model = SPACE_Graph(encoder= encoder,decoder=None,loss_type=loss_type)
+    print(model) 
+    print('Train SPACE model')
+    
+    device=train_SPACE(model, train_data, epoch=epoch, lr=lr, patience=patience, GPU=GPU, seed=seed, a=alpha,loss_type=loss_type, outdir= outdir, verbose=verbose)
     
     # Load model
     pretrained_dict = torch.load(os.path.join(outdir,'model.pt'), map_location=device)                            
     model_dict = model.state_dict()
     pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
     model_dict.update(pretrained_dict) 
     model.load_state_dict(model_dict)
     model = model.eval()
 
     node_embeddings = []
     x, edge_index = data_obj.x.to(torch.float).to(device), data_obj.edge_index.to(torch.long).to(device)
-    if encoder_type=='GAT':
-        z_nodes, attn_w = model.encode(x, edge_index)
-    elif encoder_type=='GCN':
-        z_nodes = model.encode(x, edge_index)
+    z_nodes, attn_w = model.encode(x, edge_index)
     node_embeddings.append(z_nodes.cpu().detach().numpy()) 
     node_embeddings = np.array(node_embeddings) 
     node_embeddings = node_embeddings.squeeze()
 
     adata.obsm['latent']=node_embeddings 
     sc.pp.neighbors(adata, n_neighbors=20, n_pcs=10,use_rep='latent',random_state=seed,key_added='SPACE') 
     sc.tl.umap(adata,random_state=seed, neighbors_key='SPACE')
     
     # Save attention weights
-    if save_attn and encoder_type=='GAT':
+    if save_attn:
         for i in range(2):
             edge_index, attention_weights = attn_w[i]
             edge_index, attention_weights = edge_index.detach().cpu(), attention_weights.detach().cpu()
             
             layer_filename = f'GAT_Layer_{i+1}_edge_index.pt'
             edges_filepath = os.path.join(outdir, layer_filename)
             layer_filename = f'GAT_Layer_{i+1}_attention_weights.pt'
```

### Comparing `space-srt-0.6.9/src/space/layer.py` & `space_srt-0.7.0/src/space/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Fri Mar 11 19:58:54 2022
 
 @author: liyuzhe
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from torch_geometric.nn import GATv2Conv, GCNConv
+from torch_geometric.nn import GATv2Conv
 
 
 
 class GAT_Encoder(nn.Module):
     def __init__(self, in_channels,num_heads, hidden_dims, dropout, concat):
         super(GAT_Encoder, self).__init__()
         
@@ -55,32 +55,8 @@
     """Decoder for using inner product for prediction."""
     def __init__(self,act=torch.relu):
         super(InnerProduct, self).__init__()
         self.act = act
 
     def forward(self, z):
         recon_a = self.act(torch.mm(z, z.t()))
-        return recon_a 
-
-
-class GCN_Encoder(nn.Module):
-    def __init__(self, in_channels,hidden_dims):
-        super(GCN_Encoder, self).__init__()
-
-        self.in_channels = in_channels
-        self.latent_dim = 10
-        self.conv = GCNConv
-
-        self.hidden_layer1 = self.conv(in_channels=in_channels, out_channels=hidden_dims[0])
-        self.hidden_layer2 = self.conv(in_channels=hidden_dims[0], out_channels=hidden_dims[1])
-        self.conv_z = self.conv(in_channels=hidden_dims[1], out_channels=self.latent_dim)
-
-    def forward(self, x, edge_index):
-        hidden_out1 = self.hidden_layer1(x, edge_index)
-        hidden_out1 = F.leaky_relu(hidden_out1)
-        hidden_out2 = self.hidden_layer2(hidden_out1, edge_index)
-        hidden_out2 = F.leaky_relu(hidden_out2)
-        hidden_out2 = F.dropout(hidden_out2, p=0.4, training=self.training)
-        last_out = hidden_out2
-        z = self.conv_z(last_out, edge_index)
-       
-        return z 
+        return recon_a
```

### Comparing `space-srt-0.6.9/src/space/model.py` & `space_srt-0.7.0/src/space/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -52,71 +52,17 @@
         pos_edge_index, _ = remove_self_loops(pos_edge_index)
         pos_edge_index, _ = add_self_loops(pos_edge_index)
         if neg_edge_index is None:
             neg_edge_index = negative_sampling(pos_edge_index, z.size(0))
         neg_loss = -torch.log(1 - self.decoder(z, neg_edge_index, sigmoid=True) + EPS).mean()
 
         return pos_loss + neg_loss
-
-     
-    def load_model(self, path):
-
-        pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)                            
-        model_dict = self.state_dict()
-        pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
-        model_dict.update(pretrained_dict) 
-        self.load_state_dict(model_dict)
-
-
-
-class SPACE_Graph_GCN(GAE):
-    def __init__(self, encoder, decoder,loss_type='MSE'):
-        super(SPACE_Graph_GCN, self).__init__(encoder, decoder)
-        seed_everything(seed)
-        self.decoder = InnerProductDecoder()
-        
-        if loss_type == 'BCE':
-            self.decoder_x = Sequential(Linear(in_features=self.encoder.latent_dim, out_features=128),
-                                      BatchNorm1d(128),
-                                      LeakyReLU(),
-                                      Dropout(0.1),
-                                      Linear(in_features=128, out_features=self.encoder.in_channels),
-                                      Sigmoid())
-        else:
-            self.decoder_x = Sequential(Linear(in_features=self.encoder.latent_dim, out_features=128),
-                                      BatchNorm1d(128),
-                                      LeakyReLU(),
-                                      Dropout(0.1),
-                                      Linear(in_features=128, out_features=self.encoder.in_channels),
-                                      ReLU())
-
     
-    def encode(self, *args, **kwargs):
-        
-        z = self.encoder(*args, **kwargs)
-        
-        return z
-
-
-    def graph_loss(self, z, pos_edge_index, neg_edge_index=None):
-
-        self.decoded = self.decoder(z, pos_edge_index, sigmoid=True)
-        pos_loss = -torch.log(self.decoded + EPS).mean()
-
-        # Do not include self-loops in negative samples
-        pos_edge_index, _ = remove_self_loops(pos_edge_index)
-        pos_edge_index, _ = add_self_loops(pos_edge_index)
-        if neg_edge_index is None:
-            neg_edge_index = negative_sampling(pos_edge_index, z.size(0))
-        neg_loss = -torch.log(1 - self.decoder(z, neg_edge_index, sigmoid=True) + EPS).mean()
-
-        return pos_loss + neg_loss
-
      
     def load_model(self, path):
 
         pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)                            
         model_dict = self.state_dict()
         pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
         model_dict.update(pretrained_dict) 
         self.load_state_dict(model_dict)
-
+
```

### Comparing `space-srt-0.6.9/src/space/utils.py` & `space_srt-0.7.0/src/space/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,111 @@
 @author: liyuzhe
 """
 import os
 import scanpy as sc
 import numpy as np
 import scipy as sci
 from scipy.spatial import distance
-from sklearn.preprocessing import MaxAbsScaler
 import networkx as nx
 import torch
 import torch_geometric
 import torch_geometric.transforms as T
 from torch_geometric.data import Data
 from torch_scatter import scatter_mean,scatter_sum
 from .layer import GAT_Encoder
 from .model import SPACE_Graph
 
 
+def celltype_connectivity(adata,domain_key= 'Label',celltype_key = 'cluster',nboot=100, outdir='./data'):
+    import holoviews as hv
+    import squidpy as sq
+    import pandas as pd
+    from tqdm import tqdm
+    import random
+
+    random.seed(42)
+    os.makedirs(outdir, exist_ok=True)
+
+    sq.gr.spatial_neighbors(adata, n_neighs = 20, coord_type = 'generic') 
+
+    for label in adata.obs[domain_key].unique():
+        # CCI
+        adata_batch = adata[adata.obs[domain_key] == label].copy()  
+        cell_types = adata_batch.obs[celltype_key].unique().tolist()
+        sq.gr.interaction_matrix(adata_batch, cluster_key=celltype_key)
+        CCI1=adata_batch.uns['{}_interactions'.format(celltype_key)].copy()
+        CCI2=CCI1.T.copy()
+        CCI=((CCI1+CCI2)/2).round()
+        pairwise_connection=pd.DataFrame(CCI,
+                                         index=adata_batch.obs[celltype_key].cat.categories,
+                                         columns=adata_batch.obs[celltype_key].cat.categories)
+        
+        pairwise_connection[pairwise_connection<=0]=1e-10
+        
+        
+        df_p=pd.DataFrame(columns=['celltype1','celltype2','p'])
+        for i in range(0,len(cell_types)):
+            for j in range(i,len(cell_types)):
+                df_p=df_p.append(pd.DataFrame({'celltype1':cell_types[i],
+                                               'celltype2':cell_types[j],
+                                               'p':[0]}),ignore_index=True)
+        
+        # permutation
+        for j in range(nboot):
+            adata_p=adata_batch.copy()
+            celltype_p=list(adata_batch.obs[celltype_key].values.copy())
+            random.shuffle(celltype_p)
+            adata_p.obs[celltype_key]=celltype_p
+            adata_p.obs[celltype_key]=adata_p.obs[celltype_key].astype('category')
+            
+            sq.gr.interaction_matrix(adata_p, cluster_key=celltype_key)
+            CCI1=adata_p.uns['{}_interactions'.format(celltype_key)].copy()
+            CCI2=CCI1.T.copy()
+            CCI=((CCI1+CCI2)/2).round()
+            pairwise_connection_p = pd.DataFrame(CCI,
+                                                 index=adata_p.obs[celltype_key].cat.categories,
+                                                 columns=adata_p.obs[celltype_key].cat.categories)
+            pairwise_connection_p[pairwise_connection_p<=0]=1e-10
+            
+            
+            pairwise_connection_d=pairwise_connection_p-pairwise_connection
+            for i in df_p.index:
+                idx1=df_p.loc[i,'celltype1']
+                idx2=df_p.loc[i,'celltype2']
+                if pairwise_connection_d.loc[idx1,idx2]>=0:
+                    df_p.loc[i,'p']=df_p.loc[i,'p']+1
+            
+        df_p['p']=df_p['p']/nboot
+        
+        # save data
+        celltype_sum=pd.DataFrame(adata_batch.obs[celltype_key].value_counts())
+        celltype_sub=celltype_sum[celltype_sum[celltype_key]>=10].copy()
+        df=pairwise_connection.loc[celltype_sum.index,celltype_sum.index].copy()
+        
+        df.to_csv(os.path.join(outdir,'{}_prob.csv'.format(label)))
+        celltype_sub.to_csv(os.path.join(outdir,'{}_size.csv'.format(label)))
+        
+        # from statsmodels.stats.multitest import fdrcorrection
+        # df_p['p_adj']=fdrcorrection(df_p['p'])[1]
+        
+        df_p_m=pd.DataFrame(index=celltype_sum.index,columns=celltype_sum.index)
+        for i in df_p.index:
+            idx1=df_p.loc[i,'celltype1']
+            idx2=df_p.loc[i,'celltype2']
+            df_p_m.loc[idx1,idx2]=df_p.loc[i,'p']
+            df_p_m.loc[idx2,idx1]=df_p.loc[i,'p']
+            # df_p_m.loc[idx1,idx2]=df_p.loc[i,'p_adj']
+            # df_p_m.loc[idx2,idx1]=df_p.loc[i,'p_adj']
+        df_p_m = df_p_m.fillna(1)
+        df_p_m[df_p_m==0]=1e-10
+        df_p.to_csv(os.path.join(outdir,'{}_p.csv'.format(label)),index=None)
+        df_p_m.to_csv(os.path.join(outdir,'{}_prob_p.csv'.format(label)))
+           
+    return adata
+
 
 def mad_gap(x, edge_index):
 
     #eq 1-2 masked cos similarity
     with torch.no_grad():
         dij = torch.cosine_similarity(x[edge_index[0]], x[edge_index[1]], dim=1, eps=1e-8)
         dij = 1 - dij
```

