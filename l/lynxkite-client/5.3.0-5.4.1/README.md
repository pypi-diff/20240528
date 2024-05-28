# Comparing `tmp/lynxkite_client-5.3.0.tar.gz` & `tmp/lynxkite_client-5.4.1.tar.gz`

## Comparing `lynxkite_client-5.3.0.tar` & `lynxkite_client-5.4.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/test.sh
--rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/managed_tests/run.sh
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/managed_tests/test_start_stop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/__init__.py
--rw-r--r--   0        0        0    79539 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/kite.py
--rw-r--r--   0        0        0   175339 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/operations.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/api_test_in_docker.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/strings.csv
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_boxpath.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_cleaner.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_download.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_escaping_strings.py
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_external_computation.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_hive_export.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_pandas_conversion.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_spark_conversion.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_sql_shorthand.py
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_subworkspace_decorator.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_tutorials.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace.py
--rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_builder.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_decorator.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_with_side_effects.py
--rw-r--r--   0        0        0  2077488 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/03_Airlines_Edge.csv
--rw-r--r--   0        0        0   771231 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/03_Airlines_Vertex.csv
--rw-r--r--   0        0        0   236358 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/beno_facebook_edges.csv
--rw-r--r--   0        0        0    53472 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/beno_facebook_vertices.csv
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/tutorial-02-test.yaml
--rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/tutorial-03-test.yaml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/.gitignore
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/README.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/test.sh
+-rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/managed_tests/run.sh
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/managed_tests/test_start_stop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/src/lynx/__init__.py
+-rw-r--r--   0        0        0    78809 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/src/lynx/kite.py
+-rw-r--r--   0        0        0    78873 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/src/lynx/kite.py-bak
+-rw-r--r--   0        0        0   189872 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/src/lynx/operations.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/api_test_in_docker.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/strings.csv
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_boxpath.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_cleaner.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_download.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_escaping_strings.py
+-rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_external_computation.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_hive_export.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_pandas_conversion.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_spark_conversion.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_sql_shorthand.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_subworkspace_decorator.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_tutorials.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_workspace.py
+-rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_workspace_builder.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_workspace_decorator.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/test_workspace_with_side_effects.py
+-rw-r--r--   0        0        0  2077488 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/03_Airlines_Edge.csv
+-rw-r--r--   0        0        0   771231 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/03_Airlines_Vertex.csv
+-rw-r--r--   0        0        0   236358 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/beno_facebook_edges.csv
+-rw-r--r--   0        0        0    53472 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/beno_facebook_vertices.csv
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/tutorial-02-test.yaml
+-rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/tests/data/tutorial-03-test.yaml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/.gitignore
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/pyproject.toml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 lynxkite_client-5.4.1/PKG-INFO
```

### Comparing `lynxkite_client-5.3.0/managed_tests/test_start_stop.py` & `lynxkite_client-5.4.1/managed_tests/test_start_stop.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/src/lynx/kite.py` & `lynxkite_client-5.4.1/src/lynx/kite.py-bak`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 import inspect
 import re
 import itertools
 from collections import deque, defaultdict, Counter
 from typing import (Dict, List, Union, Callable, Any, Tuple, Iterable, Set, NewType, Iterator,
                     TypeVar, Optional, Collection, TYPE_CHECKING)
 import requests
-from tempfile import NamedTemporaryFile, TemporaryDirectory, mkstemp
+from tempfile import NamedTemporaryFile, TemporaryDirectory
 import textwrap
-import shutil
 import socketserver
 import lynx.operations
 if TYPE_CHECKING:
   from pyspark.sql import SparkSession
 
 
 if sys.version_info.major < 3 or (sys.version_info.major == 3 and sys.version_info.minor < 6):
@@ -354,25 +353,14 @@
     self._password = password
     self._certfile = certfile
     self._oauth_token = oauth_token
     self._signed_token = signed_token
     self._session = None
     self._pid = None
     self._operation_names: List[str] = []
-    self._import_box_names: List[str] = [
-        'importCSV', 'importJDBC', 'importJSON',
-        'importORC', 'importParquet', 'importFromHive',
-        'importAVRO', 'importDelta',
-        'importFromNeo4j']
-    self._export_box_names: List[str] = [
-        'exportToCSV', 'exportToJSON', 'exportToParquet',
-        'exportToJDBC', 'exportToORC', 'exportToHive',
-        'exportToAVRO', 'exportToDelta',
-        'exportVertexAttributesToNeo4j', 'exportEdgeAttributesToNeo4j',
-        'exportGraphToNeo4j']
     self._box_catalog = box_catalog  # TODO: create standard offline box catalog
 
     self._lynxkite = None
     if spark:
       assert address is None, \
           'Do not specify connection parameters when this class is responsible for starting LynxKite.'
       if LynxKite._managed:
@@ -388,26 +376,22 @@
 
   def home(self) -> str:
     return f'Users/{self.username()}/'
 
   def operation_names(self) -> List[str]:
     if not self._operation_names:
       box_names = self.box_catalog().box_names()
-      self._operation_names = box_names + self.import_operation_names() + self.export_operation_names()
+      self._operation_names = box_names + self.extra_operation_names()
     return self._operation_names
 
-  def import_operation_names(self) -> List[str]:
-    '''When we use an import operation instead of an import box,
-    "run import" will be triggered automatically.'''
-    return [name + 'Now' for name in self._import_box_names]
-
-  def export_operation_names(self) -> List[str]:
-    '''When we use an export operation instead of an export box,
-    the export will be triggered automatically. '''
-    return [name + 'Now' for name in self._export_box_names]
+  def extra_operation_names(self) -> List[str]:
+    '''Synthetic operations that only exist in the API.'''
+    return [
+      n + 'Now' for n in self.box_catalog().box_names()
+      if n.startswith('import') or n.startswith('export')]
 
   def box_catalog(self) -> BoxCatalog:
     if not self._box_catalog:
       bc = self._ask(
           '/ajax/boxCatalog',
           dict(ref=dict(top='', customBoxStack=[]))).boxes
       boxes = {}
@@ -424,25 +408,25 @@
 
     def add_box_with_inputs(box_name, args, kwargs):
       inputs = _to_input_map(box_name, self.box_catalog().inputs(box_name), args)
       box = _new_box(self.box_catalog(), self, box_name, inputs=inputs, parameters=kwargs)
       return box
 
     def f(*args, **kwargs):
-      if name in self.import_operation_names():
+      if name.startswith('import') and name.endswith('Now'):
         real_name = name[:-len('Now')]
         box = add_box_with_inputs(real_name, args, kwargs)
         # If it is an import operation, we trigger the import here,
         # and return the modified (real) import box.
         box_json = box.to_json(
             id_resolver=lambda _: 'untriggered_import_box', workspace_root='', subworkspace_path='')
         import_result = self._send('/ajax/importBox', {'box': box_json})
         box.parameters['imported_table'] = import_result.guid
         box.parameters['last_settings'] = import_result.parameterSettings
-      elif name in self.export_operation_names():
+      elif name.startswith('export') and name.endswith('Now'):
         # If it is an export operation, we trigger the export here.
         box = getattr(self, name[:-len('Now')])(*args, **kwargs)
         box.trigger()
       else:
         box = add_box_with_inputs(name, args, kwargs)
       return box
 
@@ -974,20 +958,20 @@
   '''
 
   def __init__(self, box: 'Box', output_plug_name: str) -> None:
     self.output_plug_name = output_plug_name
     self.box = box
 
   def operation_names(self):
-    return self.box.bc.box_names() + self.box.lk.export_operation_names()
+    return self.box.bc.box_names() + self.box.lk.extra_operation_names()
 
   def __getattr__(self, name: str) -> Callable:
 
     def f(**kwargs):
-      if name in self.box.lk.export_operation_names():
+      if name.startswith('export') and name.endswith('Now'):
         export_box = getattr(self, name[:-len('Now')])(**kwargs)
         export_box.trigger()
         return export_box
       else:
         inputs = self.box.bc.inputs(name)
         # This chaining syntax is only allowed for boxes with exactly one input.
         assert len(inputs) > 0, '{} does not have an input'.format(name)
@@ -1525,16 +1509,14 @@
         {str(i + 1): inputs[i] for i in range(len(inputs))}, parameters, 'table', manual_box_id)
     self.fn = fn
     self.args = args
 
   def _trigger_in_ws(self, wsname: str, box: str, stack: List[str]) -> None:
     lk = self.lk
 
-    tmpfile_list: List[str] = []
-
     with _LKTableContext(lk) as ctx:
       # Find inputs.
       resp = lk.get_workspace(wsname, stack)
       boxes = {b.id: b for b in resp.workspace.boxes}
       input_tables = [getattr(boxes[box].inputs, str(i + 1)) for i in range(len(self.inputs))]
       states = {(o.boxOutput.boxId, o.boxOutput.id): o.stateId for o in resp.outputs}
       input_states = [states[t.boxId, t.id] for t in input_tables]
@@ -1791,15 +1773,16 @@
     first. So we use their inputs as their representatives in the dependency calculation.
     '''
     box = self.base
     if any([box.is_box('output'),
             box.is_box('input') and self.stack,
             box.is_box('computeInputs'),
             box.is_box('saveToSnapshot'),
-            isinstance(box, AtomicBox) and box.operation in box.lk._export_box_names]):
+            isinstance(box, AtomicBox) and box.operation in ['exportToParquetNow']]):
+            # isinstance(box, AtomicBox) and box.operation.startswith('export') and box.operation.endswith('Now')]):
       parents = self.parents()
       assert len(parents) == 1, f'Cannot follow parent chain for {box}'
       return parents[0].dependency_representative()
     else:
       return self
 
   def to_dict(self):
@@ -1845,15 +1828,15 @@
     return dag
 
 
 class SideEffectCollector:
 
   AUTO: 'SideEffectCollector'  # For @subworkspace.
 
-  def __init__(self):
+  def __init__(self) -> None:
     self.top_level_side_effects: List[Box] = []
 
   def add_box(self, box: Box) -> None:
     self.top_level_side_effects.append(box)
 
   def all_triggerables(self) -> Iterable[BoxPath]:
     for box in self.top_level_side_effects:
```

### Comparing `lynxkite_client-5.3.0/src/lynx/operations.py` & `lynxkite_client-5.4.1/src/lynx/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 ''' Python documentation for the operations in Lynxkite.
 This document has been automatically generated.
 '''
 
+
 def addConstantEdgeAttribute(name, value, type):
   '''  Adds an attribute with a fixed value to every edge.
 
   :param name:   The new attribute will be created under this name.
   :param value:   The attribute value. Should be a number if *Type* is set to `number`.
   :param type:   The operation can create either `number` (numeric) or `String` typed attributes.
   '''
 
+
 def addConstantVertexAttribute(name, value, type):
   '''  Adds an attribute with a fixed value to every vertex.
 
   :param name:   The new attribute will be created under this name.
   :param value:   The attribute value. Should be a number if *Type* is set to `number`.
   :param type:   The operation can create either `number` or `String` typed attributes.
   '''
 
+
 def addPopularityXSimilarityOptimizedEdges(externaldegree, internaldegree, exponent, seed):
   '''  Experimental Feature
 
 
   Creates a graph with given amount of vertices and average degrees. The edges
   will follow a power-law - also known as scale-free - distribution and have
   high clustering. Vertices get two edge attributes called "radial" and
@@ -41,26 +44,29 @@
   :param internaldegree:   The average number of edges created between older vertices whenever a new vertex
      is added to the growing graph.
   :param exponent:   The exponent of the power-law degree distribution. Values can be 0.5 - 1, endpoints excluded.
   :param seed:   The random seed.
     +
   '''
 
+
 def addRandomEdgeAttribute():
   '''
 
 
   '''
 
+
 def addRandomVertexAttribute():
   '''
 
 
   '''
 
+
 def addRankAttribute(rankattr, keyattr, order):
   '''  Creates a new vertex attribute that is the *rank* of the vertex when ordered by the key
   attribute. Rank 0 will be the vertex with the highest or lowest key attribute value
   (depending on the direction of the ordering). `String` attributes will be ranked
   alphabetically.
 
   This operation makes it easy to find the top (or bottom) N vertices by an attribute.
@@ -70,52 +76,57 @@
   :param keyattr:   The attribute to rank by.
   :param order:   With *ascending* ordering rank 0 belongs to the vertex with the minimal key attribute value or
     the vertex that is at the beginning of the alphabet.
     With *descending* ordering rank 0 belongs to the vertex with the maximal key attribute value or
     the vertex that is at the end of the alphabet.
   '''
 
+
 def addReversedEdges(distattr):
   '''  For every A→B edge adds a new B→A edge, copying over the attributes of the original.
   Thus this operation will double the number of edges in the graph.
 
   Using this operation you end up with a graph with symmetric edges: if A→B exists then
   B→A also exists. This is the closest you can get to an "undirected" graph.
 
   Optionally, a new edge attribute (a 'distinguishing attribute') will be created so that you can
   tell the original edges from the new edges after the operation. Edges where this attribute is 0
   are original edges; edges where this attribute is 1 are new edges.
 
   :param distattr:   The name of the distinguishing edge attribute; leave it empty if the attribute should not be created.
   '''
 
+
 def aggregateEdgeAttributeGlobally(prefix):
   '''  Aggregates edge attributes across the entire graph into one graph attribute for each attribute.
   For example you could use it to calculate the average call duration across an entire call dataset.
 
   :param prefix:   Save the aggregated values with this prefix.
   '''
 
+
 def aggregateEdgeAttributeToVertices(prefix, direction):
   '''  Aggregates an attribute on all the edges going in or out of vertices.
   For example it can calculate the average duration of calls for each person in a call dataset.
 
   :param prefix:   Save the aggregated attributes with this prefix.
   :param direction:   - `incoming edges`: Aggregate across the edges coming in to each vertex.
      - `outgoing edges`: Aggregate across the edges going out of each vertex.
      - `all edges`: Aggregate across all the edges going in or out of each vertex.
   '''
 
+
 def aggregateFromSegmentation(prefix):
   '''  Aggregates vertex attributes across all the segments that a vertex in the base graph belongs to.
   For example, it can calculate the average size of cliques a person belongs to.
 
   :param prefix:   Save the aggregated attributes with this prefix.
   '''
 
+
 def aggregateOnNeighbors(prefix, direction):
   '''  Aggregates across the vertices that are connected to each vertex. You can use
   the `Aggregate on` parameter to define how exactly this aggregation will take
   place: choosing one of the 'edges' settings can result in a neighboring
   vertex being taken into account several times (depending on the number of edges between
   the vertex and its neighboring vertex); whereas choosing one of the 'neighbors' settings
   will result in each neighboring vertex being taken into account once.
@@ -136,28 +147,31 @@
        that have an incoming edge from A.
      - `all neighbors`: For each vertex A, aggregate across those vertices
        that either have an outgoing edge to or an incoming edge from A.
      - `symmetric neighbors`: For each vertex A, aggregate across those vertices
        that have both an outgoing edge to and an incoming edge from A.
   '''
 
+
 def aggregateToSegmentation():
   '''  Aggregates vertex attributes across all the vertices that belong to a segment.
   For example, it can calculate the average age of each clique.
 
 
   '''
 
+
 def aggregateVertexAttributeGlobally(prefix):
   '''  Aggregates vertex attributes across the entire graph into one graph attribute for each attribute.
   For example you could use it to calculate the average age across an entire dataset of people.
 
   :param prefix:   Save the aggregated values with this prefix.
   '''
 
+
 def anchor(description, parameters):
   '''  This special box represents the workspace itself. There is always exactly one instance of it. It
   allows you to control workspace-wide settings as parameters on this box. It can also serve to anchor
   your workspace with a high-level description.
 
   :param description:   An overall description of the purpose of this workspace.
   :param parameters:   Workspaces containing output boxes can be used as <<custom-boxes, custom boxes>> in other
@@ -167,38 +181,41 @@
     Parameters can also be used as workspace-wide constants. For example if you want to import
     `accounts-2017.csv` and `transactions-2017.csv`, you could create a `date` parameter with default
     value set to `2017` and import the files as `accounts-$date.csv` and `transactions-$date.csv`. (Make
     sure to mark these parametric file names as <<parametric-parameters, parametric>>.)
     This makes it easy to change the date for all imported files at once later.
   '''
 
+
 def approximateClusteringCoefficient(name, bits):
   '''  Scalable algorithm to calculate the approximate local
   `clustering coefficient <http://en.wikipedia.org/wiki/Clustering_coefficient>`_
   attribute for every vertex. It quantifies how close the
   vertex's neighbors are to being a clique. In practice a high (close to
   1.0) clustering coefficient means that the neighbors of a vertex are
   highly interconnected, 0.0 means there are no edges between the
   neighbors of the vertex.
 
   :param name:   The new attribute will be created under this name.
   :param bits:   This algorithm is an approximation. This parameter sets the trade-off between
     the quality of the approximation and the memory and time consumption of the algorithm.
   '''
 
+
 def approximateEmbeddedness(name, bits):
   '''  Scalable algorithm to calculate the approximate overlap size of vertex neighborhoods
   along the edges. If an A→B edge has an embeddedness of `N`, it means A and B have
   `N` common neighbors. The approximate embeddedness is undefined for loop edges.
 
   :param name:   The new attribute will be created under this name.
   :param bits:   This algorithm is an approximation. This parameter sets the trade-off between
     the quality of the approximation and the memory and time consumption of the algorithm.
   '''
 
+
 def bundleVertexAttributesIntoAVector(output, elements):
   '''  Bundles the chosen `number` and `Vector[number]` attributes into one `Vector` attribute.
   By default, LynxKite puts the numeric attributes after each other in alphabetical order and
   then concatenates the Vector attributes to the resulting Vector in alphabetical
   order as well. The resulting attribute is undefined where any of the input attributes
   is undefined.
 
