# Comparing `tmp/scCASE-0.2.3.tar.gz` & `tmp/scCASE-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCASE-0.2.3.tar", last modified: Sun Dec 31 07:17:05 2023, max compression
+gzip compressed data, was "scCASE-0.2.5.tar", last modified: Tue May 28 11:11:36 2024, max compression
```

## Comparing `scCASE-0.2.3.tar` & `scCASE-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-12-31 07:17:05.565245 scCASE-0.2.3/
--rw-rw-rw-   0        0        0     1065 2023-12-29 07:04:56.000000 scCASE-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      593 2023-12-31 07:17:05.565245 scCASE-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5341 2023-12-31 07:11:36.000000 scCASE-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-12-31 07:17:05.553695 scCASE-0.2.3/scCASE/
-drwxrwxrwx   0        0        0        0 2023-12-31 07:17:05.564251 scCASE-0.2.3/scCASE/Aster/
--rw-rw-rw-   0        0        0      119 2023-12-29 07:31:32.000000 scCASE-0.2.3/scCASE/Aster/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-12-29 07:41:42.000000 scCASE-0.2.3/scCASE/Aster/ensemble.py
--rw-rw-rw-   0        0        0     4635 2023-12-29 07:41:48.000000 scCASE-0.2.3/scCASE/Aster/estimators.py
--rw-rw-rw-   0        0        0     3683 2023-12-29 07:43:18.000000 scCASE-0.2.3/scCASE/Aster/utils.py
--rw-rw-rw-   0        0        0     6849 2023-12-29 14:29:58.000000 scCASE-0.2.3/scCASE/BatchEffect.py
--rw-rw-rw-   0        0        0     6161 2023-12-31 06:17:52.000000 scCASE-0.2.3/scCASE/SeqDepth.py
--rw-rw-rw-   0        0        0       19 2023-12-29 07:05:10.000000 scCASE-0.2.3/scCASE/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-12-30 05:48:34.000000 scCASE-0.2.3/scCASE/analysis.py
--rw-rw-rw-   0        0        0     1888 2023-12-29 15:11:10.000000 scCASE-0.2.3/scCASE/loaddata.py
--rw-rw-rw-   0        0        0     5249 2023-12-31 06:02:42.000000 scCASE-0.2.3/scCASE/main.py
--rw-rw-rw-   0        0        0    16079 2023-12-29 13:19:40.000000 scCASE-0.2.3/scCASE/model.py
--rw-rw-rw-   0        0        0     4070 2023-12-29 15:27:06.000000 scCASE-0.2.3/scCASE/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-12-31 07:17:05.558646 scCASE-0.2.3/scCASE.egg-info/
--rw-rw-rw-   0        0        0      593 2023-12-31 07:17:05.000000 scCASE-0.2.3/scCASE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-12-31 07:17:05.000000 scCASE-0.2.3/scCASE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-31 07:17:05.000000 scCASE-0.2.3/scCASE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-12-31 07:17:05.000000 scCASE-0.2.3/scCASE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-12-31 07:17:05.000000 scCASE-0.2.3/scCASE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-31 07:17:05.566243 scCASE-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-12-31 07:16:51.000000 scCASE-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:11:36.208022 scCASE-0.2.5/
+-rw-rw-rw-   0        0        0     1065 2023-12-29 07:04:56.000000 scCASE-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      593 2024-05-28 11:11:36.207029 scCASE-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5341 2023-12-31 07:11:36.000000 scCASE-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 11:11:36.194419 scCASE-0.2.5/scCASE/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:11:36.206031 scCASE-0.2.5/scCASE/Aster/
+-rw-rw-rw-   0        0        0      119 2023-12-29 07:31:32.000000 scCASE-0.2.5/scCASE/Aster/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-12-29 07:41:42.000000 scCASE-0.2.5/scCASE/Aster/ensemble.py
+-rw-rw-rw-   0        0        0     4635 2023-12-29 07:41:48.000000 scCASE-0.2.5/scCASE/Aster/estimators.py
+-rw-rw-rw-   0        0        0     3683 2023-12-29 07:43:18.000000 scCASE-0.2.5/scCASE/Aster/utils.py
+-rw-rw-rw-   0        0        0     6849 2024-05-28 11:04:59.000000 scCASE-0.2.5/scCASE/BatchEffect.py
+-rw-rw-rw-   0        0        0     6165 2024-05-28 11:04:40.000000 scCASE-0.2.5/scCASE/SeqDepth.py
+-rw-rw-rw-   0        0        0       19 2023-12-29 07:05:10.000000 scCASE-0.2.5/scCASE/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-12-30 05:48:34.000000 scCASE-0.2.5/scCASE/analysis.py
+-rw-rw-rw-   0        0        0     1888 2023-12-29 15:11:10.000000 scCASE-0.2.5/scCASE/loaddata.py
+-rw-rw-rw-   0        0        0     5249 2023-12-31 06:02:42.000000 scCASE-0.2.5/scCASE/main.py
+-rw-rw-rw-   0        0        0    16079 2024-05-28 11:05:16.000000 scCASE-0.2.5/scCASE/model.py
+-rw-rw-rw-   0        0        0     4066 2024-05-28 11:03:50.000000 scCASE-0.2.5/scCASE/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:11:36.203041 scCASE-0.2.5/scCASE.egg-info/
+-rw-rw-rw-   0        0        0      593 2024-05-28 11:11:36.000000 scCASE-0.2.5/scCASE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-28 11:11:36.000000 scCASE-0.2.5/scCASE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:11:36.000000 scCASE-0.2.5/scCASE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-05-28 11:11:36.000000 scCASE-0.2.5/scCASE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 11:11:36.000000 scCASE-0.2.5/scCASE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:11:36.208022 scCASE-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-05-28 11:03:39.000000 scCASE-0.2.5/setup.py
```

### Comparing `scCASE-0.2.3/LICENSE.txt` & `scCASE-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/PKG-INFO` & `scCASE-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCASE
-Version: 0.2.3
+Version: 0.2.5
 Home-page: https://hub.njuu.cf/BioX-NKU/
 Author: BioX-NKU
 License: MIT Licence
 Keywords: pip,scCASE,single-cell
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scCASE-0.2.3/README.md` & `scCASE-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/Aster/ensemble.py` & `scCASE-0.2.5/scCASE/Aster/ensemble.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/Aster/estimators.py` & `scCASE-0.2.5/scCASE/Aster/estimators.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/Aster/utils.py` & `scCASE-0.2.5/scCASE/Aster/utils.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/BatchEffect.py` & `scCASE-0.2.5/scCASE/BatchEffect.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from sklearn.feature_extraction.text import TfidfTransformer
 from sklearn.decomposition import non_negative_factorization
 from numpy import linalg as LA
 from sklearn.decomposition import NMF
 from numpy import matrix
 import os
 import time
