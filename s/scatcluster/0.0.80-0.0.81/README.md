# Comparing `tmp/scatcluster-0.0.80.tar.gz` & `tmp/scatcluster-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.80.tar", last modified: Mon May 27 22:46:42 2024, max compression
+gzip compressed data, was "scatcluster-0.0.81.tar", last modified: Tue May 28 20:10:41 2024, max compression
```

## Comparing `scatcluster-0.0.80.tar` & `scatcluster-0.0.81.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 22:46:38.000000 scatcluster-0.0.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 22:46:38.000000 scatcluster-0.0.80/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:46:42.212965 scatcluster-0.0.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.208965 scatcluster-0.0.80/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.208965 scatcluster-0.0.80/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:46:42.212965 scatcluster-0.0.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 22:46:39.000000 scatcluster-0.0.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:10:41.064254 scatcluster-0.0.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 20:10:32.000000 scatcluster-0.0.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 20:10:32.000000 scatcluster-0.0.81/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 20:10:41.064254 scatcluster-0.0.81/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:10:41.060254 scatcluster-0.0.81/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:10:41.060254 scatcluster-0.0.81/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:10:41.064254 scatcluster-0.0.81/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27432 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-28 20:10:32.000000 scatcluster-0.0.81/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:10:41.064254 scatcluster-0.0.81/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 20:10:41.000000 scatcluster-0.0.81/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 20:10:41.000000 scatcluster-0.0.81/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:10:41.000000 scatcluster-0.0.81/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 20:10:41.000000 scatcluster-0.0.81/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 20:10:41.000000 scatcluster-0.0.81/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:10:41.064254 scatcluster-0.0.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 20:10:32.000000 scatcluster-0.0.81/setup.py
```

### Comparing `scatcluster-0.0.80/LICENSE` & `scatcluster-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/PKG-INFO` & `scatcluster-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.80
+Version: 0.0.81
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.80/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.81/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.81/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.81/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/predictions.py` & `scatcluster-0.0.81/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/processing.py` & `scatcluster-0.0.81/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.81/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.81/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/helper.py` & `scatcluster-0.0.81/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/processing/ica.py` & `scatcluster-0.0.81/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/processing/scattering.py` & `scatcluster-0.0.81/scatcluster/processing/scattering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import pickle
 
 import cupy as cp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from scipy import stats as sp_stats
 import xarray as xr
 from matplotlib import dates as mdates
 from obspy.clients.filesystem.sds import Client
 from obspy.core import UTCDateTime
 from obspy.core.stream import Stream
 from scatseisnet.network import ScatteringNetwork
 from scatseisnet.operation import segmentize
+from scipy import stats as sp_stats
 from tqdm import tqdm
 
 
 class Scattering:
 
     def reduce_type(self):
         """
@@ -49,32 +49,32 @@
 
         """
         try:
             file_path = f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_' \
                         f'{self.network_name}_times.npy'
             self.data_times = np.load(file_path)
         except FileNotFoundError:
-            print(f"File not found: {file_path}")
+            print(f'File not found: {file_path}')
         except Exception as e:
-            print(f"An error occurred while loading data times: {e}")        
+            print(f'An error occurred while loading data times: {e}')
 
     def build_day_list(self) -> None:
         """Build data_day_list object
         """
         try:
             start_time = UTCDateTime(self.data_starttime)
             end_time = UTCDateTime(self.data_endtime)
             exclude_days = [UTCDateTime(day).strftime('%Y-%m-%d') for day in self.data_exclude_days]
             day_list = [
-                day_start for day_start in pd.date_range(start_time.strftime('%Y%m%d'), end_time.strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist()
-                if day_start not in exclude_days
+                day_start for day_start in pd.date_range(start_time.strftime('%Y%m%d'), end_time.strftime(
+                    '%Y%m%d')).strftime('%Y-%m-%d').tolist() if day_start not in exclude_days
             ]
             self.data_day_list = day_list
         except Exception as e:
-            print(f"An error occurred while building day list: {e}")
+            print(f'An error occurred while building day list: {e}')
 
     def build_channel_list(self) -> None:
         if self.sample_stream is None:
             self.process_sample_data()
         self.channel_list = [trace.stats.channel for trace in self.sample_stream]
 
     def stream_process(self, stream: Stream) -> Stream:
@@ -546,25 +546,16 @@
             drop=True,
         )
         coefficients = self.log(coefficients, waterlevel=1e-10)
         coefficients = self.nyquist_mask(coefficients)
         coefficients = self.normalize(coefficients)
         print(coefficients)
 
-        # Extract design matrix
-        n_samples = coefficients.time.shape[0]
-        x1 = coefficients.order_1.data.reshape(n_samples, -1)
-        x2 = coefficients.order_2.data.reshape(n_samples, -1)
-        x = np.hstack((x1, x2))
-
-        # Remove NaNs
-        x[np.isnan(x)] = 0
-
         self.data_times = coefficients.time.values
-        self.data_scat_coef_vectorized = x
+        self.data_scat_coef_vectorized = self.vectorize_scattering_coefficients_xarray(coefficients)
 
         # Display statistics from the vectorization
         print(f'Number of valid time windows of size {self.network_segment}s: {int(self.data_times.shape[0])}')
         print(f'Number of days investigated: {int((self.network_segment * self.data_times.shape[0])/86400)}')
         print(f'Number of Scat Coefficients: {int(self.data_scat_coef_vectorized.shape[1])}')
         print(f'Vectorized Scat Coefficients: {self.data_scat_coef_vectorized.shape}')
 
@@ -575,14 +566,25 @@
         np.save(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_scat_coef_vectorized.npy', self.data_scat_coef_vectorized)
         coefficients.to_netcdf(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
                                f'{self.network_name}_scat_coef_xarray.nc')
 
         return coefficients
+    
+    def vectorize_scattering_coefficients_xarray(self, coefficients):
+        n_samples = coefficients.time.shape[0]
+        x1 = coefficients.order_1.data.reshape(n_samples, -1)
+        x2 = coefficients.order_2.data.reshape(n_samples, -1)
+        x = np.hstack((x1, x2))
+
+        x[np.isnan(x)] = 0        
+        
+        return x
+        
 
     def load_scattering_coefficients_xarray(self):
         """
         Load the scattering coefficients from an xarray dataset file and store them in the
         `scattering_coefficients_xarray` attribute.
 
         Returns:
```

### Comparing `scatcluster-0.0.80/scatcluster/scatcluster.py` & `scatcluster-0.0.81/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster/structure.py` & `scatcluster-0.0.81/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.81/scatcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.80
+Version: 0.0.81
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.80/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.81/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.80/setup.py` & `scatcluster-0.0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.80',
+    version='0.0.81',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