@@ -207,46 +224,50 @@
 
   |
 
   :param output:   The new attribute will be created under this name.
   :param elements:   The attributes you would like to bundle into a Vector.
   '''
 
+
 def checkCliques(selected, bothdir):
   '''  Validates that the segments of the segmentation are in fact cliques.
 
   Creates a new `invalid_cliques` graph attribute, which lists non-clique segment IDs up to a certain number.
 
   :param selected:   The validation can be restricted to a subset of the segments, resulting in quicker operation.
   :param bothdir:   Whether edges have to exist in both directions between all members of a clique.
   '''
 
+
 def classifyWithModel(name, model):
   '''  Creates classifications from a model and vertex attributes of the graph. For the classifications
   with nominal outputs, an additional probability is created to represent the corresponding
   outcome probability.
 
   :param name:   The new attribute of the classification will be created under this name.
   :param model:   The model used for the classifications and a mapping from vertex attributes to the model's
     features.
     +
     Every feature of the model needs to be mapped to a vertex attribute.
   '''
 
-def coloring(name):
+
+def findVertexColoring(name):
   '''  Finds a coloring of the vertices of the graph with no two neighbors with the same color. The colors are represented by
   numbers. Tries to find a coloring with few colors.
 
   Vertex coloring is used in scheduling problems to distribute resources among parties which simultaneously
   and asynchronously request them.
   https://en.wikipedia.org/wiki/Graph_coloring
 
   :param name:   The new attribute will be created under this name.
   '''
 
+
 def combineSegmentations(name, segmentations):
   '''  Creates a new segmentation from the selected existing segmentations.
   Each new segment corresponds to one original segment from each of the original
   segmentations, and the new segment is the intersection of all the corresponding
   segments. We keep non-empty resulting segments only. Edges between segmentations
   are discarded.
 
@@ -254,25 +275,27 @@
 
    - A
 
   :param name:   The new segmentation will be saved under this name.
   :param segmentations:   The segmentations to combine. Select two or more.
   '''
 
+
 def comment(comment):
   '''  Adds a comment to the workspace. As with any box, you can freely place your comment anywhere on the
   workspace. Adding comments does not have any effect on the computation but can potentially make your
   workflow easier to understand for others -- or even for your future self.
 
   `Markdown <https://en.wikipedia.org/wiki/Markdown#Example>`_ can be used to present formatted text or
   embed links and images.
 
   :param comment:   Markdown text to be displayed in the workspace.
   '''
 
+
 def compareSegmentationEdges(golden, test):
   '''  Compares the edge sets of two segmentations and computes *precision* and *recall*.
   In order to make this work, the edges of the both segmentation graphs should be
   matchable against each other. Therefore, this operation only allows comparing
   segmentations which were created using the <<Use base graph as segmentation>> operation
   from the same graph. (More precisely, a one to one correspondence is needed between
   the vertices of both segmentations and the base graph.)
@@ -280,25 +303,27 @@
   You can use this operation for example to evaluate different colocation results against
   a reference result.
 
   :param golden:   Segmentation containing the golden edges.
   :param test:   Segmentation containing the test edges.
   '''
 
+
 def computeAssortativity(name, attr):
   '''  Assortativity is the correlation in the values of an attribute
   along the edges of the graph. A high assortativity means connected vertices
   often have similar attribute values.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Assortativity.html>`_ implementation.
 
   :param name:   The new graph attribute will be created under this name.
   :param attr:   The attribute in which you are interested in correlations along the edges.
   '''
 
+
 def computeCentrality(name, algorithm, direction, weight, samples, maxdiameter, bits):
   '''  Calculates a centrality metric for every vertex. Higher centrality means that
   the vertex is more embedded in the graph. Multiple different centrality measures have been defined
   in the literature. You can choose the specific centrality measure as a parameter to this operation.
 
   :param name:   The new attribute will be created under this name.
   :param algorithm:   - **Average distance**
@@ -322,37 +347,40 @@
   :param bits:   Some centrality algorithms (harmonic, Lin, and average distance) are approximations.
     This parameter sets the trade-off between
     the quality of the approximation and the memory and time consumption of the algorithm.
     In most cases the default value is good enough. On very large graphs it may help to use
     a lower number in order to speed up the algorithm or meet memory constraints.
   '''
 
+
 def computeClusteringCoefficient(name):
   '''  Calculates the local
   `clustering coefficient <http://en.wikipedia.org/wiki/Clustering_coefficient>`_
   attribute for every vertex. It quantifies how close the
   vertex's neighbors are to being a clique. In practice a high (close to
   1.0) clustering coefficient means that the neighbors of a vertex are
   highly interconnected, 0.0 means there are no edges between the
   neighbors of the vertex.
 
   :param name:   The new attribute will be created under this name.
   '''
 
+
 def computeCoverageOfSegmentation(name, weight):
   '''  Computes a scalar for a non-overlapping segmentation.
   Coverage is the fraction of edges that connect vertices within the same segment.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Coverage.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   :param weight:   An edge attribute can be used to weight the edges in the coverage computation.
   '''
 
+
 def computeDegree(name, direction):
   '''  For every vertex, this operation calculates either the number of edges it is connected to
   or the number of neighboring vertices it is connected to.
   You can use the `Count` parameter to control this calculation:
   choosing one of the 'edges' settings can result in a neighboring
   vertex being counted several times (depending on the number of edges between
   the vertex and the neighboring vertex); whereas choosing one of the 'neighbors' settings
@@ -372,14 +400,15 @@
        that have an incoming edge from A.
      - `all neighbors`: For each vertex A, count those vertices
        that either have an outgoing edge to or an incoming edge from A.
      - `symmetric neighbors`: For each vertex A, count those vertices
        that have both an outgoing edge to and an incoming edge from A.
   '''
 
+
 def computeDiameter(name, max_error):
   '''  The diameter of a graph is the maximal shortest-distance path length
   between two vertices. All vertex pairs are at most this far from each
   other.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Diameter.html>`_
   implementation.
@@ -388,14 +417,15 @@
   :param max_error:   Set to 0 to get the exact diameter. This may require a lot of computation, however.
     +
     Set to a value greater than 0 to use a faster computation that gives lower and
     upper bounds on the diameter. With 0.1 maximum relative error, for example, the
     upper bound will be no more than 10% greater than the true diameter.
   '''
 
+
 def computeDispersion(name):
   '''  Calculates the extent to which two people's mutual friends are not themselves well-connected.
   The dispersion attribute for an A→B edge is the number of pairs of nodes that are both
   connected to A and B but are not directly connected to each other.
 
   Dispersion ignores edge directions.
 
@@ -405,14 +435,15 @@
   A normalized dispersion metric is also generated by this operation. This is normalized against the
   embeddedness of the edge with the formula recommended in the cited article.
   (_disp(u,v)^0.61^/(emb(u,v)+5)_) It does not necessarily fall in the _(0,1)_ range.
 
   :param name:   The new edge attribute will be created under this name.
   '''
 
+
 def computeDistanceViaShortestPath(name, edge_distance, starting_distance, iterations):
   '''  Calculates the length of the shortest path from a given set of vertices for every vertex.
   To use this operation, a set of starting _v~i~_ vertices has to be specified, each with
   a starting distance _sd(v~i~)_. Edges represent a unit distance by default, but this
   can be overridden using an attribute. This operation will compute for each vertex
   _v~i~_ the smallest distance from a starting vertex, also counting the starting
   distance of the starting vertex: _d(v~i~)
@@ -425,25 +456,27 @@
   :param starting_distance:   A numeric attribute that specifies the initial distances of the vertices that we
     consider already reachable before starting this operation. (In the above example,
     specify this for the elements of the starting set, and leave this undefined for
     the rest of the vertices.)
   :param iterations:   The maximum number of edges considered for a shortest-distance path.
   '''
 
+
 def computeEdgeCutOfSegmentation(name, weight):
   '''  Computes a scalar for a non-overlapping segmentation.
   Edge cut is the total weight of the edges going between different segments.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1EdgeCut.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   :param weight:   An edge attribute can be used as edge weight.
   '''
 
+
 def computeEffectiveDiameter(name, ratio, algorithm, bits, approximations):
   '''  The effective diameter is a distance within which a given portion
   of vertices can be found from each other.
 
   For example, at most
   `six degrees of separation <https://en.wikipedia.org/wiki/Six*degrees*of_separation>`_
   are between most people on Earth. There may be hermits and lost tribes
@@ -462,21 +495,23 @@
   :param algorithm:   Whether to compute the effective diameter exactly (slower) or approximately (faster).
   :param bits:   For estimating the effective diameter the
     http://www.cs.cmu.edu/~christos/PUBLICATIONS/kdd02-anf.pdf
   :param approximations:   For estimating the effective diameter the
     http://www.cs.cmu.edu/~christos/PUBLICATIONS/kdd02-anf.pdf
   '''
 
+
 def computeEmbeddedness(name):
   '''  `Edge embeddedness <https://arxiv.org/abs/1009.1686>`_ is the overlap size of vertex neighborhoods along
   the edges. If an A→B edge has an embeddedness of `N`, it means A and B have `N` common neighbors.
 
   :param name:   The new attribute will be created under this name.
   '''
 
+
 def computeHubDominance(name):
   '''  Computes the hub dominance metric for each segment in a segmentation.
   The hub dominance of a segment is the highest internal degree in the segment
   divided by the highest *possible* internal degree. (The segment size minus one.)
 
   If a segment has a vertex that is connected to all other vertices in that segment
   then its hub dominance will be 1. This metric is useful for comparing the structures
@@ -488,30 +523,35 @@
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1CoverHubDominance.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   '''
 
+
 def computeHyperbolicEdgeProbability(radial, angular):
   '''  Adds edge attribute *hyperbolic edge probability* based on
   hyperbolic distances between vertices. This indicates
   how likely that edge would be to exist if the input graph was
   probability x similarity-grown.
   On a general level it is a metric of *edge strength*.
   Probabilities are guaranteed to be 0
 
   :param radial:   The vertex attribute to be used as radial coordinates.
     Should not contain negative values.
   :param angular:   The vertex attribute to be used as angular coordinates.
     Values should be 0 - 2 * Pi.
   '''
 
+
 def computeInPython(code, inputs, outputs):
-  '''  Executes custom Python code to define new vertex, edge, or graph attributes.
+  '''  Executes custom Python code to define new vertex, edge, or graph attributes, to transform a table,
+  or to create plots and interactive visualizations.
+
+  **Computing new attributes**
 
   The following example computes two new vertex attributes (`with_title` and `age_squared`),
   two new edge attributes (`score` and `names`), and two new graph_attributes (`hello` and `average_age`).
   (You can try it on the <<Create example graph, example graph>> which
   has the attributes used in this code.)
 
   [source,python]
@@ -520,26 +560,124 @@
 
   :param code:   The Python code you want to run. See the operation description for details.
   :param inputs:   A comma-separated list of attributes that your code wants to use.
     For example, `vs.my_attribute, vs.another_attribute, graph_attributes.last_one`.
   :param outputs:   A comma-separated list of attributes that your code generates.
     These must be annotated with the type of the attribute.
     For example, `vs.my*new*attribute: str, vs.another*new*attribute: float, graph_attributes.also_new: str`.
+    +
+    Set to `matplotlib` or `html` to output a visualization.
   '''
 
+
+def computeInR(code, inputs, outputs):
+  '''  Executes custom R code to define new vertex, edge, or graph attributes, to transform a table,
+  or to create plots and interactive visualizations.
+
+  #### Computing new attributes
+
+  The following example computes two new vertex attributes (`with_title` and `age_squared`),
+  two new edge attributes (`score` and `names`), and two new graph_attributes (`hello` and `average_age`).
+  (You can try it on the <<Create example graph, example graph>> which
+  has the attributes used in this code.)
+
+  [source,r]
+  ----
+  vs$with_title <- paste("The Honorable", vs$name)
+  vs$age_squared <- vs$age ** 2
+  es$score <- es$weight + nchar(es$comment)
+  es$names <- paste("from", vs$name[es$src], "to", vs$name[es$dst])
+  graph_attributes$hello <- tolower(graph_attributes$greeting)
+  graph_attributes$average_age <- mean(vs$age)
+  ----
+
+  `graph_attributes` is an object you can use to get and set graph attributes.
+
+  `vs` (for "**v**ertice**s**") and `es` (for "**e**dge**s**") are both
+  `tibbles <https://tibble.tidyverse.org/reference/tibble.html>`_.
+  You can write natural R code and use the usual APIs and packages to
+  compute new attributes. Dplyr is already imported.
+  `es` can have `src` and `dst` columns which are the indexes of the source and destination
+  vertex for each edge. These can be used to index into `vs` as in the example.
+
+  Assign the new columns to these same data frames to output new vertex or edge attributes.
+
+  When you write this R code, the input data may not be available yet.
+  And you may want to keep building on the output of the box without having
+  to wait for the R code to execute. To make this possible, LynxKite has
+  to know the inputs and outputs of your code without executing it.
+  You specify them through the *Inputs* and *Outputs* parameters.
+  For outputs you must also declare their types.
+
+  The currently supported types for outputs are:
+
+  - `double` to create a `number`-typed attribute or `Double`-typed table column.
+  - `character` to create a `String`-typed attribute or table column.
+  - `integer` to create a `Long`-typed table column.
+  - `vector` to create a `Vector[number]`-typed attribute.
+
+  In the first example we would set:
+
+  - Inputs: `vs.name, vs.age, es.weight, es.comment, es.src, es.dst, graph_attributes.greeting`
+  - Outputs: `vs.with_title: character, vs.age_squared: double, es.score: double, es.names: character, graph_attributes.hello: character, graph_attributes.average_age: double`
+
+  #### Working with vectors
+
+  Vector-typed attributes are stored as list columns in the `vs` and `es` DataFrames.
+
+  To output a vector-typed attribute, you can create a list column or a matrix:
+
+  [source,r]
+  ----
+  # Put the age and its double into a vector.
+  vs$v <- outer(vs$age, c(1, 2))
+  ----
+
+  On the <<Create example graph, example graph>> this would output:
+
+  ----
+                 v
+  0   [20.3, 40.6]
+  1   [18.2, 36.4]
+  2  [50.3, 100.6]
+  3     [2.0, 4.0]
+  ----
+
+  When a vector attribute is your input, it always appears as a list column.
+  You can use https://dplyr.tidyverse.org/articles/rowwise.html[`rowwise()`]
+  to work with it more comfortably.
+
+  [source,r]
+  ----
+  vs <- vs %>%
+    rowwise() %>%
+    mutate(total_v
+
+  :param code:   The R code you want to run. See the operation description for details.
+  :param inputs:   A comma-separated list of attributes that your code wants to use.
+    For example, `vs.my_attribute, vs.another_attribute, graph_attributes.last_one`.
+  :param outputs:   A comma-separated list of attributes that your code generates.
+    These must be annotated with the type of the attribute.
+    For example, `vs.my*new*attribute: character, vs.another*new*attribute: double, graph_attributes.also_new: character`.
+    +
+    Set to `plot` or `html` to output visualizations.
+  '''
+
+
 def computeInputs():
   '''  Triggers the computations for all entities associated with its input.
 
    - For table inputs, it computes the table.
    - For graph inputs, it computes the vertices and edges, all attributes,
      and the same transitively for all segments plus the segmentation links.
 
 
   '''
 
+
 def computeModularityOfSegmentation(name, weight):
   '''  Computes a scalar for a non-overlapping segmentation.
   If the vertices were connected randomly while preserving the degrees,
   a certain fraction of all edges would fall within each segment.
   We subtract this from the observed fraction of edges that fall within
   the segments. Modularity is the total observed difference.
 
@@ -553,15 +691,16 @@
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   :param weight:   An edge attribute can be used to weight the edges instead of just looking at
     edge counts.
   '''
 
-def computePagerank(name, weights, iterations, damping, direction):
+
+def computePageRank(name, weights, iterations, damping, direction):
   '''  Calculates `PageRank <http://en.wikipedia.org/wiki/PageRank>`_ for every vertex.
   PageRank is calculated by simulating random walks on the graph. Its PageRank
   reflects the likelihood that the walk leads to a specific vertex.
 
   Let's imagine a social graph with information flowing along the edges. In this case high
   PageRank means that the vertex is more likely to be the target of the information.
 
@@ -579,14 +718,15 @@
   :param direction:   - `incoming edges`: Simulate random walk in the reverse edge direction.
        Finds the most influential sources.
      - `outgoing edges`: Simulate random walk in the original edge direction.
        Finds the most popular destinations.
      - `all edges`: Simulate random walk in both directions.
   '''
 
+
 def computeSegmentConductance(name, weight):
   '''  Computes the conductance of each segment in a non-overlapping segmentation.
   The conductance of a segment is the number of edges going between the segment
   and the rest of the graph divided by sum of the degrees in the segment or the rest
   of the graph (whichever is smaller).
 
   A high conductance value indicates a segment that is strongly connected to the rest
@@ -600,29 +740,31 @@
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   :param weight:   The definition can be rephrased to apply to weighted graphs. In this case
     the total weight of the cut is compared to the weighted degrees.
   '''
 
+
 def computeSegmentDensity(name):
   '''  Computes the density of each segment in a non-overlapping segmentation.
   The density of a segment is the number of internal edges divided by the
   number of possible internal edges.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1IntrapartitionDensity.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   '''
 
+
 def computeSegmentExpansion(name, weight):
   '''  Computes the expansion of each segment in a non-overlapping segmentation.
   The expansion of a segment is the number of edges going between the segment
-  and the rest of the graph divided by the number of vertices in the segment or 
+  and the rest of the graph divided by the number of vertices in the segment or
   in the rest of the graph (whichever is smaller).
 
   A high expansion value indicates a segment that is strongly connected to the rest
   of the graph. A value over 1 means the vertices in this segment have more than
   one external neighbor on average.
 
   See `Experiments on Density-Constrained Graph Clustering <https://arxiv.org/abs/1112.2143>`_
@@ -632,14 +774,15 @@
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   :param weight:   The definition can be rephrased to apply to weighted graphs. In this case
     the total weight of the cut is compared to the weighted degrees.
   '''
 
