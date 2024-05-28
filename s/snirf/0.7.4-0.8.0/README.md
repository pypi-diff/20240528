# Comparing `tmp/snirf-0.7.4.tar.gz` & `tmp/snirf-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snirf-0.7.4.tar", last modified: Thu Aug  4 16:44:30 2022, max compression
+gzip compressed data, was "dist/snirf-0.8.0.tar", last modified: Tue May 28 17:25:37 2024, max compression
```

## Comparing `snirf-0.7.4.tar` & `snirf-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 16:44:30.000000 snirf-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-04 16:44:30.000000 snirf-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10325 2022-08-04 16:44:30.000000 snirf-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-04 16:44:11.000000 snirf-0.7.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10325 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-04 16:44:11.000000 snirf-0.7.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 16:44:30.000000 snirf-0.7.4/snirf/
--rw-r--r--   0 runner    (1001) docker     (121)   275545 2022-08-04 16:44:11.000000 snirf-0.7.4/snirf/pysnirf2.py
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-04 16:44:11.000000 snirf-0.7.4/snirf/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-04 16:44:11.000000 snirf-0.7.4/snirf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-08-04 16:44:11.000000 snirf-0.7.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2022-08-04 16:44:11.000000 snirf-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:25:37.000000 snirf-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 17:25:25.000000 snirf-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 17:25:25.000000 snirf-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-28 17:25:37.000000 snirf-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-28 17:25:25.000000 snirf-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 17:25:25.000000 snirf-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:25:37.000000 snirf-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-28 17:25:25.000000 snirf-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 17:25:25.000000 snirf-0.8.0/snirf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 17:25:25.000000 snirf-0.8.0/snirf/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   276843 2024-05-28 17:25:25.000000 snirf-0.8.0/snirf/pysnirf2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 17:25:37.000000 snirf-0.8.0/snirf.egg-info/top_level.txt
```

### Comparing `snirf-0.7.4/PKG-INFO` & `snirf-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: snirf
-Version: 0.7.4
+Version: 0.8.0
 Summary: Interface and validator for SNIRF files
 Home-page: https://github.com/BUNPC/pysnirf2
 Author-email: sstucker@bu.edu
 License: GPLv3
 Description: 
         <h1 style="text-align:center">
         
         pysnirf2
         
         `pip install snirf`
         
         </h1>
         
