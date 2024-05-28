# Comparing `tmp/ect-0.1.3.tar.gz` & `tmp/ect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ect-0.1.3.tar", last modified: Tue May 14 17:00:26 2024, max compression
+gzip compressed data, was "ect-0.1.4.tar", last modified: Tue May 28 00:24:57 2024, max compression
```

## Comparing `ect-0.1.3.tar` & `ect-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 liz       (1000) liz       (1000)        0 2024-05-14 17:00:26.380834 ect-0.1.3/
--rw-rw-r--   0 liz       (1000) liz       (1000)    35149 2024-05-02 14:56:25.000000 ect-0.1.3/LICENSE
--rw-r--r--   0 liz       (1000) liz       (1000)     2231 2024-05-14 17:00:26.380834 ect-0.1.3/PKG-INFO
--rw-rw-r--   0 liz       (1000) liz       (1000)     1545 2024-05-14 16:59:05.000000 ect-0.1.3/README.md
-drwxrwxr-x   0 liz       (1000) liz       (1000)        0 2024-05-14 17:00:26.376834 ect-0.1.3/ect/
-drwxrwxr-x   0 liz       (1000) liz       (1000)        0 2024-05-14 17:00:26.380834 ect-0.1.3/ect/ect.egg-info/
--rw-r--r--   0 liz       (1000) liz       (1000)     2231 2024-05-14 17:00:26.000000 ect-0.1.3/ect/ect.egg-info/PKG-INFO
--rw-rw-r--   0 liz       (1000) liz       (1000)      398 2024-05-14 17:00:26.000000 ect-0.1.3/ect/ect.egg-info/SOURCES.txt
--rw-rw-r--   0 liz       (1000) liz       (1000)        1 2024-05-14 17:00:26.000000 ect-0.1.3/ect/ect.egg-info/dependency_links.txt
--rw-rw-r--   0 liz       (1000) liz       (1000)       32 2024-05-14 17:00:26.000000 ect-0.1.3/ect/ect.egg-info/requires.txt
--rw-rw-r--   0 liz       (1000) liz       (1000)       14 2024-05-14 17:00:26.000000 ect-0.1.3/ect/ect.egg-info/top_level.txt
-drwxrwxr-x   0 liz       (1000) liz       (1000)        0 2024-05-14 17:00:26.380834 ect-0.1.3/ect/ect_on_graphs/
--rw-rw-r--   0 liz       (1000) liz       (1000)      174 2024-05-02 15:40:21.000000 ect-0.1.3/ect/ect_on_graphs/__init__.py
--rw-rw-r--   0 liz       (1000) liz       (1000)    10999 2024-05-06 18:11:30.000000 ect-0.1.3/ect/ect_on_graphs/ect_graph.py
--rw-rw-r--   0 liz       (1000) liz       (1000)     3128 2024-05-02 14:56:25.000000 ect-0.1.3/ect/ect_on_graphs/ect_sarah.py
--rw-rw-r--   0 liz       (1000) liz       (1000)     4279 2024-05-02 14:56:25.000000 ect-0.1.3/ect/ect_on_graphs/ect_utils_sarah.py
--rw-r--r--   0 liz       (1000) liz       (1000)    11310 2024-05-14 16:18:22.000000 ect-0.1.3/ect/ect_on_graphs/embed_graph.py
--rw-rw-r--   0 liz       (1000) liz       (1000)      725 2024-05-14 17:00:12.000000 ect-0.1.3/pyproject.toml
--rw-rw-r--   0 liz       (1000) liz       (1000)       38 2024-05-14 17:00:26.380834 ect-0.1.3/setup.cfg
-drwxrwxr-x   0 liz       (1000) liz       (1000)        0 2024-05-14 17:00:26.380834 ect-0.1.3/tests/
--rw-rw-r--   0 liz       (1000) liz       (1000)     1626 2024-05-06 18:11:30.000000 ect-0.1.3/tests/test_ect_graph.py
--rw-r--r--   0 liz       (1000) liz       (1000)     1467 2024-05-02 23:41:58.000000 ect-0.1.3/tests/test_embed_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 00:24:53.000000 ect-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-28 00:24:57.625856 ect-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-28 00:24:53.000000 ect-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.621855 ect-0.1.4/ect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/ect/ect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/ect/ect_on_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/ect_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/embed_cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/embed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-28 00:24:53.000000 ect-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:24:57.625856 ect-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_ect_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_embed_cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_embed_graph.py
```

### Comparing `ect-0.1.3/LICENSE` & `ect-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ect-0.1.3/PKG-INFO` & `ect-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ect
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for computing the Euler Characteristic Transform
 Author-email: Liz Munch <muncheli@msu.edu>
 Project-URL: Homepage, https://munchlab.github.io/ect
 Project-URL: Repository, https://github.com/MunchLab/ect
 Project-URL: Issues, https://github.com/MunchLab/ect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: numba
+Requires-Dist: scipy
 
 # `ect`: A python package for computing the Euler Characteristic Transform
 
 Python computation tools for computing the Euler Characteristic Transform of embedded graphs. 
 
 ## Description
```

### Comparing `ect-0.1.3/README.md` & `ect-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ect-0.1.3/ect/ect.egg-info/PKG-INFO` & `ect-0.1.4/ect/ect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ect
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for computing the Euler Characteristic Transform
 Author-email: Liz Munch <muncheli@msu.edu>
 Project-URL: Homepage, https://munchlab.github.io/ect
 Project-URL: Repository, https://github.com/MunchLab/ect
 Project-URL: Issues, https://github.com/MunchLab/ect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: numba
+Requires-Dist: scipy
 
 # `ect`: A python package for computing the Euler Characteristic Transform
 
 Python computation tools for computing the Euler Characteristic Transform of embedded graphs. 
 
 ## Description
