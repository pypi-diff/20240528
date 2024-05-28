# Comparing `tmp/scatcluster-0.0.83.tar.gz` & `tmp/scatcluster-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.83.tar", last modified: Tue May 28 20:41:04 2024, max compression
+gzip compressed data, was "scatcluster-0.0.84.tar", last modified: Tue May 28 21:14:06 2024, max compression
```

## Comparing `scatcluster-0.0.83.tar` & `scatcluster-0.0.84.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:41:04.898793 scatcluster-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 20:41:01.000000 scatcluster-0.0.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 20:41:01.000000 scatcluster-0.0.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 20:41:04.898793 scatcluster-0.0.83/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:41:04.894793 scatcluster-0.0.83/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:41:04.898793 scatcluster-0.0.83/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:41:04.898793 scatcluster-0.0.83/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    27403 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-28 20:41:01.000000 scatcluster-0.0.83/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:41:04.898793 scatcluster-0.0.83/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 20:41:04.000000 scatcluster-0.0.83/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 20:41:04.000000 scatcluster-0.0.83/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:41:04.000000 scatcluster-0.0.83/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 20:41:04.000000 scatcluster-0.0.83/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 20:41:04.000000 scatcluster-0.0.83/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:41:04.898793 scatcluster-0.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 20:41:01.000000 scatcluster-0.0.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.328552 scatcluster-0.0.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 21:14:03.000000 scatcluster-0.0.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:14:03.000000 scatcluster-0.0.84/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:14:06.324551 scatcluster-0.0.84/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.320551 scatcluster-0.0.84/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:14:06.328552 scatcluster-0.0.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 21:14:03.000000 scatcluster-0.0.84/setup.py
```

### Comparing `scatcluster-0.0.83/LICENSE` & `scatcluster-0.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/PKG-INFO` & `scatcluster-0.0.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.83
+Version: 0.0.84
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.83/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.84/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.84/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.84/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/predictions.py` & `scatcluster-0.0.84/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/processing.py` & `scatcluster-0.0.84/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.84/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.84/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/helper.py` & `scatcluster-0.0.84/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/processing/ica.py` & `scatcluster-0.0.84/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/processing/scattering.py` & `scatcluster-0.0.84/scatcluster/processing/scattering.py`

 * *Files 4% similar despite different names*

```diff
@@ -454,14 +454,39 @@
         # Normalize
         dataset.order_1.data -= dataset.order_1.mean(dim=order_1_dim).data
         dataset.order_1.data /= dataset.order_1.std(dim=order_1_dim).data
         dataset.order_2.data -= dataset.order_2.mean(dim=order_2_dim).data
         dataset.order_2.data /= dataset.order_2.std(dim=order_2_dim).data
 
         return dataset
+    
+    def min_max_scaling(self, dataset):
+        """Min-Max scaling the scattering coefficients.
+
+        Parameters
+        ----------
+        dataset : xarray.Dataset
+            The scattering coefficients in the xarray.Dataset format.
+
+        Returns
+        -------
+        xarray.Dataset
+            The scattering coefficients in the xarray.Dataset format.
+        """
+        # Working dimensions for normalization
+        order_1_dim = ['time', 'f1', 'channel']
+        order_2_dim = ['time', 'f1', 'f2', 'channel']
+
+        # Normalize
+        dataset.order_1.data -= dataset.order_1.min(dim=order_1_dim).data
+        dataset.order_1.data /= (dataset.order_1.max(dim=order_1_dim).data - dataset.order_1.min(dim=order_1_dim).data)
+        dataset.order_2.data -= dataset.order_2.min(dim=order_2_dim).data
+        dataset.order_2.data /= (dataset.order_2.max(dim=order_2_dim).data - dataset.order_2.min(dim=order_2_dim).data)
+
+        return dataset
 
     def process_vectorized_scattering_coefficients(self) -> None:
         """
         Process the vectorized scattering coefficients by loading data from files, reshaping the coefficients,
         standardizing in log space, and vectorizing them. Display statistics from the vectorization and store the
         processed data.
 
@@ -544,14 +569,15 @@
         coefficients = coefficients.where(
             coefficients.order_1.sum(dim=('f1', 'channel')) > 0,
             drop=True,
         )
         coefficients = self.log(coefficients, waterlevel=1e-15)
         coefficients = self.nyquist_mask(coefficients)
         coefficients = self.normalize(coefficients)
+        coefficients = self.min_max_scaling(coefficients)
         print(coefficients)
 
         self.data_times = coefficients.time.values
         self.data_scat_coef_vectorized = self.vectorize_scattering_coefficients_xarray(coefficients)
 
         # Display statistics from the vectorization
         print(f'Number of valid time windows of size {self.network_segment}s: {int(self.data_times.shape[0])}')
```

### Comparing `scatcluster-0.0.83/scatcluster/scatcluster.py` & `scatcluster-0.0.84/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster/structure.py` & `scatcluster-0.0.84/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.84/scatcluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.83
+Version: 0.0.84
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.83/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.84/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.83/setup.py` & `scatcluster-0.0.84/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.83',
+    version='0.0.84',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

