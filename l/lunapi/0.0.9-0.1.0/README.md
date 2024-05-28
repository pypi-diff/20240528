# Comparing `tmp/lunapi-0.0.9-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.1.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,10 @@
-Zip file size: 10401570 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 22:03 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 22:03 lunapi-0.0.9.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 22:03 lunapi.libs/
--rwxr-xr-x  2.0 unx 27481472 b- defN 24-May-27 22:03 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      352 b- defN 24-May-27 22:03 lunapi/__init__.py
--rw-r--r--  2.0 unx    84522 b- defN 24-May-27 22:03 lunapi/lunapi1.py
--rw-r--r--  2.0 unx    12728 b- defN 24-May-27 22:03 lunapi/lunapi0.cpp
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 22:03 lunapi-0.0.9.dist-info/licenses/
--rw-rw-r--  2.0 unx      165 b- defN 24-May-27 22:03 lunapi-0.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx      641 b- defN 24-May-27 22:03 lunapi-0.0.9.dist-info/RECORD
--rw-rw-r--  2.0 unx     1423 b- defN 24-May-27 22:03 lunapi-0.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-27 22:03 lunapi-0.0.9.dist-info/licenses/LICENSE
-12 files, 27616452 bytes uncompressed, 10400036 bytes compressed:  62.3%
+Zip file size: 6917132 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      631 b- defN 24-May-28 03:18 lunapi-0.1.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx      118 b- defN 24-May-28 03:18 lunapi-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1398 b- defN 24-May-28 03:18 lunapi-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-28 03:18 lunapi-0.1.0.dist-info/licenses/LICENSE
+-rw-r--r--  2.0 unx      352 b- defN 24-May-28 03:18 lunapi/__init__.py
+-rw-r--r--  2.0 unx    84522 b- defN 24-May-28 03:18 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 15223136 b- defN 24-May-28 03:18 lunapi/lunapi0.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx    12728 b- defN 24-May-28 03:18 lunapi/lunapi0.cpp
+8 files, 15358034 bytes uncompressed, 6916070 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,37 +1,25 @@
-Filename: lunapi/
+Filename: lunapi-0.1.0.dist-info/RECORD
 Comment: 
 
-Filename: lunapi-0.0.9.dist-info/
+Filename: lunapi-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi.libs/
+Filename: lunapi-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
+Filename: lunapi-0.1.0.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: lunapi/__init__.py
 Comment: 
 
 Filename: lunapi/lunapi1.py
 Comment: 
 
-Filename: lunapi/lunapi0.cpp
-Comment: 
-
-Filename: lunapi-0.0.9.dist-info/licenses/
-Comment: 
-
-Filename: lunapi-0.0.9.dist-info/WHEEL
+Filename: lunapi/lunapi0.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: lunapi-0.0.9.dist-info/RECORD
-Comment: 
-
-Filename: lunapi-0.0.9.dist-info/METADATA
-Comment: 
-
-Filename: lunapi-0.0.9.dist-info/licenses/LICENSE
+Filename: lunapi/lunapi0.cpp
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## lunapi/lunapi1.py

```diff
@@ -1,11 +1,11 @@
 """lunapi1 module provides a high-level convenience wrapper around lunapi0 module functions."""
 
 # Luna Python wrapper
-# v0.0.9, 27-May-2024
+# v0.1.0, 27-May-2024
 
 import lunapi.lunapi0 as _luna
 
 import pandas as pd
 import numpy as np
 from scipy.stats.mstats import winsorize
 
@@ -20,15 +20,15 @@
 
 # resource set for Docker container version
 class resources:
    POPS_PATH = '/build/nsrr/common/resources/pops/'
    POPS_LIB = 's2'
    MODEL_PATH = '/build/luna-models/'
 
-lp_version = "v0.0.9"
+lp_version = "v0.1.0"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
```

## Comparing `lunapi-0.0.9.dist-info/METADATA` & `lunapi-0.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python interface to the Luna toolset for sleep signal analysis
 Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -22,14 +22,13 @@
 Requires-Python: >=3.9
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: plotly
 Requires-Dist: ipywidgets
-Requires-Dist: itertools
 Requires-Dist: IPython
 Description-Content-Type: text/markdown
 
 # lunapi
 
 Python bindings for C/C++ Luna library
```

## Comparing `lunapi-0.0.9.dist-info/licenses/LICENSE` & `lunapi-0.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