```

### Comparing `ect-0.1.3/ect/ect_on_graphs/ect_graph.py` & `ect-0.1.4/ect/ect_on_graphs/ect_graph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,226 @@
 import numpy as np
 from itertools import compress, combinations
 from numba import jit
 import matplotlib.pyplot as plt
+from ect.ect_on_graphs.embed_cw import EmbeddedCW
 
 
 class ECT:
-    """
-    A class to calculate the Euler Characteristic Transform (ECT) from an input ``embed_graph.EmbeddedGraph``.
-    The result is a matrix where entry ``M[i,j]`` is ``chi(K_{a_i})`` for the direction $\omega_j$ where $a_i$ is the $i$th entry in ``self.threshes``, and $\omega_j$ is the ith entry in self.thetas.
+    """A class to calculate the Euler Characteristic Transform (ECT) from an input :any:`EmbeddedGraph` or :any:`EmbeddedCW`.
 
-    ...
+    The result is a matrix where entry ``M[i,j]`` is :math:`\chi(K_{a_i})` for the direction :math:`\omega_j` where :math:`a_i` is the ith entry in ``self.threshes``, and :math:`\omega_j` is the ith entry in ``self.thetas``.
 
     Attributes
-        num_dirs : int
+        num_dirs (int):
             The number of directions to consider in the matrix.
-        num_thresh : int
+        num_thresh (int):
             The number of thresholds to consider in the matrix.
-        bound_radius : int
-            Either None, or a positive radius of the bounding circle.
-        ECT_matrix : np.array
+        bound_radius (int):
+            Either ``None``, or a positive radius of the bounding circle.
+        ECT_matrix (np.array):
             The matrix to store the ECT.
-        SECT_matrix : np.array
+        SECT_matrix (np.array):
             The matrix to store the SECT.
 
-    Methods
-        __init__(num_dirs, num_thresh):
-            Constructs all the necessary attributes for the ECT object.
-        calculate(graph):
-            Calculates the ECT from an input EmbeddedGraph.
-
     """
 
-    def __init__(self, num_dirs, num_thresh, bound_radius = None):
+    def __init__(self, num_dirs, num_thresh, bound_radius=None):
         """
         Constructs all the necessary attributes for the ECT object.
 
         Parameters:
-            num_dirs : int
+            num_dirs (int):
                 The number of directions to consider in the matrix.
-            num_thresh : int
+            num_thresh (int):
                 The number of thresholds to consider in the matrix.
-            bound_radius : int
+            bound_radius (int):
                 Either None, or a positive radius of the bounding circle.
         """
         self.num_dirs = num_dirs
 
         # Note: This version doesn't include 2pi since its the same as the 0 direction.
-        self.thetas = np.linspace(0, 2*np.pi, self.num_dirs,endpoint=False)
-
+        self.thetas = np.linspace(0, 2*np.pi, self.num_dirs, endpoint=False)
 
         self.num_thresh = num_thresh
         self.set_bounding_radius(bound_radius)
 
         self.ECT_matrix = np.zeros((num_dirs, num_thresh))
         self.SECT_matrix = np.zeros((num_dirs, num_thresh))
 
     def set_bounding_radius(self, bound_radius):
         """
         Manually sets the radius of the bounding circle centered at the origin for the ECT object.
 
         Parameters:
-            bound_radius (int): Either None, or a positive radius of the bounding circle.
+            bound_radius (int): 
+                Either None, or a positive radius of the bounding circle.
         """
         self.bound_radius = bound_radius
 
         if self.bound_radius is None:
             self.threshes = None
         else:
-            self.threshes = np.linspace(-bound_radius, bound_radius, self.num_thresh)
+            self.threshes = np.linspace(-bound_radius,
+                                        bound_radius, self.num_thresh)
+
+    def get_radius_and_thresh(self, G, bound_radius):
+        """
+        An internally used function to get the bounding radius and thresholds for the ECT calculation.
+
+        Parameters:
+            G (EmbeddedGraph / EmbeddedCW):
+                The input graph to calculate the ECT for.
+            bound_radius (float):
+                If None, uses the following in order: (i) the bounding radius stored in the class; or if not available (ii) the bounding radius of the given graph. Otherwise, should be a postive float :math:`R` where the ECC will be computed at thresholds in :math:`[-R,R]`. Default is None.
+
+        Returns:
+            float, np.array
+                The bounding radius and the thresholds for the ECT calculation.
+
+        """
+       # Either use the global radius and the set self.threshes; or use the tight bounding box and calculate
+        # the thresholds from that.
+        if bound_radius == None:
+            # First try to get the internally stored bounding radius
+            if self.bound_radius is not None:
+                r = self.bound_radius
+                r_threshes = self.threshes
+
+            # If the bounding radius is not set, use the global bounding radius
+            else:
+                r = G.get_bounding_radius()
+                r_threshes = np.linspace(-r, r, self.num_thresh)
+
+        else:
+            # The user wants to use a different bounding radius
+            if bound_radius <= 0:
+                raise ValueError(
+                    f'Bounding radius given was {bound_radius}, but must be a positive number.')
+            r = bound_radius
+            r_threshes = np.linspace(-r, r, self.num_thresh)
+
+        return r, r_threshes
 
     def get_ECT(self):
         """
         Returns the ECT matrix.
         """
         return self.ECT_matrix
 
     def get_SECT(self):
         """
         Returns the SECT matrix.
         """
         return self.SECT_matrix
 
-    def calculateECC(self, G, theta, tightbbox = False):
+    def calculateECC(self, G, theta, bound_radius=None, return_counts=False):
         """
