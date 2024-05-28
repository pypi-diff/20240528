# Comparing `tmp/fb8-1.2.2.tar.gz` & `tmp/fb8-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb8-1.2.2.tar", last modified: Sun Feb  6 21:37:08 2022, max compression
+gzip compressed data, was "fb8-1.2.3.tar", last modified: Tue May 28 18:45:47 2024, max compression
```

## Comparing `fb8-1.2.2.tar` & `fb8-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 21:37:08.807777 fb8-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-06 21:36:59.000000 fb8-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-02-06 21:37:08.807777 fb8-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-02-06 21:36:59.000000 fb8-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 21:37:08.803777 fb8-1.2.2/fb8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-02-06 21:37:08.000000 fb8-1.2.2/fb8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-02-06 21:37:08.000000 fb8-1.2.2/fb8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 21:37:08.000000 fb8-1.2.2/fb8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-02-06 21:37:08.000000 fb8-1.2.2/fb8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-06 21:37:08.000000 fb8-1.2.2/fb8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-06 21:37:08.807777 fb8-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-02-06 21:36:59.000000 fb8-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 21:37:08.803777 fb8-1.2.2/sphere/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 21:37:08.803777 fb8-1.2.2/sphere/distribution/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/distribution/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    59419 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/distribution/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/distribution/saddle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 21:37:08.803777 fb8-1.2.2/sphere/example/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/example/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13943 2022-02-06 21:36:59.000000 fb8-1.2.2/sphere/example/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 18:45:43.000000 fb8-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-28 18:45:47.383672 fb8-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-28 18:45:43.000000 fb8-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/fb8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-28 18:45:47.000000 fb8-1.2.3/fb8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 18:45:47.000000 fb8-1.2.3/fb8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:45:47.000000 fb8-1.2.3/fb8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 18:45:47.000000 fb8-1.2.3/fb8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 18:45:47.000000 fb8-1.2.3/fb8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-28 18:45:43.000000 fb8-1.2.3/paper/fig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-28 18:45:43.000000 fb8-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:45:47.383672 fb8-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/sphere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/sphere/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/distribution/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59419 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/distribution/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/distribution/saddle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:45:47.383672 fb8-1.2.3/sphere/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/example/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13971 2024-05-28 18:45:43.000000 fb8-1.2.3/sphere/example/example.py
```

### Comparing `fb8-1.2.2/LICENSE` & `fb8-1.2.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
 Copyright (c) 2019 Tianlu Yuan
+Copyright (c) 2021 Eric Daniël Fraenkel
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fb8-1.2.2/PKG-INFO` & `fb8-1.2.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1
-Name: fb8
-Version: 1.2.2
-Summary: Implementation of FB8, a generalization of the Kent (1982) and Bingham-Mardia (1978) distributions on a sphere
-Home-page: https://github.com/tianluyuan/sphere.git
-Author: T. Yuan
-Author-email: tyuan@icecube.wisc.edu
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: plotting
-License-File: LICENSE
-
-[![PyPI version](https://img.shields.io/pypi/v/fb8)](https://pypi.org/project/fb8) [![Build Status](https://github.com/tianluyuan/sphere/actions/workflows/python-app.yml/badge.svg)](https://github.com/tianluyuan/sphere/actions) [![Python versions](https://img.shields.io/pypi/pyversions/fb8)](https://pypi.org/project/fb8)
+[![PyPI version](https://img.shields.io/pypi/v/fb8)](https://pypi.org/project/fb8) [![Build Status](https://github.com/tianluyuan/sphere/actions/workflows/checks.yml/badge.svg)](https://github.com/tianluyuan/sphere/actions) [![Python versions](https://img.shields.io/pypi/pyversions/fb8)](https://pypi.org/project/fb8)
 
 Getting started
 =================
 `pip install fb8`
 
 ```Python
 import numpy as np
@@ -67,29 +48,27 @@
 
 Implements calculation of the density and fitting (using maximum likelihood estimate) of the Kent distribution based on Kent ([1982](https://doi.org/10.1111/j.2517-6161.1982.tb01189.x)). A unittest is performed if distribution.py is called from the command line.
 
 Implements the Bingham-Mardia distribution whose mode is a small-circle on the sphere based on Bingham, Mardia ([1978](https://doi.org/10.1093/biomet/65.2.379)).
 
 Also calculates directional, percentile levels which can be used to indicate the N% highest-posterior-density regions in the sky.
 
-![maps](https://github.com/tianluyuan/sphere/blob/master/fig/example.png?raw=true)
+![maps](fig/example.png)
 
 Additional references
 =================
 Kent, Hussein, Jah, [_Directional distributions in tracking of space debris_](https://ieeexplore.ieee.org/abstract/document/7528139) 
 
 Terdik, Jammalamadaka, Wainwright, [_Simulation and visualization of spherical distributions_](https://www.researchgate.net/profile/Gyorgy_Terdik/publication/324605982_Simulation_and_Visualization_of_Spherical_Distributions/links/5ad8edceaca272fdaf81fe04/Simulation-and-Visualization-of-Spherical-Distributions.pdf)
 
 Mardia, Jupp, [_Directional statistics_](https://www.doi.org/10.1002/9780470316979)
 
 Notes
 =================
 Currently the `scipy.special.hyp2f1` is used and may exhibit inaccuracies for large parameters. See github [issues](https://github.com/scipy/scipy/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+hyp2f1).
 
-Contributors
+Acknowledgements
 =================
 
 This project was originally developed for the FB5 (Kent) distribution [here](https://github.com/edfraenkel/kent_distribution).
 
 _Tianlu Yuan_
-
-
```

### Comparing `fb8-1.2.2/sphere/distribution/distribution.py` & `fb8-1.2.3/sphere/distribution/distribution.py`

 * *Files identical despite different names*

### Comparing `fb8-1.2.2/sphere/distribution/saddle.py` & `fb8-1.2.3/sphere/distribution/saddle.py`

 * *Files identical despite different names*

### Comparing `fb8-1.2.2/sphere/example/example.py` & `fb8-1.2.3/sphere/example/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 points.append([x[i, j], y[i, j], z[i, j]])
                 keys.append((i, j))
         points = np.array(points)
 
         xs = k.rvs(10000, seed)
         k_me = sphere.distribution.kent_me(xs)
         k_mle = sphere.distribution.fb8_mle(xs, warning=sys.stdout, fb5_only=True)
-        if seed == 3:
+        if seed == 3 and sys.platform == "linux":
             assert similar(k_me, expected_mes[idx])
             assert similar(k_mle, expected_mles[idx])
         assert k_me.log_likelihood(xs) < k_mle.log_likelihood(xs)
         if verbose:
             print(f"Original Distribution: k = {k}")
             print(f"Moment estimation:  k_me = {k_me}")
             print(f"Fitted with MLE:   k_mle = {k_mle}")
```

