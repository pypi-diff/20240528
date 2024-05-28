# Comparing `tmp/pycalib_rt-0.1.0.tar.gz` & `tmp/pycalib_rt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycalib_rt-0.1.0.tar", last modified: Thu Oct 26 14:10:13 2023, max compression
+gzip compressed data, was "pycalib_rt-0.1.1.tar", last modified: Tue May 28 15:56:49 2024, max compression
```

## Comparing `pycalib_rt-0.1.0.tar` & `pycalib_rt-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-10-26 14:10:13.010320 pycalib_rt-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2639 2023-10-26 14:10:13.009318 pycalib_rt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2158 2023-10-26 14:04:59.000000 pycalib_rt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-26 14:10:12.962550 pycalib_rt-0.1.0/calib_rt/
--rw-rw-rw-   0        0        0      229 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/__init__.py
--rw-rw-rw-   0        0        0     3974 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/calib_rt.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:10:12.981413 pycalib_rt-0.1.0/calib_rt/data/
--rw-rw-rw-   0        0        0   737338 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz
--rw-rw-rw-   0        0        0   472346 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz
--rw-rw-rw-   0        0        0    72650 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz
--rw-rw-rw-   0        0        0  1958218 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz
--rw-rw-rw-   0        0        0    59146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz
--rw-rw-rw-   0        0        0   142762 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz
--rw-rw-rw-   0        0        0    50234 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz
--rw-rw-rw-   0        0        0    29994 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz
--rw-rw-rw-   0        0        0   855754 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz
--rw-rw-rw-   0        0        0   761146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz
--rw-rw-rw-   0        0        0     4725 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/datasets.py
--rw-rw-rw-   0        0        0     2006 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/regression.py
--rw-rw-rw-   0        0        0     3869 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/screen.py
--rw-rw-rw-   0        0        0     1848 2023-10-25 16:04:22.000000 pycalib_rt-0.1.0/calib_rt/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:10:13.008324 pycalib_rt-0.1.0/pycalib_rt.egg-info/
--rw-rw-rw-   0        0        0     2639 2023-10-26 14:10:12.000000 pycalib_rt-0.1.0/pycalib_rt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      960 2023-10-26 14:10:12.000000 pycalib_rt-0.1.0/pycalib_rt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-26 14:10:12.000000 pycalib_rt-0.1.0/pycalib_rt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-10-26 14:10:12.000000 pycalib_rt-0.1.0/pycalib_rt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-26 14:10:12.000000 pycalib_rt-0.1.0/pycalib_rt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-26 14:10:13.011311 pycalib_rt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      982 2023-10-26 14:09:03.000000 pycalib_rt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.429202 pycalib_rt-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3074 2024-05-28 15:56:49.426202 pycalib_rt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2437 2024-05-28 15:54:17.000000 pycalib_rt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.357295 pycalib_rt-0.1.1/calib_rt/
+-rw-rw-rw-   0        0        0      286 2024-05-28 08:32:19.000000 pycalib_rt-0.1.1/calib_rt/__init__.py
+-rw-rw-rw-   0        0        0     3170 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/calib_rt.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.399311 pycalib_rt-0.1.1/calib_rt/data/
+-rw-rw-rw-   0        0        0   737338 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz
+-rw-rw-rw-   0        0        0   472346 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz
+-rw-rw-rw-   0        0        0    72650 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz
+-rw-rw-rw-   0        0        0  1958218 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz
+-rw-rw-rw-   0        0        0    59146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz
+-rw-rw-rw-   0        0        0   142762 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz
+-rw-rw-rw-   0        0        0    50234 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz
+-rw-rw-rw-   0        0        0    29994 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz
+-rw-rw-rw-   0        0        0   855754 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz
+-rw-rw-rw-   0        0        0   761146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz
+-rw-rw-rw-   0        0        0     4662 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/datasets.py
+-rw-rw-rw-   0        0        0     2554 2024-05-28 07:40:19.000000 pycalib_rt-0.1.1/calib_rt/regression.py
+-rw-rw-rw-   0        0        0     3200 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/screen.py
+-rw-rw-rw-   0        0        0     1113 2024-05-28 07:40:14.000000 pycalib_rt-0.1.1/calib_rt/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.423694 pycalib_rt-0.1.1/pycalib_rt.egg-info/
+-rw-rw-rw-   0        0        0     3074 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 15:56:49.430202 pycalib_rt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2024-05-28 15:54:25.000000 pycalib_rt-0.1.1/setup.py
```

### Comparing `pycalib_rt-0.1.0/LICENSE` & `pycalib_rt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/PKG-INFO` & `pycalib_rt-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,90 @@
 Metadata-Version: 2.1
 Name: pycalib_rt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calib-RT is designed for RT (retention time) calibration.
 Home-page: https://github.com/chenghui03/Calib_RT/tree/main/
 Author: yichi zhang
 Author-email: kszyc1001@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-# Version