-        Function to compute the Euler Characteristic of a graph with coordinates for each vertex (pos).
+        Function to compute the Euler Characteristic of an `EmbeddedGraph`, that is, a graph with coordinates for each vertex.
 
         Parameters:
-            G : Graph
+            G (nx.Graph):
                 The graph to compute the Euler Characteristic for.
-            theta : float
-                The angle (in radians) to rotate the graph by before computing the Euler Characteristic.
-            tightbbox : bool, optional
-                If True, use the tight bounding box of the graph. If False, use the bounding circle. Default is False.
-        """
-        
-        # Either use the global radius and the set self.threshes; or use the tight bounding box and calculate 
-        # the thresholds from that. 
-        if tightbbox:
-            # thresholds for filtration, r should be defined from global bounding box
-            r = G.get_bounding_radius()
-            r_threshes = np.linspace(-r,r, self.num_thresh)
-        else:
-            # The user wants to use the internally determined bounding radius
-            if self.bound_radius is None:
-                raise ValueError('Bounding radius must be set before calculating ECC when you have tightbbox=False.')
-            else:
-                r = self.bound_radius
-                r_threshes = self.threshes
+            theta (float):
+                The angle (in radians) to use for the direction function when computing the Euler Characteristic Curve.
+            bound_radius (float):
+                If None, uses the following in order: (i) the bounding radius stored in the class; or if not available (ii) the bounding radius of the given graph. Otherwise, should be a postive float :math:`R` where the ECC will be computed at thresholds in :math:`[-R,R]`. Default is None.
+            return_counts (bool):
+                Whether to return the counts of vertices, edges, and faces below the threshold. Default is False.
 
-        #--
-        def num_below_threshold(func_list,thresh):
+        """
+
+        r, r_threshes = self.get_radius_and_thresh(G, bound_radius)
+
+        # --
+        def num_below_threshold(func_list, thresh):
             """ 
             Returns the number of entries in func_list that are below the threshold thresh. 
             Warning: func_list must be sorted in ascending order.
 
             Parameters
-            func_list: list of floats
-            thresh: float
+                func_list (list): sorted list of function values
+                thresh (float): threshold value
 
             Returns
                 int 
             """
-            func_max = func_list[-1]
-            if thresh < func_max:
-                return np.argmin(func_list < thresh)
-            else: 
-                return len(func_list)
-        #--    
-        
+            # If the list is empty, return 0
+            if len(func_list) == 0:
+                return 0
+            else:
+                func_max = func_list[-1]
+                if thresh < func_max:
+                    return np.argmin(func_list < thresh)
+                else:
+                    return len(func_list)
+        # --
+
         v_list, g = G.sort_vertices(theta, return_g=True)
         g_list = [g[v] for v in v_list]
 
-        vertex_count = np.array([num_below_threshold(g_list,thresh) for thresh in r_threshes])
+        vertex_count = np.array([num_below_threshold(
+            g_list, thresh) for thresh in r_threshes])
         # print(vertex_count)
 
-
-        e_list, g_e = G.sort_edges(np.pi/2, return_g=True)
+        e_list, g_e = G.sort_edges(theta, return_g=True)
         g_e_list = [g_e[e] for e in e_list]
-        edge_count = np.array([num_below_threshold(g_e_list,thresh) for thresh in r_threshes])
+        edge_count = np.array([num_below_threshold(
+            g_e_list, thresh) for thresh in r_threshes])
         # print(edge_count)
 
+        if type(G) == EmbeddedCW:
+            f_list, g_f = G.sort_faces(theta, return_g=True)
+            g_f_list = [g_f[f] for f in f_list]
+            face_count = np.array([num_below_threshold(
+                g_f_list, thresh) for thresh in r_threshes])
+            # print(face_count)
+        else:
+            face_count = np.zeros_like(vertex_count)
+
         # print(vertex_count - edge_count)
-        ecc = vertex_count - edge_count
+        ecc = vertex_count - edge_count + face_count
 
-        return ecc
+        if return_counts:
+            return ecc, vertex_count, edge_count, face_count
+        else:
+            return ecc
 
-    def calculateECT(self, graph, tightbbox=False, compute_SECT=True):
+    def calculateECT(self, graph, bound_radius=None, compute_SECT=True):
         """
-        Calculates the ECT from an input EmbeddedGraph. The entry M[i,j] is $\chi(K_{a_j})$ for the direction $\omega_i$ where $a_j$ is the $j$th entry in self.threshes, and $\omega_i$ is the ith entry in self.thetas.
+        Calculates the ECT from an input either `EmbeddedGraph` or `EmbeddedCW`. The entry ``M[i,j]`` is :math:`\\chi(K_{a_j})` for the direction :math:`\omega_i` where :math:`a_j` is the jth entry in ``self.threshes``, and :math:`\omega_i` is the ith entry in ``self.thetas``.
 
         Parameters:
-            graph : EmbeddedGraph
+            graph (EmbeddedGraph/EmbeddedCW):
                 The input graph to calculate the ECT from.
-            tightbbox : bool, optional
-                Whether to use the tight bounding box (a different value in each direction) computed from the input graph. Otherwise, a bounding box needs to already be set manually with the `set_bounding_box` method.
-            compute_SECT : bool, optional
+            bound_radius (float):
+                If None, uses the following in order: (i) the bounding radius stored in the class; or if not available (ii) the bounding radius of the given graph. Otherwise, should be a postive float :math:`R` where the ECC will be computed at thresholds in :math:`[-R,R]`. Default is None.
+            compute_SECT (bool):
                 Whether to compute the SECT after the ECT is computed. Default is True. Sets the SECT_matrix attribute, but doesn't return it. Can be returned with the get_SECT method.
 
         Returns:
             np.array
                 The matrix representing the ECT of size (num_dirs,num_thresh).
         """
 
