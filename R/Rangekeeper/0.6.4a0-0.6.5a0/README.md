# Comparing `tmp/rangekeeper-0.6.4a0.tar.gz` & `tmp/rangekeeper-0.6.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rangekeeper-0.6.4a0.tar", max compression
+gzip compressed data, was "rangekeeper-0.6.5a0.tar", max compression
```

## Comparing `rangekeeper-0.6.4a0.tar` & `rangekeeper-0.6.5a0.tar`

### file list

```diff
@@ -1,30 +1,25 @@
--rwxr-xr-x   0        0        0     1278 2024-03-14 12:52:33.213049 rangekeeper-0.6.4a0/README.md
--rwxr-xr-x   0        0        0      836 2024-05-24 04:30:18.412157 rangekeeper-0.6.4a0/pyproject.toml
--rwxr-xr-x   0        0        0     1736 2024-03-14 12:52:33.214027 rangekeeper-0.6.4a0/rangekeeper/__init__.py
--rwxr-xr-x   0        0        0     4790 2024-03-14 12:52:33.214176 rangekeeper-0.6.4a0/rangekeeper/api.py
--rwxr-xr-x   0        0        0       43 2024-03-14 12:52:33.214303 rangekeeper-0.6.4a0/rangekeeper/conftest.py
--rwxr-xr-x   0        0        0     9159 2024-03-14 12:52:33.214433 rangekeeper-0.6.4a0/rangekeeper/distribution.py
--rwxr-xr-x   0        0        0    16273 2024-05-24 04:28:47.821802 rangekeeper-0.6.4a0/rangekeeper/duration.py
--rwxr-xr-x   0        0        0      207 2024-03-14 12:52:33.214768 rangekeeper-0.6.4a0/rangekeeper/dynamics/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-03-14 12:52:33.214969 rangekeeper-0.6.4a0/rangekeeper/dynamics/black_swan.py
--rwxr-xr-x   0        0        0    16156 2024-03-14 12:52:33.215119 rangekeeper-0.6.4a0/rangekeeper/dynamics/cyclicality.py
--rwxr-xr-x   0        0        0     5943 2024-03-14 12:52:33.215332 rangekeeper-0.6.4a0/rangekeeper/dynamics/market.py
--rwxr-xr-x   0        0        0     1322 2024-03-14 12:52:33.215541 rangekeeper-0.6.4a0/rangekeeper/dynamics/noise.py
--rwxr-xr-x   0        0        0     2361 2024-03-14 12:52:33.215737 rangekeeper-0.6.4a0/rangekeeper/dynamics/trend.py
--rwxr-xr-x   0        0        0     5162 2024-03-14 12:52:33.215880 rangekeeper-0.6.4a0/rangekeeper/dynamics/volatility.py
--rwxr-xr-x   0        0        0     2974 2024-03-14 12:52:33.216084 rangekeeper-0.6.4a0/rangekeeper/extrapolation.py
--rwxr-xr-x   0        0        0    25912 2024-03-14 12:52:33.216260 rangekeeper-0.6.4a0/rangekeeper/flux.py
--rwxr-xr-x   0        0        0    27073 2024-03-14 12:52:33.216448 rangekeeper-0.6.4a0/rangekeeper/graph.py
--rwxr-xr-x   0        0        0     4138 2024-03-14 12:52:33.216643 rangekeeper-0.6.4a0/rangekeeper/measure.py
--rwxr-xr-x   0        0        0      199 2024-03-14 12:52:33.216790 rangekeeper-0.6.4a0/rangekeeper/models/__init__.py
--rwxr-xr-x   0        0        0     5254 2024-03-14 12:52:33.216980 rangekeeper-0.6.4a0/rangekeeper/models/deterministic.py
--rwxr-xr-x   0        0        0     6631 2024-03-14 12:52:33.217147 rangekeeper-0.6.4a0/rangekeeper/models/flexible.py
--rwxr-xr-x   0        0        0     5499 2024-03-14 12:52:33.217300 rangekeeper-0.6.4a0/rangekeeper/models/linear.py
--rwxr-xr-x   0        0        0     6389 2024-03-14 12:52:33.217434 rangekeeper-0.6.4a0/rangekeeper/models/linear_graph.py
--rwxr-xr-x   0        0        0     5864 2024-03-14 12:52:33.217599 rangekeeper-0.6.4a0/rangekeeper/models/probabilistic.py
--rw-r--r--   0        0        0      567 2024-03-14 12:52:33.217760 rangekeeper-0.6.4a0/rangekeeper/policy.py
--rwxr-xr-x   0        0        0     7085 2024-03-14 12:52:33.217896 rangekeeper-0.6.4a0/rangekeeper/projection.py
--rwxr-xr-x   0        0        0     6862 2024-03-14 12:52:33.218062 rangekeeper-0.6.4a0/rangekeeper/segmentation.py
--rwxr-xr-x   0        0        0     1167 2024-03-14 12:52:33.218223 rangekeeper-0.6.4a0/rangekeeper/space.py
--rwxr-xr-x   0        0        0     7314 2024-03-14 12:52:33.218380 rangekeeper-0.6.4a0/rangekeeper/span.py
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 rangekeeper-0.6.4a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1278 2024-03-14 12:52:33.213049 rangekeeper-0.6.5a0/README.md
+-rwxr-xr-x   0        0        0      836 2024-05-28 11:39:44.758113 rangekeeper-0.6.5a0/pyproject.toml
+-rwxr-xr-x   0        0        0     1737 2024-05-28 01:51:32.037351 rangekeeper-0.6.5a0/rangekeeper/__init__.py
+-rwxr-xr-x   0        0        0     4790 2024-03-14 12:52:33.214176 rangekeeper-0.6.5a0/rangekeeper/api.py
+-rwxr-xr-x   0        0        0       43 2024-03-14 12:52:33.214303 rangekeeper-0.6.5a0/rangekeeper/conftest.py
+-rwxr-xr-x   0        0        0     9159 2024-03-14 12:52:33.214433 rangekeeper-0.6.5a0/rangekeeper/distribution.py
+-rwxr-xr-x   0        0        0    16273 2024-05-24 04:28:47.821802 rangekeeper-0.6.5a0/rangekeeper/duration.py
+-rwxr-xr-x   0        0        0      207 2024-03-14 12:52:33.214768 rangekeeper-0.6.5a0/rangekeeper/dynamics/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-03-14 12:52:33.214969 rangekeeper-0.6.5a0/rangekeeper/dynamics/black_swan.py
+-rwxr-xr-x   0        0        0    16156 2024-03-14 12:52:33.215119 rangekeeper-0.6.5a0/rangekeeper/dynamics/cyclicality.py
+-rwxr-xr-x   0        0        0     5943 2024-03-14 12:52:33.215332 rangekeeper-0.6.5a0/rangekeeper/dynamics/market.py
+-rwxr-xr-x   0        0        0     1322 2024-03-14 12:52:33.215541 rangekeeper-0.6.5a0/rangekeeper/dynamics/noise.py
+-rwxr-xr-x   0        0        0     2361 2024-03-14 12:52:33.215737 rangekeeper-0.6.5a0/rangekeeper/dynamics/trend.py
+-rwxr-xr-x   0        0        0     5162 2024-03-14 12:52:33.215880 rangekeeper-0.6.5a0/rangekeeper/dynamics/volatility.py
+-rwxr-xr-x   0        0        0     2974 2024-03-14 12:52:33.216084 rangekeeper-0.6.5a0/rangekeeper/extrapolation.py
+-rwxr-xr-x   0        0        0    25945 2024-05-28 05:35:04.094403 rangekeeper-0.6.5a0/rangekeeper/flux.py
+-rw-r--r--   0        0        0     2652 2024-05-28 06:45:25.440667 rangekeeper-0.6.5a0/rangekeeper/formula.py
+-rwxr-xr-x   0        0        0    27073 2024-03-14 12:52:33.216448 rangekeeper-0.6.5a0/rangekeeper/graph.py
+-rwxr-xr-x   0        0        0     4138 2024-03-14 12:52:33.216643 rangekeeper-0.6.5a0/rangekeeper/measure.py
+-rw-r--r--   0        0        0      567 2024-03-14 12:52:33.217760 rangekeeper-0.6.5a0/rangekeeper/policy.py
+-rwxr-xr-x   0        0        0     5847 2024-05-28 06:02:56.254787 rangekeeper-0.6.5a0/rangekeeper/projection.py
+-rwxr-xr-x   0        0        0     6862 2024-03-14 12:52:33.218062 rangekeeper-0.6.5a0/rangekeeper/segmentation.py
+-rwxr-xr-x   0        0        0     1167 2024-03-14 12:52:33.218223 rangekeeper-0.6.5a0/rangekeeper/space.py
+-rwxr-xr-x   0        0        0     7314 2024-03-14 12:52:33.218380 rangekeeper-0.6.5a0/rangekeeper/span.py
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 rangekeeper-0.6.5a0/PKG-INFO
```

### Comparing `rangekeeper-0.6.4a0/README.md` & `rangekeeper-0.6.5a0/README.md`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/pyproject.toml` & `rangekeeper-0.6.5a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rangekeeper"
-version = "0.6.4-alpha"
+version = "0.6.5-alpha"
 description = "A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like"
 authors = ["Daniel Fink <danfink@mit.edu>"]
 license = "MPL-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
@@ -13,15 +13,15 @@
 pint = "^0.23"
 pyxirr = "^0.10.3"
 scipy = "^1.13.1"
 networkx = "^3.3"
 py-moneyed = "^3.0"
 tabulate = "^0.9.0"
 pyyaml = "^6.0.1"
-specklepy = "^2.19.0"
+specklepy = "^2.19.1"
 numba = "^0.59.1"
 multiprocess = "^0.70.16"
 seaborn = "^0.13.2"
 pyvis = "^0.3.2"
 plotly = "^5.22.0"
 mpld3 = "^0.5.10"
 pyarrow = "^16.1.0"
```