-
-This document is for version 0.1.0 of calib_rt.
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=2.1.1
+Requires-Dist: networkx>=3.1
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: scipy>=1.11.3
 
 # Calib-RT
+<p align="left">
+    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=Calib-RT&color=green">
+    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
+</p>
+
+## Overview
 Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
 This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
 
 The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
 
 <div align=center>
 <img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
 </div>
 
-# Installation
-To use calib_rt, make sure you have the following dependencies installed:
+## Installation
+To use `calib_rt`, make sure you have the following dependencies installed:
 - Python (>= 3.10)
 - numpy (>= 1.26.0)
 - pandas (>= 2.1.1)
 - networkx (>= 3.1)
 - statsmodels (>= 0.14.0)
 - scipy (>= 1.11.3)
 
-You can install the calib_rt package using pip:
+You can install the `calib_rt` package using pip:
 ```bash
 pip install pycalib_rt 
 ```
 
-# Usage
-Here is an example of how to use Calib-RT for retention time calibration:
+## Usage
+Here is an example of how to use `calib_rt` for RT calibration:
 
 ```python
 import calib_rt
+
 # basic information of all built-in datasets 
 calib_rt.RTdatasets.get_datasets_list()  
          sample_type  datasets_num
    0   distort_left             2
    1  distort_right             2
    2            exp             2
    3         linear             2
    4              S             2
+
 # use first of "S" type datasets
 datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
 x = datasets["Spectral library RT"]
 y = datasets["Measured RT"]
+
 # fit and predict
 model = calib_rt.Calib_RT() 
 model.fit(x,y)
 y_pred = model.predict(x)         
 ```
 
-# Performance test
+## Performance test
 
 <div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance.jpg" alt="Your Image" width="500">
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
 </div>
 
-For a detailed analysis of the test conclusion and all performance test results, please refer to the full paper.
+Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
+For a detailed analysis of the test conclusion, please refer to our paper.
+
+## References
 
-# References
 [link of paper]()
 
-# License
+## License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `pycalib_rt-0.1.0/README.md` & `pycalib_rt-0.1.1/pycalib_rt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,90 @@
-# Version
-
-This document is for version 0.1.0 of calib_rt.
+Metadata-Version: 2.1
+Name: pycalib_rt
+Version: 0.1.1
+Summary: Calib-RT is designed for RT (retention time) calibration.
+Home-page: https://github.com/chenghui03/Calib_RT/tree/main/
+Author: yichi zhang
+Author-email: kszyc1001@163.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=2.1.1
+Requires-Dist: networkx>=3.1
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: scipy>=1.11.3
 
 # Calib-RT
+<p align="left">
+    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=Calib-RT&color=green">
+    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
+</p>
+
+## Overview
 Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
 This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
 
 The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
 
 <div align=center>
 <img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
 </div>
 