-        if tightbbox == False and self.bound_radius is None:
-            self.set_bounding_radius(graph.get_bounding_radius())
+        r, r_threshes = self.get_radius_and_thresh(graph, bound_radius)
+
+        # Note... this overwrites the self.threshes if it's not set.
+        self.set_bounding_radius(r)
 
         M = np.zeros((self.num_dirs, self.num_thresh))
-        
+
         for i, theta in enumerate(self.thetas):
-            M[i] = self.calculateECC(graph, theta, tightbbox)
-        
+            M[i] = self.calculateECC(graph, theta, r)
+
         self.ECT_matrix = M
 
         if compute_SECT:
             self.SECT_matrix = self.calculateSECT()
-       
+
         return self.ECT_matrix
 
     def calculateSECT(self):
         """
         Function to calculate the Smooth Euler Characteristic Transform (SECT) from the ECT matrix. 
 
         Returns:
@@ -186,139 +228,152 @@
                 The matrix representing the SECT of size (num_dirs,num_thresh).
         """
 
         # Calculate the SECT
         M = self.ECT_matrix
 
         # Get average of each row, corresponds to each direction
-        A = np.average(M, axis = 1)
+        A = np.average(M, axis=1)
 
         # Subtract the average from each row
         M_normalized = M - A[:, np.newaxis]
 
         # Take the cumulative sum of each row to get the SECT
-        M_SECT = np.cumsum(M_normalized, axis = 1)
+        M_SECT = np.cumsum(M_normalized, axis=1)
 
         return M_SECT
 
-    def plotECC(self, graph, theta):
+    def plotECC(self, graph, theta, bound_radius=None, draw_counts=False):
         """
         Function to plot the Euler Characteristic Curve (ECC) for a specific direction theta. Note that this calculates the ECC for the input graph and then plots it.
 
         Parameters:
-            graph : EmbeddedGraph
-                The input graph.
-            theta : float
-                The angle in [0,2*np.pi] for the direction to plot the ECC.
+            graph (EmbeddedGraph/EmbeddedCW):
+                The input graph or CW complex.
+            theta (float):
+                The angle in :math:`[0,2\pi]` for the direction to plot the ECC.
+            bound_radius (float):
+                If None, uses the following in order: (i) the bounding radius stored in the class; or if not available (ii) the bounding radius of the given graph. Otherwise, should be a postive float :math:`R` where the ECC will be computed at thresholds in :math:`[-R,R]`. Default is None. 
+            draw_counts (bool):
+                Whether to draw the counts of vertices, edges, and faces varying across thresholds. Default is False.
         """
 
-        ECC = self.calculateECC(graph, theta)
-        
-        plt.step(self.threshes,ECC)
-        theta_round = str(np.round(theta,2))
+        r, r_threshes = self.get_radius_and_thresh(graph, bound_radius)
+        if not draw_counts:
+            ECC = self.calculateECC(graph, theta, r)
+        else:
+            ECC, vertex_count, edge_count, face_count = self.calculateECC(
+                graph, theta, r, return_counts=True)
+
+        # if self.threshes is None:
+        #     self.set_bounding_radius(graph.get_bounding_radius())
+
+        plt.step(r_threshes, ECC, label='ECC')
+
+        if draw_counts:
+            plt.step(r_threshes, vertex_count, label='Vertices')
+            plt.step(r_threshes, edge_count, label='Edges')
+            plt.step(r_threshes, face_count, label='Faces')
+            plt.legend()
+
+        theta_round = str(np.round(theta, 2))
         plt.title(r'ECC for $\omega = ' + theta_round + '$')
         plt.xlabel('$a$')
         plt.ylabel(r'$\chi(K_a)$')
 
-
     def plotECT(self):
-
         """
         Function to plot the Euler Characteristic Transform (ECT) matrix. Note that the ECT matrix must be calculated before calling this function.
 
         The resulting plot will have the angle on the x-axis and the threshold on the y-axis.
         """
 
         # Make meshgrid.
         # Add back the 2pi to thetas for the pcolormesh
-        thetas = np.concatenate((self.thetas,[2*np.pi]))
-        X,Y = np.meshgrid(thetas,self.threshes)
+        thetas = np.concatenate((self.thetas, [2*np.pi]))
+        X, Y = np.meshgrid(thetas, self.threshes)
         M = np.zeros_like(X)
 
-        M[:,:-1] = self.ECT_matrix.T # Transpose to get the correct orientation
-        M[:,-1] = M[:,0] # Add the 2pi direction to the 0 direction
-        
+        # Transpose to get the correct orientation
+        M[:, :-1] = self.ECT_matrix.T
+        M[:, -1] = M[:, 0]  # Add the 2pi direction to the 0 direction
 
-        plt.pcolormesh(X,Y,M, cmap = 'viridis')
+        plt.pcolormesh(X, Y, M, cmap='viridis')
         plt.colorbar()
 
         ax = plt.gca()
-        ax.set_xticks(np.linspace(0,2*np.pi,9))
+        ax.set_xticks(np.linspace(0, 2*np.pi, 9))
 
         labels = [r'$0$',
-                r'$\frac{\pi}{4}$',
-                r'$\frac{\pi}{2}$',
-                r'$\frac{3\pi}{4}$',
-                r'$\pi$',
-                r'$\frac{5\pi}{4}$',
-                r'$\frac{3\pi}{2}$',
-                r'$\frac{7\pi}{4}$',
-                r'$2\pi$',
-                ]
+                  r'$\frac{\pi}{4}$',
+                  r'$\frac{\pi}{2}$',
+                  r'$\frac{3\pi}{4}$',
+                  r'$\pi$',
+                  r'$\frac{5\pi}{4}$',
+                  r'$\frac{3\pi}{2}$',
+                  r'$\frac{7\pi}{4}$',
+                  r'$2\pi$',
+                  ]
 
         ax.set_xticklabels(labels)
 