### Comparing `rangekeeper-0.6.4a0/rangekeeper/__init__.py` & `rangekeeper-0.6.5a0/rangekeeper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 from . import graph as graph
 from . import measure as measure
 from . import policy as policy
 from . import projection as projection
 from . import span as span
 from . import segmentation as segmentation
 from . import space as space
-
 from . import dynamics as dynamics
-
-from . import models as models
+from . import formula as formula
 
 # Helper Methods:
 import functools
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib import cm
 
@@ -48,7 +46,8 @@
     Returns the rgb value of a color from a matplotlib colormap
     from https://stackoverflow.com/a/26109298
     """
     cmap = plt.get_cmap(cmap_name)
     norm = mpl.colors.Normalize(vmin=start_val, vmax=stop_val)
     scalar_map = cm.ScalarMappable(norm=norm, cmap=cmap)
     return scalar_map.to_rgba(val)
+
```

### Comparing `rangekeeper-0.6.4a0/rangekeeper/api.py` & `rangekeeper-0.6.5a0/rangekeeper/api.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/distribution.py` & `rangekeeper-0.6.5a0/rangekeeper/distribution.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/duration.py` & `rangekeeper-0.6.5a0/rangekeeper/duration.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/black_swan.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/black_swan.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/cyclicality.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/cyclicality.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/market.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/market.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/noise.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/noise.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/trend.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/trend.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/dynamics/volatility.py` & `rangekeeper-0.6.5a0/rangekeeper/dynamics/volatility.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/extrapolation.py` & `rangekeeper-0.6.5a0/rangekeeper/extrapolation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/flux.py` & `rangekeeper-0.6.5a0/rangekeeper/flux.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,15 +424,15 @@
             self,
             tablefmt: str = 'github',
             decimals: int = 2):
 
         floatfmt = "." + str(decimals) + "f"
 
         linebreak = os.linesep
-        name = 'Name: ' + self.name
+        name = 'Name: ' + self.name if self.name is not None else ''
         units = 'Units: ' + json.dumps({flow.name: flow.units.__str__() for flow in self.flows}, indent=4)
         flows = 'Flows: ' + linebreak + self._format_flows(decimals=decimals).to_markdown(
             tablefmt=tablefmt,
             stralign="right",
             numalign="right",
             floatfmt=floatfmt)
```

### Comparing `rangekeeper-0.6.4a0/rangekeeper/graph.py` & `rangekeeper-0.6.5a0/rangekeeper/graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/measure.py` & `rangekeeper-0.6.5a0/rangekeeper/measure.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/policy.py` & `rangekeeper-0.6.5a0/rangekeeper/policy.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/projection.py` & `rangekeeper-0.6.5a0/rangekeeper/projection.py`

 * *Files 9% similar despite different names*

```diff
@@ -170,46 +170,8 @@
             frequency=rk.duration.Type.from_value(self.sequence.freq),
             bound=self.bounds[1].to_timestamp())
         datestamp_index = rk.duration.Sequence.to_datestamps(sequence=period_index)
         datestamp_index = datestamp_index.insert(loc=0, item=self.bounds[0].start_time)
 
         return pd.Series(
             data=data,
-            index=datestamp_index)
-
-# class DistributiveInterpolation(Interpolation):
-#     """
-#     A projection that apportions values over a range, according to a specified
-#     distribution type.
-#     """
-#     dist: distribution.Form
-#
-#     def __init__(
-#             self,
-#             dist: distribution.Form,
-#             sequence: Union[pd.RangeIndex, pd.PeriodIndex],
-#             bounds: Union[Tuple[int, int], Tuple[pd.Period, pd.Period]]):
-#         super().__init__(
-#             sequence=sequence,
-#             bounds=bounds)
-#         self.dist = dist
-
-# def map(
-#         self,
-#         left_padding: Padding = None,
-#         right_padding: Padding = None) -> pd.Series:
-
-
-# if isinstance(self.sequence, pd.RangeIndex):
-#     if isinstance(self, Extrapolation):
-#         factors = self.factor()
-#         left = self.pad(
-#             value=factors[0],
-#             length=self.sequence[0] - self.bounds[0],
-#             type=left_padding)
-#         right = self.pad(
-#             value=factors[-1],
-#             length=self.bounds[1] - self.sequence[-1],
-#             type=right_padding)
-#         return pd.Series(
-#             data=np.concatenate((left, factors, right)),
-#             index=range(self.bounds[0], self.bounds[1]))
+            index=datestamp_index)
```

### Comparing `rangekeeper-0.6.4a0/rangekeeper/segmentation.py` & `rangekeeper-0.6.5a0/rangekeeper/segmentation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/space.py` & `rangekeeper-0.6.5a0/rangekeeper/space.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/rangekeeper/span.py` & `rangekeeper-0.6.5a0/rangekeeper/span.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.4a0/PKG-INFO` & `rangekeeper-0.6.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rangekeeper
-Version: 0.6.4a0
+Version: 0.6.5a0
 Summary: A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like
 License: MPL-2.0
 Author: Daniel Fink
 Author-email: danfink@mit.edu
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 Requires-Dist: py-moneyed (>=3.0,<4.0)
 Requires-Dist: pyarrow (>=16.1.0,<17.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: pyxirr (>=0.10.3,<0.11.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: scipy (>=1.13.1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
-Requires-Dist: specklepy (>=2.19.0,<3.0.0)
+Requires-Dist: specklepy (>=2.19.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Rangekeeper Source
 This directory holds the source code for the Rangekeeper Library
 
 ## Installation
```