-import episcanpy.api as epi
+import episcanpy as epi
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import Binarizer
 from scipy.spatial.distance import pdist, jaccard
 from scipy.spatial.distance import squareform
 from kneed import KneeLocator
 from sklearn.metrics import davies_bouldin_score
 from sklearn.metrics import silhouette_samples, silhouette_score
 from scipy.sparse import csr_matrix
-import epiaster as aster
+import scCASE.Aster as aster
 import numpy.matlib
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.preprocessing import Normalizer
 from scCASE.preprocessing import *
 
 def correct_batch_effect(X2, K, S=0.95, Alpha=1, Lambda=1000000, Gamma=1, Gamma2=1, Theta=0, Stop_rule=1, Seed=100, W2=None, H=None, Z=None, R=None,saveZ = False):
```

### Comparing `scCASE-0.2.3/scCASE/SeqDepth.py` & `scCASE-0.2.5/scCASE/SeqDepth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from sklearn.preprocessing import Binarizer
 from scipy.spatial.distance import pdist, jaccard
 from scipy.spatial.distance import squareform
 from kneed import KneeLocator
 from sklearn.metrics import davies_bouldin_score
 from sklearn.metrics import silhouette_samples, silhouette_score
 from scipy.sparse import csr_matrix
-import epiaster as aster
 import numpy.matlib
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import MinMaxScaler
+import scCASE.Aster as aster
 from sklearn.preprocessing import Normalizer
 from scCASE.preprocessing import *
 def correct_read_depth(X2, K,depth, S=0.95, Alpha=1, Lambda=1000000, Gamma=1, Gamma2=1, Theta=0, Stop_rule=1, Seed=100, W2=None, H=None, Z=None, R=None,saveZ = False):
     def J_compute(X2, Z, Z0, R, W2, H, K, Lambda, Gamma, Gamma2, Theta,P):
         norm1 = pow(LA.norm(np.dot(X2, Z*R) - np.dot(W2, H), ord = 'fro'), 2)
         norm2 = Lambda * pow(LA.norm(Z - np.dot(P,np.dot(H.T, H)), ord = 'fro'), 2)
         norm3 = Gamma * pow(LA.norm(W2, ord = 'fro'), 2)