+
 def computeSegmentFragmentation(name):
   '''  Computes the fragmentation of each segment in a non-overlapping segmentation.
   The fragmentation of a segment is one minus the ratio of the size of its largest
   component and the whole segment.
 
   A segment that is entirely connected will have a fragmentation of zero.
   If the fragmentation approaches one, it will be made up of smaller and
@@ -647,14 +790,15 @@
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PartitionFragmentation.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   '''
 
+
 def computeSegmentStability(name):
   '''  Computes the stability of each segment in a non-overlapping segmentation.
   A vertex is considered stable if it has more neighbors inside the
   segment than outside. The stability of a segment is the fraction of
   its vertices that are stable.
 
   A high stability value (close to 1) indicates a segment where vertices are
@@ -663,92 +807,101 @@
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1StablePartitionNodes.html>`_
   implementation.
 
   :param name:   This box creates a new vertex attribute on the segmentation by this name.
   '''
 
+
 def connectVerticesOnAttribute(fromattr, toattr):
   '''  Creates edges between vertices that are equal in a chosen attribute. If the source attribute of A
   equals the destination attribute of B, an A→B edge will be generated.
 
   The two attributes must be of the same data type.
 
   For example, if you connect nodes based on the "name" attribute, then everyone called "John
   Smith" will be connected to all the other "John Smiths".
 
   :param fromattr:   An A→B edge is generated when this attribute on A matches the destination attribute on B.
   :param toattr:   An A→B edge is generated when the source attribute on A matches this attribute on B.
   '''
 
+
 def convertEdgeAttributeToNumber(attr):
   '''  Converts the selected `String` typed edge attributes to the `number` type.
 
   The attributes will be converted in-place. If you want to keep the original `String` attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
 
+
 def convertEdgeAttributeToString(attr):
   '''  Converts the selected edge attributes to `String` type.
 
   The attributes will be converted in-place. If you want to keep the original String attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
 
+
 def convertVertexAttributeToNumber(attr):
   '''  Converts the selected `String` typed vertex attributes to the `number` type.
 
   The attributes will be converted in-place. If you want to keep the original `String` attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
 
+
 def convertVertexAttributeToString(attr):
   '''  Converts the selected vertex attributes to `String` type.
 
   The attributes will be converted in-place. If you want to keep the original attributes as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
 
+
 def copyEdgeAttribute(name, destination):
   '''  Creates a copy of an edge attribute.
 
-  :param name: 
+  :param name:
   :param destination:
   '''
 
+
 def copyEdgesToBaseGraph():
   '''  Copies the edges from a segmentation to the base graph. The copy is performed along the links
   between the segmentation and the base graph. If two segments are connected with some
   edges, then each edge will be copied to each pairs of members of the segments.
 
   This operation has a potential to create trillions of edges or more.
   The number of edges created is the sum of the source and destination segment sizes multiplied
   together for each edge in the segmentation.
   It is recommended to drop very large segments before running this computation.
 
 
   '''
 
+
 def copyEdgesToSegmentation():
   '''  Copies the edges from the base graph to the segmentation. The copy is performed along the links
   between the base graph and the segmentation. If a base vertex belongs to no segments, its edges
   will not be found in the result. If a base vertex belongs to multiple segments, its edges will
   have multiple copies in the result.
 
 
   '''
 
+
 def copyGraphAttributeFromOtherGraph(sourceproject, sourcescalarname, destscalarname):
   '''  This operation can take a graph attribute from another graph and copy it
   to the current graph.
 
   It can be useful if we trained a machine learning model in one graph, and would like
   to apply this model in another graph for predicting undefined attribute values.
 
@@ -756,63 +909,70 @@
   :param sourcescalarname:   The name of the graph attribute in the other graph. If it is a simple string, then
     the graph attribute with that name has to be in the root of the other graph. If it is
     a `.`-separated string, then it means a graph attribute in a segmentation of the other graph.
     The syntax for this case is: `seg_1.seg_2.....seg_n.graph_attribute`.
   :param destscalarname:   This will be the name of the copied graph attribute in this graph.
   '''
 
+
 def copyGraphAttribute(name, destination):
   '''  Creates a copy of a graph attribute.
 
-  :param name: 
+  :param name:
   :param destination:
   '''
 
+
 def copySegmentation(name, destination):
   '''  Creates a copy of a segmentation.
 
-  :param name: 
+  :param name:
   :param destination:
   '''
 
+
 def copyVertexAttribute(name, destination):
   '''  Creates a copy of a vertex attribute.
 
-  :param name: 
+  :param name:
   :param destination:
   '''
 
+
 def copyVertexAttributesFromSegmentation(prefix):
   '''  Copies all vertex attributes from the segmentation to the parent.
 
   This operation is only available when each vertex belongs to just one segment.
   (As in the case of connected components, for example.)
 
   :param prefix:   A prefix for the new attribute names. Leave empty for no prefix.
   '''
 
+
 def copyVertexAttributesToSegmentation(prefix):
   '''  Copies all vertex attributes from the parent to the segmentation.
 
   This operation available only when each segment contains just one vertex.
 
   :param prefix:   A prefix for the new attribute names. Leave empty for no prefix.
   '''
 
+
 def correlateTwoAttributes(attra, attrb):
   '''  Calculates the Pearson correlation coefficient of two attributes.
   Only vertices where both attributes are defined are considered.
 
   Note that correlation is undefined if at least one of the
   attributes is a constant.
 
   :param attra:   The correlation of these two attributes will be calculated.
   :param attrb:   The correlation of these two attributes will be calculated.
   '''
 
+
 def createAGraphWithCertainDegrees(size, degrees, algorithm, seed):
   '''  Creates a graph in which the distribution of vertex degrees is as specified.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1StaticDegreeSequenceGenerator.html>`_ implementation.
 
   :param size:   The created graph will have this many vertices.
   :param degrees:   The algorithm will try to ensure that an equal number of vertices will
@@ -823,29 +983,31 @@
       with edge probabilities dependent on vertex "weights".
       See `Efficient Generation of Networks with Given Expected Degrees <http://aric.hagberg.org/papers/miller-2011-efficient.pdf>`_.
     - **https://en.wikipedia.org/wiki/Havel%E2%80%93Hakimi_algorithm
   :param seed:   The random seed.
     +
   '''
 
-def createBarabSiAlbertGraph(size, attachments_per_vertex, connected_at_start, seed):
+
+def createBarabásiAlbertGraph(size, attachments_per_vertex, connected_at_start, seed):
   '''  Creates a random graph using the https://en.wikipedia.org/wiki/Barab%C3%A1si%E2%80%93Albert_model[Barabási–Albert model].
   The vertices are created one by one and connected to a set number of randomly chosen
   previously created vertices. This ensures a skewed degree distribution with "older" vertices
   tending to have a higher degree.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1BarabasiAlbertGenerator.html>`_ implementation.
 
   :param size:   The created graph will have this many vertices.
   :param attachments_per_vertex:   As each vertex is added, it will be connected to this many existing vertices.
   :param connected_at_start:   This many vertices will be connected in a circle at the start of the algorithm.
   :param seed:   The random seed.
     +
   '''
 
+
 def createClusteredRandomGraph(size, clusters, probability_in, probability_out, seed):
   '''  Creates a random graph with a given number of clusters.
   It randomly places each vertex into one of the clusters then adds an edge for each
   vertex pair with the given probabilities.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1ClusteredRandomGraphGenerator.html>`_ implementation.
 
@@ -854,65 +1016,71 @@
     Each vertex will be randomly placed into one of the clusters with equal probability.
   :param probability_in:   The probablity for adding an edge between two vertices if they are in the same cluster.
   :param probability_out:   The probablity for adding an edge between two vertices if they are in different clusters.
   :param seed:   The random seed.
     +
   '''
 
+
 def createDorogovtsevMendesRandomGraph(size, seed):
   '''  Creates a planar random graph with a power-law distribution. Starts with a triangle and in each
   step adds a new node that is connected to the two endpoints of a randomly selected edge.
 
   See `Modern architecture of random graphs: Constructions and correlations <https://arxiv.org/abs/cond-mat/0206467>`_ by Dorogovtsev et al.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1DorogovtsevMendesGenerator.html>`_ implementation.
 
   :param size:   The created graph will have this many vertices.
   :param seed:   The random seed.
     +
   '''
 
-def createEdgesFromCoOccurrence():
+
+def createEdgesFromCooccurrence():
   '''  Connects vertices in the base graph if they co-occur in any segments.
   Multiple co-occurrences will result in multiple parallel edges. Loop edges
   are generated for each segment that a vertex belongs to. The attributes of
   the segment are copied to the edges created from it.
 
   This operation has a potential to create trillions of edges or more.
   The number of edges created is the sum of squares of the segment sizes.
   It is recommended to drop very large segments before running this computation.
 
 
   '''
 
+
 def createEdgesFromSetOverlaps(minoverlap):
   '''  Connects segments with large enough overlaps.
 
   :param minoverlap:   Two segments will be connected if they have at least this many members in common.
   '''
 
-def createErdSRNyiGraph(size, probability, seed):
+
+def createErdősRényiGraph(size, probability, seed):
   '''  Creates a random graph using the https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93R%C3%A9nyi_model[Erdős–Rényi model].
   In this model each pair of vertices is connected independently with the same probability.
   It creates a very uniform graph with no tendency to skewed degree distributions or clustering.
 
   Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1ErdosRenyiGenerator.html>`_ implementation.
 
   :param size:   The created graph will have this many vertices.
   :param probability:   Each pair of vertices is connected with this probability.
   :param seed:   The random seed.
     +
   '''
 
+
 def createExampleGraph():
   '''  Creates small test graph with 4 people and 4 edges between them.
 
 
   '''
 
+
 def createGraphInPython(code, outputs):
   '''  Executes custom Python code to define a graph.
   Ideal for creating complex graphs programmatically and for loading
   datasets in non-standard formats.
 
   The following example creates a small graph with some attributes.
 
@@ -922,14 +1090,33 @@
 
   :param code:   The Python code you want to run. See the operation description for details.
   :param outputs:   A comma-separated list of attributes that your code generates.
     These must be annotated with the type of the attribute.
     For example, `vs.my*new*attribute: str, vs.another*new*attribute: float, graph_attributes.also_new: str`.
   '''
 
+
+def createGraphInR(code, outputs):
+  '''  Executes custom R code to define a graph.
+  Ideal for creating complex graphs programmatically and for loading
+  datasets in non-standard formats.
+
+  The following example creates a small graph with some attributes.
+
+  [source,r]
+  ----
+  vs <- tibble(name
+
+  :param code:   The R code you want to run. See the operation description for details.
+  :param outputs:   A comma-separated list of attributes that your code generates.
+    These must be annotated with the type of the attribute.
+    For example, `vs.my*new*attribute: character, vs.another*new*attribute: double, graph_attributes.also_new: character`.
+  '''
+
+
 def createHyperbolicRandomGraph(size, avg_degree, exponent, temperature, seed):
   '''  Creates a random graph based on randomly placed points on the hyperbolic plane.
   The points corresponding to vertices are placed on a disk.
   If two points are closer than a threshold (by the hyperbolic distance metric),
   an edge will be created between those two vertices.
 
   The motivation for this is to reflect popularity (how close the point is to the center)
@@ -952,15 +1139,17 @@
   :param exponent:   The exponent of the degree distribution.
   :param temperature:   When zero, vertices are connected if they lie within a fixed threshold on the hyperbolic disk.
     Larger values add randomness while trying to preserve the degree distribution.
   :param seed:   The random seed.
     +
   '''
 
-def createLfrRandomGraph(size, avg_degree, max_degree, degree_exponent, min_community, max_community, community_exponent, avg_mixing, seed):
+
+def createLFRRandomGraph(size, avg_degree, max_degree, degree_exponent,
+                         min_community, max_community, community_exponent, avg_mixing, seed):
   '''  LFR stands for Lancichinetti, Fortunato, and Radicchi, the authors of
   `Benchmark graphs for testing community detection algorithms <https://arxiv.org/abs/0805.4770>`_
   and `Benchmarks for testing community detection algorithms on directed and weighted graphs with overlapping communities <https://arxiv.org/abs/0904.3940>`_
   upon which this generator is based.
 
   The LFR random graph features overlapping communities.
   Each vertex is randomized into multiple communities while
@@ -982,14 +1171,15 @@
   :param community_exponent:   The power-law exponent of the desired community size distribution.
     A higher number means a more skewed distribution.
   :param avg_mixing:   What ratio of the neighbors of each vertex should on average be of other communities.
   :param seed:   The random seed.
     +
   '''
 
+
 def createMocnikRandomGraph(size, dimension, density, seed):
   '''  Creates a random graph as described in
   https://www.mocnik-science.net/publications/2015c%20-%20Franz-Benjamin%20Mocnik%20-%20Modelling%20Spatial%20Structures.pdf[Modelling Spatial Structures] by Mocnik et al.
   The model is based on randomly placing the vertices in Euclidean space
   and generating edges with a higher probability for pairs of vertices
   that are closer together.
 
@@ -998,15 +1188,16 @@
   :param size:   The created graph will have this many vertices.
   :param dimension:   The vertices are placed randomly in a space with this many dimensions.
   :param density:   The desired ratio of edges to nodes.
   :param seed:   The random seed.
     +
   '''
 
-def createP2pRandomGraph(size, dense_areas, max_degree, neighborhood_radius, seed):
+
+def createP2PRandomGraph(size, dense_areas, max_degree, neighborhood_radius, seed):
   '''  Creates a random graph using the model described in `A distributed diffusive heuristic for clustering a virtual P2P supercomputer <http://parco.iti.kit.edu/henningm/data/distribClust.pdf>`_ by Gehweiler et al.
 
   The vertices are randomly placed in a 2-dimensional unit square with a torus topology.
   Vertices within a set radius are connected when permitted by the maximum degree constraint.
 
   Some dense circular areas within the unit suqare are picked at the beginning
   and these are populated first. Any remaining vertices are then placed uniformly.
@@ -1020,100 +1211,90 @@
   :param max_degree:   Each vertex will be connected to at most this many neighbors.
   :param neighborhood_radius:   The model works by placing points on the unit square. Points within this radius
     will be connected to each other.
   :param seed:   The random seed.
     +
   '''
 
+
 def createRandomEdges(degree, seed):
   '''  Creates edges randomly, so that each vertex will have a degree uniformly chosen between 0 and
   2 * the provided parameter.
 
   For example, you can create a random graph by first applying operation <<Create vertices>>
   and then creating the random edges.
 
   :param degree:   The degree of a vertex will be chosen uniformly between 0 and 2 * this number.
     This results in generating *number of vertices * average degree* edges.
   :param seed:   The random seed.
     +
   '''
 
-def createScaleFreeRandomEdges(iterations, periterationmultiplier):
+
+def createScalefreeRandomEdges(iterations, periterationmultiplier):
   '''  Creates edges randomly so that the resulting graph is scale-free.
 
   This is an iterative algorithm. We start with one edge per vertex and in each
   iteration the number of edges gets approximately multiplied by
   *Per iteration edge number multiplier*.
 
   :param iterations:   Each iteration increases the number of edges by the specified multiplier.
     A higher number of iteration will result in a more scale-free degree distribution,
     but also a slower performance.
   :param periterationmultiplier:   Each iteration increases the number of edges by the specified multiplier.
     The edge count starts from the number of vertices, so with *N* iterations and *m*
     as the multiplier you will have _m^N^_ edges by the end.
   '''
 
+
 def createVertices(size):
   '''  Creates a new vertex set with no edges. Two attributes are generated: `id` and `ordinal`. `id`
   is the internal vertex ID, while `ordinal` is an index for the vertex: it goes from zero to the
   vertex set size.
 
   :param size:   The number of vertices to create.
   '''
 
+
 def customPlot(plot_code):
   '''  Creates a plot from the input table. The plot can be defined using the
-  `Vegas <https://github.com/vegas-viz/Vegas>`_ plotting API in Scala. This API makes
-  it easy to define `Vega-Lite <https://vega.github.io/vega-lite/>`_ plots in code.
-
-  You code has to evaluate to a `vegas.Vegas` object. For your convenience `vegas._` is already
-  imported. An example of a simple plot would be:
-
-  ```
-  Vegas()
-    .withData(table)
-    .encodeX("name", Nom)
-    .encodeY("age", Quant)
-    .encodeColor("gender", Nom)
-    .mark(Bar)
-  ```
+  `Vega-Lite <https://vega.github.io/vega-lite/docs/>`_ JSON API.
 
-  `Vegas()` is the entry point to the plotting API. You can provide a title if you like: `Vegas("My
-  Favorite Plot")`.
+  The `data` field in the Vega-Lite specification will be automatically filled in
+  by LynxKite, giving you access to the input table. (Limited to 10,000 rows.)
 
-  LynxKite fetches a sample of up to 10,000 rows from your table for the purpose of the plot. This
-  data is made available in the `table` variable (as `Seq[Map[String, Any]]`). `.withData(table)`
-  binds this data to the plot. You can transform the data before plotting if necessary:
+  LynxKite comes with several <<built-ins>>, many of them based on the Custom plot box. You can dive
+  into these custom boxes to see the code used to build them.
 
-  ```
-  val doubled
-
-  :param plot_code:   Scala code for defining the plot.
+  :param plot_code:   The Vega-Lite specification in JSON.
   '''
 
+
 def defineSegmentationLinksFromMatchingAttributes(base_id_attr, seg_id_attr):
   '''  Connect vertices in the base graph with segments based on matching attributes.
 
   This operation can be used (among other things) to create connections between two graphs once
   one has been imported as a segmentation of the other.
   (See <<Use other graph as segmentation>>.)
 
   :param base_id_attr:   A vertex will be connected to a segment if the selected vertex attribute of the vertex
     matches the selected vertex attribute of the segment.
   :param seg_id_attr:   A vertex will be connected to a segment if the selected vertex attribute of the vertex
     matches the selected vertex attribute of the segment.
   '''
 
