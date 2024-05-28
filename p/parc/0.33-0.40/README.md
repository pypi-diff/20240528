# Comparing `tmp/parc-0.33.tar.gz` & `tmp/parc-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parc-0.33.tar", last modified: Tue Feb  8 00:34:39 2022, max compression
+gzip compressed data, was "parc-0.40.tar", last modified: Tue May 28 02:20:18 2024, max compression
```

## Comparing `parc-0.33.tar` & `parc-0.40.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2022-02-08 00:34:39.000000 parc-0.33/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     6529 2022-02-08 00:34:39.000000 parc-0.33/PKG-INFO
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     5155 2019-09-24 06:45:27.000000 parc-0.33/README.md
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2022-02-08 00:34:39.000000 parc-0.33/parc/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       24 2019-09-24 01:48:33.000000 parc-0.33/parc/__init__.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    33769 2022-01-25 12:43:51.000000 parc-0.33/parc/_parc.py
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     6529 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/PKG-INFO
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      188 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/SOURCES.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        1 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/dependency_links.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       71 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/requires.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        5 2022-02-08 00:34:39.000000 parc-0.33/parc.egg-info/top_level.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       38 2022-02-08 00:34:39.000000 parc-0.33/setup.cfg
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      655 2022-02-08 00:32:28.000000 parc-0.33/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 02:20:18.239540 parc-0.40/
+-rw-rw-r--   0 user      (1000) user      (1000)    12998 2024-05-28 02:20:18.239540 parc-0.40/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    12788 2024-05-28 02:11:34.000000 parc-0.40/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 02:20:18.239540 parc-0.40/parc/
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-05-28 02:08:44.000000 parc-0.40/parc/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    34401 2024-05-28 02:08:49.000000 parc-0.40/parc/_parc.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 02:20:18.239540 parc-0.40/parc.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    12998 2024-05-28 02:20:18.000000 parc-0.40/parc.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      188 2024-05-28 02:20:18.000000 parc-0.40/parc.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-28 02:20:18.000000 parc-0.40/parc.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2024-05-28 02:20:18.000000 parc-0.40/parc.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2024-05-28 02:20:18.000000 parc-0.40/parc.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-28 02:20:18.239540 parc-0.40/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      750 2024-05-28 02:18:01.000000 parc-0.40/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `parc-0.33/parc/_parc.py` & `parc-0.40/parc/_parc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-
-
 import numpy as np
 import pandas as pd
 import hnswlib
 from scipy.sparse import csr_matrix
 import igraph as ig
 import leidenalg
 import time
-import umap
+from umap.umap_ import find_ab_params, simplicial_set_embedding
 
 
-# latest github upload 26-June-2020
+#latest github upload 27-June-2020
 class PARC:
     def __init__(self, data, true_label=None, dist_std_local=3, jac_std_global='median', keep_all_local_dist='auto',
                  too_big_factor=0.4, small_pop=10, jac_weighted_edges=True, knn=30, n_iter_leiden=5, random_seed=42,
-                 num_threads=-1, distance='l2', time_smallpop=15, partition_type="ModularityVP",
-                 resolution_parameter=1.0,
-                 knn_struct=None, neighbor_graph=None, hnsw_param_ef_construction=150):
+                 num_threads=-1, distance='l2', time_smallpop=15, partition_type = "ModularityVP", resolution_parameter = 1.0,
+                 knn_struct=None, neighbor_graph=None, hnsw_param_ef_construction = 150):
         # higher dist_std_local means more edges are kept
         # highter jac_std_global means more edges are kept
         if keep_all_local_dist == 'auto':
             if data.shape[0] > 300000:
                 keep_all_local_dist = True  # skips local pruning to increase speed
             else:
                 keep_all_local_dist = False
-        if resolution_parameter != 1:
-            partition_type = "RBVP"  # Reichardt and Bornholdt’s Potts model. Note that this is the same as ModularityVertexPartition when setting 𝛾 = 1 and normalising by 2m
+        if resolution_parameter !=1:
+            partition_type = "RBVP" # Reichardt and Bornholdt’s Potts model. Note that this is the same as ModularityVertexPartition when setting 𝛾 = 1 and normalising by 2m
         self.data = data
         self.true_label = true_label
-        self.dist_std_local = dist_std_local  # similar to the jac_std_global parameter. avoid setting local and global pruning to both be below 0.5 as this is very aggresive pruning.
-        self.jac_std_global = jac_std_global  # 0.15 is also a recommended value performing empirically similar to 'median'. Generally values between 0-1.5 are reasonable.
-        self.keep_all_local_dist = keep_all_local_dist  # decides whether or not to do local pruning. default is 'auto' which omits LOCAL pruning for samples >300,000 cells.
-        self.too_big_factor = too_big_factor  # if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster. at 0.4 it does not come into play
+        self.dist_std_local = dist_std_local   # similar to the jac_std_global parameter. avoid setting local and global pruning to both be below 0.5 as this is very aggresive pruning.
+        self.jac_std_global = jac_std_global  #0.15 is also a recommended value performing empirically similar to 'median'. Generally values between 0-1.5 are reasonable.
+        self.keep_all_local_dist = keep_all_local_dist #decides whether or not to do local pruning. default is 'auto' which omits LOCAL pruning for samples >300,000 cells.
+        self.too_big_factor = too_big_factor  #if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster. at 0.4 it does not come into play
         self.small_pop = small_pop  # smallest cluster population to be considered a community
-        self.jac_weighted_edges = jac_weighted_edges  # boolean. whether to partition using weighted graph
+        self.jac_weighted_edges = jac_weighted_edges #boolean. whether to partition using weighted graph
         self.knn = knn
-        self.n_iter_leiden = n_iter_leiden  # the default is 5 in PARC
+        self.n_iter_leiden = n_iter_leiden #the default is 5 in PARC
         self.random_seed = random_seed  # enable reproducible Leiden clustering
         self.num_threads = num_threads  # number of threads used in KNN search/construction
         self.distance = distance  # Euclidean distance 'l2' by default; other options 'ip' and 'cosine'
-        self.time_smallpop = time_smallpop  # number of seconds trying to check an outlier
-        self.partition_type = partition_type  # default is the simple ModularityVertexPartition where resolution_parameter =1. In order to change resolution_parameter, we switch to RBConfigurationVP
-        self.resolution_parameter = resolution_parameter  # defaults to 1. expose this parameter in leidenalg
-        self.knn_struct = knn_struct  # the hnsw index of the KNN graph on which we perform queries
-        self.neighbor_graph = neighbor_graph  # CSR affinity matrix for pre-computed nearest neighbors
-        self.hnsw_param_ef_construction = hnsw_param_ef_construction  # set at 150. higher value increases accuracy of index construction. Even for several 100,000s of cells 150-200 is adequate
+        self.time_smallpop = time_smallpop #number of seconds trying to check an outlier
+        self.partition_type = partition_type #default is the simple ModularityVertexPartition where resolution_parameter =1. In order to change resolution_parameter, we switch to RBConfigurationVP
+        self.resolution_parameter = resolution_parameter # defaults to 1. expose this parameter in leidenalg
+        self.knn_struct = knn_struct #the hnsw index of the KNN graph on which we perform queries
+        self.neighbor_graph = neighbor_graph # CSR affinity matrix for pre-computed nearest neighbors
+        self.hnsw_param_ef_construction = hnsw_param_ef_construction #set at 150. higher value increases accuracy of index construction. Even for several 100,000s of cells 150-200 is adequate
 
     def make_knn_struct(self, too_big=False, big_cluster=None):
         if self.knn > 190: print('consider using a lower K_in for KNN graph construction')
         ef_query = max(100, self.knn + 1)  # ef always should be >K. higher ef, more accurate query
         if too_big == False:
             num_dims = self.data.shape[1]
             n_elements = self.data.shape[0]
             p = hnswlib.Index(space=self.distance, dim=num_dims)  # default to Euclidean distance
             p.set_num_threads(self.num_threads)  # allow user to set threads used in KNN construction
             if n_elements < 10000:
                 ef_query = min(n_elements - 10, 500)
                 ef_construction = ef_query
             else:
                 ef_construction = self.hnsw_param_ef_construction
-            if (num_dims > 30) & (n_elements <= 50000):
+            if (num_dims > 30) & (n_elements<=50000) :
                 p.init_index(max_elements=n_elements, ef_construction=ef_construction,
                              M=48)  ## good for scRNA seq where dimensionality is high
             else:
-                p.init_index(max_elements=n_elements, ef_construction=ef_construction, M=24)  # 30
+                p.init_index(max_elements=n_elements, ef_construction=ef_construction, M=24 ) #30
             p.add_items(self.data)
         if too_big == True:
             num_dims = big_cluster.shape[1]
             n_elements = big_cluster.shape[0]
             p = hnswlib.Index(space='l2', dim=num_dims)
             p.init_index(max_elements=n_elements, ef_construction=200, M=30)
             p.add_items(big_cluster)
         p.set_ef(ef_query)  # ef should always be > k
 
         return p
 
-    def knngraph_full(self):  # , neighbor_array, distance_array):
+    def knngraph_full(self):#, neighbor_array, distance_array):
         k_umap = 15
-        t0 = time.time()
+        t0= time.time()
         # neighbors in array are not listed in in any order of proximity
-        self.knn_struct.set_ef(k_umap + 1)
+        self.knn_struct.set_ef(k_umap+1)
         neighbor_array, distance_array = self.knn_struct.knn_query(self.data, k=k_umap)
 
         row_list = []
         n_neighbors = neighbor_array.shape[1]
         n_cells = neighbor_array.shape[0]
 
         row_list.extend(list(np.transpose(np.ones((n_neighbors, n_cells)) * range(0, n_cells)).flatten()))
 
+
         row_min = np.min(distance_array, axis=1)
         row_sigma = np.std(distance_array, axis=1)
 
-        distance_array = (distance_array - row_min[:, np.newaxis]) / row_sigma[:, np.newaxis]
+        distance_array = (distance_array - row_min[:,np.newaxis])/row_sigma[:,np.newaxis]
 
         col_list = neighbor_array.flatten().tolist()
         distance_array = distance_array.flatten()
         distance_array = np.sqrt(distance_array)
         distance_array = distance_array * -1
 
         weight_list = np.exp(distance_array)
 
-        threshold = np.mean(weight_list) + 2 * np.std(weight_list)
+
+        threshold = np.mean(weight_list) + 2* np.std(weight_list)
 
         weight_list[weight_list >= threshold] = threshold
 
         weight_list = weight_list.tolist()
 
+
         graph = csr_matrix((np.array(weight_list), (np.array(row_list), np.array(col_list))),
                            shape=(n_cells, n_cells))
 
         graph_transpose = graph.T
         prod_matrix = graph.multiply(graph_transpose)
 
         graph = graph_transpose + graph - prod_matrix
@@ -138,15 +138,15 @@
                 discard_count = discard_count + (n_neighbors - len(to_keep))
 
                 for ik in range(len(updated_nn_ind)):
                     if rowi != row[ik]:  # remove self-loops
                         row_list.append(rowi)
                         col_list.append(updated_nn_ind[ik])
                         dist = np.sqrt(updated_nn_weights[ik])
-                        weight_list.append(1 / (dist + 0.1))
+                        weight_list.append(1/(dist+0.1))
 
                 rowi = rowi + 1
 
         if self.keep_all_local_dist == True:  # dont prune based on distance
             row_list.extend(list(np.transpose(np.ones((n_neighbors, n_cells)) * range(0, n_cells)).flatten()))
             col_list = neighbor_array.flatten().tolist()
             weight_list = (1. / (distance_array.flatten() + 0.1)).tolist()
@@ -169,18 +169,17 @@
         else:
             knnbig = int(max(5, 0.2 * n_elements))
 
         neighbor_array, distance_array = hnsw.knn_query(X_data, k=knnbig)
         # print('shapes of neigh and dist array', neighbor_array.shape, distance_array.shape)
         csr_array = self.make_csrmatrix_noselfloop(neighbor_array, distance_array)
         sources, targets = csr_array.nonzero()
-
         #mask = np.zeros(len(sources), dtype=bool)
 
-        #mask |= (csr_array.data > (        np.mean(csr_array.data) + np.std(csr_array.data) * 5))  # weights are set as 1/dist. so smaller distance means stronger edge
+        #mask |= (csr_array.data < (np.mean(csr_array.data) - np.std(csr_array.data) * 5))  # weights are 1/dist so bigger weight means closer nodes
 
         #csr_array.data[mask] = 0
         #csr_array.eliminate_zeros()
         #sources, targets = csr_array.nonzero()
         edgelist = list(zip(sources.tolist(), targets.tolist()))
         edgelist_copy = edgelist.copy()
         G = ig.Graph(edgelist, edge_attrs={'weight': csr_array.data.tolist()})
@@ -200,50 +199,49 @@
 
         if jac_weighted_edges == True:
             G_sim = ig.Graph(n=n_elements, edges=list(new_edgelist), edge_attrs={'weight': sim_list_new})
         else:
             G_sim = ig.Graph(n=n_elements, edges=list(new_edgelist))
         G_sim.simplify(combine_edges='sum')
         if jac_weighted_edges == True:
-            if self.partition_type == 'ModularityVP':
+            if self.partition_type =='ModularityVP':
                 partition = leidenalg.find_partition(G_sim, leidenalg.ModularityVertexPartition, weights='weight',
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed)
+                                                 n_iterations=self.n_iter_leiden, seed=self.random_seed)
                 print('partition type MVP')
             else:
                 partition = leidenalg.find_partition(G_sim, leidenalg.RBConfigurationVertexPartition, weights='weight',
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed,
-                                                     resolution_parameter=self.resolution_parameter)
+                                                 n_iterations=self.n_iter_leiden, seed=self.random_seed, resolution_parameter=self.resolution_parameter)
                 print('partition type RBC')
         else:
             if self.partition_type == 'ModularityVP':
                 print('partition type MVP')
                 partition = leidenalg.find_partition(G_sim, leidenalg.ModularityVertexPartition,
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed)
+                                                 n_iterations=self.n_iter_leiden, seed=self.random_seed)
             else:
                 print('partition type RBC')
                 partition = leidenalg.find_partition(G_sim, leidenalg.RBConfigurationVertexPartition,
                                                      n_iterations=self.n_iter_leiden, seed=self.random_seed,
                                                      resolution_parameter=self.resolution_parameter)
         # print('Q= %.2f' % partition.quality())
         PARC_labels_leiden = np.asarray(partition.membership)
         PARC_labels_leiden = np.reshape(PARC_labels_leiden, (n_elements, 1))
         small_pop_list = []
         small_cluster_list = []
         small_pop_exist = False
         dummy, PARC_labels_leiden = np.unique(list(PARC_labels_leiden.flatten()), return_inverse=True)
         for cluster in set(PARC_labels_leiden):
             population = len(np.where(PARC_labels_leiden == cluster)[0])
-            if population < 10:
+            if population < small_pop:
                 small_pop_exist = True
                 small_pop_list.append(list(np.where(PARC_labels_leiden == cluster)[0]))
                 small_cluster_list.append(cluster)
 
         for small_cluster in small_pop_list:
             for single_cell in small_cluster:
-                old_neighbors = neighbor_array[single_cell]
+                old_neighbors = neighbor_array[single_cell, :]
                 group_of_old_neighbors = PARC_labels_leiden[old_neighbors]
                 group_of_old_neighbors = list(group_of_old_neighbors.flatten())
                 available_neighbours = set(group_of_old_neighbors) - set(small_cluster_list)
                 if len(available_neighbours) > 0:
                     available_neighbours_list = [value for value in group_of_old_neighbors if
                                                  value in list(available_neighbours)]
                     best_group = max(available_neighbours_list, key=available_neighbours_list.count)
@@ -252,15 +250,15 @@
         time_smallpop_start = time.time()
         print('handling fragments')
         while (small_pop_exist) == True & (time.time() - time_smallpop_start < self.time_smallpop):
             small_pop_list = []
             small_pop_exist = False
             for cluster in set(list(PARC_labels_leiden.flatten())):
                 population = len(np.where(PARC_labels_leiden == cluster)[0])
-                if population < 10:
+                if population < small_pop:
                     small_pop_exist = True
 
                     small_pop_list.append(np.where(PARC_labels_leiden == cluster)[0])
             for small_cluster in small_pop_list:
                 for single_cell in small_cluster:
                     old_neighbors = neighbor_array[single_cell, :]
                     group_of_old_neighbors = PARC_labels_leiden[old_neighbors]
@@ -270,22 +268,24 @@
 
         dummy, PARC_labels_leiden = np.unique(list(PARC_labels_leiden.flatten()), return_inverse=True)
 
         return PARC_labels_leiden
 
     def run_subPARC(self):
 
+
         X_data = self.data
         too_big_factor = self.too_big_factor
         small_pop = self.small_pop
         jac_std_global = self.jac_std_global
         jac_weighted_edges = self.jac_weighted_edges
         knn = self.knn
         n_elements = X_data.shape[0]
 
+
         if self.neighbor_graph is not None:
             csr_array = self.neighbor_graph
             neighbor_array = np.split(csr_array.indices, csr_array.indptr)[1:-1]
         else:
             if self.knn_struct is None:
                 print('knn struct was not available, so making one')
                 self.knn_struct = self.make_knn_struct()
@@ -322,34 +322,32 @@
         G_sim = ig.Graph(n=n_elements, edges=list(new_edgelist), edge_attrs={'weight': sim_list_new})
         # print('average degree of graph is %.1f' % (np.mean(G_sim.degree())))
         G_sim.simplify(combine_edges='sum')  # "first"
         # print('average degree of SIMPLE graph is %.1f' % (np.mean(G_sim.degree())))
         print('commencing community detection')
         if jac_weighted_edges == True:
             start_leiden = time.time()
-            if self.partition_type == 'ModularityVP':
+            if self.partition_type =='ModularityVP':
                 print('partition type MVP')
                 partition = leidenalg.find_partition(G_sim, leidenalg.ModularityVertexPartition, weights='weight',
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed)
+                                                 n_iterations=self.n_iter_leiden, seed=self.random_seed)
             else:
                 print('partition type RBC')
                 partition = leidenalg.find_partition(G_sim, leidenalg.RBConfigurationVertexPartition, weights='weight',
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed,
-                                                     resolution_parameter=self.resolution_parameter)
-            # print(time.time() - start_leiden)
+                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed, resolution_parameter = self.resolution_parameter)
+            #print(time.time() - start_leiden)
         else:
             start_leiden = time.time()
             if self.partition_type == 'ModularityVP':
                 partition = leidenalg.find_partition(G_sim, leidenalg.ModularityVertexPartition,
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed)
+                                                 n_iterations=self.n_iter_leiden, seed=self.random_seed)
                 print('partition type MVP')
             else:
                 partition = leidenalg.find_partition(G_sim, leidenalg.RBConfigurationVertexPartition,
-                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed,
-                                                     resolution_parameter=self.resolution_parameter)
+                                                     n_iterations=self.n_iter_leiden, seed=self.random_seed, resolution_parameter = self.resolution_parameter)
                 print('partition type RBC')
             # print(time.time() - start_leiden)
         time_end_PARC = time.time()
         # print('Q= %.1f' % (partition.quality()))
         PARC_labels_leiden = np.asarray(partition.membership)
         PARC_labels_leiden = np.reshape(PARC_labels_leiden, (n_elements, 1))
 
@@ -368,15 +366,15 @@
 
         while too_big == True:
 
             X_data_big = X_data[cluster_big_loc, :]
             PARC_labels_leiden_big = self.run_toobig_subPARC(X_data_big)
             # print('set of new big labels ', set(PARC_labels_leiden_big.flatten()))
             PARC_labels_leiden_big = PARC_labels_leiden_big + 100000
-            # print('set of new big labels +1000 ', set(list(PARC_labels_leiden_big.flatten())))
+            # print('set of new big labels +100000 ', set(list(PARC_labels_leiden_big.flatten())))
             pop_list = []
 
             for item in set(list(PARC_labels_leiden_big.flatten())):
                 pop_list.append([item, list(PARC_labels_leiden_big.flatten()).count(item)])
             print('pop of big clusters', pop_list)
             jj = 0
             print('shape PARC_labels_leiden', PARC_labels_leiden.shape)
@@ -436,15 +434,15 @@
                 population = len(np.where(PARC_labels_leiden == cluster)[0])
                 if population < small_pop:
                     small_pop_exist = True
                     print(cluster, ' has small population of', population, )
                     small_pop_list.append(np.where(PARC_labels_leiden == cluster)[0])
             for small_cluster in small_pop_list:
                 for single_cell in small_cluster:
-                    old_neighbors = neighbor_array[single_cell, :]
+                    old_neighbors = neighbor_array[single_cell]
                     group_of_old_neighbors = PARC_labels_leiden[old_neighbors]
                     group_of_old_neighbors = list(group_of_old_neighbors.flatten())
                     best_group = max(set(group_of_old_neighbors), key=group_of_old_neighbors.count)
                     PARC_labels_leiden[single_cell] = best_group
 
         dummy, PARC_labels_leiden = np.unique(list(PARC_labels_leiden.flatten()), return_inverse=True)
         PARC_labels_leiden = list(PARC_labels_leiden.flatten())
@@ -579,105 +577,81 @@
 
             self.f1_accumulated = f1_accumulated
             self.f1_mean = f1_mean
             self.stats_df = df_accuracy
             self.majority_truth_labels = majority_truth_labels
         return
 
-    def run_umap_hnsw(self, X_input, graph, n_components=2, alpha: float = 1.0, negative_sample_rate: int = 5,
-                      gamma: float = 1.0, spread=1.0, min_dist=0.1, init_pos='spectral', random_state=1, ):
-
-        from umap.umap_ import find_ab_params, simplicial_set_embedding
-        import matplotlib.pyplot as plt
+    def run_umap_hnsw(self, X_input, graph, n_components=2, alpha: float = 1.0,
+                      negative_sample_rate: int = 5, gamma: float = 1.0, spread=1.0, min_dist=0.1,
+                      n_epochs=0, init_pos="spectral", random_state_seed=1, densmap=False,
+                      densmap_kwds={}, output_dens=False):
+        """Perform a fuzzy simplicial set embedding, using a specified initialisation method and
+        then minimizing the fuzzy set cross entropy between the 1-skeletons of the high and
+        low-dimensional fuzzy simplicial sets.
+
+        See `umap.umap_ simplicial_set_embedding
+        <https://github.com/lmcinnes/umap/blob/master/umap/umap_.py>`__.
+
+        Args:
+            X_input: (array) an array containing the input data, with shape n_samples x n_features.
+            graph: (array) the 1-skeleton of the high dimensional fuzzy simplicial set as
+                represented by a graph for which we require a sparse matrix for the
+                (weighted) adjacency matrix.
+            n_components: (int) the dimensionality of the Euclidean space into which the data
+                will be embedded.
+            alpha: (float) the initial learning rate for stochastic gradient descent (SGD).
+            negative_sample_rate: (int) the number of negative samples to select per positive
+                sample in the optimization process. Increasing this value will result in
+                greater repulsive force being applied, greater optimization cost, but
+                slightly more accuracy.
+            gamma: (float) weight to apply to negative samples.
+            spread: (float) the upper range of the x-value to be used to fit a curve for the
+                low-dimensional fuzzy simplicial complex construction. This curve should be
+                close to an offset exponential decay. Must be greater than 0. See
+                ``umap.umap_.find_ab_params``.
+            min_dist: (float) See ``umap.umap_.find_ab_params``.
+            n_epochs: (int) the number of training epochs to be used in optimizing the
+                low-dimensional embedding. Larger values result in more accurate embeddings.
+                If 0 is specified, a value will be selected based on the size of the input dataset
+                (200 for large datasets, 500 for small).
+            init_pos: (string) how to initialize the low-dimensional embedding. One of:
+                `spectral`: use a spectral embedding of the fuzzy 1-skeleton
+                `random`: assign initial embedding positions at random
+                `pca`: use the first n components from Principal Component Analysis (PCA)
+                    applied to the input data.
+            random_state_seed: (int) an integer to pass as a seed for the Numpy RandomState.
+            densmap: (bool) whether to use the density-augmented objective function to optimize
+                the embedding according to the densMAP algorithm.
+            densmap_kwds: (dict) keyword arguments to be used by the densMAP optimization.
+            output_dens: (bool) whether to output local radii in the original data
+                and the embedding.
+
+        Returns:
+            embedding: array of shape (n_samples, n_components)
+                The optimized of ``graph`` into an ``n_components`` dimensional
+                euclidean space.
+        """
 
         a, b = find_ab_params(spread, min_dist)
-        print('a,b, spread, dist', a, b, spread, min_dist)
-        t0 = time.time()
-        X_umap = simplicial_set_embedding(data=X_input, graph=graph, n_components=n_components, initial_alpha=alpha,
-                                          a=a, b=b, n_epochs=0, metric_kwds={}, gamma=gamma,
-                                          negative_sample_rate=negative_sample_rate, init=init_pos,
-                                          random_state=np.random.RandomState(random_state), metric='euclidean',
-                                          verbose=1)
-        return X_umap
-
-
-def main1():
-    import matplotlib.pyplot as plt
-
-    data_mat = pd.read_csv('/home/shobi/Thesis/Paper_writing/10XMouseBrain/datamatrixN1300K20PC.txt', header=None)
-    print('datamat shape', data_mat.shape)
-
-    p1 = PARC(data_mat, keep_all_local_dist=True)  # without labels
-    print('started at:', time.ctime())
-    t0 = time.time()
-    p1.run_PARC()
-    print('finished run_parc')
-    p1.knn_struct = p1.make_knn_struct()
-    print('ctime', time.ctime())
-    print('time taken to make the index', round(time.time() - t0))
-    graph = p1.knngraph_full()
-    X = p1.run_umap_hnsw(data_mat, graph)
-    print('time elapsed for umap-hnsw', round(time.time() - t0))
-
-    fig, ax = plt.subplots()
-    ax.scatter(X[:, 0], X[:, 1], c='orange', s=6, alpha=0.7)
-    ax.set_title('hnsw umap. dims and samples(K):' + str(p1.data.shape[1]) + str((p1.data.shape[0]) / 1000))
-    plt.show()
-
-    print('ctime', time.ctime())
-    fig, ax = plt.subplots()
-    t0 = time.time()
-    X_umap_original = umap.UMAP().fit_transform(data_mat)
-    print('time elapsed for umap-original', round(time.time() - t0))
-    ax.scatter(X_umap_original[:, 0], X_umap_original[:, 1], c='green')
-    ax.set_title('umap original')
-    plt.show()
-
-    p1.run_PARC()
-    labels = p1.labels
-
-
-def main():
-    # dummy example to check code runs
-    import matplotlib.pyplot as plt
-
-    from sklearn import datasets
-    import umap
-    iris = datasets.load_iris()
-    X = iris.data
-    y = iris.target
-
-    p1 = PARC(X, true_label=y, too_big_factor=0.3, resolution_parameter=1, keep_all_local_dist=True)  # without labels
-    p1.knn_struct = p1.make_knn_struct()
-    graph = p1.knngraph_full()
-    X_umap = p1.run_umap_hnsw(X, graph)
-
-    plt.scatter(X_umap[:, 0], X_umap[:, 1], c=y)
-
-    plt.show()
-
-    p1.run_PARC()
-    print(type(p1.labels), p1.stats_df)
-    print('finished first parc without y label')
-    # plt.scatter(X[:, 0], X[:, 1], c=y)
-
-    plt.scatter(X_umap[:, 0], X_umap[:, 1], c=p1.labels)
-    plt.show()
-    X_umap_original = umap.UMAP().fit_transform(X)
-    plt.scatter(X_umap_original[:, 0], X_umap_original[:, 1], c=y)
-    plt.show()
-
-    # View scatterplot
-    # plt.show()
-
-
-    p1 = PARC(X, true_label=y)  # without labels
-    p1.run_PARC()
-
-    plt.scatter(X_umap[:, 0], X_umap[:, 1], c=p1.labels)
-    plt.show()
-
-
-
+        print(f"a: {a}, b: {b}, spread: {spread}, dist: {min_dist}")
 
-if __name__ == '__main__':
-    main()
+        X_umap = simplicial_set_embedding(
+            data=X_input,
+            graph=graph,
+            n_components=n_components,
+            initial_alpha=alpha,
+            a=a,
+            b=b,
+            n_epochs=0,
+            metric_kwds={},
+            gamma=gamma,
+            negative_sample_rate=negative_sample_rate,
+            init=init_pos,
+            random_state=np.random.RandomState(random_state_seed),
+            metric="euclidean",
+            verbose=1,
+            densmap=densmap,
+            densmap_kwds=densmap_kwds,
+            output_dens=output_dens
+        )
+        return X_umap[0]
```

### Comparing `parc-0.33/setup.py` & `parc-0.40/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='parc',
-    version='0.33', #Feb 8, 2022
+    version='0.40',  #May 28,2024
     packages=['parc',],
     license='MIT',
-    author_email = 'shobana.venkat88@gmail.com',
-    url = 'https://github.com/ShobiStassen/PARC',
-    setup_requires = ['numpy','pybind11'],
-    install_requires=['pybind11','numpy','scipy','pandas','hnswlib','igraph','leidenalg>=0.7.0','umap-learn'],
+    author_email='shobana.venkat88@gmail.com',
+    url='https://github.com/ShobiStassen/PARC',
+    setup_requires=['numpy', 'pybind11'],
+    install_requires=[
+        'pybind11', 'numpy', 'scipy', 'pandas', 'hnswlib', 'igraph',
+        'leidenalg>=0.7.0', 'umap-learn'
+    ],
+    extras_require={
+        "dev": ["pytest", "scikit-learn"]
+    },
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