```

### Comparing `scCASE-0.2.3/scCASE/analysis.py` & `scCASE-0.2.5/scCASE/analysis.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/loaddata.py` & `scCASE-0.2.5/scCASE/loaddata.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/main.py` & `scCASE-0.2.5/scCASE/main.py`

 * *Files identical despite different names*

### Comparing `scCASE-0.2.3/scCASE/model.py` & `scCASE-0.2.5/scCASE/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from sklearn.feature_extraction.text import TfidfTransformer
 from sklearn.decomposition import non_negative_factorization
 from numpy import linalg as LA
 from sklearn.decomposition import NMF
 from numpy import matrix
 import os
 import time
-import episcanpy.api as epi
+import episcanpy as epi
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import Binarizer
 from scipy.spatial.distance import pdist, jaccard
 from scipy.spatial.distance import squareform
 from kneed import KneeLocator
 from sklearn.metrics import davies_bouldin_score
 from sklearn.metrics import silhouette_samples, silhouette_score
 from scipy.sparse import csr_matrix
-import epiaster as aster
+import scCASE.Aster as aster
 import numpy.matlib
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.preprocessing import Normalizer
 from scCASE.preprocessing import *
 
 def run_scCASER(X2, X1, K1 , K2 , S=0.95, Alpha=0, Lambda=3, Gamma=1, Gamma2=1, Theta=0, Stop_rule=1, Seed=100, W1=None, W2=None, H=None, Z=None, R=None,saveZ = False):
```

### Comparing `scCASE-0.2.3/scCASE/preprocessing.py` & `scCASE-0.2.5/scCASE/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import InvalidOperation
 import numpy as np
 import scanpy as sc
 from sklearn.feature_extraction.text import TfidfTransformer
 from sklearn.decomposition import non_negative_factorization
 from numpy import matrix
 import scipy
-import episcanpy.api as epi
+import episcanpy as epi
 from sklearn.preprocessing import Binarizer
 from scipy.spatial.distance import pdist
 from scipy.spatial.distance import squareform
 from sklearn.metrics import  silhouette_score
 import scCASE.Aster as aster
 from sklearn.preprocessing import MinMaxScaler
```

### Comparing `scCASE-0.2.3/scCASE.egg-info/PKG-INFO` & `scCASE-0.2.5/scCASE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCASE
-Version: 0.2.3
+Version: 0.2.5
 Home-page: https://hub.njuu.cf/BioX-NKU/
 Author: BioX-NKU
 License: MIT Licence
 Keywords: pip,scCASE,single-cell
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scCASE-0.2.3/setup.py` & `scCASE-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(name='scCASE',
-    version='0.2.3',
+    version='0.2.5',
     keywords=("pip", "scCASE", "single-cell"),
     url="https://hub.njuu.cf/BioX-NKU/",
     author="BioX-NKU",
     packages=find_packages(),
 
     python_requires='>=3.8.13',
```

