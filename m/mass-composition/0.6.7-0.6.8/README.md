# Comparing `tmp/mass_composition-0.6.7.tar.gz` & `tmp/mass_composition-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.6.7.tar", max compression
+gzip compressed data, was "mass_composition-0.6.8.tar", max compression
```

## Comparing `mass_composition-0.6.7.tar` & `mass_composition-0.6.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1069 2024-05-19 07:57:49.357014 mass_composition-0.6.7/LICENSE
--rw-r--r--   0        0        0     3491 2024-05-19 07:57:49.357014 mass_composition-0.6.7/README.md
--rw-r--r--   0        0        0      360 2024-05-19 07:57:49.757016 mass_composition-0.6.7/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    14000 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     7742 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41619 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    64001 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19483 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0     7737 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     4838 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/sklearn.py
--rw-r--r--   0        0        0     1717 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-19 07:57:49.761016 mass_composition-0.6.7/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2123 2024-05-19 07:57:49.765016 mass_composition-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 mass_composition-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 13:04:51.766404 mass_composition-0.6.8/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-28 13:04:51.766404 mass_composition-0.6.8/README.md
+-rw-r--r--   0        0        0      360 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    14000 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     7742 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    43477 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    64001 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19483 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     7737 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     4838 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/sklearn.py
+-rw-r--r--   0        0        0     1717 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-28 13:04:52.174412 mass_composition-0.6.8/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2123 2024-05-28 13:04:52.178412 mass_composition-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 mass_composition-0.6.8/PKG-INFO
```

### Comparing `mass_composition-0.6.7/LICENSE` & `mass_composition-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/README.md` & `mass_composition-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/balance.py` & `mass_composition-0.6.8/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/config/config_read.py` & `mass_composition-0.6.8/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.6.8/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/dag.py` & `mass_composition-0.6.8/elphick/mass_composition/dag.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.6.8/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.6.8/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.6.8/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.6.8/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/flowsheet.py` & `mass_composition-0.6.8/elphick/mass_composition/flowsheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 class Flowsheet:
     def __init__(self, name: str = 'Flowsheet'):
         self.name: str = name
         self.graph: nx.DiGraph = nx.DiGraph()
         self._logger: logging.Logger = logging.getLogger(__class__.__name__)
 
     @classmethod
-    def from_streams(cls, streams: List[Union[Stream, MassComposition]], name: Optional[str] = 'Flowsheet') -> 'Flowsheet':
+    def from_streams(cls, streams: List[Union[Stream, MassComposition]],
+                     name: Optional[str] = 'Flowsheet') -> 'Flowsheet':
         """Instantiate from a list of objects
 
         Args:
             streams: List of MassComposition objects
             name: name of the network
 
         Returns:
@@ -157,14 +158,51 @@
         for node in fs.graph.nodes:
             mc_node = fs.graph.nodes[node]['mc']
             mc_node.inputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.in_edges(node)]
             mc_node.outputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.out_edges(node)]
 
         return fs
 
+    def to_simple(self, node_name: Optional[str] = None) -> 'Flowsheet':
+        """Return the simplified flowsheet"""
+
+        node_name = node_name if node_name is not None else self.name
+
+        # Identify the degree-1 nodes
+        degree_one_nodes = [node for node, degree in self.graph.degree() if degree == 1]
+
+        # Create a subgraph that only includes the degree-1 nodes and their edges
+        subgraph = self.graph.subgraph(degree_one_nodes).copy()
+
+        # Create a new node that represents the "system-internals"
+        system_node = max(self.graph.nodes) + 1  # Ensure the new node has a unique identifier
+        subgraph.add_node(system_node, mc=MCNode(node_id=system_node, node_name=node_name))
+
+        # Connect the degree-one nodes to the "system-internals" node
+        for node in degree_one_nodes:
+            # For in-edges, connect the node to the "system-internals" node
+            for edge in self.graph.in_edges(node, data=True):
+                subgraph.add_edge(system_node, node, **edge[2])
+
+            # For out-edges, connect the "system-internals" node to the node
+            for edge in self.graph.out_edges(node, data=True):
+                subgraph.add_edge(node, system_node, **edge[2])
+
+        # Populate the inputs and outputs properties of the MCNode objects
+        for node in subgraph.nodes:
+            mc_node = subgraph.nodes[node]['mc']
+            mc_node.inputs = [subgraph.edges[edge]['mc'] for edge in subgraph.in_edges(node)]
+            mc_node.outputs = [subgraph.edges[edge]['mc'] for edge in subgraph.out_edges(node)]
+
+        # Create a new Flowsheet from the subgraph
+        fs = self.__class__(name=self.name)
+        fs.graph = subgraph
+
+        return fs
+
     @property
     def balanced(self) -> bool:
         bal_vals: List = [self.graph.nodes[n]['mc'].balanced for n in self.graph.nodes]
         bal_vals = [bv for bv in bal_vals if bv is not None]
         return all(bal_vals)
 
     @property
@@ -219,28 +257,30 @@
         Returns:
             List of MassComposition objects
         """
 
         # Create a dictionary that maps node names to their degrees
         degrees = {n: d for n, d in self.graph.degree()}
 
-        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[u] == 1]
+        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if
+                                                     degrees[u] == 1]
         return res
 
     def get_output_streams(self) -> List[Union[Stream, MassComposition]]:
         """Get the output (product) streams (edge objects)
 
         Returns:
             List of MassComposition objects
         """
 
         # Create a dictionary that maps node names to their degrees
         degrees = {n: d for n, d in self.graph.degree()}
 
-        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[v] == 1]
+        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if
+                                                     degrees[v] == 1]
         return res
 
     def get_column_formats(self, columns: List[str], strip_percent: bool = False) -> Dict[str, str]:
         """
 
         Args:
             columns: The columns to lookup format strings for
```

### Comparing `mass_composition-0.6.7/elphick/mass_composition/layout.py` & `mass_composition-0.6.8/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/mass_composition.py` & `mass_composition-0.6.8/elphick/mass_composition/mass_composition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/mc_node.py` & `mass_composition-0.6.8/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/mc_status.py` & `mass_composition-0.6.8/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.6.8/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/plot.py` & `mass_composition-0.6.8/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/stream.py` & `mass_composition-0.6.8/elphick/mass_composition/stream.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.6.8/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/components.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/interp.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/loader.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/partition.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/size.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/sklearn.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/sklearn.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/utils/viz.py` & `mass_composition-0.6.8/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/elphick/mass_composition/variables.py` & `mass_composition-0.6.8/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.7/pyproject.toml` & `mass_composition-0.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.6.7"
+version = "0.6.8"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
```

### Comparing `mass_composition-0.6.7/PKG-INFO` & `mass_composition-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.6.7
+Version: 0.6.8
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

