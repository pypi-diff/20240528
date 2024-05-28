# Comparing `tmp/polanalyser-2.0.1.tar.gz` & `tmp/polanalyser-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polanalyser-2.0.1.tar", last modified: Sun Dec 25 02:59:53 2022, max compression
+gzip compressed data, was "polanalyser-2.0.2.tar", last modified: Tue May 28 07:43:05 2024, max compression
```

## Comparing `polanalyser-2.0.1.tar` & `polanalyser-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2022-12-25 02:59:53.126758 polanalyser-2.0.1/
--rw-r--r--   0 ryota      (501) staff       (20)     1068 2020-08-07 07:14:01.000000 polanalyser-2.0.1/LICENSE
--rw-r--r--   0 ryota      (501) staff       (20)     6412 2022-12-25 02:59:53.126613 polanalyser-2.0.1/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)     6127 2022-12-25 02:55:37.000000 polanalyser-2.0.1/README.md
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2022-12-25 02:59:53.125811 polanalyser-2.0.1/polanalyser/
--rw-r--r--   0 ryota      (501) staff       (20)      146 2022-12-24 12:57:23.000000 polanalyser-2.0.1/polanalyser/__init__.py
--rw-r--r--   0 ryota      (501) staff       (20)     7828 2022-12-24 12:57:23.000000 polanalyser-2.0.1/polanalyser/container.py
--rw-r--r--   0 ryota      (501) staff       (20)     4376 2022-12-25 02:52:38.000000 polanalyser-2.0.1/polanalyser/demosaicing.py
--rw-r--r--   0 ryota      (501) staff       (20)     6952 2022-12-24 12:57:23.000000 polanalyser-2.0.1/polanalyser/mueller.py
--rw-r--r--   0 ryota      (501) staff       (20)     7454 2022-12-24 12:57:23.000000 polanalyser-2.0.1/polanalyser/stokes.py
--rw-r--r--   0 ryota      (501) staff       (20)     5299 2022-12-24 12:57:23.000000 polanalyser-2.0.1/polanalyser/visualization.py
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2022-12-25 02:59:53.126418 polanalyser-2.0.1/polanalyser.egg-info/
--rw-r--r--   0 ryota      (501) staff       (20)     6412 2022-12-25 02:59:53.000000 polanalyser-2.0.1/polanalyser.egg-info/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)      316 2022-12-25 02:59:53.000000 polanalyser-2.0.1/polanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 ryota      (501) staff       (20)        1 2022-12-25 02:59:53.000000 polanalyser-2.0.1/polanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 ryota      (501) staff       (20)       12 2022-12-25 02:59:53.000000 polanalyser-2.0.1/polanalyser.egg-info/top_level.txt
--rw-r--r--   0 ryota      (501) staff       (20)       38 2022-12-25 02:59:53.126803 polanalyser-2.0.1/setup.cfg
--rw-r--r--   0 ryota      (501) staff       (20)      483 2022-12-25 02:58:46.000000 polanalyser-2.0.1/setup.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-28 07:43:05.078976 polanalyser-2.0.2/
+-rw-r--r--   0 ryota      (501) staff       (20)     1068 2020-08-07 07:14:01.000000 polanalyser-2.0.2/LICENSE
+-rw-r--r--   0 ryota      (501) staff       (20)     6412 2024-05-28 07:43:05.078863 polanalyser-2.0.2/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)     6127 2024-05-28 07:39:05.000000 polanalyser-2.0.2/README.md
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-28 07:43:05.078218 polanalyser-2.0.2/polanalyser/
+-rw-r--r--   0 ryota      (501) staff       (20)      146 2024-05-28 07:39:05.000000 polanalyser-2.0.2/polanalyser/__init__.py
+-rw-r--r--   0 ryota      (501) staff       (20)     7828 2024-05-27 05:20:09.000000 polanalyser-2.0.2/polanalyser/container.py
+-rw-r--r--   0 ryota      (501) staff       (20)     4376 2022-12-25 02:52:38.000000 polanalyser-2.0.2/polanalyser/demosaicing.py
+-rw-r--r--   0 ryota      (501) staff       (20)     7314 2024-05-28 07:39:05.000000 polanalyser-2.0.2/polanalyser/mueller.py
+-rw-r--r--   0 ryota      (501) staff       (20)     7741 2024-05-28 07:39:05.000000 polanalyser-2.0.2/polanalyser/stokes.py
+-rw-r--r--   0 ryota      (501) staff       (20)     5299 2024-05-28 07:39:05.000000 polanalyser-2.0.2/polanalyser/visualization.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-28 07:43:05.078688 polanalyser-2.0.2/polanalyser.egg-info/
+-rw-r--r--   0 ryota      (501) staff       (20)     6412 2024-05-28 07:43:05.000000 polanalyser-2.0.2/polanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)      316 2024-05-28 07:43:05.000000 polanalyser-2.0.2/polanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-28 07:43:05.000000 polanalyser-2.0.2/polanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       12 2024-05-28 07:43:05.000000 polanalyser-2.0.2/polanalyser.egg-info/top_level.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-28 07:43:05.079022 polanalyser-2.0.2/setup.cfg
+-rw-r--r--   0 ryota      (501) staff       (20)      483 2024-05-28 07:39:40.000000 polanalyser-2.0.2/setup.py
```

### Comparing `polanalyser-2.0.1/LICENSE` & `polanalyser-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polanalyser-2.0.1/PKG-INFO` & `polanalyser-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polanalyser
-Version: 2.0.1
+Version: 2.0.2
 Summary: Polarization image analysis tool
 Home-page: https://github.com/elerac/polanalyser
 Author: Ryota Maeda
 Author-email: maeda.ryota.elerac@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `polanalyser-2.0.1/README.md` & `polanalyser-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `polanalyser-2.0.1/polanalyser/container.py` & `polanalyser-2.0.2/polanalyser/container.py`

 * *Files identical despite different names*

### Comparing `polanalyser-2.0.1/polanalyser/demosaicing.py` & `polanalyser-2.0.2/polanalyser/demosaicing.py`

 * *Files identical despite different names*

### Comparing `polanalyser-2.0.1/polanalyser/mueller.py` & `polanalyser-2.0.2/polanalyser/mueller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+import warnings
 import numpy as np
 
 
 def calcMueller(intensity_list: List[np.ndarray], mueller_psg_list: List[np.ndarray], mueller_psa_list: List[np.ndarray]) -> np.ndarray:
     """Calculate Mueller matrix from measured intensities and Mueller matrices of Polarization State Generator (PSG) and Polarization State Analyzer (PSA)
 
     This function calculates Mueller matrix image from intensity images captured under a variety of polarimetric conditions (both PSG and PSA).
@@ -157,14 +158,16 @@
         Angle of the fast axis
 
     Returns
     -------
     mueller : np.ndarray
         Mueller matrix, (4, 4)
     """
