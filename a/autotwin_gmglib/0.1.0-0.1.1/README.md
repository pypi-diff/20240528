# Comparing `tmp/autotwin_gmglib-0.1.0.tar.gz` & `tmp/autotwin_gmglib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotwin_gmglib-0.1.0.tar", max compression
+gzip compressed data, was "autotwin_gmglib-0.1.1.tar", max compression
```

## Comparing `autotwin_gmglib-0.1.0.tar` & `autotwin_gmglib-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    68786 2024-05-14 08:37:20.000000 autotwin_gmglib-0.1.0/autotwin_gmglib.py
--rw-r--r--   0        0        0     1518 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.0/LICENSE
--rw-r--r--   0        0        0      931 2024-05-14 08:57:00.000000 autotwin_gmglib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      643 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.0/README.md
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 autotwin_gmglib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    68365 2024-05-28 08:44:34.000000 autotwin_gmglib-0.1.1/autotwin_gmglib.py
+-rw-r--r--   0        0        0     1518 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.1/LICENSE
+-rw-r--r--   0        0        0      931 2024-05-28 08:58:00.000000 autotwin_gmglib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      643 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.1/README.md
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 autotwin_gmglib-0.1.1/PKG-INFO
```

### Comparing `autotwin_gmglib-0.1.0/autotwin_gmglib.py` & `autotwin_gmglib-0.1.1/autotwin_gmglib.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import matplotlib.colors as mcolors
 import matplotlib.patches as mpatches
 import matplotlib.backend_bases as mbackend
 import matplotlib.widgets as mwidgets
 import threading
 import warnings
 import bisect
+import copy
 import scipy
 import math
 
 pandas.options.mode.copy_on_write = False
 mpyplot.rcParams["pdf.fonttype"] = 42
 mpyplot.rcParams["ps.fonttype"] = 42
 
@@ -137,15 +138,15 @@
     """
     start_time = time.time()
     model = networkx.DiGraph(name=config["name"], version=config["version"])
     station_sublogs, part_sublogs = _extract_sublogs(log)
     _normalize_activities(station_sublogs, part_sublogs, log)
     _mine_topology(model, station_sublogs, part_sublogs, log)
     _identify_operations(model, station_sublogs, part_sublogs)
-    _mine_formulas(model, station_sublogs, part_sublogs, log)
+    _mine_formulas(model, station_sublogs, part_sublogs, log, config)
     window = [-1, len(log) - 1]
     _reconstruct_states(model, station_sublogs, part_sublogs, log, window)
     _mine_capacities(model, log, window)
     _mine_processing_times(model, station_sublogs, part_sublogs, log, window, config)
     _mine_transfer_times(model, station_sublogs, part_sublogs, log, window, config)
     _mine_routing_probabilities(model, part_sublogs, window)
     model.graph["time_spent"] = time.time() - start_time
@@ -1061,22 +1062,24 @@
 
 
 def _mine_formulas(
     model: networkx.DiGraph,
     station_sublogs: dict[str, pandas.DataFrame],
     part_sublogs: dict[str, pandas.DataFrame],
     log: pandas.DataFrame,
+    config: dict[str, Any],
 ):
     """Mine input-output formulas at each station.
 
     Args:
         model: Graph model.
         station_sublogs: Station sublogs.
         part_sublogs: Part sublogs.
         log: Event log.
