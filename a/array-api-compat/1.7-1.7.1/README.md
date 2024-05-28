# Comparing `tmp/array_api_compat-1.7.tar.gz` & `tmp/array_api_compat-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "array_api_compat-1.7.tar", last modified: Fri May 24 20:33:44 2024, max compression
+gzip compressed data, was "array_api_compat-1.7.1.tar", last modified: Tue May 28 19:24:50 2024, max compression
```

## Comparing `array_api_compat-1.7.tar` & `array_api_compat-1.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.251219 array_api_compat-1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 20:33:33.000000 array_api_compat-1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-24 20:33:44.251219 array_api_compat-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-24 20:33:33.000000 array_api_compat-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.243219 array_api_compat-1.7/array_api_compat/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.243219 array_api_compat-1.7/array_api_compat/common/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/cupy/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/dask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/dask/array/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27220 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:33:44.251219 array_api_compat-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-24 20:33:33.000000 array_api_compat-1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_array_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_isdtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_no_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_vendoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.297634 array_api_compat-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.289633 array_api_compat-1.7.1/array_api_compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.289633 array_api_compat-1.7.1/array_api_compat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/_fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/common/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.289633 array_api_compat-1.7.1/array_api_compat/cupy/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/cupy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/cupy/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/cupy/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/cupy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/cupy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.289633 array_api_compat-1.7.1/array_api_compat/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/dask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/array_api_compat/dask/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/dask/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/dask/array/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/dask/array/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/array_api_compat/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/numpy/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/numpy/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/numpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/numpy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/array_api_compat/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27220 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/torch/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/torch/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/array_api_compat/torch/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/array_api_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-28 19:24:50.000000 array_api_compat-1.7.1/array_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-28 19:24:50.000000 array_api_compat-1.7.1/array_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:24:50.000000 array_api_compat-1.7.1/array_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 19:24:50.000000 array_api_compat-1.7.1/array_api_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 19:24:50.000000 array_api_compat-1.7.1/array_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:24:50.297634 array_api_compat-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:24:50.293634 array_api_compat-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_array_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_isdtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_no_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 19:24:38.000000 array_api_compat-1.7.1/tests/test_vendoring.py
```

### Comparing `array_api_compat-1.7/LICENSE` & `array_api_compat-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/PKG-INFO` & `array_api_compat-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array_api_compat
-Version: 1.7
+Version: 1.7.1
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,16 +19,16 @@
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Provides-Extra: pytorch
 Requires-Dist: pytorch; extra == "pytorch"
 Provides-Extra: dask
 Requires-Dist: dask; extra == "dask"
-Provides-Extra: sprase
-Requires-Dist: sparse>=0.15.1; extra == "sprase"
+Provides-Extra: sparse
+Requires-Dist: sparse>=0.15.1; extra == "sparse"
 
 # Array API compatibility library
 
 This is a small wrapper around common array libraries that is compatible with
 the [Array API standard](https://data-apis.org/array-api/latest/). Currently,
 NumPy, CuPy, PyTorch, Dask, JAX and `sparse` are supported. If you want support
 for other array libraries, or if you encounter any issues, please [open an
```

### Comparing `array_api_compat-1.7/array_api_compat/__init__.py` & `array_api_compat-1.7.1/array_api_compat/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 separate Array object, but rather just uses numpy.ndarray directly.
 
 Library authors using the Array API may wish to test against array_api_strict
 to ensure they are not using functionality outside of the standard, but prefer
 this implementation for the default when working with NumPy arrays.
 
 """
-__version__ = '1.7'
+__version__ = '1.7.1'
 
 from .common import *  # noqa: F401, F403
```

### Comparing `array_api_compat-1.7/array_api_compat/_internal.py` & `array_api_compat-1.7.1/array_api_compat/_internal.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/common/_aliases.py` & `array_api_compat-1.7.1/array_api_compat/common/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/common/_fft.py` & `array_api_compat-1.7.1/array_api_compat/common/_fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/common/_helpers.py` & `array_api_compat-1.7.1/array_api_compat/common/_helpers.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/common/_linalg.py` & `array_api_compat-1.7.1/array_api_compat/common/_linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/cupy/_aliases.py` & `array_api_compat-1.7.1/array_api_compat/cupy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/cupy/_typing.py` & `array_api_compat-1.7.1/array_api_compat/cupy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/cupy/fft.py` & `array_api_compat-1.7.1/array_api_compat/cupy/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/cupy/linalg.py` & `array_api_compat-1.7.1/array_api_compat/cupy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/dask/array/_aliases.py` & `array_api_compat-1.7.1/array_api_compat/dask/array/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/dask/array/linalg.py` & `array_api_compat-1.7.1/array_api_compat/dask/array/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/numpy/__init__.py` & `array_api_compat-1.7.1/array_api_compat/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/numpy/_aliases.py` & `array_api_compat-1.7.1/array_api_compat/numpy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/numpy/_typing.py` & `array_api_compat-1.7.1/array_api_compat/numpy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/numpy/fft.py` & `array_api_compat-1.7.1/array_api_compat/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/numpy/linalg.py` & `array_api_compat-1.7.1/array_api_compat/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/torch/__init__.py` & `array_api_compat-1.7.1/array_api_compat/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/torch/_aliases.py` & `array_api_compat-1.7.1/array_api_compat/torch/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/torch/fft.py` & `array_api_compat-1.7.1/array_api_compat/torch/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat/torch/linalg.py` & `array_api_compat-1.7.1/array_api_compat/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/array_api_compat.egg-info/PKG-INFO` & `array_api_compat-1.7.1/array_api_compat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array_api_compat
-Version: 1.7
+Version: 1.7.1
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,16 +19,16 @@
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Provides-Extra: pytorch
 Requires-Dist: pytorch; extra == "pytorch"
 Provides-Extra: dask
 Requires-Dist: dask; extra == "dask"
-Provides-Extra: sprase
-Requires-Dist: sparse>=0.15.1; extra == "sprase"
+Provides-Extra: sparse
+Requires-Dist: sparse>=0.15.1; extra == "sparse"
 
 # Array API compatibility library
 
 This is a small wrapper around common array libraries that is compatible with
 the [Array API standard](https://data-apis.org/array-api/latest/). Currently,
 NumPy, CuPy, PyTorch, Dask, JAX and `sparse` are supported. If you want support
 for other array libraries, or if you encounter any issues, please [open an
```

### Comparing `array_api_compat-1.7/array_api_compat.egg-info/SOURCES.txt` & `array_api_compat-1.7.1/array_api_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/setup.py` & `array_api_compat-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     license="MIT",
     extras_require={
         "numpy": "numpy",
         "cupy": "cupy",
         "jax": "jax",
         "pytorch": "pytorch",
         "dask": "dask",
-        "sprase": "sparse >=0.15.1",
+        "sparse": "sparse >=0.15.1",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
```

### Comparing `array_api_compat-1.7/tests/test_all.py` & `array_api_compat-1.7.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/tests/test_array_namespace.py` & `array_api_compat-1.7.1/tests/test_array_namespace.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/tests/test_common.py` & `array_api_compat-1.7.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/tests/test_isdtype.py` & `array_api_compat-1.7.1/tests/test_isdtype.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.7/tests/test_no_dependencies.py` & `array_api_compat-1.7.1/tests/test_no_dependencies.py`

 * *Files identical despite different names*