-
         plt.xlabel(r'$\omega$')
         plt.ylabel(r'$a$')
 
         plt.title(r'ECT of Input Graph')
-    
 
     def plotSECT(self):
-
         """
         Function to plot the Smooth Euler Characteristic Transform (SECT) matrix. Note that the SECT matrix must be calculated before calling this function.
 
         The resulting plot will have the angle on the x-axis and the threshold on the y-axis.
         """
 
         # Make meshgrid.
         # Add back the 2pi to thetas for the pcolormesh
-        thetas = np.concatenate((self.thetas,[2*np.pi]))
-        X,Y = np.meshgrid(thetas,self.threshes)
+        thetas = np.concatenate((self.thetas, [2*np.pi]))
+        X, Y = np.meshgrid(thetas, self.threshes)
         M = np.zeros_like(X)
 
-        M[:,:-1] = self.SECT_matrix.T # Transpose to get the correct orientation
-        M[:,-1] = M[:,0] # Add the 2pi direction to the 0 direction
-        
+        # Transpose to get the correct orientation
+        M[:, :-1] = self.SECT_matrix.T
+        M[:, -1] = M[:, 0]  # Add the 2pi direction to the 0 direction
 
-        plt.pcolormesh(X,Y,M, cmap = 'viridis')
+        plt.pcolormesh(X, Y, M, cmap='viridis')
         plt.colorbar()
 
         ax = plt.gca()
-        ax.set_xticks(np.linspace(0,2*np.pi,9))
+        ax.set_xticks(np.linspace(0, 2*np.pi, 9))
 
         labels = [r'$0$',
-                r'$\frac{\pi}{4}$',
-                r'$\frac{\pi}{2}$',
-                r'$\frac{3\pi}{4}$',
-                r'$\pi$',
-                r'$\frac{5\pi}{4}$',
-                r'$\frac{3\pi}{2}$',
-                r'$\frac{7\pi}{4}$',
-                r'$2\pi$',
-                ]
+                  r'$\frac{\pi}{4}$',
+                  r'$\frac{\pi}{2}$',
+                  r'$\frac{3\pi}{4}$',
+                  r'$\pi$',
+                  r'$\frac{5\pi}{4}$',
+                  r'$\frac{3\pi}{2}$',
+                  r'$\frac{7\pi}{4}$',
+                  r'$2\pi$',
+                  ]
 
         ax.set_xticklabels(labels)
 
-
         plt.xlabel(r'$\omega$')
         plt.ylabel(r'$t$')
 
         plt.title(r'SECT of Input Graph')
 
-    def plot(self, type):
+    def plot(self, plot_type):
         """
         Function to plot the ECT or SECT matrix. The type parameter should be either 'ECT' or 'SECT'.
 
         Parameters:
-            type : str
+            plot_type : str
                 The type of plot to make. Either 'ECT' or 'SECT'.
         """
 
-        if type == 'ECT':
+        if plot_type == 'ECT':
             self.plotECT()
-        elif type == 'SECT':
+        elif plot_type == 'SECT':
             self.plotSECT()
         else:
-            raise ValueError('Type must be either "ECT" or "SECT".')
+            raise ValueError('plot_type must be either "ECT" or "SECT".')
```

### Comparing `ect-0.1.3/ect/ect_on_graphs/embed_graph.py` & `ect-0.1.4/ect/ect_on_graphs/embed_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,120 +4,124 @@
 
 
 class EmbeddedGraph(nx.Graph):
     """
     A class to represent a graph with 2D embedded coordinates for each vertex.
 
     Attributes
+        graph : nx.Graph
+            a NetworkX graph object
         coordinates : dict
             a dictionary mapping vertices to their (x, y) coordinates
 
-    Methods
-        add_vertex(vertex, x, y):
-            Adds a vertex to the graph and assigns it the given coordinates.
-        add_edge(u, v):
-            Adds an edge between the vertices u and v.
-        get_coordinates(vertex):
-            Returns the coordinates of the given vertex.
-        set_coordinates(vertex, x, y):
-            Sets the coordinates of the given vertex.
-
     """
 
     def __init__(self):
         """
-        Constructs all the necessary attributes for the EmbeddedGraph object.
+        Initializes an empty EmbeddedGraph object.
 
         """
         super().__init__()
         self.coordinates = {}
 
-    def add_vertex(self, vertex, x, y):
+    def add_node(self, vertex, x, y):
         """
         Adds a vertex to the graph and assigns it the given coordinates.
 
         Parameters:
-            vertex: str
+            vertex (str):
                 The vertex to be added.
-            x : float
+            x (float):
                 The x-coordinate of the vertex.
-            y : float
+            y (float):
                 The y-coordinate of the vertex.
 
         """
-        self.add_node(vertex)
+        super().add_node(vertex)
         self.coordinates[vertex] = (x, y)
 