-# Installation
-To use calib_rt, make sure you have the following dependencies installed:
+## Installation
+To use `calib_rt`, make sure you have the following dependencies installed:
 - Python (>= 3.10)
 - numpy (>= 1.26.0)
 - pandas (>= 2.1.1)
 - networkx (>= 3.1)
 - statsmodels (>= 0.14.0)
 - scipy (>= 1.11.3)
 
-You can install the calib_rt package using pip:
+You can install the `calib_rt` package using pip:
 ```bash
 pip install pycalib_rt 
 ```
 
-# Usage
-Here is an example of how to use Calib-RT for retention time calibration:
+## Usage
+Here is an example of how to use `calib_rt` for RT calibration:
 
 ```python
 import calib_rt
+
 # basic information of all built-in datasets 
 calib_rt.RTdatasets.get_datasets_list()  
          sample_type  datasets_num
    0   distort_left             2
    1  distort_right             2
    2            exp             2
    3         linear             2
    4              S             2
+
 # use first of "S" type datasets
 datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
 x = datasets["Spectral library RT"]
 y = datasets["Measured RT"]
+
 # fit and predict
 model = calib_rt.Calib_RT() 
 model.fit(x,y)
 y_pred = model.predict(x)         
 ```
 
-# Performance test
+## Performance test
 
 <div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance.jpg" alt="Your Image" width="500">
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
 </div>
 
-For a detailed analysis of the test conclusion and all performance test results, please refer to the full paper.
+Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
+For a detailed analysis of the test conclusion, please refer to our paper.
+
+## References
 
-# References
 [link of paper]()
 
-# License
+## License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `pycalib_rt-0.1.0/calib_rt/calib_rt.py` & `pycalib_rt-0.1.1/calib_rt/calib_rt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 # -*- coding:utf-8 -*-
 
-'''
-main function of calib_rt
-
-.. calib_rt:
-    url
-
-'''
-
 import numpy as np
 
 from .screen import screen_by_hist, screen_by_graph, polish_ends
 from .regression import fit_by_lowess, Predictor
 from .utils import Normalization
 
 class Calib_RT(object):
     """
-    Calib_RT is used for TODO ...
+    Calib_RT is used for RT calibration.
 
     Attributes:
         fit(): fit by Calib_RT model
         predict(): predict by Calib_RT model
         setdata(): Set data for Calib_RT model
-        result(): TODO
     """
     
-    def __init__(self,bins:int=100,tol_bins:float=5) -> None:
+    def __init__(self,bins:int=100,tol_bins:float=10) -> None:
         """
         Set params for Calib_RT model
 
         Args:
             bins(int): 
             tol_bins(float):
         
         Examples:
             >>> import calib_rt 
             >>> model = calib_rt.Calib_RT(bin=100,tol_bin=5)
-        
-        References:
-            url
         """
-        # TODO 输入检查
-
         self.bins = bins
         self.tol_bins = tol_bins
 
     def setdata(self,x,y) -> None:
         """
         Set data for Calib_RT model
 
@@ -53,20 +39,15 @@
             x(array_like): 1-D array_like for Spectral library RT
             y(array_like): 1-D array_like for Measured RT
         
         Examples:
             >>> import calib_rt 
             >>> model = calib_rt.Calib_RT(bin=100,tol_bin=5)
             >>> model.setdata(x,y)
-        
-        References:
-            url
         """
-        # TODO 输入检查
-
         self.x = x
         self.y = y
         self.nomral = Normalization(x,y)
         self.x_normal,self.y_normal = self.nomral.get_normalized_data()
 
     def fit(self,x,y,manual_frac:float=-1) -> None:
         """
@@ -75,47 +56,30 @@
         Args:
             x(array_like): 1-D array_like for Spectral library RT
             y(array_like): 1-D array_like for Measured RT
             manual_frac(float): 
         
         Examples:
             >>> import calib_rt 
-            >>> model = calib_rt.Calib_RT(bin=100,tol_bin=5)
+            >>> model = calib_rt.Calib_RT(bin=100,tol_bin=20)
             >>> model.fit(x,y)
-        
-        References:
-            url
         """
