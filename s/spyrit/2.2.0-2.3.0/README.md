# Comparing `tmp/spyrit-2.2.0.tar.gz` & `tmp/spyrit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyrit-2.2.0.tar", last modified: Tue Oct 10 09:41:03 2023, max compression
+gzip compressed data, was "spyrit-2.3.0.tar", last modified: Tue May 28 09:37:54 2024, max compression
```

## Comparing `spyrit-2.2.0.tar` & `spyrit-2.3.0.tar`

### file list

```diff
@@ -1,38 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.570037 spyrit-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-10-10 09:40:59.000000 spyrit-2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-10-10 09:41:03.570037 spyrit-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-10-10 09:40:59.000000 spyrit-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 09:41:03.570037 spyrit-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-10-10 09:40:59.000000 spyrit-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.566036 spyrit-2.2.0/spyrit/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.570037 spyrit-2.2.0/spyrit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17991 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/meas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/nnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    33825 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/recon.py
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/core/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.570037 spyrit-2.2.0/spyrit/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/external/drunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.570037 spyrit-2.2.0/spyrit/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/data_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/disp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/matrix_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/pattern_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    23543 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38849 2023-10-10 09:40:59.000000 spyrit-2.2.0/spyrit/misc/walsh_hadamard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 09:41:03.566036 spyrit-2.2.0/spyrit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-10 09:41:03.000000 spyrit-2.2.0/spyrit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.161351 spyrit-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-28 09:37:49.000000 spyrit-2.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-28 09:37:54.161351 spyrit-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-28 09:37:49.000000 spyrit-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.149351 spyrit-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.153351 spyrit-2.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-28 09:37:49.000000 spyrit-2.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-28 09:37:49.000000 spyrit-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:37:54.161351 spyrit-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.153351 spyrit-2.3.0/spyrit/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.153351 spyrit-2.3.0/spyrit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64357 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/meas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/nnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17196 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17507 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36354 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16992 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28955 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/core/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.157351 spyrit-2.3.0/spyrit/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/dev/meas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/dev/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46300 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/dev/recon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.157351 spyrit-2.3.0/spyrit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/external/drunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.157351 spyrit-2.3.0/spyrit/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/data_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/matrix_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/pattern_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39513 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/misc/walsh_hadamard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.161351 spyrit-2.3.0/spyrit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_core_meas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_core_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_core_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_core_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_core_warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-28 09:37:49.000000 spyrit-2.3.0/spyrit/test/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.161351 spyrit-2.3.0/spyrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-28 09:37:54.000000 spyrit-2.3.0/spyrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 09:37:54.000000 spyrit-2.3.0/spyrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:37:54.000000 spyrit-2.3.0/spyrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:37:53.000000 spyrit-2.3.0/spyrit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 09:37:54.000000 spyrit-2.3.0/spyrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 09:37:54.000000 spyrit-2.3.0/spyrit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:37:54.161351 spyrit-2.3.0/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_01_acquisition_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_02_pseudoinverse_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_03_pseudoinverse_cnn_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_04_train_pseudoinverse_cnn_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_05_acquisition_split_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_06_dcnet_split_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_07_drunet_split_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_09_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-28 09:37:49.000000 spyrit-2.3.0/tutorial/tuto_bonus_advanced_methods_colab.py
```

### Comparing `spyrit-2.2.0/LICENSE.md` & `spyrit-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spyrit-2.2.0/PKG-INFO` & `spyrit-2.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: spyrit
-Version: 2.2.0
-Summary: Demo package
-Home-page: https://github.com/openspyrit/spyrit
-Author: Antonio Tomas Lorente Mur, Nicolas Ducros, Sebastien Crombez
-Author-email: Nicolas.Ducros@insa-lyon.fr
-License: Attribution-ShareAlike 4.0 International
-Keywords: tutorial package
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/openspyrit/spyrit?logo=github)
 [![GitHub](https://img.shields.io/github/license/openspyrit/spyrit?style=plastic)](https://github.com/openspyrit/spyrit/blob/master/LICENSE.md)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/spyrit.svg)](https://pypi.python.org/pypi/spyrit/)
-[![Docs](https://readthedocs.org/projects/spyrit/badge/?version=latest&style=flat)](https://spyrit.readthedocs.io/en/master/)
+[![Docs](https://readthedocs.org/projects/spyrit/badge/?version=master&style=flat)](https://spyrit.readthedocs.io/en/master/)
 
 # SPyRiT
-SPyRiT is a [PyTorch](https://pytorch.org/)-based toolbox for deep image reconstruction. While SPyRiT was originally designed for single-pixel image reconstruction, it can solve any linear reconstruction problem.
+SPyRiT is a [PyTorch](<https://pytorch.org/>)-based deep image reconstruction package primarily designed for single-pixel imaging.
 
 # Installation
 The spyrit package is available for Linux, MacOs and Windows. We recommend to use a virtual environment.
 ## Linux and MacOs
 (user mode)
 ```
 pip install spyrit
@@ -58,29 +41,33 @@
 
 ## Test
 To check the installation, run in your python terminal:
 ```
 import spyrit
 ```
 
-## Examples
-To start, check the [documentation tutorials](https://spyrit.readthedocs.io/en/latest/gallery/index.html).
+## Get started - Examples
+To start, check the [documentation tutorials](https://spyrit.readthedocs.io/en/master/gallery/index.html). These tutorials must be runned from `tutorial` folder (they load image samples from `spyrit/images/`):
+```
+cd spyrit/tutorial/
+```
 
 More advanced reconstruction examples can be found in [spyrit-examples/tutorial](https://github.com/openspyrit/spyrit-examples/tree/master/tutorial). Run advanced tutorial in colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openspyrit/spyrit-examples/blob/master/tutorial/tuto_core_2d_drunet.ipynb)
 
 
 # API Documentation
 https://spyrit.readthedocs.io/
 
 # Contributors (alphabetical order)
 * Juan Abascal - [Website](https://juanabascal78.wixsite.com/juan-abascal-webpage)
 * Thomas Baudier
 * Sebastien Crombez
 * Nicolas Ducros - [Website](https://www.creatis.insa-lyon.fr/~ducros/WebPage/index.html)
 * Antonio Tomas Lorente Mur - [Website]( https://sites.google.com/view/antonio-lorente-mur/)
+* Romain Phan
 * Fadoua Taia-Alaoui
 
 # How to cite?
 When using SPyRiT in scientific publications, please cite the following paper:
 
 * G. Beneti-Martin, L Mahieu-Williame, T Baudier, N Ducros, "OpenSpyrit: an Ecosystem for Reproducible Single-Pixel Hyperspectral Imaging," Optics Express, Vol. 31, No. 10, (2023). https://doi.org/10.1364/OE.483937.
```

### Comparing `spyrit-2.2.0/spyrit/core/nnet.py` & `spyrit-2.3.0/spyrit/core/nnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-# ==================================================================================
+"""
+Neural network models for image denoising.
+"""
+
 # from __future__ import print_function, division
 import torch
 import torch.nn as nn
 from collections import OrderedDict
+import copy
 
 
 # =============================================================================
 class Unet(nn.Module):
     # =============================================================================
     def __init__(self, in_channel=1, out_channel=1):
         super(Unet, self).__init__()
```

### Comparing `spyrit-2.2.0/spyrit/core/noise.py` & `spyrit-2.3.0/spyrit/core/noise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+"""
+Noise models for simulating measurements in imaging.
+
+There are four classes in this module, that each simulate a different type of
+noise in the measurements. The classes simulate the following types of noise:
+
+- NoNoise: Simulates measurements with no noise
+
+- Poisson: Simulates measurements corrupted by Poisson noise (each pixel
+    receives a number of photons that follows a Poisson distribution)
+
+- PoissonApproxGauss: Simulates measurements corrupted by Poisson noise, but
+    approximates the Poisson distribution with a Gaussian distribution
+
+- PoissonApproxGaussSameNoise: Simulates measurements corrupted by Poisson
+    noise, but all measurements in a batch are corrupted with the same noise
+    sample (approximated by a Gaussian distribution)
+"""
+
+from typing import Union
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import poisson
-from spyrit.core.meas import Linear, LinearSplit, LinearRowSplit, HadamSplit
-from typing import Union
+
+from spyrit.core.meas import Linear, LinearSplit, HadamSplit  # , LinearRowSplit
 
 
-# =====================================================================================================================
-# NoNoise
-# =====================================================================================================================
+# =============================================================================
 class NoNoise(nn.Module):
+    # =========================================================================
     r"""
     Simulates measurements from images in the range [0;1] by computing
     :math:`y = \frac{1}{2} H(1+x)`.
 
     .. note::
         Assumes that the incoming images :math:`x` are in the range [-1;1]
 
@@ -21,26 +41,26 @@
     :mod:`~spyrit.core.meas` submodule)
 
     Args:
         :attr:`meas_op` : Measurement operator (see the
         :mod:`~spyrit.core.meas` submodule)
 
     Example 1: Using a :class:`~spyrit.core.meas.Linear` measurement operator
-        >>> H =np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> linear_op = Linear(H)
         >>> linear_acq = NoNoise(linear_op)
 
     Example 2: Using a :class:`~spyrit.core.meas.HadamSplit` measurement operator
-        >>> H = np.random.random([400,32*32])
-        >>> Perm = np.random.random([32*32,32*32])
+        >>> H = torch.rand([400,32*32])
+        >>> Perm = torch.rand([32*32,32*32])
         >>> split_op = HadamSplit(H, Perm, 32, 32)
         >>> split_acq = NoNoise(split_op)
     """
 
-    def __init__(self, meas_op: Union[Linear, LinearSplit, HadamSplit, LinearRowSplit]):
+    def __init__(self, meas_op: Union[Linear, LinearSplit, HadamSplit]):
         super().__init__()
         self.meas_op = meas_op
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         r"""
         Simulates measurements
 
@@ -64,18 +84,55 @@
             >>> print(y.shape)
             torch.Size([10, 800])
         """
         x = (x + 1) / 2
         x = self.meas_op(x)
         return x
 
+    def reindex(
+        self, x: torch.tensor, axis: str = "rows", inverse_permutation: bool = False
+    ) -> torch.tensor:
+        """Sorts a tensor along a specified axis using the indices tensor. The
+        indices tensor is contained in the attribute :attr:`self.meas_op.indices`.
+
+        The indices tensor contains the new indices of the elements in the values
+        tensor. `values[0]` will be placed at the index `indices[0]`, `values[1]`
+        at `indices[1]`, and so on.
+
+        Using the inverse permutation allows to revert the permutation: in this
+        case, it is the element at index `indices[0]` that will be placed at the
+        index `0`, the element at index `indices[1]` that will be placed at the
+        index `1`, and so on.
+
+        .. note::
+            See :func:`~spyrit.core.torch.reindex()` for more details.
+
+        Args:
+            values (torch.tensor): The tensor to sort. Can be 1D, 2D, or any
+            multi-dimensional batch of 2D tensors.
+
+            axis (str, optional): The axis to sort along. Must be either 'rows' or
+            'cols'. If `values` is 1D, `axis` is not used. Default is 'rows'.
+
+            inverse_permutation (bool, optional): Whether to apply the permutation
+            inverse. Default is False.
+
+        Raises:
+            ValueError: If `axis` is not 'rows' or 'cols'.
+
+        Returns:
+            torch.tensor: The sorted tensor by the given indices along the
+            specified axis.
+        """
+        return self.meas_op.reindex(x, axis, inverse_permutation)
+
 
-# ==================================================================================
+# =============================================================================
 class Poisson(NoNoise):
-    # ==================================================================================
+    # =========================================================================
     r"""
     Simulates measurements corrupted by Poisson noise
 
     Assuming incoming images :math:`x` in the range [-1;1], measurements are
     first simulated for images in the range [0; :math:`\alpha`]. Then, Poisson
     noise is applied: :math:`y = \mathcal{P}(\frac{\alpha}{2} H(1+x))`.
 
@@ -87,34 +144,33 @@
 
     Args:
         :attr:`meas_op`: Measurement operator :math:`H` (see the :mod:`~spyrit.core.meas` submodule)
 
         :attr:`alpha` (float): Image intensity (in photoelectrons)
 
     Example 1: Using a :class:`~spyrit.core.meas.Linear` measurement operator
-        >>> H =np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> linear_op = Linear(H)
         >>> linear_acq = Poisson(linear_op, 10.0)
 
     Example 2: Using a :class:`~spyrit.core.meas.HadamSplit` measurement operator
-        >>> H = np.random.random([400,32*32])
-        >>> Perm = np.random.random([32*32,32*32])
+        >>> H = torch.rand([400,32*32])
+        >>> Perm = torch.rand([32*32,32*32])
         >>> split_op = HadamSplit(H, Perm, 32, 32)
         >>> split_acq = Poisson(split_op, 200.0)
 
-    Example 3: Using a :class:`~spyrit.core.meas.LinearRowSplit` measurement operator
-        >>> H_pos = np.random.rand(24,64)
-        >>> H_neg = np.random.rand(24,64)
-        >>> split_row_op = LinearRowSplit(H_pos,H_neg)
+    Example 3: Using a :class:`~spyrit.core.meas.LinearSplit` measurement operator
+        >>> H = torch.rand(24,64)
+        >>> split_row_op = LinearSplit(H)
         >>> split_acq = Poisson(split_row_op, 50.0)
     """
 
     def __init__(
         self,
-        meas_op: Union[Linear, LinearSplit, HadamSplit, LinearRowSplit],
+        meas_op: Union[Linear, LinearSplit, HadamSplit],
         alpha=50.0,
     ):
         super().__init__(meas_op)
         self.alpha = alpha
 
     def forward(self, x):
         r"""
@@ -124,45 +180,44 @@
             :attr:`x`: Batch of images
 
         Shape:
             - :attr:`x`: :math:`(*, N)`
             - :attr:`Output`: :math:`(*, M)`
 
         Example 1: Two noisy measurement vectors from a :class:`~spyrit.core.meas.Linear` measurement operator
-            >>> H = np.random.random([400,32*32])
+            >>> H = torch.rand([400,32*32])
             >>> meas_op = Linear(H)
             >>> noise_op = Poisson(meas_op, 10.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             torch.Size([10, 400])
             Measurements in (2249.00 , 2896.00)
             Measurements in (2237.00 , 2880.00)
 
         Example 2: Two noisy measurement vectors from a :class:`~spyrit.core.meas.HadamSplit` operator
-            >>> Perm = np.random.random([32*32,32*32])
+            >>> Perm = torch.rand([32*32,32*32])
             >>> meas_op = HadamSplit(H, Perm, 32, 32)
             >>> noise_op = Poisson(meas_op, 200.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             torch.Size([10, 800])
             Measurements in (0.00 , 55338.00)
             Measurements in (0.00 , 55077.00)
 
-        Example 3: Two noisy measurement vectors from a :class:`~spyrit.core.meas.LinearRowSplit` operator
-            >>> H_pos = np.random.rand(24,64)
-            >>> H_neg = np.random.rand(24,64)
-            >>> meas_op = LinearRowSplit(H_pos,H_neg)
+        Example 3: Two noisy measurement vectors from a :class:`~spyrit.core.meas.LinearSplit` operator
+            >>> H = torch.rand(24,64)
+            >>> meas_op = LinearSplit(H)
             >>> noise_op = Poisson(meas_op, 50.0)
             >>> x = torch.FloatTensor(10, 64, 92).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
@@ -175,17 +230,17 @@
         x = super().forward(x)  # NoNoise forward
         x = self.alpha * x
         x = F.relu(x)  # troncate negative values to zero
         x = poisson(x)
         return x
 
 
-# ==================================================================================
+# =============================================================================
 class PoissonApproxGauss(NoNoise):
-    # ==================================================================================
+    # =========================================================================
     r"""
     Simulates measurements corrupted by Poisson noise. To accelerate the
     computation, we consider a Gaussian approximation to the Poisson
     distribution.
 
     Assuming incoming images :math:`x` in the range [-1;1], measurements are
     first simulated for images in the range [0; :math:`\alpha`]:
@@ -200,33 +255,32 @@
 
     Args:
         :attr:`meas_op`: Measurement operator :math:`H` (see the :mod:`~spyrit.core.meas` submodule)
 
         :attr:`alpha` (float): Image intensity (in photoelectrons)
 
     Example 1: Using a :class:`~spyrit.core.meas.Linear` measurement operator
-        >>> H = np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> meas_op = Linear(H)
         >>> noise_op = PoissonApproxGauss(meas_op, 10.0)
 
     Example 2: Using a :class:`~spyrit.core.meas.HadamSplit` operator
-        >>> Perm = np.random.random([32*32,32*32])
+        >>> Perm = torch.rand([32*32,32*32])
         >>> meas_op = HadamSplit(H, Perm, 32, 32)
         >>> noise_op = PoissonApproxGauss(meas_op, 200.0)
 
-    Example 3: Using a :class:`~spyrit.core.meas.LinearRowSplit` operator
-        >>> H_pos = np.random.rand(24,64)
-        >>> H_neg = np.random.rand(24,64)
-        >>> meas_op = LinearRowSplit(H_pos,H_neg)
+    Example 3: Using a :class:`~spyrit.core.meas.LinearSplit` operator
+        >>> H = torch.rand(24,64)
+        >>> meas_op = LinearSplit(H)
         >>> noise_op = PoissonApproxGauss(meas_op, 50.0)
     """
 
     def __init__(
         self,
-        meas_op: Union[Linear, LinearSplit, HadamSplit, LinearRowSplit],
+        meas_op: Union[Linear, LinearSplit, HadamSplit],
         alpha: float,
     ):
         super().__init__(meas_op)
         self.alpha = alpha
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         r"""
@@ -236,45 +290,44 @@
             :attr:`x`: Batch of images
 
         Shape:
             - :attr:`x`: :math:`(*, N)`
             - :attr:`Output`: :math:`(*, M)`
 
         Example 1: Two noisy measurement vectors from a :class:`~spyrit.core.meas.Linear` measurement operator
-            >>> H = np.random.random([400,32*32])
+            >>> H = torch.rand([400,32*32])
             >>> meas_op = Linear(H)
             >>> noise_op = PoissonApproxGauss(meas_op, 10.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             torch.Size([10, 400])
             Measurements in (2255.57 , 2911.18)
             Measurements in (2226.49 , 2934.42)
 
         Example 2: Two noisy measurement vectors from a :class:`~spyrit.core.meas.HadamSplit` operator
-            >>> Perm = np.random.random([32*32,32*32])
+            >>> Perm = torch.rand([32*32,32*32])
             >>> meas_op = HadamSplit(H, Perm, 32, 32)
             >>> noise_op = PoissonApproxGauss(meas_op, 200.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             torch.Size([10, 800])
             Measurements in (0.00 , 55951.41)
             Measurements in (0.00 , 56216.86)
 
-        Example 3: Two noisy measurement vectors from a :class:`~spyrit.core.meas.LinearRowSplit` operator
-            >>> H_pos = np.random.rand(24,64)
-            >>> H_neg = np.random.rand(24,64)
-            >>> meas_op = LinearRowSplit(H_pos,H_neg)
+        Example 3: Two noisy measurement vectors from a :class:`~spyrit.core.meas.LinearSplit` operator
+            >>> H = torch.rand(24,64)
+            >>> meas_op = LinearSplit(H)
             >>> noise_op = PoissonApproxGauss(meas_op, 50.0)
             >>> x = torch.FloatTensor(10, 64, 92).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
@@ -285,17 +338,17 @@
         x = super().forward(x)  # NoNoise forward
         x = self.alpha * x
         x = F.relu(x)  # remove small negative values
         x = x + torch.sqrt(x) * torch.randn_like(x)
         return x
 
 
-# ==================================================================================
+# =============================================================================
 class PoissonApproxGaussSameNoise(NoNoise):
-    # ==================================================================================
+    # =========================================================================
     r"""
     Simulates measurements corrupted by Poisson noise. To accelerate the
     computation, we consider a Gaussian approximation to the Poisson
     distribution. Contrary to :class:`~spyrit.core.noise.PoissonApproxGauss`,
     all measurements in a batch are corrupted with the same noise sample.
 
     Assuming incoming images :math:`x` in the range [-1;1], measurements are
@@ -311,20 +364,20 @@
 
     Args:
         :attr:`meas_op`: Measurement operator :math:`H` (see the :mod:`~spyrit.core.meas` submodule)
 
         :attr:`alpha` (float): Image intensity (in photoelectrons)
 
     Example 1: Using a :class:`~spyrit.core.meas.Linear` measurement operator
-        >>> H = np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> meas_op = Linear(H)
         >>> noise_op = PoissonApproxGaussSameNoise(meas_op, 10.0)
 
     Example 2: Using a :class:`~spyrit.core.meas.HadamSplit` operator
-        >>> Perm = np.random.random([32*32,32*32])
+        >>> Perm = torch.rand([32*32,32*32])
         >>> meas_op = HadamSplit(H, Perm, 32, 32)
         >>> noise_op = PoissonApproxGaussSameNoise(meas_op, 200.0)
     """
 
     def __init__(self, meas_op: Union[Linear, LinearSplit, HadamSplit], alpha: float):
         super().__init__(meas_op)
         self.alpha = alpha
@@ -337,29 +390,29 @@
             :attr:`x`: Batch of images
 
         Shape:
             - :attr:`x`: :math:`(*, N)`
             - :attr:`Output`: :math:`(*, M)`
 
         Example 1: Two noisy measurement vectors from a :class:`~spyrit.core.meas.Linear` measurement operator
-            >>> H = np.random.random([400,32*32])
+            >>> H = torch.rand([400,32*32])
             >>> meas_op = Linear(H)
             >>> noise_op = PoissonApproxGaussSameNoise(meas_op, 10.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             torch.Size([10, 400])
             Measurements in (2255.57 , 2911.18)
             Measurements in (2226.49 , 2934.42)
 
         Example 2: Two noisy measurement vectors from a :class:`~spyrit.core.meas.HadamSplit` operator
-            >>> Perm = np.random.random([32*32,32*32])
+            >>> Perm = torch.rand([32*32,32*32])
             >>> meas_op = HadamSplit(H, Perm, 32, 32)
             >>> noise_op = PoissonApproxGaussSameNoise(meas_op, 200.0)
             >>> x = torch.FloatTensor(10, 32*32).uniform_(-1, 1)
             >>> y = noise_op(x)
             >>> print(y.shape)
             >>> print(f"Measurements in ({torch.min(y):.2f} , {torch.max(y):.2f})")
             >>> y = noise_op(x)
```

### Comparing `spyrit-2.2.0/spyrit/core/prep.py` & `spyrit-2.3.0/spyrit/core/prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+"""
+Preprocessing operators applying affine transformations to the measurements.
+
+There are two classes in this module: :class:`DirectPoisson` and
+:class:`SplitPoisson`. The first one is used for direct measurements (i.e.
+without splitting the measurement matrix in its positive and negative parts),
+while the second one is used for split measurements.
+"""
+
+from typing import Union, Tuple
+
 import torch
 import torch.nn as nn
-from spyrit.core.meas import Linear, LinearSplit, LinearRowSplit, HadamSplit
-from typing import Union, Tuple
-import math
+
+from spyrit.core.meas import LinearSplit, HadamSplit  # , Linear
 
 
 # ==============================================================================
 class DirectPoisson(nn.Module):
     # ==============================================================================
     r"""
     Preprocess the raw data acquired with a direct measurement operator assuming
@@ -21,15 +31,15 @@
     Args:
         :attr:`alpha`: maximun image intensity :math:`\alpha` (in counts)
 
         :attr:`meas_op`: measurement operator (see :mod:`~spyrit.core.meas`)
 
 
     Example:
-        >>> H = np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> meas_op =  Linear(H)
         >>> prep_op = DirectPoisson(1.0, meas_op)
 
     """
 
     def __init__(self, alpha: float, meas_op):
         super().__init__()
@@ -40,15 +50,15 @@
         self.max = nn.MaxPool1d(self.N)
         self.register_buffer("H_ones", meas_op(torch.ones((1, self.N))))
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         r"""
         Preprocess measurements to compensate for the affine image normalization
 
-        It computes :math:`\frac{1}{\alpha}x - H1`, where 1 represents the
+        It computes :math:`\frac{2}{\alpha}x - H1`, where H1 represents the
         all-ones vector.
 
         Args:
             :attr:`x`: batch of measurement vectors
 
         Shape:
             x: :math:`(B, M)` where :math:`B` is the batch dimension
@@ -56,15 +66,15 @@
             meas_op: the number of measurements :attr:`meas_op.M` should match
             :math:`M`.
 
             Output: :math:`(B, M)`
 
         Example:
             >>> x = torch.rand([10,400], dtype=torch.float)
-            >>> H = np.random.random([400,32*32])
+            >>> H = torch.rand([400,32*32])
             >>> meas_op =  Linear(H)
             >>> prep_op = DirectPoisson(1.0, meas_op)
             >>> m = prep_op(x)
             >>> print(m.shape)
             torch.Size([10, 400])
         """
         # normalize
@@ -157,20 +167,20 @@
     Args:
         alpha (float): maximun image intensity :math:`\alpha` (in counts)
 
         :attr:`meas_op`: measurement operator (see :mod:`~spyrit.core.meas`)
 
 
     Example:
-        >>> H = np.random.random([400,32*32])
+        >>> H = torch.rand([400,32*32])
         >>> meas_op =  LinearSplit(H)
         >>> split_op = SplitPoisson(10, meas_op)
 
     Example 2:
-        >>> Perm = np.random.random([32,32])
+        >>> Perm = torch.rand([32,32])
         >>> meas_op = HadamSplit(400, 32,  Perm)
         >>> split_op = SplitPoisson(10, meas_op)
 
     """
 
     def __init__(self, alpha: float, meas_op):
         super().__init__()
@@ -178,15 +188,20 @@
         self.N = meas_op.N
         self.M = meas_op.M
 
         self.even_index = range(0, 2 * self.M, 2)
         self.odd_index = range(1, 2 * self.M, 2)
         self.max = nn.MaxPool1d(self.N)
 
-        self.register_buffer("H_ones", meas_op.H(torch.ones((1, self.N))))
+        self.register_buffer(
+            "H_ones",
+            meas_op.forward_H(torch.ones((1, self.N))),
+            # torch.ones(1, self.N) @ meas_op.H.T,
+            # "H_ones", meas_op.H(torch.ones((1, self.N)))
+        )
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         r"""
         Preprocess to compensates for image normalization and splitting of the
         measurement operator.
 
         It computes :math:`\frac{x[0::2]-x[1::2]}{\alpha} - H1`
@@ -200,24 +215,24 @@
             meas_op: the number of measurements :attr:`meas_op.M` should match
             :math:`M`.
 
             Output: :math:`(*, M)`
 
         Example:
             >>> x = torch.rand([10,2*400], dtype=torch.float)
-            >>> H = np.random.random([400,32*32])
+            >>> H = torch.rand([400,32*32])
             >>> meas_op =  LinearSplit(H)
             >>> split_op = SplitPoisson(10, meas_op)
             >>> m = split_op(x)
             >>> print(m.shape)
             torch.Size([10, 400])
 
         Example 2:
             >>> x = torch.rand([10,2*400], dtype=torch.float)
-            >>> Perm = np.random.random([32,32])
+            >>> Perm = torch.rand([32,32])
             >>> meas_op = HadamSplit(400, 32,  Perm)
             >>> split_op = SplitPoisson(10, meas_op)
             >>> m = split_op(x)
             >>> print(m.shape)
             torch.Size([10, 400])
         """
         s = x.shape[:-1] + torch.Size([self.M])  # torch.Size([*,M])
@@ -263,15 +278,15 @@
 
             :math:`m`: :math:`(B, M)`
 
             :math:`\alpha`: :math:`(B)`
 
         Example:
             >>> x = torch.rand([10,2*400], dtype=torch.float)
-            >>> Perm = np.random.random([32,32])
+            >>> Perm = torch.rand([32,32])
             >>> meas_op = HadamSplit(400, 32,  Perm)
             >>> split_op = SplitPoisson(10, meas_op)
             >>> m, alpha = split_op.forward_expe(x, meas_op)
             >>> print(m.shape)
             >>> print(alpha.shape)
             torch.Size([10, 400])
             torch.Size([10])
@@ -392,15 +407,15 @@
             :attr:`meas_op`: An operator such that :attr:`meas_op.N` :math:`=N`
             and :attr:`meas_op.M` :math:`=M`
 
             Output: :math:`(*, M)`
 
         Example:
             >>> x = torch.rand([10,2*400], dtype=torch.float)
-            >>> Perm = np.random.random([32,32])
+            >>> Perm = torch.rand([32,32])
             >>> meas_op = HadamSplit(400, 32,  Perm)
             >>> split_op = SplitPoisson(10, meas_op)
             >>> v = split_op.sigma_from_image(x, meas_op)
             >>> print(v.shape)
             torch.Size([10, 400])
 
         """
@@ -444,75 +459,78 @@
         beta = beta.expand(bc, 1, h, w)
         x = (x + 1) / 2 * beta
 
         return x
 
 
 # ==============================================================================
-class SplitRowPoisson(nn.Module):
-    # ==============================================================================
-    r"""
-    Preprocess raw data acquired with a split measurement operator
-
-    It computes :math:`m = \frac{y_{+}-y_{-}}{\alpha}` and the variance
-    :math:`\sigma^2 = \frac{2(y_{+} + y_{-})}{\alpha^{2}}`, where
-    :math:`y_{+} = H_{+}x` and :math:`y_{-} = H_{-}x` are obtained using
-    a split measurement operator such as :class:`spyrit.core.LinearRowSplit`.
-
-    Args:
-        - :math:`\alpha` (float): maximun image intensity (in counts)
-        - :math:`M` (int): number of measurements
-        - :math:`h` (int): number of rows in the image, i.e., image height
-
-    Example:
-        >>> split_op = SplitRawPoisson(2.0, 24, 64)
-
-    """
-
-    def __init__(self, alpha: float, M: int, h: int):
-        super().__init__()
-        self.alpha = alpha
-        self.M = M
-        self.h = h
-
-        self.even_index = range(0, 2 * M, 2)
-        self.odd_index = range(1, 2 * M, 2)
-        # self.max = nn.MaxPool1d(h)
-
-    def forward(
-        self,
-        x: torch.tensor,
-        meas_op: LinearRowSplit,
-    ) -> torch.tensor:
-        """
-        Args:
-            x: batch of images that are Hadamard transformed across rows
-            meas_op: measurement operator
-
-        Shape:
-            x: :math:`(b*c, 2M, w)` with :math:`b` the batch size, :math:`c` the
-            number of channels, :math:`2M` is twice the number of patterns (as
-            it includes both positive and negative components), and :math:`w`
-            is the image width.
-
-            meas_op: The number of measurement `meas_op.M` should match `M`,
-            while the length of the measurements :math:`meas_op.N` should match
-            image height :math:`h`.
-
-            Output: :math:`(b*c,M)`
-
-        Example:
-            >>> x = torch.rand([10,48,64], dtype=torch.float)
-            >>> H_pos = np.random.random([24,64])
-            >>> H_neg = np.random.random([24,64])
-            >>> meas_op = LinearRowSplit(H_pos, H_neg)
-            >>> m = split_op(x, meas_op)
-            >>> print(m.shape)
-            torch.Size([10, 24, 64])
-
-        """
-        # unsplit
-        x = x[:, self.even_index] - x[:, self.odd_index]
-        # normalize
-        e = torch.ones([x.shape[0], meas_op.N, self.h], device=x.device)
-        x = 2 * x / self.alpha - meas_op.forward_H(e)
-        return x
+# class SplitRowPoisson(nn.Module):
+#     # ==============================================================================
+#     r"""
+#     Preprocess raw data acquired with a split measurement operator
+
+#     It computes :math:`m = \frac{y_{+}-y_{-}}{\alpha}` and the variance
+#     :math:`\sigma^2 = \frac{2(y_{+} + y_{-})}{\alpha^{2}}`, where
+#     :math:`y_{+} = H_{+}x` and :math:`y_{-} = H_{-}x` are obtained using
+#     a split measurement operator such as :class:`spyrit.core.LinearSplit`.
+
+#     Args:
+#         - :math:`\alpha` (float): maximun image intensity (in counts)
+#         - :math:`M` (int): number of measurements
+#         - :math:`h` (int): number of rows in the image, i.e., image height
+
+#     Example:
+#         >>> split_op = SplitRawPoisson(2.0, 24, 64)
+
+#     """
+
+#     def __init__(self, alpha: float, M: int, h: int):
+#         super().__init__()
+#         self.alpha = alpha
+#         self.M = M
+#         self.h = h
+
+#         self.even_index = range(0, 2 * M, 2)
+#         self.odd_index = range(1, 2 * M, 2)
+#         # self.max = nn.MaxPool1d(h)
+
+#     def forward(
+#         self,
+#         x: torch.tensor,
+#         meas_op: LinearSplit,
+#     ) -> torch.tensor:
+#         """
+#         Args:
+#             x: batch of images that are Hadamard transformed across rows
+#             meas_op: measurement operator
+
+#         Shape:
+#             x: :math:`(b*c, 2M, w)` with :math:`b` the batch size, :math:`c` the
+#             number of channels, :math:`2M` is twice the number of patterns (as
+#             it includes both positive and negative components), and :math:`w`
+#             is the image width.
+
+#             meas_op: The number of measurement `meas_op.M` should match `M`,
+#             while the length of the measurements :math:`meas_op.N` should match
+#             image height :math:`h`.
+
+#             Output: :math:`(b*c,M)`
+
+#         Example:
+#             >>> x = torch.rand([10,48,64], dtype=torch.float)
+#             >>> H_pos = torch.rand([24,64])
+#             >>> H_neg = torch.rand([24,64])
+#             >>> meas_op = LinearSplit(H_pos, H_neg)
+#             >>> m = split_op(x, meas_op)
+#             >>> print(m.shape)
+#             torch.Size([10, 24, 64])
+
+#         """
+#         # unsplit
+#         x = x[:, self.even_index] - x[:, self.odd_index]
+#         # normalize
+#         e = torch.ones([x.shape[0], meas_op.N, self.h], device=x.device)
+#         print("shape of e:", e.shape)
+#         print("shape of x:", x.shape)
+#         print("shape of fwd:", meas_op.forward_H(e).shape)
+#         x = 2 * x / self.alpha - meas_op.forward_H(e)
+#         return x
```

### Comparing `spyrit-2.2.0/spyrit/core/recon.py` & `spyrit-2.3.0/spyrit/core/recon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-# -*- coding: utf-8 -*-
 """
-Reconstruction methods
+Reconstruction methods and networks.
+"""
 
-Created on Fri Jan 20 11:03:12 2023
+import warnings
+from typing import Union
 
-@author: ducros
-"""
+import math
 import torch
+
+# import torchvision
 import torch.nn as nn
 import numpy as np
-from spyrit.core.meas import HadamSplit, LinearRowSplit, Linear
-import math
 
+from spyrit.core.meas import Linear, DynamicLinear, HadamSplit
+from spyrit.core.noise import NoNoise
+from spyrit.core.prep import DirectPoisson, SplitPoisson
+
+warnings.filterwarnings("ignore", ".*Sparse CSR tensor support is in beta state.*")
 
-# ==================================================================================
+
+# =============================================================================
 class PseudoInverse(nn.Module):
-    # ==================================================================================
-    r"""Moore-Penrose Pseudoinverse
+    # =========================================================================
+    r"""Moore-Penrose pseudoinverse.
 
     Considering linear measurements :math:`y = Hx`, where :math:`H` is the
     measurement matrix and :math:`x` is a vectorized image, it estimates
     :math:`x` from :math:`y` by computing :math:`\hat{x} = H^\dagger y`, where
     :math:`H` is the Moore-Penrose pseudo inverse of :math:`H`.
 
     Example:
-        >>> H = np.random.random([400,32*32])
-        >>> Perm = np.random.random([32*32,32*32])
+        >>> H = torch.rand([400,32*32])
+        >>> Perm = torch.rand([32*32,32*32])
         >>> meas_op =  HadamSplit(H, Perm, 32, 32)
         >>> y = torch.rand([85,400], dtype=torch.float)
         >>> pinv_op = PseudoInverse()
         >>> x = pinv_op(y, meas_op)
         >>> print(x.shape)
         torch.Size([85, 1024])
     """
 
     def __init__(self):
         super().__init__()
 
-    def forward(self, x: torch.tensor, meas_op) -> torch.tensor:
-        r"""Compute pseudo-inverse of measurements.
+    def forward(
+        self,
+        x: torch.tensor,
+        meas_op: Union[Linear, DynamicLinear],
+        **kwargs,
+    ) -> torch.tensor:
+        r"""Computes pseudo-inverse of measurements.
 
         Args:
             :attr:`x`: Batch of measurement vectors.
 
             :attr:`meas_op`: Measurement operator. Any class that
             implements a :meth:`pinv` method can be used, e.g.,
             :class:`~spyrit.core.forwop.HadamSplit`.
@@ -52,130 +63,127 @@
             :attr:`x`: :math:`(*, M)`
 
             :attr:`meas_op`: not applicable
 
             :attr:`output`: :math:`(*, N)`
 
         Example:
-            >>> H = np.random.random([400,32*32])
-            >>> Perm = np.random.random([32*32,32*32])
+            >>> H = torch.rand([400,32*32])
+            >>> Perm = torch.rand([32*32,32*32])
             >>> meas_op =  HadamSplit(H, Perm, 32, 32)
             >>> y = torch.rand([85,400], dtype=torch.float)
             >>> pinv_op = PseudoInverse()
             >>> x = pinv_op(y, meas_op)
             >>> print(x.shape)
             torch.Size([85, 1024])
         """
-        x = meas_op.pinv(x)
-        return x
+        return meas_op.pinv(x, **kwargs)
 
 
-# ===========================================================================================
+# =============================================================================
 class TikhonovMeasurementPriorDiag(nn.Module):
-    # ===========================================================================================
+    # =========================================================================
     r"""
-    Tikhonov regularization with prior in the measurement domain
+    Tikhonov regularisation with prior in the measurement domain.
 
-    Considering linear measurements :math:`y = Hx`, where :math:`H = GF` is the
-    measurement matrix and :math:`x` is a vectorized image, it estimates
-    :math:`x` from :math:`y` by approximately minimizing
+    Considering linear measurements :math:`m = Hx \in\mathbb{R}^M`, where :math:`H = GF` is the measurement matrix and :math:`x\in\mathbb{R}^N` is a vectorized image, it estimates :math:`x` from :math:`m` by approximately minimizing
 
     .. math::
-        \| y - GFx \|^2_{\Sigma^{-1}_\alpha} + \|F(x - x_0)\|^2_{\Sigma^{-1}}
+        \|m - GFx \|^2_{\Sigma^{-1}_\alpha} + \|F(x - x_0)\|^2_{\Sigma^{-1}}
 
-    where :math:`x_0` is a mean image prior, :math:`\Sigma` is a covariance
-    prior, and :math:`\Sigma_\alpha` is the measurement noise covariance.
+    where :math:`x_0\in\mathbb{R}^N` is a mean image prior, :math:`\Sigma\in\mathbb{R}^{N\times N}` is a covariance prior, and :math:`\Sigma_\alpha\in\mathbb{R}^{M\times M}` is the measurement noise covariance. The matrix :math:`G\in\mathbb{R}^{M\times N}` is a subsampling matrix.
 
-    The class is constructed from :math:`\Sigma`.
+    .. note::
+        The class is instantiated from :math:`\Sigma`, which represents the covariance of :math:`Fx`.
 
     Args:
-        - :attr:`sigma`:  covariance prior with shape :math:`(N, N)`
-        - :attr:`M`: number of measurements
+        - :attr:`sigma`:  covariance prior with shape :math:`N` x :math:`N`
+        - :attr:`M`: number of measurements :math:`M`
 
 
     Attributes:
         :attr:`comp`: The learnable completion layer initialized as
         :math:`\Sigma_1 \Sigma_{21}^{-1}`. This layer is a :class:`nn.Linear`
 
         :attr:`denoi`: The learnable denoising layer initialized from
         :math:`\Sigma_1`.
 
     Example:
-        >>> sigma = np.random.random([32*32, 32*32])
+        >>> sigma = torch.rand([32*32, 32*32])
         >>> recon_op = TikhonovMeasurementPriorDiag(sigma, 400)
     """
 
-    def __init__(self, sigma: np.array, M: int):
+    def __init__(self, sigma: torch.tensor, M: int):
         super().__init__()
 
         N = sigma.shape[0]
 
         self.comp = nn.Linear(M, N - M, False)
         self.denoi = Denoise_layer(M)
 
-        diag_index = np.diag_indices(N)
-        var_prior = sigma[diag_index]
-        var_prior = var_prior[:M]
+        var_prior = sigma.diag()[:M]
 
-        self.denoi.weight.data = torch.from_numpy(np.sqrt(var_prior))
+        self.denoi.weight.data = torch.sqrt(var_prior)
         self.denoi.weight.data = self.denoi.weight.data.float()
         self.denoi.weight.requires_grad = False
 
         Sigma1 = sigma[:M, :M]
         Sigma21 = sigma[M:, :M]
-        W = Sigma21 @ np.linalg.inv(Sigma1)
+        # W = Sigma21 @ torch.linalg.inv(Sigma1)
+        W = torch.linalg.solve(Sigma1.T, Sigma21.T).T
 
-        self.comp.weight.data = torch.from_numpy(W)
+        self.comp.weight.data = W
         self.comp.weight.data = self.comp.weight.data.float()
         self.comp.weight.requires_grad = False
 
     def forward(
         self, x: torch.tensor, x_0: torch.tensor, var: torch.tensor, meas_op: HadamSplit
     ) -> torch.tensor:
         r"""
+        Computes the Tikhonov regularization with prior in the measurement domain.
 
-        We approximate the solution as
+        We approximate the solution as:
 
         .. math::
-            \hat{x} = x_0 + F^{-1} \begin{bmatrix} y_1 \\ y_2\end{bmatrix}
+            \hat{x} = x_0 + F^{-1} \begin{bmatrix} m_1 \\ m_2\end{bmatrix}
 
-        with :math:`y_1 = D_1(D_1 + \Sigma_\alpha)^{-1} (y - GF x_0)` and
-        :math:`y_2 = \Sigma_1 \Sigma_{21}^{-1} y_1`, where
+        with :math:`m_1 = D_1(D_1 + \Sigma_\alpha)^{-1} (m - GF x_0)` and
+        :math:`m_2 = \Sigma_1 \Sigma_{21}^{-1} m_1`, where
         :math:`\Sigma = \begin{bmatrix} \Sigma_1 & \Sigma_{21}^\top \\ \Sigma_{21} & \Sigma_2\end{bmatrix}`
         and  :math:`D_1 =\textrm{Diag}(\Sigma_1)`. Assuming the noise
         covariance :math:`\Sigma_\alpha` is diagonal, the matrix inversion
-        involded in the computation of :math:`y_1` is straigtforward.
+        involved in the computation of :math:`m_1` is straightforward.
 
         This is an approximation to the exact solution
 
         .. math::
             \hat{x} &= x_0 + F^{-1}\begin{bmatrix}\Sigma_1 \\ \Sigma_{21} \end{bmatrix}
-                      [\Sigma_1 + \Sigma_\alpha]^{-1} (y - GF x_0)
+                      [\Sigma_1 + \Sigma_\alpha]^{-1} (m - GF x_0)
 
 
         See Lemma B.0.5 of the PhD dissertation of A. Lorente Mur (2021):
         https://theses.hal.science/tel-03670825v1/file/these.pdf
 
         Args:
-            - :attr:`x`: A batch of measurement vectors :math:`y`
+            - :attr:`x`: A batch of measurement vectors :math:`m`
             - :attr:`x_0`: A batch of prior images :math:`x_0`
             - :attr:`var`: A batch of measurement noise variances :math:`\Sigma_\alpha`
             - :attr:`meas_op`: A measurement operator that provides :math:`GF` and :math:`F^{-1}`
 
         Shape:
             - :attr:`x`: :math:`(*, M)`
             - :attr:`x_0`: :math:`(*, N)`
             - :attr:`var` :math:`(*, M)`
             - Output: :math:`(*, N)`
 
         Example:
             >>> B, H, M = 85, 32, 512
-            >>> sigma = np.random.random([H**2, H**2])
+            >>> sigma = torch.rand([H**2, H**2])
             >>> recon_op = TikhonovMeasurementPriorDiag(sigma, M)
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >> meas = HadamSplit(M, H, Ord)
             >>> y = torch.rand([B,M], dtype=torch.float)
             >>> x_0 = torch.zeros((B, H**2), dtype=torch.float)
             >>> var = torch.zeros((B, M), dtype=torch.float)
             >>> x = recon_op(y, x_0, var, meas)
             torch.Size([85, 1024])
         """
@@ -184,123 +192,161 @@
         y2 = self.comp(y1)
 
         y = torch.cat((y1, y2), -1)
         x = x_0 + meas_op.inverse(y)
         return x
 
 
-# ===========================================================================================
+# =============================================================================
 class Denoise_layer(nn.Module):
-    # ===========================================================================================
-    r"""Wiener filter that assumes additive white Gaussian noise
+    # =========================================================================
+    r"""Wiener filter that assumes additive white Gaussian noise.
 
     .. math::
         y = \sigma_\text{prior}^2/(\sigma^2_\text{prior} + \sigma^2_\text{meas}) x,
-    where :math:`\sigma^2_\text{prior}` is the variance prior and
-    :math:`\sigma^2_\text{meas}` is the variance of the measurement,
-    x is the input vector and y is the output vector.
+        where :math:`\sigma^2_\text{prior}` is the variance prior and
+        :math:`\sigma^2_\text{meas}` is the variance of the measurement,
+        x is the input vector and y is the output vector.
 
     Args:
-        :attr:`M`: size of incoming vector
+        :attr:`M` (int): size of incoming vector
 
     Shape:
         - Input: :math:`(*, M)`.
         - Output: :math:`(*, M)`.
 
     Attributes:
-        :attr:`sigma`:
-            the learnable standard deviation prior
-            :math:`\sigma_\text{prior}` of shape :math:`(M, 1)`. The
-            values are initialized from
-            :math:`\mathcal{U}(-\sqrt{k}, \sqrt{k})`, where
-            :math:`k = 1/M`.
+        :attr:`weight`:
+        The learnable standard deviation prior :math:`\sigma_\text{prior}` of
+        shape :math:`(M, 1)`. The values are initialized from
+        :math:`\mathcal{U}(-\sqrt{k}, \sqrt{k})`, where :math:`k = 1/M`.
+
+        :attr:`in_features`:
+        The number of input features equal to :math:`M`.
 
     Example:
         >>> m = Denoise_layer(30)
         >>> input = torch.randn(128, 30)
         >>> output = m(input)
         >>> print(output.size())
         torch.Size([128, 30])
     """
 
-    def __init__(self, M):
+    def __init__(self, M: int):
         super(Denoise_layer, self).__init__()
         self.in_features = M
         self.weight = nn.Parameter(torch.Tensor(M))
         self.reset_parameters()
 
     def reset_parameters(self):
+        r"""
+        Resets the standard deviation prior :math:`\sigma_\text{prior}`.
+
+        The values are initialized from :math:`\mathcal{U}(-\sqrt{k}, \sqrt{k})`,
+        where :math:`k = 1/M`. They are stored in the :attr:`weight` attribute.
+        """
         nn.init.uniform_(self.weight, 0, 2 / math.sqrt(self.in_features))
 
-    def forward(self, inputs):
+    def forward(self, inputs: torch.tensor) -> torch.tensor:
+        r"""
+        Applies a transformation to the incoming data: :math:`y = A^2/(A^2+x)`.
+
+        :math:`x` is the input tensor (see :attr:`inputs`) and :math:`A` is the
+        standard deviation prior (see :attr:`self.weight`).
+
+        Args:
+            :attr:`inputs` (torch.tensor): input tensor :math:`x` of shape
+            :math:`(N, *, in\_features)`
+
+        Returns:
+            torch.tensor: The transformed data :math:`y` of shape
+            :math:`(N, in\_features)`
+
+        Shape:
+
+        """
         return self.tikho(inputs, self.weight)
 
     def extra_repr(self):
         return "in_features={}".format(self.in_features)
 
     @staticmethod
-    def tikho(inputs, weight):
+    def tikho(inputs: torch.tensor, weight: torch.tensor) -> torch.tensor:
         # type: (torch.Tensor, torch.Tensor) -> torch.Tensor
         r"""
         Applies a transformation to the incoming data: :math:`y = A^2/(A^2+x)`.
 
+        :math:`x` is the input tensor (see :attr:`inputs`) and :math:`A` is the
+        standard deviation prior (see :attr:`weight`).
+
+        Args:
+            :attr:`inputs` (torch.tensor): input tensor :math:`x` of shape
+            :math:`(N, *, in\_features)`
+
+            :attr:`weight` (torch.tensor): standard deviation prior :math:`A` of
+            shape :math:`(in\_features)`
+
+        Returns:
+            torch.tensor: The transformed data :math:`y` of shape
+            :math:`(N, in\_features)`
+
         Shape:
-            - Input: :math:`(N, *, in\_features)` where `*` means any number of
+            - :attr:`inputs`: :math:`(N, *, in\_features)` where `*` means any number of
               additional dimensions - Variance of measurements
-            - Weight: :math:`(in\_features)` - corresponds to the standard deviation
+            - :attr:`weight`: :math:`(in\_features)` - corresponds to the standard deviation
               of our prior.
-            - Output: :math:`(N, in\_features)`
+            - :attr:`output`: :math:`(N, in\_features)`
         """
-        var = weight**2  # prefer to square it, because when leant, it can got to the
+        a = weight**2  # prefer to square it, because when learnt, it can go to the
         # negative, which we do not want to happen.
         # TO BE Potentially done : square inputs.
-        den = var + inputs
-        ret = var / den
-        return ret
+        b = a + inputs
+        return a / b
+
+
+# -----------------------------------------------------------------------------
+# |                      RECONSTRUCTION NETWORKS                              |
+# -----------------------------------------------------------------------------
 
 
-#  %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
-#  RECONSTRUCTION NETWORKS
-#  %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # =============================================================================
 class PinvNet(nn.Module):
-    # =============================================================================
+    # =========================================================================
     r"""Pseudo inverse reconstruction network
 
-    .. math:
-
-
     Args:
         :attr:`noise`: Acquisition operator (see :class:`~spyrit.core.noise`)
 
         :attr:`prep`: Preprocessing operator (see :class:`~spyrit.core.prep`)
 
         :attr:`denoi` (optional): Image denoising operator
         (see :class:`~spyrit.core.nnet`).
         Default :class:`~spyrit.core.nnet.Identity`
 
     Input / Output:
         :attr:`input`: Ground-truth images with shape :math:`(B,C,H,W)`
+        corresponding to the batch size, number of channels, height, and width.
 
         :attr:`output`: Reconstructed images with shape :math:`(B,C,H,W)`
+        corresponding to the batch size, number of channels, height, and width.
 
     Attributes:
         :attr:`Acq`: Acquisition operator initialized as :attr:`noise`
 
         :attr:`prep`: Preprocessing operator initialized as :attr:`prep`
 
         :attr:`pinv`: Analytical reconstruction operator initialized as
         :class:`~spyrit.core.recon.PseudoInverse()`
 
         :attr:`Denoi`: Image denoising operator initialized as :attr:`denoi`
 
 
     Example:
         >>> B, C, H, M = 10, 1, 64, 64**2
-        >>> Ord = np.ones((H,H))
+        >>> Ord = torch.ones((H,H))
         >>> meas = HadamSplit(M, H, Ord)
         >>> noise = NoNoise(meas)
         >>> prep = SplitPoisson(1.0, M, H*H)
         >>> recnet = PinvNet(noise, prep)
         >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
         >>> z = recnet(x)
         >>> print(z.shape)
@@ -325,155 +371,134 @@
         Shape:
             :attr:`x`: ground-truth images with shape :math:`(B,C,H,W)`
 
             :attr:`output`: reconstructed images with shape :math:`(B,C,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
             >>> recnet = PinvNet(noise, prep)
             >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
             >>> z = recnet(x)
             >>> print(z.shape)
             >>> print(torch.linalg.norm(x - z)/torch.linalg.norm(x))
             torch.Size([10, 1, 64, 64])
             tensor(5.8912e-06)
         """
-
         b, c, _, _ = x.shape
 
         # Acquisition
         x = x.view(b * c, self.acqu.meas_op.N)  # shape x = [b*c,h*w] = [b*c,N]
         x = self.acqu(x)  # shape x = [b*c, 2*M]
 
         # Reconstruction
         x = self.reconstruct(x)  # shape x = [bc, 1, h,w]
-        x = x.view(b, c, self.acqu.meas_op.h, self.acqu.meas_op.w)
-
-        return x
+        return x.view(b, c, self.acqu.meas_op.h, self.acqu.meas_op.w)
 
     def acquire(self, x):
-        r"""Simulate data acquisition
+        r"""Simulates data acquisition
 
         Args:
             :attr:`x`: ground-truth images
 
         Shape:
             :attr:`x`: ground-truth images with shape :math:`(B,C,H,W)`
 
             :attr:`output`: measurement vectors with shape :math:`(BC,2M)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
             >>> recnet = PinvNet(noise, prep)
             >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
             >>> z = recnet.acquire(x)
             >>> print(z.shape)
             torch.Size([10, 8192])
         """
-
         b, c, _, _ = x.shape
-
         # Acquisition
         x = x.view(b * c, self.acqu.meas_op.N)  # shape x = [b*c,h*w] = [b*c,N]
-        x = self.acqu(x)  # shape x = [b*c, 2*M]
-
-        return x
+        return self.acqu(x)  # shape x = [b*c, 2*M]
 
     def meas2img(self, y):
-        """Return images from raw measurement vectors
+        """Returns images from raw measurement vectors
 
         Args:
             :attr:`x`: raw measurement vectors
 
         Shape:
             :attr:`x`: :math:`(BC,2M)`
 
             :attr:`output`: :math:`(BC,1,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H**2)
             >>> recnet = PinvNet(noise, prep)
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct(x)
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
         m = self.prep(y)
         m = torch.nn.functional.pad(m, (0, self.acqu.meas_op.N - self.acqu.meas_op.M))
-        z = m @ self.acqu.meas_op.Perm.weight.data.T
-        z = z.view(-1, 1, self.acqu.meas_op.h, self.acqu.meas_op.w)
-
-        return z
+        # z = m @ self.acqu.meas_op.get_Perm().T  # old way
+        # new way, tested and working :
+        z = self.acqu.meas_op.reindex(m, "cols", False)
+        return z.view(-1, 1, self.acqu.meas_op.h, self.acqu.meas_op.w)
 
     def reconstruct(self, x):
-        r"""Reconstruction step of a reconstruction network
+        r"""Preprocesses, reconstructs, and denoises raw measurement vectors.
 
         Args:
             :attr:`x`: raw measurement vectors
 
         Shape:
             :attr:`x`: :math:`(BC,2M)`
 
             :attr:`output`: :math:`(BC,1,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H**2)
             >>> recnet = PinvNet(noise, prep)
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct(x)
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
-        # Measurement to image domain mapping
-        bc, _ = x.shape
-
-        # Preprocessing in the measurement domain
-        x = self.prep(x)  # shape x = [b*c, M]
-
-        # measurements to image-domain processing
-        x = self.pinv(x, self.acqu.meas_op)  # shape x = [b*c,N]
-
-        # Image-domain denoising
-        x = x.view(
-            bc, 1, self.acqu.meas_op.h, self.acqu.meas_op.w
-        )  # shape x = [b*c,1,h,w]
-        x = self.denoi(x)
-
-        return x
+        # Denoise image-domain
+        return self.denoi(self.reconstruct_pinv(x))
 
     def reconstruct_pinv(self, x):
-        r"""Reconstruction step of a reconstruction network
+        r"""Preprocesses and reconstructs raw measurement vectors.
 
         Args:
             :attr:`x`: raw measurement vectors
 
         Shape:
             :attr:`x`: :math:`(BC,2M)`
 
             :attr:`output`: :math:`(BC,1,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H**2)
             >>> recnet = PinvNet(noise, prep)
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct_pinv(x)
             >>> print(z.shape)
@@ -488,15 +513,14 @@
         # measurements to image-domain processing
         x = self.pinv(x, self.acqu.meas_op)  # shape x = [b*c,N]
 
         # Image-domain denoising
         x = x.view(
             bc, 1, self.acqu.meas_op.h, self.acqu.meas_op.w
         )  # shape x = [b*c,1,h,w]
-
         return x
 
     def reconstruct_expe(self, x):
         r"""Reconstruction step of a reconstruction network
 
         Same as :meth:`reconstruct` reconstruct except that:
 
@@ -507,15 +531,14 @@
         Args:
             :attr:`x`: raw measurement vectors
 
         Shape:
             :attr:`x`: :math:`(BC,2M)`
 
             :attr:`output`: :math:`(BC,1,H,W)`
-
         """
         # x of shape [b*c, 2M]
         bc, _ = x.shape
 
         # Preprocessing
         x, N0_est = self.prep.forward_expe(x, self.acqu.meas_op)  # shape x = [b*c, M]
         print(N0_est)
@@ -533,29 +556,35 @@
         # Denormalization
         x = self.prep.denormalize_expe(
             x, N0_est, self.acqu.meas_op.h, self.acqu.meas_op.w
         )
         return x
 
 
-# %%===========================================================================================
+# =============================================================================
 class DCNet(nn.Module):
-    # ===========================================================================================
-    r"""Denoised completion reconstruction network
+    # =========================================================================
+    r"""Denoised completion reconstruction network.
 
-    .. math:
+    This is a four step reconstruction method:
+
+    #. Denoising in the measurement domain.
+    #. Estimation of the missing measurements from the denoised ones.
+    #. Image-domain mapping.
+    #. (Learned) Denoising in the image domain.
 
+    The first three steps corresponds to Tikhonov regularisation. Typically, only the last step involves learnable parameters.
 
     Args:
         :attr:`noise`: Acquisition operator (see :class:`~spyrit.core.noise`)
 
         :attr:`prep`: Preprocessing operator (see :class:`~spyrit.core.prep`)
 
-        :attr:`sigma`: UPDATE!! Tikhonov reconstruction operator of type
-        :class:`~spyrit.core.recon.TikhonovMeasurementPriorDiag()`
+        :attr:`sigma`: Covariance prior (for details, see the
+        :class:`~spyrit.core.recon.TikhonovMeasurementPriorDiag()` class)
 
         :attr:`denoi` (optional): Image denoising operator
         (see :class:`~spyrit.core.nnet`).
         Default :class:`~spyrit.core.nnet.Identity`
 
     Input / Output:
         :attr:`input`: Ground-truth images with shape :math:`(B,C,H,W)`
@@ -570,53 +599,73 @@
         :attr:`DC_Layer`: Data consistency layer initialized as :attr:`tikho`
 
         :attr:`Denoi`: Image denoising operator initialized as :attr:`denoi`
 
 
     Example:
         >>> B, C, H, M = 10, 1, 64, 64**2
-        >>> Ord = np.ones((H,H))
+        >>> Ord = torch.ones((H,H))
         >>> meas = HadamSplit(M, H, Ord)
         >>> noise = NoNoise(meas)
         >>> prep = SplitPoisson(1.0, M, H*H)
-        >>> sigma = np.random.random([H**2, H**2])
+        >>> sigma = torch.rand([H**2, H**2])
         >>> recnet = DCNet(noise,prep,sigma)
         >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
         >>> z = recnet(x)
         >>> print(z.shape)
         torch.Size([10, 1, 64, 64])
     """
 
-    def __init__(self, noise, prep, sigma, denoi=nn.Identity()):
+    def __init__(
+        self,
+        noise: NoNoise,
+        prep: Union[DirectPoisson, SplitPoisson],
+        sigma: torch.tensor,
+        denoi=nn.Identity(),
+    ):
         super().__init__()
         self.Acq = noise
         self.prep = prep
-        Perm = noise.meas_op.Perm.weight.data.cpu().numpy().T
-        sigma_perm = Perm @ sigma @ Perm.T
-        self.tikho = TikhonovMeasurementPriorDiag(sigma_perm, noise.meas_op.M)
         self.denoi = denoi
+        sigma = sigma.to(torch.float32)
+
+        # old way
+        # Perm = noise.meas_op.get_Perm().cpu().T #.numpy()
+        # sigma = Perm @ sigma @ Perm.T
+
+        # new way
+        # Ord = noise.meas_op.Ord
+        # Perm = torch.from_numpy(samp.Permutation_Matrix(noise.meas_op.Ord)).to(torch.float32)
+        # sigma = samp.sort_by_significance(sigma, Ord, 'rows', True)
+        # sigma = samp.sort_by_significance(sigma, Ord, 'cols', False)
+        sigma = noise.reindex(sigma, "rows", False)
+        sigma = noise.reindex(sigma, "cols", True)
+        sigma_perm = sigma
+
+        # save in tikho
+        self.tikho = TikhonovMeasurementPriorDiag(sigma_perm, noise.meas_op.M)
 
     def forward(self, x):
         r"""Full pipeline of the reconstruction network
 
         Args:
             :attr:`x`: ground-truth images
 
         Shape:
             :attr:`x`: ground-truth images with shape :math:`(B,C,H,W)`
 
             :attr:`output`: reconstructed images with shape :math:`(B,C,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
-            >>> sigma = np.random.random([H**2, H**2])
+            >>> sigma = torch.rand([H**2, H**2])
             >>> recnet = DCNet(noise,prep,sigma)
             >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
             >>> z = recnet(x)
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
 
@@ -641,19 +690,19 @@
         Shape:
             :attr:`x`: ground-truth images with shape :math:`(B,C,H,W)`
 
             :attr:`output`: measurement vectors with shape :math:`(BC,2M)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
-            >>> sigma = np.random.random([H**2, H**2])
+            >>> sigma = torch.rand([H**2, H**2])
             >>> recnet = DCNet(noise,prep,sigma)
             >>> x = torch.FloatTensor(B,C,H,H).uniform_(-1, 1)
             >>> z = recnet.acquire(x)
             >>> print(z.shape)
             torch.Size([10, 8192])
         """
 
@@ -674,19 +723,19 @@
         Shape:
             :attr:`x`: raw measurement vectors with shape :math:`(BC,2M)`
 
             :attr:`output`: reconstructed images with shape :math:`(BC,1,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
-            >>> sigma = np.random.random([H**2, H**2])
+            >>> sigma = torch.rand([H**2, H**2])
             >>> recnet = DCNet(noise,prep,sigma)
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct(x)
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
         # x of shape [b*c, 2M]
@@ -755,17 +804,17 @@
 
         # Denormalization
         x = self.prep.denormalize_expe(x, norm, self.Acq.meas_op.h, self.Acq.meas_op.w)
 
         return x
 
 
-# %%===========================================================================================
+# =============================================================================
 class DCDRUNet(DCNet):
-    # ===========================================================================================
+    # =========================================================================
     r"""Denoised completion reconstruction network based on DRUNet wich concatenates a
         noise level map to the input
 
     .. math:
 
 
     Args:
@@ -798,19 +847,19 @@
 
         :attr:`Denoi`: Image (DRUNet architecture type) denoising operator
         initialized as :attr:`denoi`
 
 
     Example:
         >>> B, C, H, M = 10, 1, 64, 64**2
-        >>> Ord = np.ones((H,H))
+        >>> Ord = torch.ones((H,H))
         >>> meas = HadamSplit(M, H, Ord)
         >>> noise = NoNoise(meas)
         >>> prep = SplitPoisson(1.0, M, H*H)
-        >>> sigma = np.random.random([H**2, H**2])
+        >>> sigma = torch.rand([H**2, H**2])
         >>> n_channels = 1                   # 1 for grayscale image
         >>> model_drunet_path = './spyrit/drunet/model_zoo/drunet_gray.pth'
         >>> denoi_drunet = drunet(in_nc=n_channels+1, out_nc=n_channels, nc=[64, 128, 256, 512], nb=4, act_mode='R',
             downsample_mode="strideconv", upsample_mode="convtranspose")
         >>> recnet = DCDRUNet(noise,prep,sigma,denoi_drunet)
         >>> z = recnet(x)
         >>> print(z.shape)
@@ -830,19 +879,19 @@
         Shape:
             :attr:`x`: raw measurement vectors with shape :math:`(BC,2M)`
 
             :attr:`output`: reconstructed images with shape :math:`(BC,1,H,W)`
 
         Example:
             >>> B, C, H, M = 10, 1, 64, 64**2
-            >>> Ord = np.ones((H,H))
+            >>> Ord = torch.ones((H,H))
             >>> meas = HadamSplit(M, H, Ord)
             >>> noise = NoNoise(meas)
             >>> prep = SplitPoisson(1.0, M, H*H)
-            >>> sigma = np.random.random([H**2, H**2])
+            >>> sigma = torch.rand([H**2, H**2])
             >>> n_channels = 1                   # 1 for grayscale image
             >>> model_drunet_path = './spyrit/drunet/model_zoo/drunet_gray.pth'
             >>> denoi_drunet = drunet(in_nc=n_channels+1, out_nc=n_channels, nc=[64, 128, 256, 512], nb=4, act_mode='R',
                 downsample_mode="strideconv", upsample_mode="convtranspose")
             >>> recnet = DCDRUNet(noise,prep,sigma,denoi_drunet)
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct(x)
@@ -897,42 +946,42 @@
             :attr:`noise_level`: float value noise level :math:`(1)`
 
             :attr:`output`: noise level tensor with shape :math:`(1)`
         """
         self.noise_level = torch.FloatTensor([noise_level / 255.0])
 
 
-# %%===========================================================================================
+# =============================================================================
 class PositiveParameters(nn.Module):
-    # ===========================================================================================
+    # ==========================================================================
     def __init__(self, size, val_min=1e-6):
         super(PositiveParameters, self).__init__()
         self.val_min = torch.tensor(val_min)
         self.params = nn.Parameter(
             torch.abs(val_min * torch.ones(size, 1)), requires_grad=True
         )
 
     def forward(self):
         return torch.abs(self.params)
 
 
-# %%===========================================================================================
+# =============================================================================
 class PositiveMonoIncreaseParameters(PositiveParameters):
-    # ===========================================================================================
+    # =========================================================================
     def __init__(self, size, val_min=0.000001):
         super().__init__(size, val_min)
 
     def forward(self):
         # cumsum in opposite order
         return super().forward().cumsum(dim=0).flip(dims=[0])
 
 
-# %%===========================================================================================
+# =============================================================================
 class UPGD(PinvNet):
-    # ===========================================================================================
+    # =========================================================================
     def __init__(
         self,
         noise,
         prep,
         denoi=nn.Identity(),
         num_iter=6,
         lamb=1e-5,
```

### Comparing `spyrit-2.2.0/spyrit/core/train.py` & `spyrit-2.3.0/spyrit/core/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # -----------------------------------------------------------------------------
 #   This software is distributed under the terms
 #   of the GNU Lesser General  Public Licence (LGPL)
 #   See LICENSE.md for further details
 # -----------------------------------------------------------------------------
+
+"""
+Training functions for deep learning models.
+"""
+
 from __future__ import print_function, division
 import sys
-import torch
-import torch.nn as nn
-import torch.optim as optim
-import numpy as np
-import torchvision
-from torchvision import datasets, models, transforms
-from torch.utils.tensorboard import SummaryWriter
-
 import os
-import matplotlib.pyplot as plt
 import time
-from pathlib import Path
 import datetime
 import copy
 import pickle
-import statistics
 from collections import OrderedDict
 import re
 
+# from pathlib import Path
+# import statistics
+
+import torch
+import torch.nn as nn
+import numpy as np
+import torchvision
+import matplotlib.pyplot as plt
+
+# import torch.optim as optim
+# from torchvision import datasets, models, transforms
+
+
 ######################################################################
 # 1. Visualize a few images from the training set
 # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 # Let's visualize a few training images so as to understand the data
 # augmentations.
 
 
@@ -73,14 +80,16 @@
 
 def images_norm(images):
     return 0.5 * (images + 1)
 
 
 def tb_writer_init(tb_path, samples=None):
     """Tensorboard log for torch"""
+    from torch.utils.tensorboard import SummaryWriter
+
     writer = SummaryWriter(tb_path)
 
     # Add model graph for visualization
     # with torch.no_grad():
     #    writer.add_graph(model, samples)
 
     # Add sample image
@@ -795,14 +804,17 @@
     print(model_out_path)
     torch.save(model.state_dict(), model_out_path)
     print("Model Saved")
 
 
 def load_net(title, model, device=None, strict=True):
     """Loads net defined by title"""
+    # if title.endswith(".pth"):
+    #     model_out_path = "{}".format(title)
+    # else:
     model_out_path = "{}.pth".format(title)
     try:
         if device is None:
             model.load_state_dict(torch.load(model_out_path), strict=strict)
         else:
             model.load_state_dict(
                 torch.load(model_out_path, map_location=torch.device(device)),
```

### Comparing `spyrit-2.2.0/spyrit/external/drunet.py` & `spyrit-2.3.0/spyrit/external/drunet.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,29 +38,29 @@
             )
 
         self.m_down1 = sequential(
             *[
                 ResBlock(nc[0], nc[0], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
             ],
-            downsample_block(nc[0], nc[1], bias=False, mode="2")
+            downsample_block(nc[0], nc[1], bias=False, mode="2"),
         )
         self.m_down2 = sequential(
             *[
                 ResBlock(nc[1], nc[1], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
             ],
-            downsample_block(nc[1], nc[2], bias=False, mode="2")
+            downsample_block(nc[1], nc[2], bias=False, mode="2"),
         )
         self.m_down3 = sequential(
             *[
                 ResBlock(nc[2], nc[2], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
             ],
-            downsample_block(nc[2], nc[3], bias=False, mode="2")
+            downsample_block(nc[2], nc[3], bias=False, mode="2"),
         )
 
         self.m_body = sequential(
             *[
                 ResBlock(nc[3], nc[3], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
             ]
@@ -79,29 +79,29 @@
             )
 
         self.m_up3 = sequential(
             upsample_block(nc[3], nc[2], bias=False, mode="2"),
             *[
                 ResBlock(nc[2], nc[2], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
-            ]
+            ],
         )
         self.m_up2 = sequential(
             upsample_block(nc[2], nc[1], bias=False, mode="2"),
             *[
                 ResBlock(nc[1], nc[1], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
-            ]
+            ],
         )
         self.m_up1 = sequential(
             upsample_block(nc[1], nc[0], bias=False, mode="2"),
             *[
                 ResBlock(nc[0], nc[0], bias=False, mode="C" + act_mode + "C")
                 for _ in range(nb)
-            ]
+            ],
         )
 
         self.m_tail = conv(nc[0], out_nc, bias=False, mode="C")
 
     def forward(self, x0):
         x1 = self.m_head(x0)
         x2 = self.m_down1(x1)
@@ -112,14 +112,71 @@
         x = self.m_up2(x + x3)
         x = self.m_up1(x + x2)
         x = self.m_tail(x + x1)
 
         return x
 
 
+class DRUNet(UNetRes):
+    def __init__(
+        self,
+        noise_level=5,
+        n_channels=1,
+        nc=[64, 128, 256, 512],
+        nb=4,
+        act_mode="R",
+        downsample_mode="strideconv",
+        upsample_mode="convtranspose",
+    ):
+        super(DRUNet, self).__init__(
+            n_channels + 1, n_channels, nc, nb, act_mode, downsample_mode, upsample_mode
+        )
+        self.register_buffer("noise_level", torch.FloatTensor([noise_level / 255.0]))
+
+    def forward(self, x):
+        # Image domain denoising
+        x = self.concat_noise_map(x)
+
+        # Pass input images through the network
+        x = super(DRUNet, self).forward(x)
+        return x
+
+    def concat_noise_map(self, x):
+        r"""Concatenation of noise level map to reconstructed images
+
+        Args:
+            :attr:`x`: reconstructed images from the reconstruction layer
+
+        Shape:
+            :attr:`x`: reconstructed images with shape :math:`(BC,1,H,W)`
+
+            :attr:`output`: reconstructed images with concatenated noise level map with shape :math:`(BC,2,H,W)`
+        """
+
+        b, c, h, w = x.shape
+        x = 0.5 * (x + 1)
+        x = torch.cat((x, self.noise_level.expand(b, 1, h, w)), dim=1)
+        return x
+
+    def set_noise_level(self, noise_level):
+        r"""Reset noise level value
+
+        Args:
+            :attr:`noise_level`: noise level value in the range [0, 255]
+
+        Shape:
+            :attr:`noise_level`: float value noise level :math:`(1)`
+
+            :attr:`output`: noise level tensor with shape :math:`(1)`
+        """
+        self.noise_level = torch.FloatTensor([noise_level / 255.0]).to(
+            self.noise_level.device
+        )
+
+
 # ----------------------------------------------
 # Functions taken from basicblock.py
 # https://github.com/cszn/DPIR/tree/master/models
 # ----------------------------------------------
 
 
 # --------------------------------------------
```

### Comparing `spyrit-2.2.0/spyrit/misc/data_visualisation.py` & `spyrit-2.3.0/spyrit/misc/data_visualisation.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.2.0/spyrit/misc/disp.py` & `spyrit-2.3.0/spyrit/misc/disp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 from PIL import Image
 import numpy as np
 from numpy import linalg as LA
 import time
 from scipy import signal
 from scipy import misc
 from scipy import sparse
-from imutils.video import FPS
-import imutils
-import cv2
 import torch
+import math
 
 
 def display_vid(video, fps, title="", colormap=plt.cm.gray):
     """
     video is a numpy array of shape [nb_frames, 1, nx, ny]
     """
     plt.ion()
@@ -173,14 +171,15 @@
             ax, width="100%", height="5%", loc="lower center", borderpad=-5
         )
         plt.colorbar(cax=cax, orientation="horizontal")
     else:
         cax = plt.axes([0.85, 0.1, 0.075, 0.8])
         plt.colorbar(cax=cax, orientation="vertical")
 
+    # fig.tight_layout() # it raises warnings in some cases
     if show is True:
         plt.show()
 
 
 def imagecomp(
     Img1,
     Img2,
@@ -301,14 +300,18 @@
 
 def histogram(s):
     count, bins, ignored = plt.hist(s, 30, density=True)
     plt.show()
 
 
 def vid2batch(root, img_dim, start_frame, end_frame):
+    from imutils.video import FPS
+    import imutils
+    import cv2
+
     stream = cv2.VideoCapture(root)
     fps = FPS().start()
     frame_nb = 0
     output_batch = torch.zeros(1, end_frame - start_frame, 1, img_dim, img_dim)
     while True:
         (grabbed, frame) = stream.read()
         if not grabbed:
@@ -322,14 +325,16 @@
                 frame[:, :, 1]
             )
 
     return output_batch
 
 
 def pre_process_video(video, crop_patch, kernel_size):
+    import cv2
+
     batch_size, seq_length, c, h, w = video.shape
     batched_frames = video.view(batch_size * seq_length * c, h, w)
     output_batch = torch.zeros(batched_frames.shape)
 
     for i in range(batch_size * seq_length * c):
         img = torch2numpy(batched_frames[i, :, :])
         img[crop_patch] = 0
```

### Comparing `spyrit-2.2.0/spyrit/misc/examples.py` & `spyrit-2.3.0/spyrit/misc/examples.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.2.0/spyrit/misc/load_data.py` & `spyrit-2.3.0/spyrit/misc/load_data.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.2.0/spyrit/misc/metrics.py` & `spyrit-2.3.0/spyrit/misc/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import torch.optim as optim
 from torch.optim import lr_scheduler
 import numpy as np
 import torchvision
 from torchvision import datasets, models, transforms
 import torch.nn.functional as F
 import imageio
-import cv2
 import matplotlib.pyplot as plt
 
 
 def batch_psnr(torch_batch, output_batch):
     list_psnr = []
     for i in range(torch_batch.shape[0]):
         img = torch_batch[i, 0, :, :]
```

### Comparing `spyrit-2.2.0/spyrit/misc/pattern_choice.py` & `spyrit-2.3.0/spyrit/misc/pattern_choice.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # -----------------------------------------------------------------------------
 
 from __future__ import print_function, division
 import torch
 import torch.nn as nn
 import torch.optim as optim
 import numpy as np
+from PIL import Image
 import torchvision
 from torchvision import datasets, models, transforms
 import matplotlib.pyplot as plt
 import time
 import os
 import copy
 from abc import ABC, abstractmethod
@@ -59,15 +60,16 @@
     def save_measurement_matrix(self, root):
         K = self.P.bias.shape[0]
         np.save(root + "T.npy", self.T)
         for i in range(K):
             pat = self.P.weight[i, 0, :, :]
             pattern = pat.cpu().detach().numpy()
 
-            cv2.imwrite(root + "pat_{}x{}".format(i) + ".png", pattern)
+            im = Image.fromarray(pattern)
+            im.save(root + "pat_{}x{}".format(i) + ".png")
 
     @abstractmethod
     def set_desired_pattern(self, def_matrix):
         pass
 
     @abstractmethod
     def add_desired_patterns(self, def_matrix):
```

### Comparing `spyrit-2.2.0/spyrit/misc/statistics.py` & `spyrit-2.3.0/spyrit/misc/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # from torchvision import datasets, transforms
 from pathlib import Path
 
 # from spyrit.learning.model_Had_DCAN import *
 import time
 import spyrit.misc.walsh_hadamard as wh
 import numpy as np
+from PIL import Image
 from scipy.stats import rankdata
 
 
 def stat_walsh_ImageNet(
     stat_root=Path("./stats/"),
     data_root=Path("./data/ILSVRC2012_img_test_v10102019/"),
     img_size=128,
@@ -417,17 +418,16 @@
 # todo: rewrite in a fashion similar to stat_walsh_stl10
 def stat_fwalsh_S_stl10(
     stat_root=Path("./stats/"), data_root=Path("./data/"), img_size=64, batch_size=1024
 ):
     """Fast Walsh S-transform of X in "2D"
 
     Args:
-        :attr:`X` (torch.tensor):  input image with shape `(*, n, n)`. `n`**2
-                                    should be a power of two.
-
+        :attr:`X` (torch.tensor): input image with shape `(*, n, n)`. `n`**2
+        should be a power of two.
 
     Returns:
         torch.tensor: S-transformed signal with shape `(*, n, n)`
 
     Examples:
         >>> import spyrit.misc.statistics as st
         >>> st.stat_fwalsh_S_stl10()
@@ -621,15 +621,16 @@
             h_img = wh.walsh2(img, H) / len(img)
             h_img = np.abs(h_img) / tot_num
             Cumulated_had += h_img
 
     Cumulated_had = Cumulated_had / np.max(Cumulated_had) * 255
     np.save(root + "{}x{}".format(nx, ny) + ".npy", Cumulated_had)
     np.savetxt(root + "{}x{}".format(nx, ny) + ".txt", Cumulated_had)
-    cv2.imwrite(root + "{}x{}".format(nx, ny) + ".png", Cumulated_had)
+    im = Image.fromarray(Cumulated_had)
+    im.save(root + "{}x{}".format(nx, ny) + ".png")
     return Cumulated_had
 
 
 # %% What for? Still in use? Ask Antonio?
 def stat_mean_coef_from_model(dataloader, device, model_exp):
     # A rediscuter avec Nicolas
     # Get dimensions and estimate total number of images in the dataset
```

### Comparing `spyrit-2.2.0/spyrit/misc/walsh_hadamard.py` & `spyrit-2.3.0/spyrit/misc/walsh_hadamard.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 __maintainer__ = "developer"
 __status__ = "Development"
 # __version__ = "0.0.1"
 
 
 import math
 import numpy as np
-from scipy.linalg import hadamard
 from sympy.combinatorics.graycode import GrayCode
 import torch
 
+import spyrit.core.torch as spytorch
+
 
 # ------------------------------------------------------------------------------
 # -- To generate sequency (aka Walsh) order --------------------------------------
 # ------------------------------------------------------------------------------
 def b2_to_b10(l):
     r"""Convert a list of numbers in base 2 to base 10
 
@@ -78,15 +79,15 @@
     graycode = GrayCode(N)
     graycode_list = list(graycode.generate_gray())
     return b2_to_b10(graycode_list)
 
 
 def bit_reverse_traverse(a):  # internet function to generate bit reverse
     n = a.shape[0]
-    assert not n & (n - 1)  # assert that n is a power of 2
+    assert not n & (n - 1), "n must be a power of 2"  # assert n is power of 2
 
     if n == 1:
         yield a[0]
     else:
         even_index = np.arange(n // 2) * 2
         odd_index = np.arange(n // 2) * 2 + 1
         for even in bit_reverse_traverse(a[even_index]):
@@ -215,17 +216,44 @@
         np.ndarray: A n-by-n array
 
     Examples:
         Walsh-ordered Hadamard matrix of order 8
 
         >>> print(walsh_matrix(8))
     """
-    P = sequency_perm_matrix(n)
-    H = hadamard(n)
-    return P @ H
+    # P = sequency_perm_matrix(n)
+    # H = hadamard(n)                   # old way with matrix multiplication
+    # return P @ H
+
+    # check that the input is a power of 2
+    spytorch.assert_power_of_2(n, raise_error=True)
+
+    # define recursive function
+    def recursive_walsh(k):
+        if k >= 3:
+            j = k // 2
+            a = recursive_walsh(j)
+            out = np.empty((k, k), dtype=int)
+
+            # generate upper half of the matrix
+            out[:j, ::2] = a
+            out[:j, 1::2] = a
+            # by symmetry, fill in lower left corner
+            out[j:, :j] = out[:j, j:].T
+            # fill in lower right corner
+            alternate = np.tile([1, -1], j // 2)
+            out[j:, j:] = alternate * out[:j, j:][::-1, :]
+            return out
+
+        elif k == 2:
+            return np.array([[1, 1], [1, -1]])
+        else:
+            return np.array[[1]]
+
+    return recursive_walsh(n)
 
 
 def fwht(x, order=True):
     """Fast Walsh-Hadamard transform of x
 
     Args:
         x (np.ndarray): n-by-1 input signal, where n is a power of two.
@@ -642,23 +670,16 @@
 
     Args:
         n (int): Order of the matrix, which must be a power of two.
 
     Returns:
         H (np.ndarray): A n*n-by-n*n matrix
     """
-    H = np.zeros((n**2, n**2))
     H1d = walsh_matrix(n)
-    for i in range(n**2):
-        image = np.zeros((n**2, 1))
-        image[i] = 1
-        image = np.reshape(image, (n, n))
-        hadamard = walsh2(image, H1d)
-        H[:, i] = np.reshape(hadamard, (1, n**2))
-    return H
+    return np.kron(H1d, H1d)
 
 
 def walsh2(X, H=None):
     r"""Return 2D Walsh-ordered Hadamard transform of an image :math:`H^\top X H`
 
     Args:
         X (np.ndarray): image as a 2d array. The size is a power of two.
@@ -1279,19 +1300,20 @@
     return x @ H.mT
 
 
 def walsh2_torch(im, H=None):
     """Return 2D Walsh-ordered Hadamard transform of an image
 
     Args:
-        im (torch.Tensor): Image, typically a B-by-C-by-W-by-H Tensor
-        H (torch.Tensor, optional): 1D Walsh-ordered Hadamard transformation matrix. A 2-D tensor of size W-by-H.
+        im (torch.tensor): Image, typically a B-by-C-by-W-by-H Tensor
+        H (torch.tensor, optional): 1D Walsh-ordered Hadamard transformation
+        matrix. A 2-D tensor of size W-by-H.
 
     Returns:
-        torch.Tensor: Hadamard transformed image. Same size as im
+        torch.tensor: Hadamard transformed image. Same size as im
 
     Examples:
         >>> im = torch.randn(256, 1, 64, 64)
         >>> had = walsh2_torch(im)
     """
     if H is None:
         H = torch.from_numpy(walsh_matrix(im.shape[3]).astype("float32"))
```