+
 def deriveColumn(name, value):
   '''  Derives a new column on a table input via an SQL expression. Outputs a table.
 
   :param name:   The name of the new column.
   :param value:   The SQL expression to define the new column.
   '''
 
+
 def deriveEdgeAttribute(output, defined_attrs, expr, persist):
   '''  Generates a new attribute based on existing attributes. The value expression can be
   an arbitrary Scala expression, and it can refer to existing attributes on the edge as if
   they were local variables. It can also refer to attributes of the source and destination
   vertex of the edge using the format `src$attribute` and `dst$attribute`.
 
   For example you can write `weight * scala.math.abs(src$age - dst$age)` to generate a new
@@ -1144,26 +1325,28 @@
       an attribute `income: Double` you would see it as `income: Option
   :param expr:   The Scala expression. You can enter multiple lines in the editor.
   :param persist:   If enabled, the output attribute will be saved to disk once it is calculated. If disabled, the
     attribute will be re-computed each time its output is used. Persistence can improve performance
     at the cost of disk space.
   '''
 
+
 def deriveGraphAttribute(output, expr):
   '''  Generates a new <<graph-attributes, graph attribute>> based on existing graph attributes.
   The value expression can be an arbitrary Scala expression, and it can refer to existing
   graph attributes as if they were local variables.
 
   For example you could derive a new graph attribute as `something_sum / something_count` to get the average
   of something.
 
   :param output:   The new graph attribute will be created under this name.
   :param expr:   The Scala expression. You can enter multiple lines in the editor.
   '''
 
+
 def deriveVertexAttribute(output, defined_attrs, expr, persist):
   '''  Generates a new attribute based on existing vertex attributes. The value expression can be
   an arbitrary Scala expression, and it can refer to existing attributes as if they
   were local variables.
 
   For example you can write `age * 2` to generate a new attribute
   that is the double of the *age* attribute. Or you can write
@@ -1177,65 +1360,98 @@
       an attribute `income: Double` you would see it as `income: Option
   :param expr:   The Scala expression. You can enter multiple lines in the editor.
   :param persist:   If enabled, the output attribute will be saved to disk once it is calculated. If disabled, the
     attribute will be re-computed each time its output is used. Persistence can improve performance
     at the cost of disk space.
   '''
 
+
 def discardEdgeAttributes(name):
   '''  Throws away edge attributes.
 
   :param name:   The attributes to discard.
   '''
 
+
 def discardEdges():
   '''  Throws away all edges. This implies discarding all edge attributes too.
 
 
   '''
 
+
 def discardGraphAttributes(name):
   '''  Throws away graph attributes.
 
   :param name:   The graph attributes to discard.
   '''
 
+
 def discardLoopEdges():
   '''  Discards edges that connect a vertex to itself.
 
 
   '''
 
+
 def discardSegmentation(name):
   '''  Throws away a segmentation value.
 
   :param name:   The segmentation to discard.
   '''
 
+
 def discardVertexAttributes(name):
   '''  Throws away vertex attributes.
 
   :param name:   The vertex attributes to discard.
   '''
 
+
+def embedStringAttribute(attr, save_as, method, model_name, batch_size):
+  '''  Creates a string embedding for the selected edge or vertex attribute.
+  The resulting Vector attribute can be used with other machine learning boxes.
+
+  :param attr:   The String edge or vertex attribute to use as the input.
+  :param save_as:   The new attribute will be created under this name.
+  :param method:   What to use for creating the embedding.
+    To use the OpenAI method, the `OPENAI*API*KEY` environment variable must be set.
+    The other methods rely on local models that can run on your GPU.
+    The models are large and will be downloaded when used for the first time.
+  :param model_name:   Leave empty to use the default model for the selected method.
+    - For OpenAI the default is `text-embedding-3-small`.
+      See the `OpenAI documentation <https://platform.openai.com/docs/guides/embeddings/embedding-models>`_ for available models.
+    - For SentenceTransformers the default is `nomic-ai/nomic-embed-text-v1`.
+      Any model that is loaded with `SentenceTransformer(model_name)` can be used.
+    - For AnglE the default is `WhereIsAI/UAE-Large-V1`.
+      Any model loaded with `AnglE.from_pretrained(model_name)` can be used.
+    - For causal transformers the default is `microsoft/DialoGPT-small`.
+      Any model loaded with `AutoModelForCausalLM.from_pretrained(model_name)` can be used.
+      The `echo embeddings <https://arxiv.org/abs/2402.15449>`_ algorithm is used to generate the sentence embeddings.
+  :param batch_size:   Leave empty to use the default batch size for the selected method.
+    Higher values will use more GPU memory and generate embeddings faster.
+  '''
+
+
 def embedVertices(save_as, iterations, dimensions, walks_per_node, walk_length, context_size):
   '''  Creates a vertex embedding using the
   `PyTorch Geometric implementation <https://pytorch-geometric.readthedocs.io/en/1.4.1/modules/nn.html#torch_geometric.nn.models.Node2Vec>`_
   of the `node2vec <https://arxiv.org/abs/1607.00653>`_ algorithm.
 
   :param save_as:   The new attribute will be created under this name.
   :param iterations:   Number of training iterations.
   :param dimensions:   The size of each embedding vector.
   :param walks_per_node:   Number of random walks collected for each vertex.
   :param walk_length:   Length of the random walks collected for each vertex.
   :param context_size:   The random walks will be cut with a rolling window of this size.
     This allows reusing the same walk for multiple vertices.
   '''
 
-def exportEdgeAttributesToNeo4j(url, username, password, version, labels, keys):
+
+def exportEdgeAttributesToNeo4j(url, username, password, database, version, labels, keys):
   '''  Exports edge attributes from a graph in LynxKite to a
   corresponding graph in `Neo4j <https://neo4j.com/>`_.
 
   The relationships in Neo4j are identified by a key property (or properties).
   You must have a corresponding edge attribute in LynxKite by the same name.
   This will be used to find the right relationship to update in Neo4j.
 
@@ -1246,25 +1462,31 @@
       MATCH ()-[r:TYPE {`key`: event.`key`}]-()
       SET r +
 
   :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
   :param username:   Username for the connection.
   :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
     access to the workspace.
+  :param database:   If the Neo4j server has multiple databases, you can specify which one to write to.
   :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
     This is true for exports too. If you want to repeat a previous export, you can increase this
     export repetition ID parameter.
   :param labels:   Makes it possible to restrict the export to one relationship type in Neo4j.
     This is useful to make sure no other relationship type is accidentally affected.
     The format is as in Cypher: `:TYPE`. Leave empty to allow updating any node.
   :param keys:   Select the attribute (or attributes) to identify the Neo4j relationships by.
     The attribute name must match the property name in Neo4j.
   '''
 
-def exportGraphToNeo4j(url, username, password, version, node_labels, relationship_type):
+
+def exportEdgeAttributesToNeo4jNow(url, username, password, database, version, labels, keys):
+  '''The immediate version of :py:meth:`exportEdgeAttributesToNeo4j()`.'''
+
+
+def exportGraphToNeo4j(url, username, password, database, version, node_labels, relationship_type):
   '''  Exports a graph from LynxKite to `Neo4j <https://neo4j.com/>`_.
   The whole graph will be copied to Neo4j with all attributes.
   No existing data is modified in Neo4j.
 
   A `!LynxKite export timestamp` property is added to each new
   node and relationship in Neo4j. This helps clean up the export if needed.
 
@@ -1275,26 +1497,33 @@
       CREATE (n)
       SET n +
 
   :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
   :param username:   Username for the connection.
   :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
     access to the workspace.
+  :param database:   If the Neo4j server has multiple databases, you can specify which one to write to.
   :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
     This is true for exports too. If you want to repeat a previous export, you can increase this
     export repetition ID parameter.
   :param node_labels:   A string vertex attribute that is a comma-separated list of labels to apply to the newly
     created nodes. Optional. You must have `Neo4j APOC <https://neo4j.com/developer/neo4j-apoc/>`_
     installed on the Neo4j instance to use this.
   :param relationship_type:   A string edge attribute that specifies the relationship type for each newly created relationship.
     Optional. You must have `Neo4j APOC <https://neo4j.com/developer/neo4j-apoc/>`_
     installed on the Neo4j instance to use this.
   '''
 
-def exportToAvro(path, version, for_download):
+
+def exportGraphToNeo4jNow(url, username, password, database,
+                          version, node_labels, relationship_type):
+  '''The immediate version of :py:meth:`exportGraphToNeo4j()`.'''
+
+
+def exportToAVRO(path, version, for_download):
   '''  `Apache AVRO <https://avro.apache.org/>`_ is a row-oriented remote procedure call and data serialization framework.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
   :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
     LynxKite treats export operations as other operations: it remembers the result (which in this case
@@ -1304,15 +1533,21 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
-def exportToCsv(path, delimiter, quote, quote_all, header, escape, null_value, date_format, timestamp_format, drop_leading_white_space, drop_trailing_white_space, version, for_download):
+
+def exportToAVRONow(path, version, for_download):
+  '''The immediate version of :py:meth:`exportToAVRO()`.'''
+
+
+def exportToCSV(path, delimiter, quote, quote_all, header, escape, null_value, date_format,
+                timestamp_format, drop_leading_white_space, drop_trailing_white_space, version, for_download):
   '''  CSV stands for comma-separated values. It is a common human-readable file format where each record
   is on a separate line and fields of the record are simply separated with a comma or other delimiter.
   CSV does not store data types, so all fields become strings when importing from this format.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
@@ -1340,14 +1575,20 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
+
+def exportToCSVNow(path, delimiter, quote, quote_all, header, escape, null_value, date_format,
+                   timestamp_format, drop_leading_white_space, drop_trailing_white_space, version, for_download):
+  '''The immediate version of :py:meth:`exportToCSV()`.'''
+
+
 def exportToDelta(path, version, for_download):
   '''  Export data to a Delta table.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
   :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
@@ -1358,14 +1599,19 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
+
+def exportToDeltaNow(path, version, for_download):
+  '''The immediate version of :py:meth:`exportToDelta()`.'''
+
+
 def exportToHive(table, mode, partition_by):
   '''  Export a table directly to `Apache Hive <https://hive.apache.org/>`_.
 
   :param table:   The name of the database table to export to.
   :param mode:   Describes whether LynxKite should expect a table to already exist and how to handle this case.
     +
     **The table must not exist** means the table will be created and it is an error if it already
@@ -1379,15 +1625,20 @@
     +
     **Insert into an existing table** requires the
     table to already exist and it will add the exported data at the end of the existing table.
   :param partition_by:   The list of column names (if any) which you wish the table to be partitioned by. This cannot
     be used in conjunction with the "Drop the table if it already exists" mode.
   '''
 
-def exportToJdbc(url, table, mode):
+
+def exportToHiveNow(table, mode, partition_by):
+  '''The immediate version of :py:meth:`exportToHive()`.'''
+
+
+def exportToJDBC(url, table, mode):
   '''  JDBC is used to connect to relational databases such as MySQL. See <<jdbc-details>> for setup steps
   required for connecting to a database.
 
   :param url:   The connection URL for the database. This typically includes the username and password. The exact
     syntax entirely depends on the database type. Please consult the documentation of the database.
   :param table:   The name of the database table to export to.
   :param mode:   Describes whether LynxKite should expect a table to already exist and how to handle this case.
@@ -1398,15 +1649,20 @@
     **Drop the table if it already exists** means the table will be deleted and re-created if
     it already exists. Use this mode with great care.
     +
     **Insert into an existing table** requires the
     table to already exist and it will add the exported data at the end of the existing table.
   '''
 
-def exportToJson(path, version, for_download):
+
+def exportToJDBCNow(url, table, mode):
+  '''The immediate version of :py:meth:`exportToJDBC()`.'''
+
+
+def exportToJSON(path, version, for_download):
   '''  JSON is a rich human-readable data format. It produces larger files than CSV but can represent
   data types. Each line of the file stores one record encoded as a
   `JSON <https://en.wikipedia.org/wiki/JSON>`_ object.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
@@ -1418,15 +1674,20 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
-def exportToOrc(path, version, for_download):
+
+def exportToJSONNow(path, version, for_download):
+  '''The immediate version of :py:meth:`exportToJSON()`.'''
+
+
+def exportToORC(path, version, for_download):
   '''  `Apache ORC <https://orc.apache.org/>`_ is a columnar data storage format.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
   :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
     LynxKite treats export operations as other operations: it remembers the result (which in this case
@@ -1436,14 +1697,19 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
+
+def exportToORCNow(path, version, for_download):
+  '''The immediate version of :py:meth:`exportToORC()`.'''
+
+
 def exportToParquet(path, version, for_download):
   '''  `Apache Parquet <https://parquet.apache.org/>`_ is a columnar data storage format.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
     This means that the same export operation with the same parameters always generates the same path.
   :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
@@ -1454,15 +1720,20 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
-def exportVertexAttributesToNeo4j(url, username, password, version, labels, keys):
+
+def exportToParquetNow(path, version, for_download):
+  '''The immediate version of :py:meth:`exportToParquet()`.'''
+
+
+def exportVertexAttributesToNeo4j(url, username, password, database, version, labels, keys):
   '''  Exports vertex attributes from a graph in LynxKite to a
   corresponding graph in `Neo4j <https://neo4j.com/>`_.
 
   The nodes in Neo4j are identified by a key property (or properties).
   You must have a corresponding vertex attribute in LynxKite by the same name.
   This will be used to find the right nodes to update in Neo4j.
 
@@ -1473,117 +1744,137 @@
       MATCH (n:Label1:Label2 {`key`: event.`key`})
       SET n +
 
   :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
   :param username:   Username for the connection.
   :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
     access to the workspace.
+  :param database:   If the Neo4j server has multiple databases, you can specify which one to write to.
   :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
     This is true for exports too. If you want to repeat a previous export, you can increase this
     export repetition ID parameter.
   :param labels:   Makes it possible to restrict the export to one label (or combination of labels) in Neo4j.
     This is useful to make sure no other node type is accidentally affected.
     The format is as in Cypher: `:Label1:Label2`. Leave empty to allow updating any node.
   :param keys:   Select the attribute (or attributes) to identify the Neo4j nodes by.
     The attribute name must match the property name in Neo4j.
   '''
 
-def exposeInternalEdgeId(name):
+
+def exportVertexAttributesToNeo4jNow(url, username, password, database, version, labels, keys):
+  '''The immediate version of :py:meth:`exportVertexAttributesToNeo4j()`.'''
+
+
+def exposeInternalEdgeID(name):
   '''  Exposes the internal edge ID as an attribute. Useful if you want to identify edges, for example in
   an exported dataset.
 
   :param name:   The ID attribute will be saved under this name.
   '''
 
-def exposeInternalVertexId(name):
+
+def exposeInternalVertexID(name):
   '''  Exposes the internal vertex ID as an attribute. This attribute is automatically generated
   by operations that generate new vertex sets. (In most cases this is already available as attribute ‘id’.)
   But you can regenerate it with this operation if necessary.
 
   :param name:   The ID attribute will be saved under this name.
   '''
 
+
 def externalComputation1():
   '''
 
 
   '''
 
+
 def externalComputation10():
   '''
 
 
   '''
 
+
 def externalComputation2():
   '''
 
 
   '''
 
+
 def externalComputation3():
   '''
 
 
   '''
 
+
 def externalComputation4():
   '''
 
 
   '''
 
+
 def externalComputation5():
   '''
 
 
   '''
 
+
 def externalComputation6():
   '''
 
 
   '''
 
+
 def externalComputation7():
   '''
 
 
   '''
 
+
 def externalComputation8():
   '''
 
 
   '''
 
+
 def externalComputation9():
   '''
 
 
   '''
 
+
 def fillEdgeAttributesWithConstantDefaultValues(title):
   '''  An attribute may not be defined on every edge. This operation sets a default value
   for the edges where it was not defined.
 
   :param title:   The given value will be set for edges where the attribute is not defined. No change for
     attributes for which the default value is left empty. The default value
     must be numeric for `number` attributes.
   '''
 
+
 def fillVertexAttributesWithConstantDefaultValues(title):
   '''  An attribute may not be defined on every vertex. This operation sets a default value
   for the vertices where it was not defined.
 
   :param title:   The given value will be set for vertices where the attribute is not defined. No change for
     attributes for which the default value is left empty. The default value
     must be numeric for `number` attributes.
   '''
 
+
 def filterByAttributes(ref1, ref2, ref3, ref4, ref5, ref6, ref7, ref8, ref9):
   '''  Keeps only vertices and edges that match the specified filters.
 
   You can specify filters for multiple attributes at the same time, in which case you will be left
   with vertices/edges that match all of your filters.
 
   Regardless of the exact the filter, whenever you specify a filter for an attribute you always
@@ -1618,30 +1909,31 @@
     and the square bracket (`
   :param ref5:   For `String` attributes, regex filters can also be applied. The following tips and examples
     can be useful:
     * `regex(xyz)` for finding strings that contain `xyz`.
     * `regex(^Abc)` for strings that start with `Abc`.
     * `regex(Abc$)` for strings that end with `Abc`.
     * `regex((.)\1)` for strings with double letters, like `abbc`.
-    * `regex(\d)` or `regex(
+    * `regex(\\d)` or `regex(
   :param ref6:   For the `Vector
   :param ref7:   These filters can be used for attributes whose type is `Vector`.
     The filter `all(...)` will match the `Vector` only when the internal filter matches all elements of the
     `Vector`. You can also use `forall` and `Ɐ` as synonyms. For example `all(<0)` for a `Vector
   :param ref8:   Any filter can be prefixed with `!` to negate it. For example `!medium` will exclude
     `medium` values. Another typical usecase for this is specifying `!` (a single exclamation mark
     character) as the filter for a String attribute. This is interpreted as non-empty, so it will
     restrict to those vertices/edges where the String attribute is defined and its value is not empty
     string. Remember, all filters work on defined values only, so `!*` will not match any
     vertices/edges.
   :param ref9:   If you need a string filter that contains a character with a special meaning (e.g., `>`), use double quotes around
     the string. E.g., `>"
   '''
 
