# Comparing `tmp/lunapi-0.0.8-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.0.9-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,10 @@
-Zip file size: 10401402 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 02:33 lunapi-0.0.8.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 02:33 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 02:33 lunapi.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-26 02:33 lunapi-0.0.8.dist-info/licenses/
--rw-rw-r--  2.0 unx      165 b- defN 24-May-26 02:33 lunapi-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      641 b- defN 24-May-26 02:33 lunapi-0.0.8.dist-info/RECORD
--rw-rw-r--  2.0 unx     1350 b- defN 24-May-26 02:33 lunapi-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-26 02:33 lunapi-0.0.8.dist-info/licenses/LICENSE
--rwxr-xr-x  2.0 unx 27477376 b- defN 24-May-26 02:33 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      352 b- defN 24-May-26 02:33 lunapi/__init__.py
--rw-r--r--  2.0 unx    84530 b- defN 24-May-26 02:33 lunapi/lunapi1.py
--rw-r--r--  2.0 unx    12728 b- defN 24-May-26 02:33 lunapi/lunapi0.cpp
-12 files, 27612291 bytes uncompressed, 10399868 bytes compressed:  62.3%
+Zip file size: 6917140 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      631 b- defN 24-May-27 21:59 lunapi-0.0.9.dist-info/RECORD
+-rw-rw-r--  2.0 unx      118 b- defN 24-May-27 21:59 lunapi-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1423 b- defN 24-May-27 21:59 lunapi-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-27 21:59 lunapi-0.0.9.dist-info/licenses/LICENSE
+-rw-r--r--  2.0 unx      352 b- defN 24-May-27 21:59 lunapi/__init__.py
+-rw-r--r--  2.0 unx    84522 b- defN 24-May-27 21:59 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 15223136 b- defN 24-May-27 21:59 lunapi/lunapi0.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx    12728 b- defN 24-May-27 21:59 lunapi/lunapi0.cpp
+8 files, 15358059 bytes uncompressed, 6916078 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,37 +1,25 @@
-Filename: lunapi-0.0.8.dist-info/
+Filename: lunapi-0.0.9.dist-info/RECORD
 Comment: 
 
-Filename: lunapi/
+Filename: lunapi-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi.libs/
+Filename: lunapi-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: lunapi-0.0.8.dist-info/licenses/
-Comment: 
-
-Filename: lunapi-0.0.8.dist-info/WHEEL
-Comment: 
-
-Filename: lunapi-0.0.8.dist-info/RECORD
-Comment: 
-
-Filename: lunapi-0.0.8.dist-info/METADATA
-Comment: 
-
-Filename: lunapi-0.0.8.dist-info/licenses/LICENSE
-Comment: 
-
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
+Filename: lunapi-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: lunapi/__init__.py
 Comment: 
 
 Filename: lunapi/lunapi1.py
 Comment: 
 
+Filename: lunapi/lunapi0.pypy39-pp73-darwin.so
+Comment: 
+
 Filename: lunapi/lunapi0.cpp
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
-# v0.0.8, 23-May-2024
+# v0.0.9, 27-May-2024
 
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
 
-lp_version = "v0.0.8"
+lp_version = "v0.0.9"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
 
@@ -2120,15 +2120,15 @@
                 g.data[ gidx ].visible = True
 
     def rescale(change):
         ss.set_scaling( len(chbox.value) , len( anbox.value) , 2**float(yscale.value) , float(yspace.value) , header_height, footer_height , annot_height )
         redraw()
     
     def update_bandpower(change):
-        if type( pow_sel.value ) is None: return 
+        if pow_sel.value is None: return 
         if len( pow_sel.value ) == 0: return
         if band_hjorth_sel.value is True:
            S = np.transpose( ss.get_hjorths( pow_sel.value ) )
            S = np.asarray(S,dtype=object)
            S[np.isnan(S.astype(np.float_))] = None
            bg.update_traces({'z': S } , selector = {'type':'heatmap'} )
         else:
```

## Comparing `lunapi-0.0.8.dist-info/METADATA` & `lunapi-0.0.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python interface to the Luna toolset for sleep signal analysis
 Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -20,13 +20,16 @@
 Project-URL: Www, https://zzz.bwh.harvard.edu/luna
 Project-URL: Github, http://github.com/remnrem/luna-api
 Requires-Python: >=3.9
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: plotly
+Requires-Dist: ipywidgets
+Requires-Dist: itertools
 Requires-Dist: IPython
 Description-Content-Type: text/markdown
 
 # lunapi
 
 Python bindings for C/C++ Luna library
```

## Comparing `lunapi-0.0.8.dist-info/licenses/LICENSE` & `lunapi-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