+    def add_nodes_from(self, nodes, coordinates):
+        """
+        Adds multiple vertices to the graph and assigns them the given coordinates.
+
+        Parameters:
+            nodes (list):
+                A list of vertices to be added.
+            coordinates (dict):
+                A dictionary mapping vertices to their coordinates.
+
+        """
+        super().add_nodes_from(nodes)
+        self.coordinates.update(coordinates)
+
     def add_edge(self, u, v):
         """
         Adds an edge between the vertices u and v if they exist.
 
         Parameters:
-            u : str
+            u (str):
                 The first vertex of the edge.
-            v : str
+            v (str):
                 The second vertex of the edge.
 
         """
         if not self.has_node(u) or not self.has_node(v):
             raise ValueError("One or both vertices do not exist in the graph.")
         else:
             super().add_edge(u, v)
 
     def get_coordinates(self, vertex):
         """
         Returns the coordinates of the given vertex.
 
         Parameters:
-            vertex : str
+            vertex (str):
                 The vertex whose coordinates are to be returned.
 
         Returns:
             tuple: The coordinates of the vertex.
 
         """
         return self.coordinates.get(vertex)
 
     def set_coordinates(self, vertex, x, y):
         """
         Sets the coordinates of the given vertex.
 
         Parameters:
-            vertex : str
+            vertex (str):
                 The vertex whose coordinates are to be set.
-            x : float
+            x (float):
                 The new x-coordinate of the vertex.
-            y : float 
+            y (float): 
                 The new y-coordinate of the vertex.
 
         Raises:
             ValueError: If the vertex does not exist in the graph.
 
         """
         if vertex in self.coordinates:
             self.coordinates[vertex] = (x, y)
         else:
             raise ValueError("Vertex does not exist in the graph.")
 
-
-
     def get_bounding_box(self):
         """
         Method to find a bounding box of the vertex coordinates in the graph.
 
         Returns:
             list: A list of tuples representing the minimum and maximum x and y coordinates.
 
         """
         if not self.coordinates:
             return None
 
         x_coords, y_coords = zip(*self.coordinates.values())
         return [(min(x_coords), max(x_coords)), (min(y_coords), max(y_coords))]
-    
+
     def get_bounding_radius(self):
         """
         Method to find the radius of the bounding circle of the vertex coordinates in the graph.
 
         Returns:
             float: The radius of the bounding circle.
 
@@ -125,15 +129,15 @@
         if not self.coordinates:
             return 0
 
         x_coords, y_coords = zip(*self.coordinates.values())
         norms = [np.linalg.norm(point) for point in zip(x_coords, y_coords)]
 
         return max(norms)
-    
+
     def get_mean_centered_coordinates(self):
         """
         Method to find the mean-centered coordinates of the vertices in the graph.
 
         Returns:
             dict: A dictionary mapping vertices to their mean-centered coordinates.
 
@@ -141,201 +145,203 @@
         if not self.coordinates:
             return None
 
         x_coords, y_coords = zip(*self.coordinates.values())
         mean_x, mean_y = np.mean(x_coords), np.mean(y_coords)
 
         return {v: (x - mean_x, y - mean_y) for v, (x, y) in self.coordinates.items()}
-    
-
 
     def set_mean_centered_coordinates(self):
         """
         Method to set the mean-centered coordinates of the vertices in the graph. Warning: This overwrites the original coordinates
 
         """
-        
-        self.coordinates = self.get_mean_centered_coordinates()
-
-
 
+        self.coordinates = self.get_mean_centered_coordinates()
 
     def g_omega(self, theta):
         """
-        Function to compute the function g_omega(v) for all vertices v in the graph in the direction of theta \in [0,2*np.pi]. This function is defined by $g_\omega(v) = < pos(v), \omega >$.
+        Function to compute the function :math:`g_\omega(v)` for all vertices :math:`v` in the graph in the direction of :math:`\\theta \in [0,2\pi]` . This function is defined by :math:`g_\omega(v) = \langle \\texttt{pos}(v), \omega \\rangle` .
 
         Parameters:
 
-            theta : float
-                The angle in [0,2*np.pi] for the direction to compute the g(v) values.
+            theta (float):
+                The angle in :math:`[0,2\pi]` for the direction to compute the :math:`g(v)` values.
 
         Returns:
 
-            dict: A dictionary mapping vertices to their g(v) values.
+            dict: A dictionary mapping vertices to their :math:`g(v)` values.
 
         """
-        
+
         omega = (np.cos(theta), np.sin(theta))
 
         g = {}
         for v in self.nodes:
             g[v] = np.dot(self.coordinates[v], omega)
         return g
-    
+
     def g_omega_edges(self, theta):
         """
         Calculates the function value of the edges of the graph by making the value equal to the max vertex value 
 
         Parameters:
-            theta : float 
+
+            theta (float): 
                 The direction of the function to be calculated.
-            
-            Returns
-                g_edges : dict
-                    A dictionary of the function values of the edges.
+
+        Returns:
+            dict
+                A dictionary of the function values of the edges.
         """
         g = self.g_omega(theta)
 
         g_edges = {}
         for e in self.edges:
             g_edges[e] = max(g[e[0]], g[e[1]])
 
-        return g_edges 
- 
-    def sort_vertices(self, theta,return_g = False):
+        return g_edges
+
+    def sort_vertices(self, theta, return_g=False):
         """
         Function to sort the vertices of the graph according to the function g_omega(v) in the direction of theta \in [0,2*np.pi].
 
         TODO: eventually, do we want this to return a sorted list of g values as well? Since we're already doing the sorting work, it might be helpful.
 
         Parameters:
-            theta : float
+            theta (float):
                 The angle in [0,2*np.pi] for the direction to sort the vertices.
-            return_g : bool
+            return_g (bool):
                 Whether to return the g(v) values along with the sorted vertices.
 
         Returns:
-            list: 
-                A list of vertices sorted in increasing order of the g(v) values. 
-            dict: 
-                If return_g is True, also returns the g dictionary with the function values. 
+            list
+                A list of vertices sorted in increasing order of the :math:`g(v)` values. 
+                If ``return_g`` is True, also returns the ``g`` dictionary with the function values ``g[vertex_name]=func_value``. 
 
         """
         g = self.g_omega(theta)
 
         v_list = sorted(self.nodes, key=lambda v: g[v])
 
         if return_g:
             # g_sorted = [g[v] for v in v_list]