-def filterWithSql(vertex_filter, edge_filter, filter):
+
+def filterWithSQL(vertex_filter, edge_filter, filter):
   '''  Filters a graph or table with SQL expressions.
 
   This has the same effect as using a SQL box with
   ``select * from vertices where <FILTER>`` and ``select * from edge_attributes where <FILTER>``
   and then recombining the tables into a graph. But it is more efficient.
 
   When used with a table input it is identical to a SQL box with
@@ -1651,14 +1943,15 @@
     For example you could write ``age > 30 and income < age * 2000``.
   :param edge_filter:   Filter the edges with this SQL expression when the input is a graph.
     For example you could write ``duration > count * 10 or kind like '%*message*%'``.
   :param filter:   Filter with this SQL expression when the input is a table.
     For example you could write ``age > 30 and income < age * 2000``.
   '''
 
+
 def findCommunitiesWithLabelPropagation(name, weight, variant):
   '''  Uses the `label propagation algorithm <https://en.wikipedia.org/wiki/Label*propagation*algorithm>`_
   to identify communities in the graph. The communities are represented as a segmentation on
   the graph.
 
   Label propagation starts with assigning a unique label to each vertex.
   Then each vertex takes on the most common label in their neighborhood.
@@ -1674,50 +1967,55 @@
   :param variant:   The results of label propagation depend greatly on the order of the updates.
     The available options are:
     - **classic:** An efficient method that uses an arbitrary ordering and parallel updates.
     - **degree-ordered:** A more predictable method that performs the updates in increasing
       order of degree.
   '''
 
+
 def findCommunitiesWithTheLouvainMethod(name, weight, resolution):
   '''  Uses the `Louvain method <https://en.wikipedia.org/wiki/Louvain_method>`_ to identify
   communities in the graph. The communities are represented as a segmentation on
   the graph.
 
   The Louvain method is a greedy optimization toward maximal *modularity*.
   High modularity means many edges within communities and few edges between communities.
   Specifically we compare the edge counts to what we would expect if the clusters
   were chosen at random.
 
-  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PLM.html>`_ implementation.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PLM.html>`_
+  implementation otherwise.
 
   :param name:   The name of the newly created segmentation.
   :param weight:   Edges can be weighted to contribute more or less to modularity.
   :param resolution:   A lower resolution will result in bigger communities.
     +
     Also known as the 𝛾 parameter, the expected edge probabilities in the modularity
     calculation are multiplied by this number.
     +
     For details of the physical basis of this parameter see
     `Statistical Mechanics of Community Detection <https://arxiv.org/abs/cond-mat/0603718>`_
     by Joerg Reichardt and Stefan Bornholdt.
   '''
 
+
 def findConnectedComponents(name, directions):
   '''  Creates a segment for every connected component of the graph.
 
   Connected components are maximal vertex sets where a path exists between each pair of vertices.
 
   :param name:   The new segmentation will be saved under this name.
   :param directions:   Ignore directions:::
     The algorithm adds reversed edges before calculating the components.
     Require both directions:::
     The algorithm discards non-symmetric edges before calculating the components.
   '''
 
+
 def findInfocomCommunities(cliques_name, communities_name, bothdir, min, adjacency_threshold):
   '''  Creates a segmentation of overlapping communities.
 
   The algorithm finds maximal cliques then merges them to communities.
   Two cliques are merged if they sufficiently overlap.
   More details can be found in
   https://papers.ssrn.com/sol3/papers.cfm?abstract_id
@@ -1730,42 +2028,45 @@
     +
     This improves the performance of the algorithm, and small cliques are often not
     a good indicator anyway.
   :param adjacency_threshold:   Clique overlap is a measure of the overlap between two cliques relative to
     their sizes. It is normalized to
   '''
 
-def findKCoreDecomposition(name):
+
+def findKcoreDecomposition(name):
   '''  If we deleted all parts of a graph outside of the **k**-core, all vertices would
   still have a degree of at least *k*. More visually, the 0-core is the whole graph.
   If we discard the isolated vertices we get the 1-core. If we repeatedly discard
   all degree-1 vertices, we get the 2-core. And so on.
 
   Read more on `Wikipedia <https://en.wikipedia.org/wiki/Degeneracy_(graph_theory)#k-Cores>`_.
 
   This operation outputs the number of the highest core that each vertex belongs to
   as a vertex attribute.
 
   :param name:   The new attribute will be created under this name.
   '''
 
+
 def findMaximalCliques(name, bothdir, min):
   '''  Creates a segmentation of vertices based on the maximal cliques they are the member of.
   A maximal clique is a maximal set of vertices where there is an edge between every two vertex.
   Since one vertex can be part of multiple maximal cliques this segmentation might be overlapping.
 
   :param name:   The new segmentation will be saved under this name.
   :param bothdir:   Whether edges have to exist in both directions between all members of a clique.
     +
   :param min:   Cliques smaller than this will not be collected.
     +
     This improves the performance of the algorithm, and small cliques are often not a good indicator
     anyway.
   '''
 
+
 def findModularClustering(name, weights, max_iterations, min_increment_per_iteration):
   '''  Tries to find a partitioning of the vertices with high
   `modularity <http://en.wikipedia.org/wiki/Modularity_(networks)>`_.
 
   Edges that go between vertices in the same segment increase modularity, while edges that go from
   one segment to the other decrease modularity. The algorithm iteratively merges and splits segments
   and moves vertices between segments until it cannot find changes that would significantly improve
@@ -1774,14 +2075,15 @@
   :param name:   The new segmentation will be saved under this name.
   :param weights:   The attribute to use as edge weights.
   :param max_iterations:   After this number of iterations we stop regardless of modularity increment. Use -1 for unlimited.
   :param min_increment_per_iteration:   If the average modularity increment in the last few iterations goes below this then we stop
     the algorithm and settle with the clustering found.
   '''
 
+
 def findOptimalSpanningTree(name, weight, optimize, seed):
   '''  Finds the https://en.wikipedia.org/wiki/Minimum*spanning*tree[minimum (or maximum) spanning tree]
   in a graph. The edges marked by the emitted edge attribute (``in_tree`` by default)
   form a tree for each component in the graph. This tree will have the lowest
   (or highest) possible total edge weight.
 
   Uses the
@@ -1794,14 +2096,15 @@
   :param weight:   Choose a numerical attribute that represents the cost or value of the edges.
     With unit weights the result is just a random tree for each component.
   :param optimize:   Whether to find the tree with the lowest or highest possible total edge weight.
   :param seed:   When multiple trees have the optimal weight, one is chosen at random.
     +
   '''
 
+
 def findSteinerTree(ename, vname, pname, rname, edge_costs, root_costs, gain):
   '''  Given a directed graph in which each vertex has two associated quantities, the "gain",
   and the "root cost", and each edge has an associated quantity, the "cost",
   this operation will yield a forest (a set of trees) that is a subgraph of the given
   graph. Furthermore, in this subgraph, the sum of the gains
   minus the sum of the (edge and root) costs approximate the maximal possible value.
 
@@ -1830,28 +2133,30 @@
   :param root_costs:   The vertex attribute specified here determines the cost for allowing
     the given vertex to be a starting point (the root) of a tree in the solution forest.
     Negative or undefined values mean that the vertex cannot be used as a root point.
   :param gain:   This vertex attribute specifies the reward (gain) for including the given
     vertex in the solution. Negative or undefined values are treated as 0.
   '''
 
+
 def findTriangles(name, bothdir):
   '''  Creates a segment for every triangle in the graph.
   A triangle is defined as 3 pairwise connected vertices, regardless of the direction and number of edges between them.
   This means that triangles with one or more multiple edges are still only counted once,
   and the operation does not differentiate between directed and undirected triangles.
   Since one vertex can be part of multiple triangles this segmentation might be overlapping.
 
   :param name:   The new segmentation will be saved under this name.
   :param bothdir:   Whether edges have to exist in both directions between all members of a triangle.
     +
     If the direction of the edges is not important, set this to `false`. This will allow placing two
     vertices into the same clique even if they are only connected in one direction.
   '''
 
+
 def fingerprintBasedOnAttributes(leftname, rightname, weights, mo, ms, extra):
   '''  In a graph that has two different String identifier attributes (e.g. Facebook ID and
   MSISDN) this operation will match the vertices that only have the first attribute defined
   with the vertices that only have the second attribute defined. For the well-matched vertices
   the new attributes will be added. (For example if a vertex only had an MSISDN and we found a
   matching Facebook ID, this will be saved as the Facebook ID of the vertex.)
 
@@ -1868,14 +2173,15 @@
     anyway.)
   :param ms:   The similarity threshold below which two vertices will not be considered a match even if there are
     no better matches for them. Similarity is normalized to
   :param extra:   You can use this box to further tweak how the fingerprinting operation works. Consult with a Lynx
     expert if you think you need this.
   '''
 
+
 def graphRejoin(attrs, segs, edge):
   '''  This operation allows the user to join (i.e., carry over) attributes from one graph to another one.
   This is only allowed when the target of the join (where the attributes are taken to) and the source
   (where the attributes are taken from) are compatible. Compatibility in this context means that
   the source and the target have a "common ancestor", which makes it possible to perform the join.
   Suppose, for example, that operation <<take-edges-as-vertices>> have been applied, and then some
   new vertex attributes have been computed on the resulting graph. These new vertex
@@ -1904,47 +2210,51 @@
     target graph which have identical names.
   :param segs:   Segmentations to join to the graph. They overwrite segmentations in the target
     side of the graph which have identical names.
   :param edge:   When set, the edges of the source graph (and their attributes) will replace
     the edges of the target graph.
   '''
 
+
 def graphUnion():
   '''  The resulting graph is just a disconnected graph containing the vertices and edges of
   the two originating graphs. All vertex and edge attributes are preserved. If an attribute
   exists in both graphs, it must have the same data type in both.
 
   The resulting graph will have as many vertices as the sum of the vertex counts in the two
   source graphs. The same with the edges.
 
   Segmentations are discarded.
 
 
   '''
 
+
 def graphVisualization():
   '''  Creates a visualization from the input graph. You can use the box parameter popup to
   define the parameters and layout of the visualization. See <<graph-visualizations>> for more details.
 
 
   '''
 
+
 def growSegmentation(direction):
   '''  Grows the segmentation along edges of the parent graph.
 
   This operation modifies this segmentation by growing each segment with the neighbors of its elements.
   For example if vertex A is a member of segment X and edge A→B exists in the original graph
   then B also becomes the member of X (depending on the value of the direction parameter).
 
   This operation can be used together with <<Use base graph as segmentation>> to create a
   segmentation of neighborhoods.
 
   :param direction:   Adds the neighbors to the segments using this direction.
   '''
 
+
 def hashVertexAttribute(attr, salt):
   '''  Uses the `SHA-256 <https://en.wikipedia.org/wiki/SHA-256>`_ algorithm to hash an attribute: all values
   of the attribute get replaced by a seemingly random value. The same original values get replaced by
   the same new value and different original values get (almost certainly) replaced by different new
   values.
 
   Treat the salt like a password for the data. Choose a long string that the recipient of the data has
@@ -1963,22 +2273,29 @@
   up in the graph. He can also apply hashing to the phone numbers of all the knights of the round
   table and see which knight has Guinevere been making calls to.
 
   :param attr:   The attribute(s) which will be hashed.
   :param salt:   The value of the salt.
   '''
 
-def importAvro(filename):
+
+def importAVRO(filename):
   '''  `Apache AVRO <https://avro.apache.org/>`_ is a row-oriented remote procedure call and data serialization framework.
 
   :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
     paths.
   '''
 
-def importCsv(filename, columns, delimiter, quote, escape, null_value, date_format, timestamp_format, ignore_leading_white_space, ignore_trailing_white_space, comment, error_handling, infer):
+
+def importAVRONow(filename):
+  '''The immediate version of :py:meth:`importAVRO()`.'''
+
+
+def importCSV(filename, columns, delimiter, quote, escape, null_value, date_format, timestamp_format,
+              ignore_leading_white_space, ignore_trailing_white_space, comment, error_handling, infer):
   '''  CSV stands for comma-separated values. It is a common human-readable file format where each record
   is on a separate line and fields of the record are simply separated with a comma or other delimiter.
   CSV does not store data types, so all fields become strings when importing from this format.
 
   :param filename:   Upload a file by clicking the
     +++<label class
   :param columns:   The names of all the columns in the file, as a comma-separated list. If empty, the column names will
@@ -2006,29 +2323,97 @@
     +
     **Salvage malformed lines: truncate or fill with nulls** will still import the problematic lines,
     dropping some data or inserting undefined values.
   :param infer:   Automatically detects data types in the CSV. For example a column full of numbers will become a
     `Double`. If disabled, all columns are imported as ``String``s.
   '''
 
+
+def importCSVNow(filename, columns, delimiter, quote, escape, null_value, date_format, timestamp_format,
+                 ignore_leading_white_space, ignore_trailing_white_space, comment, error_handling, infer):
+  '''The immediate version of :py:meth:`importCSV()`.'''
+
+
 def importDelta(filename, version_as_of):
   '''  Import a Delta Table.
 
   :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
     paths.
   :param version_as_of:   Version of the Delta table to be imported. The empty string corresponds to the latest version.
   '''
 
+
+def importDeltaNow(filename, version_as_of):
+  '''The immediate version of :py:meth:`importDelta()`.'''
+
+
+def importFromBigQueryRawTable(parent_project_id, project_id, dataset_id,
+                               table_id, credentials_file, views_enabled):
+  '''  Import a table from BigQuery without a SQL query. (See also <<Import from BigQuery (Standard SQL result)>>.)
+
+  Some BigQuery-specific datatypes like `ARRAY<STRUCT>` are not fully supported within LynxKite.
+
+  BigQuery access is provided through the `Apache Spark SQL connector for Google BigQuery <https://github.com/GoogleCloudDataproc/spark-bigquery-connector/tree/0.25.0#apache-spark-sql-connector-for-google-bigquery>`_.
+
+  :param parent_project_id:   The GCP Project ID for billing purposes. This may be different from the dataset being read.
+    `roles/bigquery.readSessionUser` is required on the billed project.
+    `roles/bigquery.jobUser` is additionally required if using views.
+  :param project_id:   Used together with dataset ID and table ID. Defaults to service account's GCP project if unspecified.
+  :param dataset_id:   Used together with table ID to import. Requires `roles/bigquery.dataEditor` on the dataset to store
+    materialized tables if querying from views.
+  :param table_id:   The BigQuery table/view to import from. Requires `roles/bigquery.dataViewer` on the view AND underlying table.
+  :param credentials_file:   Local path to the service account JSON key to authenticate with GCP.
+    Leave this field empty if running on Dataproc or to use `GOOGLE*APPLICATION*CREDENTIALS`.
+  :param views_enabled:   Allow reading from BigQuery views. Preliminary support.
+    See https://github.com/GoogleCloudDataproc/spark-bigquery-connector/tree/0.25.0#reading-from-views
+  '''
+
+
+def importFromBigQueryRawTableNow(parent_project_id, project_id,
+                                  dataset_id, table_id, credentials_file, views_enabled):
+  '''The immediate version of :py:meth:`importFromBigQueryRawTable()`.'''
+
+
+def importFromBigQueryStandardSQLResult(
+        parent_project_id, materialization_project_id, materialization_dataset_id, bq_standard_sql, credentials_file):
+  '''  Execute a BigQuery Standard SQL query and get the result as a table. (See also <<Import from BigQuery (raw table)>>.)
+
+  Some BigQuery-specific datatypes like `ARRAY<STRUCT>` are not fully supported within LynxKite.
+
+  BigQuery access is provided through the `Apache Spark SQL connector for Google BigQuery <https://github.com/GoogleCloudDataproc/spark-bigquery-connector/tree/0.25.0#apache-spark-sql-connector-for-google-bigquery>`_.
+
+  :param parent_project_id:   The GCP Project ID for billing purposes. This may be different from the dataset being read.
+    `roles/bigquery.readSessionUser` and `roles/bigquery.jobUser` are both required on the billed project.
+  :param materialization_project_id:   Used together with dataset ID. Defaults to service account's GCP project if unspecified.
+    Requires `roles/bigquery.dataEditor` on the dataset.
+  :param materialization_dataset_id:   Place to create temporary (24h) tables to store the results of the SQL query.
+    Dataset must already exist with `roles/bigquery.dataEditor` granted on it.
+  :param bq_standard_sql:   The SQL query to run on BigQuery. `roles/bigquery.dataViewer` is required for SELECT.
+  :param credentials_file:   Local path to the service account JSON key to authenticate with GCP.
+    Leave this field empty if running on Dataproc or to use `GOOGLE*APPLICATION*CREDENTIALS`.
+  '''
+
+
+def importFromBigQueryStandardSQLResultNow(
+        parent_project_id, materialization_project_id, materialization_dataset_id, bq_standard_sql, credentials_file):
+  '''The immediate version of :py:meth:`importFromBigQueryStandardSQLResult()`.'''
+
+
 def importFromHive(table_name):
   '''  Import an `Apache Hive <https://hive.apache.org/>`_ table directly to LynxKite.
 
   :param table_name:   The name of the Hive table to import.
   '''
 
