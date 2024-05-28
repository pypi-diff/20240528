# Comparing `tmp/batchstats-0.3.3.tar.gz` & `tmp/batchstats-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchstats-0.3.3.tar", last modified: Tue May 21 22:04:00 2024, max compression
+gzip compressed data, was "batchstats-0.4.tar", last modified: Tue May 28 17:24:31 2024, max compression
```

## Comparing `batchstats-0.3.3.tar` & `batchstats-0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 22:03:49.000000 batchstats-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-21 22:03:59.999523 batchstats-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-21 22:03:49.000000 batchstats-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/batchstats/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/batchstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:03:59.999523 batchstats-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-21 22:03:49.000000 batchstats-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 22:03:49.000000 batchstats-0.3.3/tests/test_nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-21 22:03:49.000000 batchstats-0.3.3/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:31.289987 batchstats-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 17:24:21.000000 batchstats-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-28 17:24:31.289987 batchstats-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-28 17:24:21.000000 batchstats-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:31.285987 batchstats-0.4/batchstats/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 17:24:21.000000 batchstats-0.4/batchstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 17:24:21.000000 batchstats-0.4/batchstats/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-28 17:24:21.000000 batchstats-0.4/batchstats/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-28 17:24:21.000000 batchstats-0.4/batchstats/nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-05-28 17:24:21.000000 batchstats-0.4/batchstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:31.289987 batchstats-0.4/batchstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-28 17:24:31.000000 batchstats-0.4/batchstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 17:24:31.000000 batchstats-0.4/batchstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:24:31.000000 batchstats-0.4/batchstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 17:24:31.000000 batchstats-0.4/batchstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 17:24:31.000000 batchstats-0.4/batchstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:24:31.289987 batchstats-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 17:24:21.000000 batchstats-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:24:31.289987 batchstats-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-28 17:24:21.000000 batchstats-0.4/tests/test_nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-28 17:24:21.000000 batchstats-0.4/tests/test_stats.py
```

### Comparing `batchstats-0.3.3/LICENSE` & `batchstats-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.3/PKG-INFO` & `batchstats-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3.3
+Version: 0.4
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
-[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
+[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/) [![conda Version](
+https://anaconda.org/conda-forge/batchstats/badges/version.svg)](https://anaconda.org/conda-forge/batchstats)
 
 # <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
-```
+``` console
 pip install batchstats
 ```
+The package is also available on conda-forge:
+``` console
+conda install -c conda-forge batchstats
+```
+
+``` console
+mamba install batchstats
+```
 
 ## Usage
 
 Here's an example of how to use `batchstats` to compute batch mean and variance:
 
 ```python
 from batchstats import BatchMean, BatchVar
@@ -59,15 +68,15 @@
 for batch_index in np.array_split(np.arange(n_samples), n_batches):
     batchcov.update_batch(batch1=data1[batch_index], batch2=data2[batch_index])
 true_cov = (data1 - data1.mean(axis=0)).T@(data2 - data2.mean(axis=0))/n_samples
 np.allclose(true_cov, batchcov()), batchcov().shape
 >>> (True, (100, 50))
 ```
 
-`batchstats` is also flexible in terms of input shapes, with the first dimension always representing the samples and the remaining dimensions representing the features:
+`batchstats` is also flexible in terms of input shapes. By default, statistics are applied on the first axis: the first dimension representing the samples and the remaining dimensions representing the features:
 
 ```python
 import numpy as np
 from batchstats import BatchSum
 
 data = np.random.randn(10_000, 80, 90)
 n_batches = 7
@@ -77,21 +86,43 @@
     batchsum.update_batch(batch_data)
 
 true_sum = np.sum(data, axis=0)
 np.allclose(true_sum, batchsum()), batchsum().shape
 >>> (True, (80, 90))
 ```
 
+But as in the ``numpy`` associated functions, the user can specify the reduction axis or axes:
+
+```python
+import numpy as np
+from batchstats import BatchMean
+
+data = [np.random.randn(24, 7, 128) for _ in range(100)]
+
+batchmean = BatchMean(axis=(0, 2))
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (7,)
+
+batchmean = BatchMean(axis=2)
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (24, 7)
+```
+
 ## Available Classes/Stats
 
 - `BatchCov`: Compute the covariance matrix of two datasets (not necessarily square)
 - `BatchMax`: Compute the maximum value (associated to `np.max`)
 - `BatchMean`: Compute the mean (associated to `np.mean`)
 - `BatchMin`: Compute the minimum value (associated to `np.min`)
 - `BatchPeakToPeak`: Compute maximum - minimum value (associated to `np.ptp`)
+- `BatchStd`: Compute the standard deviation (associated to `np.std`)
 - `BatchSum`: Compute the sum (associated to `np.sum`)
 - `BatchVar`: Compute the variance (associated to `np.var`)
 
 Each class is tested against numpy results to ensure accuracy. For example:
 
 ```python
 import numpy as np
```

### Comparing `batchstats-0.3.3/README.md` & `batchstats-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
+[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/) [![conda Version](
+https://anaconda.org/conda-forge/batchstats/badges/version.svg)](https://anaconda.org/conda-forge/batchstats)
 
 # <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
-```
+``` console
 pip install batchstats
 ```
+The package is also available on conda-forge:
+``` console
+conda install -c conda-forge batchstats
+```
+
+``` console
+mamba install batchstats
+```
 
 ## Usage
 
 Here's an example of how to use `batchstats` to compute batch mean and variance:
 
 ```python
 from batchstats import BatchMean, BatchVar
@@ -49,15 +58,15 @@
 for batch_index in np.array_split(np.arange(n_samples), n_batches):
     batchcov.update_batch(batch1=data1[batch_index], batch2=data2[batch_index])
 true_cov = (data1 - data1.mean(axis=0)).T@(data2 - data2.mean(axis=0))/n_samples
 np.allclose(true_cov, batchcov()), batchcov().shape
 >>> (True, (100, 50))
 ```
 
-`batchstats` is also flexible in terms of input shapes, with the first dimension always representing the samples and the remaining dimensions representing the features:
+`batchstats` is also flexible in terms of input shapes. By default, statistics are applied on the first axis: the first dimension representing the samples and the remaining dimensions representing the features:
 
 ```python
 import numpy as np
 from batchstats import BatchSum
 
 data = np.random.randn(10_000, 80, 90)
 n_batches = 7
@@ -67,21 +76,43 @@
     batchsum.update_batch(batch_data)
 
 true_sum = np.sum(data, axis=0)
 np.allclose(true_sum, batchsum()), batchsum().shape
 >>> (True, (80, 90))
 ```
 
+But as in the ``numpy`` associated functions, the user can specify the reduction axis or axes:
+
+```python
+import numpy as np
+from batchstats import BatchMean
+
+data = [np.random.randn(24, 7, 128) for _ in range(100)]
+
+batchmean = BatchMean(axis=(0, 2))
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (7,)
+
+batchmean = BatchMean(axis=2)
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (24, 7)
+```
+
 ## Available Classes/Stats
 
 - `BatchCov`: Compute the covariance matrix of two datasets (not necessarily square)
 - `BatchMax`: Compute the maximum value (associated to `np.max`)
 - `BatchMean`: Compute the mean (associated to `np.mean`)
 - `BatchMin`: Compute the minimum value (associated to `np.min`)
 - `BatchPeakToPeak`: Compute maximum - minimum value (associated to `np.ptp`)
+- `BatchStd`: Compute the standard deviation (associated to `np.std`)
 - `BatchSum`: Compute the sum (associated to `np.sum`)
 - `BatchVar`: Compute the variance (associated to `np.var`)
 
 Each class is tested against numpy results to ensure accuracy. For example:
 
 ```python
 import numpy as np
```

### Comparing `batchstats-0.3.3/batchstats/_misc.py` & `batchstats-0.4/batchstats/_misc.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.3/batchstats/nanstats.py` & `batchstats-0.4/batchstats/nanstats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,24 @@
 import numpy as np
 
 from ._misc import NoValidSamplesError
-
-
-class BatchNanStat:
-    """
-    Base class for calculating statistics over batches of data that can contain NaN values.
-
-    Attributes:
-        n_samples (numpy.ndarray): Total number of samples processed, accounting for NaN values.
-
-    """
-
-    def __init__(self):
-        """
-        Initialize the BatchNanStat object.
-        """
-        self.n_samples = None
-
-    def _process_batch(self, batch):
-        """
-        Process the input batch, counting NaN values.
-
-        Args:
-            batch (numpy.ndarray): Input batch.
-
-        Returns:
-            numpy.ndarray: Processed batch.
-
-        """
-        batch = np.atleast_2d(np.asarray(batch))
-        axis = tuple(range(1, batch.ndim))
-        if self.n_samples is None:
-            self.n_samples = np.isfinite(batch).sum(axis=0)
-        else:
-            self.n_samples += np.isfinite(batch).sum(axis=0)
-        return batch
+from .core import BatchNanStat
 
 
 class BatchNanSum(BatchNanStat):
     """
     Class for calculating the sum of batches of data that can contain NaN values.
 
     """
 
-    def __init__(self):
+    def __init__(self, axis=0):
         """
         Initialize the BatchNanSum object.
         """
-        super().__init__()
+        super().__init__(axis=axis)
         self.sum = None
 
     def update_batch(self, batch):
         """
         Update the sum with a new batch of data that can contain NaN values.
 
         Args:
@@ -61,17 +27,17 @@
         Returns:
             BatchNanSum: Updated BatchNanSum object.
 
         """
         batch = self._process_batch(batch)
         axis = tuple(range(1, batch.ndim))
         if self.sum is None:
-            self.sum = np.nansum(batch, axis=0)
+            self.sum = np.nansum(batch, axis=self.axis)
         else:
-            self.sum += np.nansum(batch, axis=0)
+            self.sum += np.nansum(batch, axis=self.axis)
         return self
 
     def __call__(self):
         """
         Calculate the sum of the batches that can contain NaN values.
 
         Returns:
@@ -89,20 +55,20 @@
 
 class BatchNanMean(BatchNanStat):
     """
     Class for calculating the mean of batches of data that can contain NaN values.
 
     """
 
-    def __init__(self):
+    def __init__(self, axis=0):
         """
         Initialize the BatchNanMean object.
         """
-        super().__init__()
-        self.sum = BatchNanSum()
+        super().__init__(axis=axis)
+        self.sum = BatchNanSum(axis=axis)
 
     def update_batch(self, batch):
         """
         Update the mean with a new batch of data that can contain NaN values.
 
         Args:
             batch (numpy.ndarray): Input batch.
```

### Comparing `batchstats-0.3.3/batchstats/stats.py` & `batchstats-0.4/batchstats/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,23 @@
 import string
 
 import numpy as np
 
 from ._misc import NoValidSamplesError, UnequalSamplesNumber, any_nan, check_params
-
-
-class BatchStat:
-    """
-    Base class for calculating statistics over batches of data.
-
-    Attributes:
-        n_samples (int): Total number of samples processed.
-
-    """
-
-    def __init__(self):
-        self.n_samples = 0
-
-    def _process_batch(self, batch, assume_valid=False):
-        """
-        Process the input batch, handling NaN values if necessary.
-
-        Args:
-            batch (numpy.ndarray): Input batch.
-            assume_valid (bool, optional): If True, assumes all elements in the batch are valid. Default is False.
-
-        Returns:
-            numpy.ndarray: Processed batch.
-
-        """
-        batch = np.atleast_2d(np.asarray(batch))
-        if assume_valid:
-            self.n_samples += len(batch)
-            return batch
-        else:
-            axis = tuple(range(1, batch.ndim))
-            nan_mask = any_nan(batch, axis=axis)
-            if nan_mask.any():
-                valid_batch = batch[~nan_mask]
-            else:
-                valid_batch = batch
-            self.n_samples += len(valid_batch)
-            return valid_batch
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}()"
+from .core import BatchStat
 
 
 class BatchSum(BatchStat):
     """
     Class for calculating the sum of batches of data.
 
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, axis=0):
+        super().__init__(axis=axis)
         self.sum = None
 
     def update_batch(self, batch, assume_valid=False):
         """
         Update the sum with a new batch of data.
 
         Args:
@@ -69,17 +28,17 @@
             BatchSum: Updated BatchSum object.
 
         """
         valid_batch = self._process_batch(batch=batch, assume_valid=assume_valid)
         n = len(valid_batch)
         if n > 0:
             if self.sum is None:
-                self.sum = np.sum(a=valid_batch, axis=0)
+                self.sum = np.sum(a=valid_batch, axis=self.axis)
             else:
-                self.sum += np.sum(a=valid_batch, axis=0)
+                self.sum += np.sum(a=valid_batch, axis=self.axis)
         return self
 
     def __call__(self) -> np.ndarray:
         """
         Calculate the sum.
 
         Returns:
@@ -97,16 +56,16 @@
 
 class BatchMax(BatchStat):
     """
     Class for calculating the maximum of batches of data.
 
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, axis=0):
+        super().__init__(axis=axis)
         self.max = None
 
     def update_batch(self, batch, assume_valid=False):
         """
         Update the maximum with a new batch of data.
 
         Args:
@@ -117,17 +76,17 @@
             BatchMax: Updated BatchMax object.
 
         """
         valid_batch = self._process_batch(batch=batch, assume_valid=assume_valid)
         n = len(valid_batch)
         if n > 0:
             if self.max is None:
-                self.max = np.max(valid_batch, axis=0)
+                self.max = np.max(valid_batch, axis=self.axis)
             else:
-                np.maximum(self.max, np.max(valid_batch, axis=0), out=self.max)
+                np.maximum(self.max, np.max(valid_batch, axis=self.axis), out=self.max)
         return self
 
     def __call__(self) -> np.ndarray:
         """
         Calculate the maximum.
 
         Returns:
@@ -145,16 +104,16 @@
 
 class BatchMin(BatchStat):
     """
     Class for calculating the minimum of batches of data.
 
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, axis=0):
+        super().__init__(axis=axis)
         self.min = None
 
     def update_batch(self, batch, assume_valid=False):
         """
         Update the minimum with a new batch of data.
 
         Args:
@@ -165,17 +124,17 @@
             BatchMin: Updated BatchMin object.
 
         """
         valid_batch = self._process_batch(batch=batch, assume_valid=assume_valid)
         n = len(valid_batch)
         if n > 0:
             if self.min is None:
-                self.min = np.min(valid_batch, axis=0)
+                self.min = np.min(valid_batch, axis=self.axis)
             else:
-                np.minimum(self.min, np.min(valid_batch, axis=0), out=self.min)
+                np.minimum(self.min, np.min(valid_batch, axis=self.axis), out=self.min)
         return self
 
     def __call__(self) -> np.ndarray:
         """
         Calculate the minimum.
 
         Returns:
@@ -193,16 +152,16 @@
 
 class BatchMean(BatchStat):
     """
     Class for calculating the mean of batches of data.
 
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, axis=0):
+        super().__init__(axis=axis)
         self.mean = None
 
     def update_batch(self, batch, assume_valid=False):
         """
         Update the mean with a new batch of data.
 
         Args:
@@ -213,17 +172,17 @@
             BatchMean: Updated BatchMean object.
 
         """
         valid_batch = self._process_batch(batch=batch, assume_valid=assume_valid)
         n = len(valid_batch)
         if n > 0:
             if self.mean is None:
-                self.mean = np.mean(valid_batch, axis=0)
+                self.mean = np.mean(valid_batch, axis=self.axis)
             else:
-                self.mean = ((self.n_samples - n) * self.mean + np.sum(valid_batch, axis=0)) / self.n_samples
+                self.mean = ((self.n_samples - n) * self.mean + np.sum(valid_batch, axis=self.axis)) / self.n_samples
         return self
 
     def __call__(self) -> np.ndarray:
         """
         Calculate the mean.
 
         Returns:
@@ -240,18 +199,18 @@
 
 
 class BatchPeakToPeak(BatchStat):
     """
     Class for calculating the peak-to-peak (max - min) of batches of data.
     """
 
-    def __init__(self):
-        super().__init__()
-        self.batchmax = BatchMax()
-        self.batchmin = BatchMin()
+    def __init__(self, axis=0):
+        super().__init__(axis=axis)
+        self.batchmax = BatchMax(axis=axis)
+        self.batchmin = BatchMin(axis=axis)
 
     def update_batch(self, batch, assume_valid=False):
         """
         Update the peak-to-peak with a new batch of data.
 
         Args:
             batch (numpy.ndarray): Input batch.
@@ -283,17 +242,17 @@
     """
     Class for calculating the variance of batches of data.
 
     Args:
         ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
 
-    def __init__(self, ddof=0):
-        super().__init__()
-        self.mean = BatchMean()
+    def __init__(self, axis=0, ddof=0):
+        super().__init__(axis=axis)
+        self.mean = BatchMean(axis=axis)
         self.var = None
         self.ddof = check_params(param=ddof, types=int)
 
     @classmethod
     def init_var(cls, v, vm):
         """
         Initialize variance.
@@ -382,17 +341,17 @@
 class BatchStd(BatchStat):
     """Class for calculating the standard deviation of batches of data.
 
     Args:
         ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
 
-    def __init__(self, ddof=0):
-        super().__init__()
-        self.var = BatchVar(ddof=ddof)
+    def __init__(self, axis=0, ddof=0):
+        super().__init__(axis=axis)
+        self.var = BatchVar(axis=axis, ddof=ddof)
 
     def update_batch(self, batch, assume_valid=False):
         """Update the standard deviation with a new batch of data.
 
         Args:
             batch (numpy.ndarray): Input batch.
             assume_valid (bool, optional): If True, assumes all elements in the batch are valid. Default is False.
@@ -508,8 +467,7 @@
         Raises:
             NoValidSamplesError: If no valid samples are available.
 
         """
         if self.cov is None:
             raise NoValidSamplesError("No valid samples for calculating covariance.")
         return self.n_samples/(self.n_samples - self.ddof)*self.cov
-        return self.n_samples/(self.n_samples - self.ddof)*self.cov
```

### Comparing `batchstats-0.3.3/batchstats.egg-info/PKG-INFO` & `batchstats-0.4/batchstats.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3.3
+Version: 0.4
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
-[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
+[![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/) [![conda Version](
+https://anaconda.org/conda-forge/batchstats/badges/version.svg)](https://anaconda.org/conda-forge/batchstats)
 
 # <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
-```
+``` console
 pip install batchstats
 ```
+The package is also available on conda-forge:
+``` console
+conda install -c conda-forge batchstats
+```
+
+``` console
+mamba install batchstats
+```
 
 ## Usage
 
 Here's an example of how to use `batchstats` to compute batch mean and variance:
 
 ```python
 from batchstats import BatchMean, BatchVar
@@ -59,15 +68,15 @@
 for batch_index in np.array_split(np.arange(n_samples), n_batches):
     batchcov.update_batch(batch1=data1[batch_index], batch2=data2[batch_index])
 true_cov = (data1 - data1.mean(axis=0)).T@(data2 - data2.mean(axis=0))/n_samples
 np.allclose(true_cov, batchcov()), batchcov().shape
 >>> (True, (100, 50))
 ```
 
-`batchstats` is also flexible in terms of input shapes, with the first dimension always representing the samples and the remaining dimensions representing the features:
+`batchstats` is also flexible in terms of input shapes. By default, statistics are applied on the first axis: the first dimension representing the samples and the remaining dimensions representing the features:
 
 ```python
 import numpy as np
 from batchstats import BatchSum
 
 data = np.random.randn(10_000, 80, 90)
 n_batches = 7
@@ -77,21 +86,43 @@
     batchsum.update_batch(batch_data)
 
 true_sum = np.sum(data, axis=0)
 np.allclose(true_sum, batchsum()), batchsum().shape
 >>> (True, (80, 90))
 ```
 
+But as in the ``numpy`` associated functions, the user can specify the reduction axis or axes:
+
+```python
+import numpy as np
+from batchstats import BatchMean
+
+data = [np.random.randn(24, 7, 128) for _ in range(100)]
+
+batchmean = BatchMean(axis=(0, 2))
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (7,)
+
+batchmean = BatchMean(axis=2)
+for batch in data:
+    batchmean.update_batch(batch)
+batchmean().shape
+>>> (24, 7)
+```
+
 ## Available Classes/Stats
 
 - `BatchCov`: Compute the covariance matrix of two datasets (not necessarily square)
 - `BatchMax`: Compute the maximum value (associated to `np.max`)
 - `BatchMean`: Compute the mean (associated to `np.mean`)
 - `BatchMin`: Compute the minimum value (associated to `np.min`)
 - `BatchPeakToPeak`: Compute maximum - minimum value (associated to `np.ptp`)
+- `BatchStd`: Compute the standard deviation (associated to `np.std`)
 - `BatchSum`: Compute the sum (associated to `np.sum`)
 - `BatchVar`: Compute the variance (associated to `np.var`)
 
 Each class is tested against numpy results to ensure accuracy. For example:
 
 ```python
 import numpy as np
```

### Comparing `batchstats-0.3.3/setup.py` & `batchstats-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.3/tests/test_nanstats.py` & `batchstats-0.4/tests/test_nanstats.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.3/tests/test_stats.py` & `batchstats-0.4/tests/test_stats.py`

 * *Files identical despite different names*

