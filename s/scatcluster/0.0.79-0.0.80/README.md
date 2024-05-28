# Comparing `tmp/scatcluster-0.0.79.tar.gz` & `tmp/scatcluster-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.79.tar", last modified: Mon May 27 22:34:30 2024, max compression
+gzip compressed data, was "scatcluster-0.0.80.tar", last modified: Mon May 27 22:46:42 2024, max compression
```

## Comparing `scatcluster-0.0.79.tar` & `scatcluster-0.0.80.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:34:30.696756 scatcluster-0.0.79/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 22:34:24.000000 scatcluster-0.0.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 22:34:24.000000 scatcluster-0.0.79/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:34:30.696756 scatcluster-0.0.79/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:34:30.692756 scatcluster-0.0.79/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:34:30.692756 scatcluster-0.0.79/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:34:30.696756 scatcluster-0.0.79/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 22:34:24.000000 scatcluster-0.0.79/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:34:30.696756 scatcluster-0.0.79/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:34:30.000000 scatcluster-0.0.79/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 22:34:30.000000 scatcluster-0.0.79/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:34:30.000000 scatcluster-0.0.79/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 22:34:30.000000 scatcluster-0.0.79/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:34:30.000000 scatcluster-0.0.79/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:34:30.696756 scatcluster-0.0.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 22:34:24.000000 scatcluster-0.0.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 22:46:38.000000 scatcluster-0.0.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 22:46:38.000000 scatcluster-0.0.80/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:46:42.212965 scatcluster-0.0.80/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.208965 scatcluster-0.0.80/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.208965 scatcluster-0.0.80/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 22:46:38.000000 scatcluster-0.0.80/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:46:42.212965 scatcluster-0.0.80/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:46:42.000000 scatcluster-0.0.80/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:46:42.212965 scatcluster-0.0.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 22:46:39.000000 scatcluster-0.0.80/setup.py
```

### Comparing `scatcluster-0.0.79/LICENSE` & `scatcluster-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/PKG-INFO` & `scatcluster-0.0.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.79
+Version: 0.0.80
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.79/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.80/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.80/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.80/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/predictions.py` & `scatcluster-0.0.80/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/processing.py` & `scatcluster-0.0.80/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.80/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.80/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/helper.py` & `scatcluster-0.0.80/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/processing/ica.py` & `scatcluster-0.0.80/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/processing/scattering.py` & `scatcluster-0.0.80/scatcluster/processing/scattering.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,15 +541,15 @@
         )
 
         # Drop empty channels (where transform_waveform returned None)
         coefficients = coefficients.where(
             coefficients.order_1.sum(dim=('f1', 'channel')) > 0,
             drop=True,
         )
-        coefficients = self.log(coefficients, waterlevel=1e-15)
+        coefficients = self.log(coefficients, waterlevel=1e-10)
         coefficients = self.nyquist_mask(coefficients)
         coefficients = self.normalize(coefficients)
         print(coefficients)
 
         # Extract design matrix
         n_samples = coefficients.time.shape[0]
         x1 = coefficients.order_1.data.reshape(n_samples, -1)
```

### Comparing `scatcluster-0.0.79/scatcluster/scatcluster.py` & `scatcluster-0.0.80/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster/structure.py` & `scatcluster-0.0.80/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.80/scatcluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.79
+Version: 0.0.80
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.79/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.80/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.79/setup.py` & `scatcluster-0.0.80/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.79',
+    version='0.0.80',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