-def importFromNeo4j(url, username, password, vertex_query, edge_query):
+
+def importFromHiveNow(table_name):
+  '''The immediate version of :py:meth:`importFromHive()`.'''
+
+
+def importFromNeo4j(url, username, password, database, vertex_query, edge_query):
   '''  Import a graph from the `Neo4j <https://neo4j.com/>`_ graph database.
 
   Neo4j does not have a strict schema. Different nodes may have different attributes.
   In LynxKite the list of vertex attributes is defined for the whole graph.
   But each vertex may leave any attribute undefined.
 
   If you import Neo4j nodes that have different attributes, such as movies that have
@@ -2040,21 +2425,27 @@
 
   If multiple node types have attributes of the same name, those attributes need to have
   the same type. If this is not the case, you can narrow down the query by node label.
 
   :param url:   The connection URI for Neo4j.
   :param username:   The username to use for the connection.
   :param password:   The password to use for the connection.
+  :param database:   If the Neo4j server has multiple databases, you can specify which one to read from.
   :param vertex_query:   The Cypher query to run on Neo4j to get the vertices. This query must return a node named `node`.
     The default query imports all the nodes from Neo4j. Leave empty to not import vertex attributes.
   :param edge_query:   The Cypher query to run on Neo4j to get the edges. This query must return a relationship named `rel`.
     The default query imports all the relationships from Neo4j. Leave empty to not import edges.
   '''
 
-def importJdbc(jdbc_url, jdbc_table, key_column, num_partitions, partition_predicates):
+
+def importFromNeo4jNow(url, username, password, database, vertex_query, edge_query):
+  '''The immediate version of :py:meth:`importFromNeo4j()`.'''
+
+
+def importJDBC(jdbc_url, jdbc_table, key_column, num_partitions, partition_predicates):
   '''  JDBC is used to connect to relational databases such as MySQL. See <<jdbc-details>> for setup steps
   required for connecting to a database.
 
   :param jdbc_url:   The connection URL for the database. This typically includes the username and password. The exact
     syntax entirely depends on the database type. Please consult the documentation of the database.
   :param jdbc_table:   The name of the database table to import.
     +
@@ -2087,78 +2478,122 @@
   :param partition_predicates:   This advanced option provides even greater control over the partitioning. It is an alternative
     option to specifying the key column. Here you can specify a comma-separated list of `WHERE` clauses,
     which will be used as the partitions.
     +
     For example you could provide `AGE < 30, AGE >
   '''
 
-def importJson(filename):
+
+def importJDBCNow(jdbc_url, jdbc_table, key_column, num_partitions, partition_predicates):
+  '''The immediate version of :py:meth:`importJDBC()`.'''
+
+
+def importJSON(filename):
   '''  JSON is a rich human-readable data format. JSON files are larger than CSV files but can represent
   data types. Each line of the file in this format stores one record encoded as a
   `JSON <https://en.wikipedia.org/wiki/JSON>`_ object.
 
   :param filename:   Upload a file by clicking the
     +++<label class
   '''
 
-def importOrc(filename):
+
+def importJSONNow(filename):
+  '''The immediate version of :py:meth:`importJSON()`.'''
+
+
+def importORC(filename):
   '''  `Apache ORC <https://orc.apache.org/>`_ is a columnar data storage format.
 
   :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
     paths.
   '''
 
-def importParquet(filename):
+
+def importORCNow(filename):
+  '''The immediate version of :py:meth:`importORC()`.'''
+
+
+def importParquet(filename, eager, schema):
   '''  `Apache Parquet <https://parquet.apache.org/>`_ is a columnar data storage format.
 
   :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
     paths.
+  :param eager:   Importing data into LynxKite normally means reading the source data and writing it to
+    LynxKite's storage directory as a Parquet file. The "Import now" option does this.
+    +
+    When the source data is already a Parquet file, you have the option to avoid copying
+    the data to LynxKite. In this case the schema has to be provided explicitly, so
+    that you can work with the table even before LynxKite first touches it.
+  :param schema:   A semi-colon separated list of column names and types. The types are to be specified
+    using Apache Spark's syntax. For example: `col1: string; col2: int; col3: decimal(8, 2)`.
   '''
 
+
+def importParquetNow(filename, eager, schema):
+  '''The immediate version of :py:meth:`importParquet()`.'''
+
+
 def importSnapshot(path):
   '''  Makes a previously saved snapshot accessible from the workspace.
 
   :param path:   The full path to the snapshot in LynxKite's virtual filesystem.
   '''
 
+
+def importSnapshotNow(path):
+  '''The immediate version of :py:meth:`importSnapshot()`.'''
+
+
 def importUnionOfTableSnapshots(paths):
   '''  Makes the union of a list of previously saved table snapshots accessible from the workspace
   as a single table.
 
   The union works as the UNION ALL command in SQL and does not remove duplicates.
 
   :param paths:   The comma separated set of full paths to the snapshots in LynxKite's virtual filesystem.
 
      - Each path has to refer to a table snapshot.
      - The tables have to have the same schema.
      - The output table will union the input tables in the same order as defined here.
   '''
 
-def importWellKnownGraphDataset(name):
+
+def importUnionOfTableSnapshotsNow(paths):
+  '''The immediate version of :py:meth:`importUnionOfTableSnapshots()`.'''
+
+
+def importWellknownGraphDataset(name):
   '''  Gives easy access to graph datasets commonly used for benchmarks.
 
   See the `PyTorch Geometric documentation <https://pytorch-geometric.readthedocs.io/en/1.4.1/modules/datasets.html>`_
   for details about the specific datasets.
 
   :param name:   Which dataset to import.
   '''
 
+
+def importWellknownGraphDatasetNow(name):
+  '''The immediate version of :py:meth:`importWellknownGraphDataset()`.'''
+
+
 def input(name):
   '''  This special box represents an input that comes from outside of this workspace.
   This box will not have a valid output on its own. When this workspace is used as a custom
   box in another workspace, the custom box will have one input for each input box.
   When the inputs are connected, those input states will appear on the outputs of the input boxes.
 
   Input boxes without a name are ignored. Each input box must have a different name.
 
   See the section on <<custom-boxes>> on how to use this box.
 
   :param name:   The name of the input, when the workspace is used as a custom box.
   '''
 
+
 def linkBaseGraphAndSegmentationByFingerprint(mo, ms, extra):
   '''  Finds the best matching between a base graph and a segmentation.
   It considers a base vertex A and a segment B a good "match"
   if the neighborhood of A (including A) is very connected to the neighborhood of B (including B)
   according to the current connections between the graph and the segmentation.
 
   The result of this operation is a new edge set between the base graph and the
@@ -2169,14 +2604,15 @@
     anyway.)
   :param ms:   The similarity threshold below which two vertices will not be considered a match even if there are
     no better matches for them. Similarity is normalized to
   :param extra:   You can use this box to further tweak how the fingerprinting operation works. Consult with a Lynx
     expert if you think you need this.
   '''
 
+
 def lookupRegion(position, shapefile, attribute, ignoreUnsupportedShapes, output):
   '''  For every `position` vertex attribute looks up features in a Shapefile and returns a specified
   attribute.
 
   * The lookup depends on the coordinate reference system of the feature. The input position must
     use the same coordinate reference system as the one specified in the Shapefile.
   * If there are no matching features the output is omitted.
@@ -2192,20 +2628,22 @@
     and `.dbf` file of the same name.
   :param attribute:   The attribute in the Shapefile used for the output.
   :param ignoreUnsupportedShapes:   If set `true`, silently ignores unknown shape types potentially contained by the Shapefile.
     Otherwise throws an error.
   :param output:   The name of the new vertex attribute.
   '''
 
-def makeAllSegmentsEmpy():
+
+def makeAllSegmentsEmpty():
   '''  Throws away all segmentation links.
 
 
   '''
 
+
 def mapHyperbolicCoordinates(seed):
   '''  Experimental Feature
 
 
   Map an undirected graph to a hyperbolic surface. Vertices get two attributes called
   "radial" and "angular" that can be used for edge strength evaluation or link prediction.
   The algorithm is based on
@@ -2215,67 +2653,73 @@
   are most useful when the graph to be mapped follows a power-law degree distribution
   and has high clustering.
 
   :param seed:   The random seed.
     +
   '''
 
+
 def mergeParallelEdgesByAttribute(key):
   '''  Multiple edges going from A to B that share the same value of the given edge attribute
   will be merged into a single edge. The edges going from A to B are not merged with edges
   going from B to A.
 
   :param key:   The edge attribute on which the merging will be based.
 
     include::glossary.asciidoc
   '''
 
+
 def mergeParallelEdges():
   '''  Multiple edges going from A to B will be merged into a single edge.
   The edges going from A to B are not merged with edges going from B to A.
 
   Edge attributes can be aggregated across the merged edges.
 
 
   '''
 
+
 def mergeParallelSegmentationLinks():
   '''  Multiple segmentation links going from A base vertex to B segmentation vertex
   will be merged into a single link.
 
   After performing a <<merge-vertices-by-attribute, Merge vertices by attribute>> operation, there might
   be multiple parallel links going between some of the base graph and segmentation vertices.
   This can cause unexpected behavior when aggregating to or from the segmentation.
   This operation addresses this behavior by merging parallel segmentation links.
 
 
   '''
 
+
 def mergeTwoEdgeAttributes(name, attr1, attr2):
   '''  An attribute may not be defined on every edge. This operation uses the secondary
   attribute to fill in the values where the primary attribute is undefined. If both are
   undefined on an edge then the result is undefined too.
 
   :param name:   The new attribute will be created under this name.
   :param attr1:   If this attribute is defined on an edge, then its value will be copied to the output attribute.
   :param attr2:   If the primary attribute is not defined on an edge but the secondary attribute is, then the
     secondary attribute's value will be copied to the output variable.
   '''
 
+
 def mergeTwoVertexAttributes(name, attr1, attr2):
   '''  An attribute may not be defined on every vertex. This operation uses the secondary
   attribute to fill in the values where the primary attribute is undefined. If both are
   undefined on a vertex then the result is undefined too.
 
   :param name:   The new attribute will be created under this name.
   :param attr1:   If this attribute is defined on a vertex, then its value will be copied to the output attribute.
   :param attr2:   If the primary attribute is not defined on a vertex but the secondary attribute is, then the
     secondary attribute's value will be copied to the output variable.
   '''
 
+
 def mergeVerticesByAttribute(key):
   '''  Merges each set of vertices that are equal by the chosen attribute. Vertices where the chosen
   attribute is not defined are discarded. Aggregations can be specified for how to handle the rest of
   the attributes, which may be different among the merged vertices. Any edge that connected two
   vertices that are merged will become a loop.
 
   Merge vertices by attributes might create parallel links between the base graph
@@ -2284,75 +2728,82 @@
   make sure to run the <<merge-parallel-segmentation-links, Merge parallel segmentation links>>
   operation on the segmentations in question.
 
   :param key:   If a set of vertices have the same value for the selected attribute, they will all be merged
     into a single vertex.
   '''
 
-def oneHotEncodeAttribute(output, catAttr, categories):
+
+def onehotEncodeAttribute(output, catAttr, categories):
   '''  Encodes a categorical `String` attribute into a `one-hot <https://en.wikipedia.org/wiki/One-hot>`_
   `Vector[number]`. For example, if you apply it to the `name` attribute of the example graph
   with categories `Adam,Eve,Isolated Joe,Sue`, you end up with
 
   |
 
   :param output:   The new attribute will be created under this name.
   :param catAttr:   The attribute you would like to turn into a one-hot Vector.
   :param categories:   Possible categories separated by commas.
   '''
 
+
 def output(name):
   '''  This special box represents an output that goes outside of this workspace.
   When this workspace is used as a custom box in another workspace, the custom box
   will have one output for each output box.
 
   Output boxes without a name are ignored. Each output box must have a different name.
 
   See the section on <<custom-boxes>> on how to use this box.
 
   :param name:   The name of the output, when the workspace is used as a custom box.
   '''
 
+
 def placeVerticesWithEdgeLengths(name, dimensions, length, algorithm, pivots, radius, tolerance):
   '''  These methods create a graph layout as a new ``Vector[number]`` vertex attribute
   where the edges have the given lengths, or as close to those as possible.
 
   Uses the NetworKit implementations for
   `PivotMDS <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PivotMDS.html>`_ and
   `MaxentStress <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1MaxentStress.html>`_.
 
   :param name:   The position attribute will be saved under this name.
   :param dimensions:   The dimensions of the space where the vertices are placed.
     The created ``Vector``s will be this long.
   :param length:   This edge attribute can specify the length that each edge should be.
   :param algorithm:   The algorithms offered are:
     - **Pivot MDS** picks a number of pivot vertices (spread out as much as possible) and
-      finds a solution that puts all other vertices the right distance from the pivots
-      through an iterative matrix eigendecomposition method.
-      +
-      See `Eigensolver Methods for Progressive Multidimensional Scaling of Large Data <https://kops.uni-konstanz.de/bitstream/handle/123456789/5741/bp*empmdsld*06.pdf>`_
-      by Ulrik Brandes and Christian Pich for the detailed definition and analysis.
+    finds a solution that puts all other vertices the right distance from the pivots
+    through an iterative matrix eigendecomposition method.
+    +
+    See `Eigensolver Methods for Progressive Multidimensional Scaling of Large Data <https://kops.uni-konstanz.de/bitstream/handle/123456789/5741/bp*empmdsld*06.pdf>`_
+    by Ulrik Brandes and Christian Pich for the detailed definition and analysis.
     - **Maxent-Stress** is recommended when there are many different ways to
-      satisfy the edge length constraints. (Such as in graphs with low degrees or in
-      high-dimensional spaces.) It picks from the large solution space by
-      maximizing the solution's entropy.
-      +
-      Cannot handle disconnected graphs.
-      +
-      See `A Maxent-Stress Model for Graph Layout <http://yifanhu.net/PUB/maxent.pdf>`_
-      by Gansner et al for the detailed definition and analysis.
+    satisfy the edge length constraints. (Such as in graphs with low degrees or in
+    high-dimensional spaces.) It picks from the large solution space by
+    maximizing the solution's entropy.
+    +
+    Cannot handle disconnected graphs.
+    +
+    See `A Maxent-Stress Model for Graph Layout <http://yifanhu.net/PUB/maxent.pdf>`_
+    by Gansner et al for the detailed definition and analysis.
+    - *ForceAtlas2* is a force-based method introduced in
+    https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4051631/
   :param pivots:   The number of pivots to choose for Pivot MDS.
     More pivots result in a more accurate layout and a longer computation time.
   :param radius:   Maxent-Stress applies the stress model between vertices within this many
     hops from each other.
   :param tolerance:   Maxent-Stress uses an algebraic solver to optimize the vertex positions.
     This parameter allows tuning the solver to provide faster but less accurate solutions.
   '''
 
-def predictEdgesWithHyperbolicPositions(size, externaldegree, internaldegree, exponent, radial, angular):
+
+def predictEdgesWithHyperbolicPositions(
+        size, externaldegree, internaldegree, exponent, radial, angular):
   '''  Creates additional edges in a graph based on
   hyperbolic distances between vertices.
    *2 * size* edges will be added because
   the new edges are undirected.
   Vertices must have two *number* vertex attributes to be
   used as radial and angular coordinates.
 
@@ -2371,14 +2822,15 @@
     Values can be 0.5 - 1, endpoints excluded.
   :param radial:   The vertex attribute to be used as radial coordinates.
     Should not contain negative values.
   :param angular:   The vertex attribute to be used as angular coordinates.
     Values should be 0 - 2 * Pi.
   '''
 
+
 def predictVertexAttribute(label, features, method):
   '''  If an attribute is defined for some vertices but not for others, machine learning can be used to
   fill in the blanks. A model is built from the vertices where the attribute is defined and the
   model predictions are generated for all the vertices.
 
   The prediction is created in a new attribute named after the predicted attribute, such as
   `age_prediction`.
@@ -2398,45 +2850,49 @@
      - **Naive Bayes** classifier with multinomial event model.
      - **Decision tree** with maximum depth 5 and 32 bins for all features.
      - **Random forest** of 20 trees of depth 5 with 32 bins. One third of features are considered
        for splits at each node.
      - **Gradient-boosted trees** produce ensembles of decision trees with depth 5 and 32 bins.
   '''
 
-def predictWithGcn(save_as, features, label, model):
+
+def predictWithGCN(save_as, features, label, model):
   '''  Uses a trained `Graph Convolutional Network <https://tkipf.github.io/graph-convolutional-networks/>`_
   to make predictions.
 
   :param save_as:   The prediction will be saved as an attribute under this name.
   :param features:   Vector attribute containing the features to be used as inputs for the algorithm.
   :param label:   The attribute we want to predict. (This is used if the model was trained to use
     the target labels as additional inputs.)
   :param model:   The model to use for the prediction.
   '''
 
+
 def predictWithModel(name, model):
   '''  Creates predictions from a model and vertex attributes of the graph.
 
   :param name:   The new attribute of the predictions will be created under this name.
   :param model:   The model used for the predictions and a mapping from vertex attributes to the model's
     features.
     +
     Every feature of the model needs to be mapped to a vertex attribute.
   '''
 
+
 def pullSegmentationOneLevelUp():
   '''  Creates a copy of a segmentation in the parent of its parent segmentation.
   In the created segmentation, the set of segments will be the same as in the
   original. A vertex will be made member of a segment if it was transitively
   member of the corresponding segment in the original segmentation. The attributes
   and sub-segmentations of the segmentation are also copied.
 
 
   '''
 
+
 def reduceAttributeDimensions(save_as, vector, dimensions, method, perplexity):
   '''  Transforms (embeds) a `Vector` attribute to a lower-dimensional space.
   This is great for laying out graphs for visualizations based on vertex attributes
   rather than graph structure.
 
   :param save_as:   The new attribute will be created under this name.
   :param vector:   The high-dimensional vertex attribute that we want to embed.
@@ -2444,41 +2900,46 @@
   :param method:   The dimensionality reduction method to use.
     `Principal component analysis <https://en.wikipedia.org/wiki/Principal*component*analysis>`_ or
     `t-SNE <https://en.wikipedia.org/wiki/T-distributed*stochastic*neighbor_embedding>`_.
     (Implementations provided by `scikit-learn <https://scikit-learn.org/>`_.)
   :param perplexity:   Size of the vertex neighborhood to consider for t-SNE.
   '''
 