-        # TODO 输入检查，同时将x,y转化为np.ndarray
-
         self.setdata(x,y)
         self.__fit(manual_frac)
 
-
     def __fit(self,manual_frac):
 
-        x_hist,y_hist,rho_hist = screen_by_hist(self.x_normal,self.y_normal,
+        x_hist,y_hist,rho_hist = screen_by_hist(self.x_normal,
+                                                self.y_normal,
                                                 self.bins)
-        x_graph,y_graph = screen_by_graph(x_hist,y_hist,
-                                          rho_hist)
-        x_polish,y_polish = polish_ends(x_graph,y_graph,
-                                        self.tol_bins)
+        x_graph,y_graph = screen_by_graph(x_hist,y_hist, rho_hist)
+        x_polish,y_polish = polish_ends(x_graph,y_graph,self.tol_bins)
         self.x_fit,self.y_fit = fit_by_lowess(x_polish,y_polish,manual_frac)
         self.Predor = Predictor(self.x_fit,self.y_fit)
 
-
-    def result(self) -> str:
-        """
-        """
-        # TODO ：用何指标衡量拟合的好坏，现有合适的 Spectral library RT 范围
-        self.result_dict = dict()
-        xmin,xmax = np.min(self.x_fit),np.max(self.x_fit)
-        self.result_dict["good Spectral library RT range"] = np.array((xmin,xmax))
-
-
     def predict(self,x) -> np.ndarray:
         """
         predict Measured RT by Spectral library RT on the basis of Calib_RT model
 
         Args:
             x(array_like): 1-D array_like for Spectral library RT for predict
         
@@ -123,19 +87,15 @@
             1-D np.ndarray Measured RT predict
         
         Examples:
             >>> import calib_rt 
             >>> model = calib_rt.Calib_RT(bin=100,tol_bin=5)
             >>> model.fit(x,y)
             >>> model.predict(x)
-        
-        References:
-            url
         """
-        # TODO 输入检查
         return self.__predict(x)
         
 
     def __predict(self,x):
         x_pred_normal = self.nomral.normal("x",x)
         y_pred_normal = self.Predor.predict(x_pred_normal)
         y_pred = self.nomral.denormal("y",y_pred_normal)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pycalib_rt-0.1.0/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz` & `pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/calib_rt/datasets.py` & `pycalib_rt-0.1.1/calib_rt/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 # -*- coding:utf-8 -*-
 
-'''
-data sets for calib_rt
-
-.. calib_rt:
-    url
-
-'''
-
 import pandas as pd
 import numpy as np
 import os
 
 
 class RTdatasets(object):
     """
```

### Comparing `pycalib_rt-0.1.0/pycalib_rt.egg-info/SOURCES.txt` & `pycalib_rt-0.1.1/pycalib_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.0/setup.py` & `pycalib_rt-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="pycalib_rt",
-    version="0.1.0",
+    version="0.1.1",
     author="yichi zhang",
     author_email="kszyc1001@163.com",
     description="Calib-RT is designed for RT (retention time) calibration.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/chenghui03/Calib_RT/tree/main/",  
+    url="https://github.com/chenghui03/Calib_RT/tree/main/", 
     packages=setuptools.find_packages(),
     package_data={'calib_rt': ['data/*.npz',]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",  
         "Operating System :: OS Independent",
     ],
     install_requires=['numpy>=1.26.0',
                       'pandas>=2.1.1',
                       'networkx>=3.1',
                       'statsmodels>=0.14.0',
                       'scipy>=1.11.3'],
     python_requires='>=3.10'
-)
+)
+
+#   python setup.py sdist build
+#   twine upload dist/*  
+
+#   git tag [new version] -m "detail"
+#   git push origin [new version]
```