-            return  v_list, g
+            return v_list, g
         else:
             return v_list
 
-    def sort_edges(self, theta,return_g = False):
+    def sort_edges(self, theta, return_g=False):
         """
-        Function to sort the edges of the graph according to the function 
-            g_omega(e) = max { g_omega(v) for v in e }
-        in the direction of theta \in [0,2*np.pi].
+        Function to sort the edges of the graph according to the function
+
+        .. math ::
+
+            g_\omega(e) = \max \{ g_\omega(v) \mid  v \in e \}
+
+        in the direction of :math:`\\theta \in [0,2\pi]` .
 
         Parameters:
-            theta : float
-                The angle in [0,2*np.pi] for the direction to sort the vertices.
-            return_g : bool
-                Whether to return the g(v) values along with the sorted vertices.
+            theta (float):
+                The angle in :math:`[0,2\pi]` for the direction to sort the edges.
+            return_g (bool):
+                Whether to return the :math:`g(v)` values along with the sorted edges.
 
         Returns:
-            list: 
-                A list of vertices sorted in increasing order of the g(v) values. 
-            dict: 
-                If return_g is True, also returns the g dictionary with the function values. 
+            A list of edges sorted in increasing order of the :math:`g(v)` values. 
+            If ``return_g`` is True, also returns the ``g`` dictionary with the function values ``g[vertex_name]=func_value``. 
 
         """
         g_e = self.g_omega_edges(theta)
 
         e_list = sorted(self.edges, key=lambda e: g_e[e])
 
         if return_g:
             # g_sorted = [g[v] for v in v_list]
-            return  e_list, g_e
+            return e_list, g_e
         else:
             return e_list
-        
-    
+
     def lower_edges(self, v, omega):
         """
         Function to compute the number of lower edges of a vertex v for a specific direction (included by the use of sorted v_list).
 
         Parameters:
-            v : str
+            v (str):
                 The vertex to compute the number of lower edges for.
-            omega : tuple 
+            omega (tuple): 
                 The direction vector to consider given as an angle in [0, 2pi].
 
         Returns:
             int: The number of lower edges of the vertex v.
 
         """
         L = [n for n in self.neighbors(v)]
-        gv = np.dot(self.coordinates[v],omega)
-        Lg = [np.dot(self.coordinates[v],omega) for v in L]
-        return sum(n >= gv for n in Lg) # includes possible duplicate counts 
+        gv = np.dot(self.coordinates[v], omega)
+        Lg = [np.dot(self.coordinates[v], omega) for v in L]
+        return sum(n >= gv for n in Lg)  # includes possible duplicate counts
 
-    def plot(self, bounding_circle = False, color_nodes_theta = None):
+    def plot(self, bounding_circle=False, color_nodes_theta=None, ax=None, **kwargs):
         """
         Function to plot the graph with the embedded coordinates.
 
         If ``bounding_circle`` is True, a bounding circle is drawn around the graph.
 
-        If ``color_nodes_theta`` is not None, it should be given as a theta in [0,2pi]. Then the nodes are colored according to the g(v) values in the direction of theta.
+        If ``color_nodes_theta`` is not None, it should be given as a theta in :math:`[0,2\pi]`. Then the nodes are colored according to the :math:`g(v)` values in the direction of theta.
 
         """
-
-        fig, ax = plt.subplots()
+        if ax is None:
+            fig, ax = plt.subplots()
+            # print("making new figure")
+        else:
+            fig = ax.get_figure()
 
         pos = self.coordinates
         if color_nodes_theta == None:
-            nx.draw(self, pos, with_labels=True)
+            nx.draw(self, pos, with_labels=True, ax=ax, **kwargs)
         else:
             g = self.g_omega(color_nodes_theta)
             color_map = [g[v] for v in self.nodes]
             # Some weird plotting to make the colorbar work.
-            pathcollection = nx.draw_networkx_nodes(self, pos, node_color=color_map)
-            nx.draw_networkx_labels(self, pos=pos, font_color='black')
-            nx.draw_networkx_edges(self, pos)
-            plt.colorbar(pathcollection)
+            pathcollection = nx.draw_networkx_nodes(
+                self, pos, node_color=color_map, ax=ax)
+            nx.draw_networkx_labels(self, pos=pos, font_color='black', ax=ax)
+            nx.draw_networkx_edges(self, pos, ax=ax, width=1, **kwargs)
+            fig.colorbar(pathcollection, ax=ax, **kwargs)
 
         plt.axis('on')
-        ax.tick_params(left=True, bottom=True, labelleft=True, labelbottom=True)
+        ax.tick_params(left=True, bottom=True,
+                       labelleft=True, labelbottom=True)
 
         if bounding_circle:
             r = self.get_bounding_radius()
             ax = plt.gca()
-            circle1 = plt.Circle((0, 0), r, fill = False, linestyle = '--', color = 'r')
+            circle1 = plt.Circle((0, 0), r, fill=False,
+                                 linestyle='--', color='r')
             ax.add_patch(circle1)
             plt.axis('square')
-        
-        
+
+        return ax
 
 
-def create_example_graph(mean_centered = True):
+def create_example_graph(mean_centered=True):
     """
-    Function to create an example EmbeddedGraph object. Helpful for testing.
+    Function to create an example ``EmbeddedGraph`` object. Helpful for testing.
 
     Returns:
-        EmbeddedGraph: An example EmbeddedGraph object.
+        EmbeddedGraph: An example ``EmbeddedGraph`` object.
 
     """
     graph = EmbeddedGraph()
 