-        
         ![testing](https://github.com/BUNPC/pysnirf2/actions/workflows/test.yml/badge.svg)
         ![lazydocs](https://github.com/BUNPC/pysnirf2/actions/workflows/lazydocs.yml/badge.svg)
         [![PyPI version](https://badge.fury.io/py/snirf.svg)](https://badge.fury.io/py/snirf)
         [![DOI](https://zenodo.org/badge/426339949.svg)](https://zenodo.org/badge/latestdoi/426339949)
         
         Dynamically generated Python library for reading, writing, and validating [Shared Near Infrared Spectroscopy Format (SNIRF) files](https://github.com/fNIRS/snirf).
         
@@ -31,15 +30,15 @@
         ## Installation
         `pip install snirf`
         
         pysnirf2 requires Python > 3.6.
         
         # Features
         
-        The library generated via metaprogramming, but the resulting classes explicitly implement each and every specified SNIRF field so as to provide an extensible object-oriented foundation for SNIRF applications.
+        pysnirf2 explicitly implements all SNIRF fields so as to provide an extensible object-oriented foundation for SNIRF applications.
         
         ## Open a SNIRF file
         `Snirf(<path>, <mode>)` opens a SNIRF file at `<path>` _or creates a new one if it doesn't exist._ Use mode 'w' to create a new file, 'r' to read a file, and 'r+' to edit an existing file.
         ```python
         from snirf import Snirf
         snirf = Snirf(r'some\path\subj1_run01.snirf', 'r+')
         ```
```

### Comparing `snirf-0.7.4/snirf.egg-info/PKG-INFO` & `snirf-0.8.0/snirf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: snirf
-Version: 0.7.4
+Version: 0.8.0
 Summary: Interface and validator for SNIRF files
 Home-page: https://github.com/BUNPC/pysnirf2
 Author-email: sstucker@bu.edu
 License: GPLv3
 Description: 
         <h1 style="text-align:center">
         
         pysnirf2
         
         `pip install snirf`
         
         </h1>
         
-        
         ![testing](https://github.com/BUNPC/pysnirf2/actions/workflows/test.yml/badge.svg)
         ![lazydocs](https://github.com/BUNPC/pysnirf2/actions/workflows/lazydocs.yml/badge.svg)
         [![PyPI version](https://badge.fury.io/py/snirf.svg)](https://badge.fury.io/py/snirf)
         [![DOI](https://zenodo.org/badge/426339949.svg)](https://zenodo.org/badge/latestdoi/426339949)
         
         Dynamically generated Python library for reading, writing, and validating [Shared Near Infrared Spectroscopy Format (SNIRF) files](https://github.com/fNIRS/snirf).
         
@@ -31,15 +30,15 @@
         ## Installation
         `pip install snirf`
         
         pysnirf2 requires Python > 3.6.
         
         # Features
         
-        The library generated via metaprogramming, but the resulting classes explicitly implement each and every specified SNIRF field so as to provide an extensible object-oriented foundation for SNIRF applications.
+        pysnirf2 explicitly implements all SNIRF fields so as to provide an extensible object-oriented foundation for SNIRF applications.
         
         ## Open a SNIRF file
         `Snirf(<path>, <mode>)` opens a SNIRF file at `<path>` _or creates a new one if it doesn't exist._ Use mode 'w' to create a new file, 'r' to read a file, and 'r+' to edit an existing file.
         ```python
         from snirf import Snirf
         snirf = Snirf(r'some\path\subj1_run01.snirf', 'r+')
         ```
```

### Comparing `snirf-0.7.4/LICENSE` & `snirf-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snirf-0.7.4/snirf/pysnirf2.py` & `snirf-0.8.0/snirf/pysnirf2.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,20 +133,22 @@
 _varlen_str_type = h5py.string_dtype(
     encoding='ascii',
     length=None)  # Length=None creates HDF5 variable length string
 _DTYPE_FLOAT32 = 'f4'
 _DTYPE_FLOAT64 = 'f8'
 _DTYPE_INT32 = 'i4'
 _DTYPE_INT64 = 'i8'
+_DTYPE_UINT32 = 'u4'
+_DTYPE_UINT64 = 'u8'
 _DTYPE_FIXED_LEN_STR = 'S'  # Not sure how robust this is, but fixed length strings will always at least contain S
 _DTYPE_VAR_LEN_STR = 'O'  # Variable length string
 
 _INT_DTYPES = [int, np.int32, np.int64]
 _FLOAT_DTYPES = [float, np.float64]
-_STR_DTYPES = [str, np.string_]
+_STR_DTYPES = [str, np.bytes_]
 
 # -- Dataset creators  ---------------------------------------
 
 
 def _get_padded_shape(name: str, data: np.ndarray,
                       desired_ndim: int) -> np.ndarray:
     """Utility function which pads data shape to ndim."""
@@ -758,16 +760,20 @@
     """
     if type(dataset) is not h5py.Dataset:
         raise TypeError("'dataset' must be type h5py.Dataset")
     if dataset.size > 1 or dataset.ndim > 0:
         return 'INVALID_DATASET_SHAPE'
     if _DTYPE_INT32 in dataset.dtype.str:
         return 'OK'
+    if _DTYPE_UINT32 in dataset.dtype.str:
+        return 'OK'
     if _DTYPE_INT64 in dataset.dtype.str:
-        return 'INT_64'
+        return 'OK'
+    if _DTYPE_UINT64 in dataset.dtype.str:
+        return 'OK'
     else:
         return 'INVALID_DATASET_TYPE'
 
 
 def _validate_float(dataset: h5py.Dataset) -> str:
     """Determines an issue code (as predefined in `_CODES`) based on the contents an `h5py.Dataset` instance.
 
@@ -836,15 +842,15 @@
         dataset (h5py.Dataset): An open` h5py.Dataset` instance
 
     Returns:
         An issue code describing the validity of the dataset based on its format and shape
     """
     if type(dataset) is not h5py.Dataset:
         raise TypeError("'dataset' must be type h5py.Dataset")
-    if dataset.ndim not in ndims:
+    if dataset.ndim != ndims[0]:
         return 'INVALID_DATASET_SHAPE'
     if _DTYPE_FLOAT32 in dataset.dtype.str or _DTYPE_FLOAT64 in dataset.dtype.str:
         return 'OK'
     else:
         return 'INVALID_DATASET_TYPE'
 
 
@@ -1273,17 +1279,17 @@
             h = self._parent._h
         if len(self._list) == 1 and self._name == 'nirs':
             e = self._list[0]
             indexstr = e.location.split('/' + self._name)[-1]
             if len(indexstr) > 0:  # Rename the element
                 h.move(e.location,
                        '/'.join(e.location.split('/')[:-1]) + '/' + self._name)
-                self._cfg.logger.info(
-                    e.location, '--->',
-                    '/'.join(e.location.split('/')[:-1]) + '/' + self._name)
+                self._cfg.logger.info(e.location + '--->' +
+                                      '/'.join(e.location.split('/')[:-1]) +
+                                      '/' + self._name)
         elif all([
                 len(e.location.split('/' + self._name)[-1]) > 0
                 for e in self._list
         ]):
             if not [
                     int(e.location.split('/' + self._name)[-1])
                     for e in self._list
@@ -1380,15 +1386,20 @@
                                          for name in g_src._unspecified_names]:
                 g_dst.add(
                     name, sub_src_unspec
                 )  # If a Group hasattr _unspecified names, it should have add
     return g_dst
 
 
-# generated by sstucker on 2022-08-04
+# ================================================================================
+# DO NOT EDIT THE BELOW CODE! IT IS GENERATED VIA TEMPLATE. SEE README FOR DETAILS
+# ================================================================================
+# <<< BEGIN TEMPLATE INSERT >>>
+
+# generated by sstucker on 2023-09-18
 # version v1.1 SNIRF specification parsed from https://raw.githubusercontent.com/fNIRS/snirf/v1.1/snirf_specification.md
 
 
 class MetaDataTags(Group):
     """Wrapper for Group of type `metaDataTags`.
 
     The `metaDataTags` group contains the metadata associated with the measurements.
@@ -5731,15 +5742,14 @@
                     raise ValueError(
                         "Invalid mode: '{}'. Only 'r', 'r+' and 'w' are supported."
                         .format(args[1]))
             else:
                 warn(
                     'Use `Snirf(<path>, <mode>)` to open SNIRF file from path. Path-only construction is deprecated.',
                     DeprecationWarning)
-                # fmode is ''
             if type(path) is str:
                 if not path.endswith('.snirf'):
                     path.replace('.', '')
                     path = path + '.snirf'
                 if os.path.exists(path):
                     self._cfg.logger.info('Loading from file %s', path)
                     if self._cfg.fmode == '':
@@ -5927,14 +5937,19 @@
     'NIHPD',
     'OASIS30AntsOASISAnts',
     'OASIS30Atropos',
     'Talairach',
     'UNCInfant',
 ]
 
+# <<< END TEMPLATE INSERT >>>
+# ================================================================================
+# DO NOT EDIT THE ABOVE CODE! IT IS GENERATED VIA TEMPLATE. SEE README FOR DETAILS
+# ================================================================================
+
 # -- Extend metaDataTags to support addition of new unspecified datasets ------
 
 
 class MetaDataTags(MetaDataTags):
     def add(self, name, value):
         """Add a new tag to the list.
         
@@ -6119,15 +6134,15 @@
     def copy(self) -> Snirf:
         """Return a copy of the Snirf instance.
             
         A copy of a Snirf instance is a brand new HDF5 file in memory. This can 
         be expensive to create. Note that in lieu of copying you can make assignments
         between Snirf instances. 
         """
-        s = Snirf('r+')
+        s = Snirf()
         s = _recursive_hdf5_copy(s, self)
         return s
 
     def validate(self) -> ValidationResult:
         """Validate a `Snirf` instance.
 
         Returns the validity of the current state of a `Snirf` object, including
@@ -6179,15 +6194,15 @@
         super()._validate(result)
 
         # TODO INVALID_FILENAME, INVALID_FILE detection
 
         for nirs in self.nirs:
             if type(nirs.probe) not in [type(None), type(_AbsentGroup)]:
                 if nirs.probe.sourceLabels is not None:
-                    lenSourceLabels = nirs.probe.sourceLabels.shape[0]
+                    lenSourceLabels = nirs.probe.sourceLabels.size
                 else:
                     lenSourceLabels = 0
                 if nirs.probe.detectorLabels is not None:
                     lenDetectorLabels = nirs.probe.detectorLabels.size
                 else:
                     lenDetectorLabels = 0
                 if nirs.probe.wavelengths is not None:
@@ -6268,7 +6283,25 @@
     if not path.endswith('.snirf'):
         path += '.snirf'
     if os.path.exists(path):
         with Snirf(path, 'r') as snirf:
             return snirf.validate()
     else:
         raise FileNotFoundError('No SNIRF file at ' + path)
+
+
+if __name__ == "__main__":
+    appdir = (os.path.dirname(os.path.abspath(__file__)) + '/').replace(
+        '\\', '/')
+    if len(sys.argv) < 2:
+        sys.exit()
+    else:
+        filename = sys.argv[1]
+    if not os.path.exists(filename):
+        filename = os.path.join(appdir, filename)
+        if not os.path.exists(filename):
+            raise FileNotFoundError('Cannot find {}\n'.format(filename))
+            sys.exit()
+    print('\nValidating file {}\n'.format(os.path.abspath(filename)))
+    snirf = Snirf(filename, 'r')
+    r = snirf.validate()
+    r.display()
```

### Comparing `snirf-0.7.4/setup.py` & `snirf-0.8.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 # -*- coding: utf-8 -*-
 # Based on https://github.com/kennethreitz/setup.py
 # To upload to PyPI
 # >>> setup.py upload
 
 import io
 import os
+from pathlib import Path
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
-from snirf.__version__ import __version__ as VERSION
+# Do not "import snirf" here because that requires h5py to be installed
+with open(Path(__file__).parent / "snirf" / "__version__.py") as f:
+    VERSION = f.readline().split("=")[1].strip().strip('()')
+VERSION = ".".join(VERSION.replace(' ', '').replace(',', '.').split(','))
 
 NAME = 'snirf'
 
 about = {}
 about['__version__'] = VERSION
 
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `snirf-0.7.4/README.md` & `snirf-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 pysnirf2
 
 `pip install snirf`
 
 </h1>
 
-
 ![testing](https://github.com/BUNPC/pysnirf2/actions/workflows/test.yml/badge.svg)
 ![lazydocs](https://github.com/BUNPC/pysnirf2/actions/workflows/lazydocs.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/snirf.svg)](https://badge.fury.io/py/snirf)
 [![DOI](https://zenodo.org/badge/426339949.svg)](https://zenodo.org/badge/latestdoi/426339949)
 
 Dynamically generated Python library for reading, writing, and validating [Shared Near Infrared Spectroscopy Format (SNIRF) files](https://github.com/fNIRS/snirf).
 
@@ -23,15 +22,15 @@
 ## Installation
 `pip install snirf`
 
 pysnirf2 requires Python > 3.6.
 
 # Features
 
-The library generated via metaprogramming, but the resulting classes explicitly implement each and every specified SNIRF field so as to provide an extensible object-oriented foundation for SNIRF applications.
+pysnirf2 explicitly implements all SNIRF fields so as to provide an extensible object-oriented foundation for SNIRF applications.
 
 ## Open a SNIRF file
 `Snirf(<path>, <mode>)` opens a SNIRF file at `<path>` _or creates a new one if it doesn't exist._ Use mode 'w' to create a new file, 'r' to read a file, and 'r+' to edit an existing file.
 ```python
 from snirf import Snirf
 snirf = Snirf(r'some\path\subj1_run01.snirf', 'r+')
 ```
```