+        config: Configuration.
     """
     log["input"] = None
     log["output"] = None
     for i in range(len(log) - 1):
         event = log.loc[i]
         activity = event["activity"]
         if activity == "ENTER_BP":
@@ -1205,14 +1208,24 @@
                     and len(formula["input"]) > 0
                     and len(formula["output"]) > 0
                 ):
                     formulas.append(formula)
                     frequencies.append(1)
                     formula = None
 
+        indexes = []
+        max_frequency = max(frequencies)
+        min_ratio = config["model"]["formula"]["ratio"]
+        for x in range(len(frequencies)):
+            if frequencies[x] / max_frequency < min_ratio:
+                indexes.append(x)
+        indexes.reverse()
+        for x in indexes:
+            del formulas[x]
+
 
 def _reconstruct_states(
     model: networkx.DiGraph,
     station_sublogs: dict[str, pandas.DataFrame],
     part_sublogs: dict[str, pandas.DataFrame],
     log: pandas.DataFrame,
     window: list[int],
@@ -1232,36 +1245,57 @@
         station = event["station"]
         activity = event["activity"]
         if not model.nodes[station]["is_sink"] and activity.startswith("EXIT"):
             i = sublog.index[j]
             if i < window[1]:
                 window[1] = i
 
+    zero_state = dict()
+    for station in model.nodes.keys():
+        zero_state[station] = dict()
+        zero_state[station]["B"] = dict()
+        zero_state[station]["M"] = dict()
+        sublog = station_sublogs[station]
+        for j in range(len(sublog)):
+            event = sublog.iloc[j]
+            type_ = event["type"]
+            activity = event["activity"]
+            if activity.startswith("ENTER"):
+                zero_state[station]["B"][type_] = 0
+                zero_state[station]["M"][type_] = 0
+            else:
+                zero_state[station]["M"][type_] = 0
+
     log["state"] = None
     for i in range(window[0], window[1]):
-        log.at[i, "state"] = _create_state(model)
+        log.at[i, "state"] = copy.deepcopy(zero_state)
     for sublog in station_sublogs.values():
         sublog["state"] = None
         sublog.update(log["state"])
     for sublog in part_sublogs.values():
         sublog["state"] = None
         sublog.update(log["state"])
 
     previous_state = log.at[window[0], "state"]
-    floor_state = _create_state(model)
+    floor_state = copy.deepcopy(zero_state)
     for i in range(window[0] + 1, window[1]):
         event = log.loc[i]
         station = event["station"]
         part = event["part"]
         type_ = event["type"]
         activity = event["activity"]
         input_ = event["input"]
         output = event["output"]
         state = event["state"]
-        _copy_state(previous_state, state)
+        for station_ in previous_state.keys():
+            for location_ in previous_state[station_].keys():
+                for type__ in previous_state[station_][location_].keys():
+                    state[station_][location_][type__] = (
+                        previous_state[station_][location_][type__]
+                    )
         is_source = model.nodes[station]["is_source"]
         is_sink = model.nodes[station]["is_sink"]
         operation = model.nodes[station]["operation"]
         if activity.startswith("ENTER"):
             if not is_source:
                 state[station]["B"][type_] -= 1
             if (
@@ -1289,81 +1323,31 @@
                 state[next_station]["B"][type_] += 1
         if activity.startswith("ENTER"):
             floor_state[station]["B"][type_] = min(
                 state[station]["B"][type_],
                 floor_state[station]["B"][type_],
             )
         else:
-            for input_type in state[station]["M"].keys():
-                floor_state[station]["M"][input_type] = min(
-                    state[station]["M"][input_type],
-                    floor_state[station]["M"][input_type],
+            for type__ in state[station]["M"].keys():
+                floor_state[station]["M"][type__] = min(
+                    state[station]["M"][type__],
+                    floor_state[station]["M"][type__],
                 )
         previous_state = state
 
     for i in range(window[0], window[1]):
         state = log.at[i, "state"]
         for station in state.keys():
             for location in state[station].keys():
                 for type_ in state[station][location].keys():
                     state[station][location][type_] -= (
                         floor_state[station][location][type_]
                     )
 
 
-def _create_state(model: networkx.DiGraph) -> dict[str, dict[str, dict[str, int]]]:
-    """Create a new state.
-
-    Args:
-        model: Graph model.
-
-    Returns:
-        New state.
-    """
-    state = dict()
-    for station in model.nodes.keys():
-        state[station] = dict()
-        operation = model.nodes[station]["operation"]
-        formulas = model.nodes[station]["formulas"]
-        for location in ["B", "M"]:
-            state[station][location] = dict()
-            if location == "B":
-                for formula in formulas:
-                    for type_ in formula["input"].keys():
-                        state[station][location][type_] = 0
-            else:
-                if operation in {"ORDINARY", "REPLACE", "ATTACH", "COMPOSE"}:
-                    for formula in formulas:
-                        for type_ in formula["input"].keys():
-                            state[station][location][type_] = 0
-                else:
-                    for formula in formulas:
-                        for type_ in formula["output"].keys():
-                            state[station][location][type_] = 0
-    return state
-
-
-def _copy_state(
-    source_state: dict[str, dict[str, dict[str, int]]],
-    target_state: dict[str, dict[str, dict[str, int]]],
-):
-    """Copy one state to another.
-
-    Args:
-        source_state: Source state.
-        target_state: Target state.
-    """
-    for station in source_state.keys():
-        for location in source_state[station].keys():
-            for type_ in source_state[station][location].keys():
-                target_state[station][location][type_] = (
-                    source_state[station][location][type_]
-                )
-
-
 def _mine_capacities(model: networkx.DiGraph, log: pandas.DataFrame, window: list[int]):
     """Mine buffer and machine capacities at each station.
 
     Args:
         model: Graph model.
         log: Event log.
         window: Definite window.
```

### Comparing `autotwin_gmglib-0.1.0/LICENSE` & `autotwin_gmglib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotwin_gmglib-0.1.0/pyproject.toml` & `autotwin_gmglib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autotwin_gmglib"
-version = "0.1.0"
+version = "0.1.1"
 description = "Graph Model Generation Library for Auto-Twin"
 license = "BSD-3-Clause"
 authors = [
     "Lulai Zhu <lulai.zhu@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/AutotwinEU/graph-model-gen"
```

### Comparing `autotwin_gmglib-0.1.0/README.md` & `autotwin_gmglib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autotwin_gmglib-0.1.0/PKG-INFO` & `autotwin_gmglib-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotwin_gmglib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Graph Model Generation Library for Auto-Twin
 Home-page: https://github.com/AutotwinEU/graph-model-gen
 License: BSD-3-Clause
 Keywords: auto-twin,system discovery,graph model
 Author: Lulai Zhu
 Author-email: lulai.zhu@gmail.com
 Requires-Python: >=3.10,<4.0
```