+
 def renameEdgeAttributes(title):
   '''  Changes the name of edge attributes.
 
   :param title:   If the new name is empty, the attribute will be discarded.
   '''
 
+
 def renameGraphAttributes(title):
   '''  Changes the name of graph attributes.
 
   :param title:   If the new name is empty, the attribute will be discarded.
   '''
 
+
 def renameSegmentation(before, after):
   '''  Changes the name of a segmentation.
 
   This operation is more easily accessed from the segmentation's dropdown menu in the graph state view.
 
   :param before:   The segmentation to rename.
   :param after:   The new name.
   '''
 
+
 def renameVertexAttributes(title):
   '''  Changes the name of vertex attributes.
 
   :param title:   If the new name is empty, the attribute will be discarded.
   '''
 
+
 def replaceEdgesWithTriadicClosure():
   '''  For every A→B→C triplet, creates an A→C edge. The original edges are discarded.
   The new A→C edge gets the attributes of the original A→B and B→C edges with prefixes "ab_" and "bc_".
 
   Be aware, in dense graphs a plenty of new edges can be generated.
 
   Possible use case: we are looking for connections between vertices, like same subscriber with multiple devices.
@@ -2487,43 +2948,48 @@
   that would be the winner does not exist.
   Often we think that a transitive closure would add the missing edge.
   For example, I don't call my second phone, but I call a lot of the same people from the two phones.
 
 
   '''
 
+
 def replaceWithEdgeGraph():
   '''  Creates the `edge graph <http://en.wikipedia.org/wiki/Edge_graph>`_ (or line graph),
   where each vertex corresponds to an edge in the current graph.
   The vertices will be connected, if one corresponding edge is the continuation of the other.
 
 
   '''
 
+
 def reverseEdgeDirection():
   '''  Replaces every A→B edge with its reverse edge (B→A).
 
   Attributes are preserved. Running this operation twice gets back the original graph.
 
 
   '''
 
-def sampleEdgesFromCoOccurrence(probability, seed):
+
+def sampleEdgesFromCooccurrence(probability, seed):
   '''  Connects vertices in the parent graph with a given probability
   if they co-occur in any segments.
   Multiple co-occurrences will have the same chance of being selected
   as single ones. Loop edges are also included with the same probability.
 
   :param probability:   The probability of choosing a vertex pair. The expected value of the number of
     created vertices will be *probability * number of edges without parallel edges*.
   :param seed:   The random seed.
     +
   '''
 
-def sampleGraphByRandomWalks(startpoints, walksfromonepoint, walkabortionprobability, vertexattrname, edgeattrname, seed):
+
+def sampleGraphByRandomWalks(startpoints, walksfromonepoint,
+                             walkabortionprobability, vertexattrname, edgeattrname, seed):
   '''  This operation realizes a random walk on the graph which can be used as a small smart sample to
   test your model on. The walk starts from a randomly selected vertex and at every step either aborts
   the current walk (with probability *Walk abortion probability*) and jumps back to the start point
   or moves to a randomly selected (directed sense) neighbor of the current vertex. After _Number of
   walks from each start point_ restarts it selects a new start vertex. After *Number of start points*
   new start points were selected, it stops. The performance of this algorithm according to different
   metrics can be found in the following publication,
@@ -2560,21 +3026,23 @@
     on vertices that were never reached.
   :param edgeattrname:   The name of the attribute which shows which step traversed the given edge first. It is not defined
     on edges that were never traversed.
   :param seed:   The random seed.
     +
   '''
 
+
 def saveToSnapshot(path):
   '''  Saves the input to a snapshot. The location of the snapshot has to be specified as
   a full path.
 
   :param path:   The full path of the target snapshot in the LynxKite directory system.
   '''
 
+
 def scoreEdgesWithTheForestFireModel(name, spread_prob, burn_ratio, seed):
   '''  Produces an edge attribute that reflects the importance of each edge in
   the spread of information or other communicable effects across the network.
 
   A simple summary of the algorithm would be:
 
   1. Pick a random vertex. The fire starts here.
@@ -2606,15 +3074,16 @@
   :param seed:   The seed used for picking where the fires start, which way they spread,
     and when they stop spreading.
     +
     Due to parallelization the algorithm may give different results even with the same seed.
     +
   '''
 
-def segmentByDoubleAttribute(name, attr, interval_size, overlap):
+
+def segmentByNumericAttribute(name, attr, interval_size, overlap):
   '''  Segments the vertices by a `number` vertex attribute.
 
   The domain of the attribute is split into intervals of the given size and every vertex that
   belongs to a given interval will belong to one segment. Empty segments are not created.
 
   :param name:   The new segmentation will be saved under this name.
   :param attr:   The `number` attribute to segment by.
@@ -2622,15 +3091,17 @@
     zero.
   :param overlap:   If you enable overlapping intervals, then each interval will have a 50% overlap
     with both the previous and the next interval. As a result each vertex will belong
     to two segments, guaranteeing that any vertices with an attribute value difference
     less than half the interval size will share at least one segment.
   '''
 
-def segmentByEventSequence(name, time_attr, location, algorithm, sequence_length, time_window_step, time_window_length):
+
+def segmentByEventSequence(name, time_attr, location, algorithm,
+                           sequence_length, time_window_step, time_window_length):
   '''  Treat vertices as people attending events, and segment them by attendance of sequences of events.
   There are several algorithms for generating event sequences, see under
   <<segment-by-event-sequence-algorithm, Algorithm>>.
 
   This operation runs on a segmentation which contains events as vertices, and it is a segmentation
   over a graph containing people as vertices.
 
@@ -2647,14 +3118,15 @@
     Takes all event sequences that are no longer than *Time window length* and then creates a segment
     for each subsequence with *Sequence length*.
   :param sequence_length:   Number of events in each segment.
   :param time_window_step:   Bucket size used for discretizing events.
   :param time_window_length:   Maximum time difference between first and last event in a segment.
   '''
 
+
 def segmentByGeographicalProximity(name, position, shapefile, distance, ignoreUnsupportedShapes):
   '''  Creates a segmentation from the features in a Shapefile. A vertex is connected to a segment if the
   the `position` vertex attribute is within a specified distance from the segment's geometry
   attribute. Feature attributes from the Shapefile become segmentation attributes.
 
   * The lookup depends on the coordinate reference system and distance metric of the feature. All
     inputs must use the same coordinate reference system and distance metric.
@@ -2671,14 +3143,15 @@
     and `.dbf` file of the same name.
   :param distance:   Vertices are connected to geographical segments if within this distance. The distance has to use
     the same metric and coordinate reference system as the features within the Shapefile.
   :param ignoreUnsupportedShapes:   If set `true`, silently ignores unknown shape types potentially contained by the Shapefile.
     Otherwise throws an error.
   '''
 
+
 def segmentByInterval(name, begin_attr, end_attr, interval_size, overlap):
   '''  Segments the vertices by a pair of `number` vertex attributes representing intervals.
 
   The domain of the attributes is split into intervals of the given size. Each of these
   intervals will represent a segment. Each vertex will belong to each segment whose
   interval intersects with the interval of the vertex. Empty segments are not created.
 
@@ -2687,80 +3160,87 @@
   :param end_attr:   The `number` attribute corresponding the end of intervals to segment by.
   :param interval_size:   The attribute's domain will be split into intervals of this size. The splitting always starts at
     zero.
   :param overlap:   If you enable overlapping intervals, then each interval will have a 50% overlap
     with both the previous and the next interval.
   '''
 
+
 def segmentByStringAttribute(name, attr):
   '''  Segments the vertices by a `String` vertex attribute.
 
   Every vertex with the same attribute value will belong to one segment.
 
   :param name:   The new segmentation will be saved under this name.
   :param attr:   The `String` attribute to segment by.
   '''
 
+
 def segmentByVectorAttribute(name, attr):
   '''  Segments the vertices by a vector vertex attribute.
 
   Segments are created from the values in all of the vector attributes. A vertex is connected
   to every segment corresponding to the elements in the vector.
 
   :param name:   The new segmentation will be saved under this name.
   :param attr:   The vector attribute to segment by.
   '''
 
+
 def setEdgeAttributeIcons(title):
   '''  Associates icons with edge attributes. It has no effect beyond highlighting something on the
   user interface.
 
   The icons are a subset of the Unicode characters in the "emoji" range, as provided by the
   `Google Noto Font <https://www.google.com/get/noto/help/emoji/>`_.
 
   :param title:   Leave empty to *remove* the icon for the corresponding attribute
     or add one of the supported icon names, such as `snowman*without*snow`.
   '''
 
+
 def setGraphAttributeIcon(name, icon):
   '''  Associates an icon with a graph attribute. It has no effect beyond highlighting something on the user
   interface.
 
   The icons are a subset of the Unicode characters in the "emoji" range, as provided by the
   `Google Noto Font <https://www.google.com/get/noto/help/emoji/>`_.
 
   :param name:   The graph attribute to highlight.
   :param icon:   One of the supported icon names, such as `snowman*without*snow`. Leave empty to *remove* the icon.
   '''
 
+
 def setSegmentationIcon(name, icon):
   '''  Associates an icon with a segmentation. It has no effect beyond highlighting something on the user
   interface.
 
   The icons are a subset of the Unicode characters in the "emoji" range, as provided by the
   `Google Noto Font <https://www.google.com/get/noto/help/emoji/>`_.
 
   This operation is more easily accessed from the segmentation's dropdown menu in the graph state view.
 
   :param name:   The segmentation to highlight.
   :param icon:   One of the supported icon names, such as `snowman*without*snow`. Leave empty to *remove* the icon.
   '''
 
+
 def setVertexAttributeIcons(title):
   '''  Associates icons vertex attributes. It has no effect beyond highlighting something on the
   user interface.
 
   The icons are a subset of the Unicode characters in the "emoji" range, as provided by the
   `Google Noto Font <https://www.google.com/get/noto/help/emoji/>`_.
 
   :param title:   Leave empty to *remove* the icon for the corresponding attribute
     or add one of the supported icon names, such as `snowman*without*snow`.
   '''
 
-def snowballSample(ratio, radius, attrname, seed):
+
+def createSnowballSample(ratio, radius, attrname, seed):
   '''  This operation creates a small smart sample of a graph. First, a subset of the original vertices is chosen
   for start points; the ratio of the size of this subset to the size of the original vertex set
   is the first parameter for the operation.
   Then a certain neighborhood of each start point is added to the sample; the radius of this neighborhood
   is controlled by another parameter.
   The result of the operation is a subgraph of the original graph consisting of the vertices of the sample and
   the edges between them.
@@ -2773,14 +3253,15 @@
   :param ratio:   The (approximate) fraction of vertices to use as starting points.
   :param radius:   Limits the size of the neighborhoods of the start points.
   :param attrname:   The name of the attribute which shows how far the sample vertices are from the closest start point.
   :param seed:   The random seed.
     +
   '''
 
+
 def splitEdges(rep, idx):
   '''  Split (multiply) edges in a graph. A numeric edge attribute controls how many
   copies of the edge should exist after the operation. If this attribute is
   1, the edge will be kept as it is. If this attribute is zero, the edge
   will be discarded entirely. Higher values (e.g., 2) will result in
   more identical copies of the given edge.
 
@@ -2794,25 +3275,27 @@
   :param rep:   A numeric edge attribute that specifies how many copies of the edge should
     exist after the operation.
     (The value is rounded to the nearest integer, so 1.8 will mean 2 copies.)
   :param idx:   The name of the attribute that will contain unique identifiers for the otherwise
     identical copies of the edge.
   '''
 
+
 def splitToTrainAndTestSet(source, test_set_ratio, seed):
   '''  Based on the source attribute, 2 new attributes are created, source*train and source*test.
   The attribute is partitioned, so every instance is copied to either the training or the test set.
 
   :param source:   The attribute you want to create train and test sets from.
   :param test_set_ratio:   A test set is a random sample of the vertices. This parameter gives the size of the test set
     as a fraction of the total vertex count.
   :param seed:   Random seed.
     +
   '''
 
+
 def splitVertices(rep, idx):
   '''  Split (multiply) vertices in a graph. A numeric vertex attribute controls how many
   copies of the vertex should exist after the operation. If this attribute is
   1, the vertex will be kept as it is. If this attribute is zero, the vertex
   will be discarded entirely. Higher values (e.g., 2) will result in
   more identical copies of the given vertex.
   All edges coming from and going to this vertex are
@@ -2831,14 +3314,15 @@
   :param rep:   A numberic vertex attribute that specifies how many copies of the vertex should
     exist after the operation.
     (The number value is rounded to the nearest integer, so 1.8 will mean 2 copies.)
   :param idx:   The name of the attribute that will contain unique identifiers for the otherwise
     identical copies of the vertex.
   '''
 
+
 def sql1():
   '''  Executes a SQL query on a single input, which can be either a graph or a table. Outputs a table.
   If the input is a table, it is available in the query as `input`. For example:
 
   ```
   select * from input
   ```
@@ -2850,14 +3334,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql10():
   '''  Executes an SQL query on its ten inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`, `six`, `seven`,
   `eight`, `nine`, `ten`. For example:
 
   ```
   select * from one
@@ -2877,41 +3362,44 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql2():
   '''  Executes an SQL query on its two inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one` and `two`. For example:
 
   ```
   select one.*, two.*
   from one
   join two
   on one.id
 
 
   '''
 
+
 def sql3():
   '''  Executes an SQL query on its three inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`. For example:
 
   ```
   select one.*, two.*, three.*
   from one
   join two
   join three
   on one.id
 
 
   '''
 
+
 def sql4():
   '''  Executes an SQL query on its four inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`. For example:
 
   ```
   select * from one
   union select * from two
@@ -2924,14 +3412,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql5():
   '''  Executes an SQL query on its five inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`. For example:
 
   ```
   select * from one
   union select * from two
@@ -2945,14 +3434,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql6():
   '''  Executes an SQL query on its six inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`, `six`. For example:
 
   ```
   select * from one
   union select * from two
@@ -2967,14 +3457,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql7():
   '''  Executes an SQL query on its seven inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`, `six`, `seven`.
   For example:
 
   ```
   select * from one
@@ -2991,14 +3482,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql8():
   '''  Executes an SQL query on its eight inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`, `six`, `seven`,
   `eight`. For example:
 
   ```
   select * from one
@@ -3016,14 +3508,15 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def sql9():
   '''  Executes an SQL query on its nine inputs, which can be either graphs or tables. Outputs a table.
   The inputs are available in the query as `one`, `two`, `three`, `four`, `five`, `six`, `seven`,
   `eight`, `nine`. For example:
 
   ```
   select * from one
@@ -3042,38 +3535,43 @@
 
   :prefix!:
   :maybe-tick!:
 
 
   '''
 
+
 def takeEdgesAsVertices():
   '''  Takes a graph and creates a new one where the vertices correspond to the original graph's
   edges. All edge attributes in the original graph are converted to vertex attributes in the new
   graph with the `edge_` prefix. All vertex attributes are converted to two vertex attributes with
   `src_` and `dst_` prefixes. Segmentations of the original graph are lost.
 
 
   '''
 
+
 def takeSegmentationAsBaseGraph():
   '''  Takes a segmentation of a graph and returns the segmentation as a base graph itself.
 
 
   '''
 
+
 def takeSegmentationLinksAsBaseGraph():
   '''  Replaces the current graph with the links from its base graph to the selected segmentation, represented
   as vertices. The vertices will have `base_` and `segment_` prefixed attributes generated for the
   attributes on the base graph and the segmentation respectively.
 
 
   '''
 
-def trainADecisionTreeClassificationModel(name, label, features, impurity, maxbins, maxdepth, mininfogain, minInstancesPerNode, seed):
+
+def trainADecisionTreeClassificationModel(
+        name, label, features, impurity, maxbins, maxdepth, mininfogain, minInstancesPerNode, seed):
   '''  Trains a decision tree classifier model using the graph's vertex attributes.
   The algorithm recursively partitions the feature space into two parts. The tree
   predicts the same label for each bottommost (leaf) partition. Each binary
   partitioning is chosen from a set of possible splits in order to maximize the
   information gain at the corresponding tree node. For calculating the information
   gain the impurity of the nodes is used (read more about impurity at the description
   of the impurity parameter): the information gain is the difference between the
@@ -3097,15 +3595,17 @@
   :param mininfogain:   Minimum information gain for a split to be considered as a tree node.
   :param minInstancesPerNode:   For a node to be split further, the split must improve at least this much
     (in terms of information gain).
   :param seed:   We maximize the information gain only among a subset of the possible splits.
     This random seed is used for selecting the set of splits we consider at a node.
   '''
 
-def trainADecisionTreeRegressionModel(name, label, features, maxbins, maxdepth, mininfogain, minInstancesPerNode, seed):
+
+def trainADecisionTreeRegressionModel(
+        name, label, features, maxbins, maxdepth, mininfogain, minInstancesPerNode, seed):
   '''  Trains a decision tree regression model using the graph's vertex attributes.
   The algorithm recursively partitions the feature space into two parts. The tree
   predicts the same label for each bottommost (leaf) partition. Each binary
   partitioning is chosen from a set of possible splits in order to maximize the
   information gain at the corresponding tree node. For calculating the information
   gain the variance of the nodes is used:
   the information gain is the difference between the parent node variance and the
@@ -3125,15 +3625,17 @@
   :param mininfogain:   Minimum information gain for a split to be considered as a tree node.
   :param minInstancesPerNode:   For a node to be split further, the split must improve at least this much
     (in terms of information gain).
   :param seed:   We maximize the information gain only among a subset of the possible splits.
     This random seed is used for selecting the set of splits we consider at a node.
   '''
 
-def trainAGcnClassifier(save_as, iterations, features, label, forget, batch_size, learning_rate, hidden_size, num_conv_layers, conv_op, seed):
+
+def trainAGCNClassifier(save_as, iterations, features, label, forget, batch_size,
+                        learning_rate, hidden_size, num_conv_layers, conv_op, seed):
   '''  Trains a `Graph Convolutional Network <https://tkipf.github.io/graph-convolutional-networks/>`_
   using `Pytorch Geometric <https://pytorch-geometric.readthedocs.io/en/latest/>`_.
   Applicable for classification problems.
 
   :param save_as:   The resulting model will be saved as a graph attribute using this name.
   :param iterations:   Number of training iterations.
   :param features:   Vector attribute containing the features to be used as inputs for the training algorithm.