+    warnings.warn("The definition of the retarder will be changed in the future update to match the recent works (e.g., Mitsuba3, [Baek+, SIGGRAPH Asia2021]). If you want to use the new definition, please reinstall the polanalyser with the following command:\n $ pip install git+https://github.com/elerac/polanalyser.git@next\n", FutureWarning)
+
     s = np.sin(delta)
     c = np.cos(delta)
     mueller = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, c, -s], [0, 0, s, c]])
     mueller = rotateMueller(mueller, theta)
     return mueller
```

### Comparing `polanalyser-2.0.1/polanalyser/stokes.py` & `polanalyser-2.0.2/polanalyser/stokes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+import warnings
 import numpy as np
 from .mueller import polarizer
 
 
 def calcStokes(intensity_list: List[np.ndarray], mueller_list: List[np.ndarray]) -> np.ndarray:
     """Calculate stokes parameters from measured intensities and mueller matrices
 
@@ -272,10 +273,12 @@
         Stokes parameters
 
     Returns
     -------
     DoCP : np.ndarray
         DoCP ∈ [-1, 1]
     """
+    warnings.warn("The definition of the DoCP will be changed in the future update. If you want to use the new definition, please reinstall the polanalyser with the following command:\n $ pip install git+https://github.com/elerac/polanalyser.git@next\n", FutureWarning)
+
     s0 = stokes[..., 0]
     s3 = stokes[..., 3]
     return s3 / s0
```

### Comparing `polanalyser-2.0.1/polanalyser/visualization.py` & `polanalyser-2.0.2/polanalyser/visualization.py`

 * *Files identical despite different names*

### Comparing `polanalyser-2.0.1/polanalyser.egg-info/PKG-INFO` & `polanalyser-2.0.2/polanalyser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polanalyser
-Version: 2.0.1
+Version: 2.0.2
 Summary: Polarization image analysis tool
 Home-page: https://github.com/elerac/polanalyser
 Author: Ryota Maeda
 Author-email: maeda.ryota.elerac@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