-    graph.add_vertex('A', 1, 2)
-    graph.add_vertex('B', 3, 4)
-    graph.add_vertex('C', 5, 7)
-    graph.add_vertex('D', 3, 6)
-    graph.add_vertex('E', 4, 3)
-    graph.add_vertex('F', 4, 5)
+    graph.add_node('A', 1, 2)
+    graph.add_node('B', 3, 4)
+    graph.add_node('C', 5, 7)
+    graph.add_node('D', 3, 6)
+    graph.add_node('E', 4, 3)
+    graph.add_node('F', 4, 5)
 
     graph.add_edge('A', 'B')
     graph.add_edge('B', 'C')
     graph.add_edge('B', 'D')
     graph.add_edge('B', 'E')
     graph.add_edge('C', 'D')
     graph.add_edge('E', 'F')
@@ -349,17 +355,17 @@
 if __name__ == "__main__":
     # Example usage of the EmbeddedGraph class
 
     # Create an instance of the EmbeddedGraph class
     graph = EmbeddedGraph()
 
     # Add vertices with their coordinates
-    graph.add_vertex('A', 1, 2)
-    graph.add_vertex('B', 3, 4)
-    graph.add_vertex('C', 5, 6)
+    graph.add_node('A', 1, 2)
+    graph.add_node('B', 3, 4)
+    graph.add_node('C', 5, 6)
 
     # Add edges between vertices
     graph.add_edge('A', 'B')
     graph.add_edge('B', 'C')
 
     # Get coordinates of a vertex
     coords = graph.get_coordinates('A')
@@ -368,8 +374,8 @@
     # Set new coordinates for a vertex
     graph.set_coordinates('A', 7, 8)
     coords = graph.get_coordinates('A')
     print(f'New coordinates of A: {coords}')
 
     # Get the bounding box of the vertex coordinates
     bbox = graph.get_bounding_box()
-    print(f'Bounding box: {bbox}')
+    print(f'Bounding box: {bbox}')
```

### Comparing `ect-0.1.3/pyproject.toml` & `ect-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ect"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Liz Munch", email="muncheli@msu.edu" },
 ]
 description = "A python package for computing the Euler Characteristic Transform"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,14 +12,15 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = ["numpy",
             "networkx",
             "matplotlib",
             "numba",
+            "scipy"
             ]
 
 [tool.setuptools.packages.find]
 where = ["ect"]
 
 
 [project.urls]
```

### Comparing `ect-0.1.3/tests/test_ect_graph.py` & `ect-0.1.4/tests/test_ect_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,31 +25,33 @@
 
         myect = ect_graph.ECT(num_dirs, num_thresh)
 
         # At this point, there shouldn't be a radius set 
         self.assertIs( myect.bound_radius, None)
 
         # Try to calculate the ECC without a radius set
-        myect.calculateECC(G, 0, tightbbox=True)
+        myect.calculateECC(G, 0, bound_radius=None)
 
-        # Try to calculate the ECC without a radius set.
+        # Try to calculate the ECC with a negative radius.
         # It should throw an error.
         with self.assertRaises(ValueError):  
-            myect.calculateECC(G, 0, tightbbox=False)
+            myect.calculateECC(G, 0, bound_radius= -1)
 
         # Try to calculate the ECC with tightbbox set to True 
         # This should  work fine 
-        ecc = myect.calculateECC(G, 0, tightbbox=True)
+        ecc = myect.calculateECC(G, 0, bound_radius=None)
         self.assertEqual( len(ecc), num_thresh)
 
         # Now set the bounding radius 
         r = G.get_bounding_radius()
         myect.set_bounding_radius(1.2*r)
-        ecc = myect.calculateECC(G, 0, tightbbox=False)
+        ecc = myect.calculateECC(G, 0, bound_radius=None)
         self.assertEqual( len(ecc), num_thresh)
 
+        # TODO: write a test where we check that if None is passed and the radius is set internally, it will use that one.
+
 
     
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ect-0.1.3/tests/test_embed_graph.py` & `ect-0.1.4/tests/test_embed_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 class TestEmbeddedGraph(unittest.TestCase):
     def test_example_graph(self):
         # Make sure we can build a grpah in the first place
         G = embed_graph.create_example_graph()
         self.assertEqual( len(G.nodes), 6)  # assuming my_function squares its input
 
 
-    def test_add_vertex(self):
+    def test_add_node(self):
         # Make sure adding a vertex updates the coordiantes list 
         G = embed_graph.create_example_graph()
-        G.add_vertex('G', 1, 2)
+        G.add_node('G', 1, 2)
         self.assertEqual( len(G.nodes), 7)
         self.assertEqual( len(G.coordinates), 7)
 
     def test_add_edge(self):
         # Make sure adding an edge updates the edge list
         G = embed_graph.create_example_graph()
         G.add_edge('A', 'B')
@@ -25,14 +25,20 @@
 
     def test_get_coordinates(self):
         # Make sure we can get the coordinates of a vertex
         G = embed_graph.create_example_graph(mean_centered=False)
         coords = G.get_coordinates('A')
         self.assertEqual( coords, (1, 2))
 
+    def test_coords_list(self):
+        # Make sure the keys in the coordinates list are the same as the nodes
+        G = embed_graph.create_example_graph(mean_centered=False)
+        self.assertEqual( len(G.nodes), len(G.coordinates))
+        self.assertEqual( set(G.nodes), set(G.coordinates.keys()))
+
     def test_mean_centered_coordinates(self):
         # Make sure the mean centered coordinates are correct
         G = embed_graph.create_example_graph(mean_centered=False)
         G.set_mean_centered_coordinates()
         x_coords = [x for x, y in G.coordinates.values()]
 
         self.assertAlmostEqual( np.average(x_coords), 0, places = 1)
```