@@ -3147,15 +3649,17 @@
   :param num_conv_layers:   Number of convolution layers.
   :param conv_op:   The type of graph convolution to use.
     `GCNConv <https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.conv.GCNConv>`_
     or `GatedGraphConv <https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.conv.GatedGraphConv>`_.
   :param seed:   Random seed for initializing network weights and choosing training batches.
   '''
 
-def trainAGcnRegressor(save_as, iterations, features, label, forget, batch_size, learning_rate, hidden_size, num_conv_layers, conv_op, seed):
+
+def trainAGCNRegressor(save_as, iterations, features, label, forget, batch_size,
+                       learning_rate, hidden_size, num_conv_layers, conv_op, seed):
   '''  Trains a `Graph Convolutional Network <https://tkipf.github.io/graph-convolutional-networks/>`_
   using `Pytorch Geometric <https://pytorch-geometric.readthedocs.io/en/latest/>`_.
   Applicable for regression problems.
 
   :param save_as:   The resulting model will be saved as a graph attribute using this name.
   :param iterations:   Number of training iterations.
   :param features:   Vector attribute containing the features to be used as inputs for the training algorithm.
@@ -3169,14 +3673,15 @@
   :param num_conv_layers:   Number of convolution layers.
   :param conv_op:   The type of graph convolution to use.
     `GCNConv <https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.conv.GCNConv>`_
     or `GatedGraphConv <https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.conv.GatedGraphConv>`_.
   :param seed:   Random seed for initializing network weights and choosing training batches.
   '''
 
+
 def trainAKmeansClusteringModel(name, features, k, max_iter, seed):
   '''  Trains a k-means clustering model using the graph's vertex attributes. The
   algorithm converges when the maximum number of iterations is reached or every
   cluster center does not move in the last iteration.
 
   `k-means clustering <https://en.wikipedia.org/wiki/K-means_clustering>`_ aims
   to partition *n* observations into *k* clusters in which each observation belongs
@@ -3188,15 +3693,16 @@
   :param features:   Attributes to be used as inputs for the training algorithm. The trained model
     will have a list of features with the same names and semantics.
   :param k:   The number of clusters to be created.
   :param max_iter:   The maximum number of iterations (>
   :param seed:   The random seed.
   '''
 
-def trainALogisticRegressionModel(name, label, features, max_iter):
+
+def trainALogisticRegressionModel(name, label, features, max_iter, elastic_net_param, reg_param):
   '''  Trains a logistic regression model using the graph's vertex attributes. The
   algorithm converges when the maximum number of iterations is reached or no
   coefficient has changed in the last iteration. The threshold of the model is
   chosen to maximize the `F-score <https://en.wikipedia.org/wiki/F1_score>`_.
 
   `Logistic regression <https://en.wikipedia.org/wiki/Logistic_regression>`_ measures
   the relationship between the categorical dependent variable and one or more
@@ -3205,35 +3711,41 @@
   The current implementation of logistic regression only supports binary classes.
 
   :param name:   The model will be stored as a graph attribute using this name.
   :param label:   The vertex attribute for which the model is trained to classify. The attribute should
     be binary label of either 0.0 or 1.0.
   :param features:   Attributes to be used as inputs for the training algorithm.
   :param max_iter:   The maximum number of iterations (>
+  :param elastic_net_param:   This parameter ("alpha") allows combining L1 and L2 regularization.
+    At alpha
+  :param reg_param:   The parameter of L1/L2 regularization, depending on how the elastic net mixing parameter is set.
   '''
 
+
 def trainLinearRegressionModel(name, label, features, method):
   '''  Trains a linear regression model using the graph's vertex attributes.
 
   :param name:   The model will be stored as a graph attribute using this name.
   :param label:   The vertex attribute for which the model is trained.
   :param features:   Attributes to be used as inputs for the training algorithm. The trained model
     will have a list of features with the same names and semantics.
   :param method:   The algorithm used to train the linear regression model.
   '''
 
+
 def transform():
   '''  Transforms all columns of a table input via SQL expressions. Outputs a table.
 
   An input parameter is generated for every table column. The parameters are
   SQL expressions interpreted on the input table. The default value leaves the column alone.
 
 
   '''
 
+
 def useBaseGraphAsSegmentation(name):
   '''  Creates a new segmentation which is a copy of the base graph. Also creates segmentation links
   between the original vertices and their corresponding vertices in the segmentation.
 
   For example, let's say we have a social network and we want to make a segmentation containing a
   selected group of people and the segmentation links should represent the original connections
   between the members of this selected group and other people.
@@ -3242,37 +3754,40 @@
   the <<Grow segmentation>> operation to add the necessary segmentation links. Finally, using the
   <<Filter by attributes>> operation, we can ensure that the segmentation contains only members of
   the selected group.
 
   :param name:   The name assigned to the new segmentation. It defaults to the graph's name.
   '''
 
+
 def useMetagraphAsGraph(timestamp):
   '''  Loads the relationships between LynxKite entities such as attributes and operations as a graph.
   This complex graph can be useful for debugging or demonstration purposes. Because it exposes
   data about all graphs, it is only accessible to administrator users.
 
   :param timestamp:   This number will be used to identify the current state of the metagraph. If you edit the history
     and leave the timestamp unchanged, you will get the same metagraph as before. If you change the
     timestamp, you will get the latest version of the metagraph.
   '''
 
+
 def useOtherGraphAsSegmentation():
   '''  Copies another graph into a new segmentation for this one. There will be no
   connections between the segments and the base vertices. You can import/create those via
   other operations. (See <<Use table as segmentation links>> and
   <<Define segmentation links from matching attributes>>.)
 
   It is possible to import the graph itself as segmentation. But even in this
   special case, there will be no connections between the segments and the base vertices.
   Another operation, <<Use base graph as segmentation>> can be used if edges are desired.
 
 
   '''
 
+
 def useTableAsEdgeAttributes(id_attr, id_column, prefix, unique_keys, if_exists):
   '''  Imports edge attributes for existing edges from a table. This is
   useful when you already have edges and just want to import one or more attributes.
 
   There are two different use cases for this operation:
   - Import using unique edge attribute values. For example if the edges represent relationships
   between people (identified by `src` and `dst` IDs) we can import the number of total calls between
@@ -3299,63 +3814,68 @@
       are identical to the values in the graph on edges where both are defined.
     - **Keep the graph's version**: The data in the table is ignored.
     - **Use the table's version**: The attribute is deleted from the graph and replaced with
       the attribute imported from the table.
     - **Disallow this**: A name conflict is treated as an error.
   '''
 
+
 def useTableAsEdges(attr, src, dst):
   '''  Imports edges from a table. Your vertices must have an identifying attribute, by which
   the edges can be attached to them.
 
   :param attr:   The IDs that are used in the file when defining the edges.
   :param src:   The table column that specifies the source of the edge.
   :param dst:   The table column that specifies the destination of the edge.
   '''
 
+
 def useTableAsGraph(src, dst):
   '''  Imports edges from a table. Each line in the table represents one edge.
   Each column in the table will be accessible as an edge attribute.
 
   Vertices will be generated for the endpoints of the edges with two vertex attributes:
 
    - `stringId` will contain the ID string that was used in the table.
    - `id` will contain the internal vertex ID.
 
   This is useful when your table contains edges (e.g., calls) and there is no separate
   table for vertices. This operation makes it possible to load edges and use them
   as a graph. Note that this graph will never have zero-degree vertices.
 
-  :param src: 
+  :param src:
   :param dst:
   '''
 
+
 def useTableAsSegmentationLinks(base_id_attr, base_id_column, seg_id_attr, seg_id_column):
   '''  Import the connection between the main graph and this segmentation from a table.
   Each row in the table represents a connection between one base vertex and one segment.
 
   :param base_id_attr:   The `String` vertex attribute that can be joined to the identifying column in the table.
   :param base_id_column:   The table column that can be joined to the identifying attribute on the base graph.
   :param seg_id_attr:   The `String` vertex attribute that can be joined to the identifying column in the table.
   :param seg_id_column:   The table column that can be joined to the identifying attribute on the segmentation.
   '''
 
+
 def useTableAsSegmentation(name, base_id_attr, base_id_column, seg_id_column):
   '''  Imports a segmentation from a table. The table must have a column identifying an existing vertex by
   a String attribute and another column that specifies the segment it belongs to.
   Each vertex may belong to any number of segments.
 
   The rest of the columns in the table are ignored.
 
   :param name:   The imported segmentation will be created under this name.
   :param base_id_attr:   The `String` vertex attribute that identifies the base vertices.
   :param base_id_column:   The table column that identifies vertices.
   :param seg_id_column:   The table column that identifies segments.
   '''
 
+
 def useTableAsVertexAttributes(id_attr, id_column, prefix, unique_keys, if_exists):
   '''  Imports vertex attributes for existing vertices from a table. This is
   useful when you already have vertices and just want to import one or more attributes.
 
   There are two different use cases for this operation:
   - Import using unique vertex attribute values. For example if the vertices represent people
   this attribute can be a personal ID. In this case the operation fails in case of duplicate
@@ -3381,50 +3901,55 @@
       are identical to the values in the graph on vertices where both are defined.
     - **Keep the graph's version**: The data in the table is ignored.
     - **Use the table's version**: The attribute is deleted from the graph and replaced with
       the attribute imported from the table.
     - **Disallow this**: A name conflict is treated as an error.
   '''
 
+
 def useTableAsVertices():
   '''  Imports vertices (no edges) from a table.
   Each column in the table will be accessible as a vertex attribute.
 
 
   '''
 
+
 def weightedAggregateEdgeAttributeGlobally(prefix, weight):
   '''  Aggregates edge attributes across the entire graph into one graph attribute for each attribute.
   For example you could use it to calculate the total income as the sum of call durations
   weighted by the rates across an entire call dataset.
 
   :param prefix:   Save the aggregated values with this prefix.
   :param weight:   The `number` attribute to use as weight.
   '''
 
+
 def weightedAggregateEdgeAttributeToVertices(prefix, weight, direction):
   '''  Aggregates an attribute on all the edges going in or out of vertices.
   For example it can calculate the average cost per second of calls for each person.
 
   :param prefix:   Save the aggregated attributes with this prefix.
   :param weight:   The `number` attribute to use as weight.
   :param direction:   - `incoming edges`: Aggregate across the edges coming in to each vertex.
      - `outgoing edges`: Aggregate across the edges going out of each vertex.
      - `all edges`: Aggregate across all the edges going in or out of each vertex.
   '''
 
+
 def weightedAggregateFromSegmentation(prefix, weight):
   '''  Aggregates vertex attributes across all the segments that a vertex in the base graph belongs to.
   For example, it can calculate an average over the cliques a person belongs to, weighted by
   the size of the cliques.
 
   :param prefix:   Save the aggregated attributes with this prefix.
   :param weight:   The `number` attribute to use as weight.
   '''
 
+
 def weightedAggregateOnNeighbors(prefix, weight, direction):
   '''  Aggregates across the vertices that are connected to each vertex. You can use
   the `Aggregate on` parameter to define how exactly this aggregation will take
   place: choosing one of the 'edges' settings can result in a neighboring
   vertex being taken into account several times (depending on the number of edges between
   the vertex and its neighboring vertex); whereas choosing one of the 'neighbors' settings
   will result in each neighboring vertex being taken into account once.
@@ -3446,21 +3971,23 @@
        that have an incoming edge from A.
      - `all neighbors`: For each vertex A, aggregate across those vertices
        that either have an outgoing edge to or an incoming edge from A.
      - `symmetric neighbors`: For each vertex A, aggregate across those vertices
        that have both an outgoing edge to and an incoming edge from A.
   '''
 
+
 def weightedAggregateToSegmentation(weight):
   '''  Aggregates vertex attributes across all the vertices that belong to a segment.
   For example, it can calculate the average age per kilogram of each clique.
 
   :param weight:   The `number` attribute to use as weight.
   '''
 
+
 def weightedAggregateVertexAttributeGlobally(prefix, weight):
   '''  Aggregates vertex attributes across the entire graph into one graph attribute for each attribute.
   For example you could use it to calculate the average age across an entire dataset of people
   weighted by their PageRank.
 
   :param prefix:   Save the aggregated values with this prefix.
   :param weight:   The `number` attribute to use as weight.
```

### Comparing `lynxkite_client-5.3.0/tests/test_boxpath.py` & `lynxkite_client-5.4.1/tests/test_boxpath.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_cleaner.py` & `lynxkite_client-5.4.1/tests/test_cleaner.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_download.py` & `lynxkite_client-5.4.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_escaping_strings.py` & `lynxkite_client-5.4.1/tests/test_escaping_strings.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_external_computation.py` & `lynxkite_client-5.4.1/tests/test_external_computation.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     # The triggerables are in insertion order.
     self.assertEqual([
         'saveToSnapshot', 'exportToParquet', 'exportToParquet', 'externalComputation2',
         'saveToSnapshot'],
         [t.base.operation for t in sec.all_triggerables()])
     deps = lynx.kite.BoxPath.dependencies(list(sec.all_triggerables()))
     # Dependencies are correctly found.
+    self.maxDiff = None
     self.assertEqual({
         'compute_?/join_0/exportToParquet_0': {'compute_?/saveToSnapshot_1'},
         'compute_?/join_0/exportToParquet_1': {'compute_?/saveToSnapshot_1'},
         'compute_?/join_0/externalComputation2_0': {'compute_?/join_0/exportToParquet_0',
                                                     'compute_?/join_0/exportToParquet_1',
                                                     'compute_?/saveToSnapshot_0',
                                                     'compute_?/saveToSnapshot_1'},
@@ -180,31 +181,30 @@
     t = f(eg)
     t.trigger()
     # Second time we should get the same snapshot
     second_entry_list = [e.name for e in lk.list_dir(tmp_dir)]
     self.assertEqual(first_entry_list, second_entry_list)
 
   def test_external_box_callable_edge_cases(self):
-    lk = lynx.kite.LynxKite()
-    with self.assertRaises(Exception) as context:
-      f = lynx.kite.external(lambda x: 1)
-      self.assertTrue(
-          'You cannot use lambda functions for external computation.' in str(
-              cm.exception))
+    with self.assertRaises(Exception) as cm:
+      lynx.kite.external(lambda x: 1)
+    self.assertTrue(
+        'You cannot use lambda functions for external computation.' in str(
+            cm.exception))
 
     class A:
       def g(x):
         return 1
 
     o = A()
-    with self.assertRaises(Exception) as context:
-      f = lynx.kite.external(o.g)
-      self.assertTrue(
-          'You cannot use instance methods for external computation.' in str(
-              cm.exception))
+    with self.assertRaises(Exception) as cm:
+      lynx.kite.external(o.g)
+    self.assertTrue(
+        'You cannot use instance methods for external computation.' in str(
+            cm.exception))
 
 
 class TestTmpFilesHandling(unittest.TestCase):
   # On Jenkins all jobs are using the same /tmp folder so we are setting the tmp dir used by the
   # tempfile module to be a separate folder.
   tmp_dir = tempfile.gettempdir() + '/external_tests'
   shutil.rmtree(tmp_dir, ignore_errors=True)
```

### Comparing `lynxkite_client-5.3.0/tests/test_hive_export.py` & `lynxkite_client-5.4.1/tests/test_hive_export.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_pandas_conversion.py` & `lynxkite_client-5.4.1/tests/test_pandas_conversion.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_spark_conversion.py` & `lynxkite_client-5.4.1/tests/test_spark_conversion.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_sql_shorthand.py` & `lynxkite_client-5.4.1/tests/test_sql_shorthand.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_subworkspace_decorator.py` & `lynxkite_client-5.4.1/tests/test_subworkspace_decorator.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_tutorials.py` & `lynxkite_client-5.4.1/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_workspace.py` & `lynxkite_client-5.4.1/tests/test_workspace.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_workspace_builder.py` & `lynxkite_client-5.4.1/tests/test_workspace_builder.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_workspace_decorator.py` & `lynxkite_client-5.4.1/tests/test_workspace_decorator.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/test_workspace_with_side_effects.py` & `lynxkite_client-5.4.1/tests/test_workspace_with_side_effects.py`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/03_Airlines_Edge.csv` & `lynxkite_client-5.4.1/tests/data/03_Airlines_Edge.csv`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/03_Airlines_Vertex.csv` & `lynxkite_client-5.4.1/tests/data/03_Airlines_Vertex.csv`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/beno_facebook_edges.csv` & `lynxkite_client-5.4.1/tests/data/beno_facebook_edges.csv`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/beno_facebook_vertices.csv` & `lynxkite_client-5.4.1/tests/data/beno_facebook_vertices.csv`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/tutorial-02-test.yaml` & `lynxkite_client-5.4.1/tests/data/tutorial-02-test.yaml`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/tests/data/tutorial-03-test.yaml` & `lynxkite_client-5.4.1/tests/data/tutorial-03-test.yaml`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/.gitignore` & `lynxkite_client-5.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lynxkite_client-5.3.0/pyproject.toml` & `lynxkite_client-5.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lynxkite-client"
-version = "5.3.0"
+version = "5.4.1"
 authors = [
   { name="Lynx Analytics", email="lynxkite@lynxkite.com" },
 ]
 description = "Python API for LynxKite"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+  "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 requires-python = ">=3.6"
 dependencies = [
   "requests",
   "pandas",
 ]
```

