# Comparing `tmp/PyKrige-1.7.1.tar.gz` & `tmp/pykrige-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyKrige-1.7.1.tar", last modified: Mon Oct 16 11:46:42 2023, max compression
+gzip compressed data, was "pykrige-1.7.2.tar", last modified: Mon May 27 22:14:31 2024, max compression
```

## Comparing `PyKrige-1.7.1.tar` & `pykrige-1.7.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.897737 PyKrige-1.7.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1515 2023-10-16 11:44:17.000000 PyKrige-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2023-10-16 11:46:42.897737 PyKrige-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2023-10-16 11:44:17.000000 PyKrige-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2023-10-16 11:44:17.000000 PyKrige-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 11:46:42.897737 PyKrige-1.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      655 2023-10-16 11:44:17.000000 PyKrige-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.889736 PyKrige-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.893736 PyKrige-1.7.1/src/PyKrige.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-16 11:46:42.000000 PyKrige-1.7.1/src/PyKrige.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.893736 PyKrige-1.7.1/src/pykrige/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2454 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-16 11:46:42.000000 PyKrige-1.7.1/src/pykrige/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/ck.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/compat_gstools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30262 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16093 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/kriging_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.893736 PyKrige-1.7.1/src/pykrige/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/lib/cok.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/lib/variogram_models.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/lib/variogram_models.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    43574 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/ok.py
--rw-r--r--   0 runner    (1001) docker     (127)    39816 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/ok3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/rk.py
--rw-r--r--   0 runner    (1001) docker     (127)    58126 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/uk.py
--rw-r--r--   0 runner    (1001) docker     (127)    49153 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/uk3d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2173 2023-10-16 11:44:17.000000 PyKrige-1.7.1/src/pykrige/variogram_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.893736 PyKrige-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_classification_krige.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    96574 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 11:46:42.893736 PyKrige-1.7.1/tests/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)   200392 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test1_answer.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      260 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test1_settings.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   200392 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test2_answer.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test2_settings.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   331260 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test3_answer.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)  1065466 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test3_dem.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test3_settings.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19999 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test3d_answer.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test3d_data.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_data/test_data.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-10-16 11:44:17.000000 PyKrige-1.7.1/tests/test_regression_krige.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.967528 pykrige-1.7.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1515 2024-05-27 22:12:38.000000 pykrige-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-27 22:14:31.967528 pykrige-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-27 22:12:38.000000 pykrige-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-27 22:12:38.000000 pykrige-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:14:31.967528 pykrige-1.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-05-27 22:12:38.000000 pykrige-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.955528 pykrige-1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.963528 pykrige-1.7.2/src/PyKrige.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-27 22:14:31.000000 pykrige-1.7.2/src/PyKrige.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.959528 pykrige-1.7.2/src/pykrige/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2454 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 22:14:31.000000 pykrige-1.7.2/src/pykrige/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/ck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/compat_gstools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30262 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16093 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/kriging_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.959528 pykrige-1.7.2/src/pykrige/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/lib/cok.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/lib/variogram_models.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/lib/variogram_models.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/ok.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39816 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/ok3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/rk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58126 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/uk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49153 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/uk3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2173 2024-05-27 22:12:38.000000 pykrige-1.7.2/src/pykrige/variogram_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.959528 pykrige-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_classification_krige.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    96574 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:14:31.963528 pykrige-1.7.2/tests/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   200392 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test1_answer.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test1_settings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   200392 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test2_answer.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test2_settings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   331260 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test3_answer.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1065466 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test3_dem.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test3_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test3d_answer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test3d_data.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_data/test_data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-27 22:12:38.000000 pykrige-1.7.2/tests/test_regression_krige.py
```

### Comparing `PyKrige-1.7.1/LICENSE` & `pykrige-1.7.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2022, PyKrige Developers
+Copyright (c) 2015-2024, PyKrige Developers
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `PyKrige-1.7.1/PKG-INFO` & `pykrige-1.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyKrige
-Version: 1.7.1
+Version: 1.7.2
 Summary: Kriging Toolkit for Python.
 Author-email: "Benjamin S. Murphy, Sebastian Müller" <info@geostat-framework.org>
 Maintainer-email: "Sebastian Müller, Roman Yurchak" <info@geostat-framework.org>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/GeoStat-Framework/PyKrige/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/pykrige
 Project-URL: Documentation, https://pykrige.readthedocs.io
@@ -32,34 +32,39 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<2,>=1.14.5
+Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy<2,>=1.1.0
 Provides-Extra: doc
-Requires-Dist: gstools<2,>=1.3; extra == "doc"
+Requires-Dist: gstools<2,>=1.4; extra == "doc"
 Requires-Dist: pillow; extra == "doc"
 Requires-Dist: scikit-learn>=0.19; extra == "doc"
 Requires-Dist: m2r2>=0.2.8; extra == "doc"
 Requires-Dist: matplotlib>=3; extra == "doc"
 Requires-Dist: numpydoc>=1.1; extra == "doc"
-Requires-Dist: sphinx>=4; extra == "doc"
+Requires-Dist: sphinx>=7; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.8; extra == "doc"
-Requires-Dist: sphinx-rtd-theme>=1; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=2; extra == "doc"
 Provides-Extra: plot
 Requires-Dist: matplotlib<4,>=3; extra == "plot"
 Provides-Extra: sklearn
 Requires-Dist: scikit-learn>=0.19; extra == "sklearn"
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: scikit-learn>=0.19; extra == "test"
 Requires-Dist: gstools<2,>=1.4; extra == "test"
+Provides-Extra: lint
+Requires-Dist: black<24,>=23; extra == "lint"
+Requires-Dist: pylint; extra == "lint"
+Requires-Dist: isort[colors]; extra == "lint"
+Requires-Dist: cython-lint; extra == "lint"
 
 # PyKrige
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3738604.svg)](https://doi.org/10.5281/zenodo.3738604)
 [![PyPI version](https://badge.fury.io/py/PyKrige.svg)](https://badge.fury.io/py/PyKrige)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pykrige.svg)](https://anaconda.org/conda-forge/pykrige)
 [![Build Status](https://github.com/GeoStat-Framework/PyKrige/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/GeoStat-Framework/PyKrige/actions)
```

### Comparing `PyKrige-1.7.1/README.md` & `pykrige-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/pyproject.toml` & `pykrige-1.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [build-system]
 requires = [
     "setuptools>=64",
     "setuptools_scm>=7",
-    "oldest-supported-numpy",
-    "scipy>=1.1.0,<2",
-    "Cython>=0.28.3,<3.0",
+    "numpy>=2.0.0rc1,<2.3; python_version >= '3.9'",
+    "scipy>=1.13.0,<2; python_version >= '3.9'",
+    "oldest-supported-numpy; python_version < '3.9'",
+    "scipy>=1.3.2,<2; python_version < '3.9'",
+    "Cython>=3.0.10,<3.1.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
 name = "PyKrige"
 description = "Kriging Toolkit for Python."
@@ -42,37 +44,43 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "numpy>=1.14.5,<2",
+    "numpy>=1.20.0",
     "scipy>=1.1.0,<2",
 ]
 
 [project.optional-dependencies]
 doc = [
-    "gstools>=1.3,<2",
+    "gstools>=1.4,<2",
     "pillow",
     "scikit-learn>=0.19",
     "m2r2>=0.2.8",
     "matplotlib>=3",
     "numpydoc>=1.1",
-    "sphinx>=4",
+    "sphinx>=7",
     "sphinx-gallery>=0.8",
-    "sphinx-rtd-theme>=1",
+    "sphinx-rtd-theme>=2",
 ]
 plot = ["matplotlib>=3,<4"]
 sklearn = ["scikit-learn>=0.19"]
 test = [
     "pytest-cov>=3",
     "scikit-learn>=0.19",
     "gstools>=1.4,<2",
 ]
+lint = [
+    "black>=23,<24",
+    "pylint",
+    "isort[colors]",
+    "cython-lint",
+]
 
 [project.urls]
 Changelog = "https://github.com/GeoStat-Framework/PyKrige/blob/main/CHANGELOG.md"
 Conda-Forge = "https://anaconda.org/conda-forge/pykrige"
 Documentation = "https://pykrige.readthedocs.io"
 Homepage = "https://github.com/GeoStat-Framework/PyKrige"
 Source = "https://github.com/GeoStat-Framework/PyKrige"
@@ -88,15 +96,24 @@
 fallback_version = "0.0.0.dev0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
-target-version = ["py38"]
+target-version = [
+    "py38",
+    "py39",
+    "py310",
+    "py311",
+    "py312",
+]
+
+[tool.cython-lint]
+max-line-length = 100
 
 [tool.coverage]
     [tool.coverage.run]
     source = ["pykrige"]
     omit = [
         "*docs*",
         "*examples*",
@@ -117,14 +134,15 @@
         "scipy",
     ]
     ignore = "_version.py"
 
     [tool.pylint.message_control]
     disable = [
         "R0801",
+        "C0103",  # lots of invalid variable names
     ]
 
     [tool.pylint.reports]
     output-format = "colorized"
 
     [tool.pylint.design]
     max-args = 20
@@ -133,16 +151,12 @@
     max-statements = 80
     max-attributes = 25
     max-public-methods = 75
 
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
-# Disable building PyPy wheels on all platforms, 32bit for py3.10/11/12 and musllinux builds, py3.6/7
-skip = ["cp36-*", "cp37-*", "pp*", "cp31*-win32", "cp31*-manylinux_i686", "*-musllinux_*"]
+# Disable building PyPy wheels on all platforms, 32bit and musllinux builds, py3.6/7
+skip = ["cp36-*", "cp37-*", "pp*", "*-win32", "*-manylinux_i686", "*-musllinux_*"]
 # Run the package tests using `pytest`
 test-extras = "test"
 test-command = "pytest -v {package}/tests"
-# Skip trying to test arm64 builds on Intel Macs
-test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
-# no wheels for linux-32bit anymore for numpy>=1.22
-environment = "PIP_PREFER_BINARY=1"
```

### Comparing `PyKrige-1.7.1/setup.py` & `pykrige-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/PyKrige.egg-info/SOURCES.txt` & `pykrige-1.7.2/src/PyKrige.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/__init__.py` & `pykrige-1.7.2/src/pykrige/__init__.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/ck.py` & `pykrige-1.7.2/src/pykrige/ck.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/compat.py` & `pykrige-1.7.2/src/pykrige/compat.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/compat_gstools.py` & `pykrige-1.7.2/src/pykrige/compat_gstools.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/core.py` & `pykrige-1.7.2/src/pykrige/core.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/kriging_tools.py` & `pykrige-1.7.2/src/pykrige/kriging_tools.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/lib/cok.pyx` & `pykrige-1.7.2/src/pykrige/lib/cok.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
-# -*- coding: utf-8 -*-
+# cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
 import numpy as np
 
 cimport numpy as np
-from libc.math cimport sqrt
 
 import scipy.linalg
 
 from scipy.linalg.cython_blas cimport dgemv
 from scipy.linalg.cython_lapack cimport dgesv
 
 from .variogram_models cimport get_variogram_model
 
 
-cpdef _c_exec_loop(double [:, ::1] a_all,
-              double [:, ::1] bd_all,
-              char [::1] mask,
-              long n,
-              dict pars):
-    cdef long i, j, k
+cpdef _c_exec_loop(
+    double [:, ::1] a_all,
+    double [:, ::1] bd_all,
+    char [::1] mask,
+    long n,
+    dict pars
+):
+    cdef long i, k
 
     npt = bd_all.shape[0]
 
     cdef double [::1] zvalues = np.zeros(npt, dtype='float64')
     cdef double [::1] sigmasq = np.zeros(npt, dtype='float64')
     cdef double [::1] x = np.zeros(n+1, dtype='float64')
     cdef double [::1] b = np.zeros(n+1, dtype='float64')
@@ -30,85 +30,83 @@
     cdef double [::1] bd
     cdef double z_tmp, ss_tmp, eps=pars['eps']
     cdef int nb, inc=1
     cdef double alpha=1.0, beta=0.0
 
     nb = n + 1
 
-
     c_variogram_function = get_variogram_model(pars['variogram_function'].__name__)
 
     cdef double [::1] variogram_model_parameters = np.asarray(pars['variogram_model_parameters'])
 
-    cdef double [::1,:] a_inv = np.asfortranarray(np.empty_like(a_all))
-
+    cdef double [::1, :] a_inv = np.asfortranarray(np.empty_like(a_all))
 
     if pars['pseudo_inv']:
         if pars['pseudo_inv_type'] == "pinv":
             a_inv = np.asfortranarray(scipy.linalg.pinv(a_all))
         elif pars['pseudo_inv_type'] == "pinv2":
             a_inv = np.asfortranarray(scipy.linalg.pinv2(a_all))
         elif pars['pseudo_inv_type'] == "pinvh":
             a_inv = np.asfortranarray(scipy.linalg.pinvh(a_all))
         else:
             raise ValueError('Unknown pseudo inverse method selected.')
     else:
         a_inv = np.asfortranarray(scipy.linalg.inv(a_all))
 
-
-    for i in range(npt):   # same thing as range(npt) if mask is not defined, otherwise take the non masked elements
+    # same thing as range(npt) if mask is not defined, otherwise take the non masked elements
+    for i in range(npt):
         if mask[i]:
             continue
         bd = bd_all[i]
 
         c_variogram_function(variogram_model_parameters, n, bd, b)
 
         for k in range(n):
             b[k] *= -1
         b[n] = 1.0
 
         if pars['exact_values']:
             check_b_vect(n, bd, b, eps)
 
-
         # Do the BLAS matrix-vector multiplication call
-        dgemv(
-                                  # # Compute y := alpha*A*x + beta*y
-             'N',                 # char *trans, # {'T','C'}: o(A)=A'; {'N'}: o(A)=A
-             &nb,                 # int *m, # Rows of A (prior to transpose from *trans)
-             &nb,                 # int *n, # Columns of A / min(len(x))
-             &alpha,              # np.float64_t *alpha, # Scalar multiple
-             &(a_inv[0,0]),          # np.float64_t *a, # Matrix A: mxn
-             &nb,                 # int *lda, # The size of the first dimension of A (in memory)
-             &(b[0]),             # np.float64_t *x, # Vector x, min(len(x)) = n
-             &inc,                # int *incx, # The increment between elements of x (usually 1)
-             &beta,               # np.float64_t *beta, # Scalar multiple
-             &(x[0]),           # np.float64_t *y, # Vector y, min(len(y)) = m
-             &inc                 # int *incy # The increment between elements of y (usually 1)
-            )
+        dgemv(                   # Compute y := alpha*A*x + beta*y
+            'N',                 # char *trans, # {'T','C'}: o(A)=A'; {'N'}: o(A)=A
+            &nb,                 # int *m, # Rows of A (prior to transpose from *trans)
+            &nb,                 # int *n, # Columns of A / min(len(x))
+            &alpha,              # np.float64_t *alpha, # Scalar multiple
+            &(a_inv[0, 0]),      # np.float64_t *a, # Matrix A: mxn
+            &nb,                 # int *lda, # The size of the first dimension of A (in memory)
+            &(b[0]),             # np.float64_t *x, # Vector x, min(len(x)) = n
+            &inc,                # int *incx, # The increment between elements of x (usually 1)
+            &beta,               # np.float64_t *beta, # Scalar multiple
+            &(x[0]),             # np.float64_t *y, # Vector y, min(len(y)) = m
+            &inc                 # int *incy # The increment between elements of y (usually 1)
+        )
 
         z_tmp = 0.0
         ss_tmp = 0.0
         for k in range(n):
             z_tmp += x[k]*Z[k]
 
         for k in range(nb):
             ss_tmp += x[k]*b[k]
 
         zvalues[i] = z_tmp
         sigmasq[i] = -ss_tmp
 
     return zvalues.base, sigmasq.base
 
-cpdef _c_exec_loop_moving_window(double [:, ::1] a_all,
-              double [:, ::1] bd_all,
-              char [::1] mask,
-              long [:,::1] bd_idx,
-              long n_max,
-              dict pars):
+cpdef _c_exec_loop_moving_window(
+    double [:, ::1] a_all,
+    double [:, ::1] bd_all,
+    char [::1] mask,
+    long [:, ::1] bd_idx,
+    long n_max,
+    dict pars
+):
     cdef long i, j, k, p_i, p_j, npt, n
 
     npt = bd_all.shape[0]
     n = bd_idx.shape[1]
 
     cdef double [::1] zvalues = np.zeros(npt, dtype='float64')
     cdef double [::1] sigmasq = np.zeros(npt, dtype='float64')
@@ -117,36 +115,30 @@
     cdef double [::1] b = np.zeros(n_max+1, dtype='float64')
     cdef double [::1] Z = pars['Z']
     cdef double [::1] a_selection = np.zeros((n_max+1)*(n_max+1), dtype='float64')
     cdef double [::1] bd = np.zeros(n_max, dtype='float64')
     cdef double z_tmp, ss_tmp, eps=pars['eps']
     cdef int nb, nrhs=1, info
     cdef int [::1] ipiv = np.zeros(n_max+1, dtype='int32')
-    cdef double alpha=1.0, beta=0.0
     cdef long [::1] bd_idx_sel
 
     nb = n + 1
 
-
-
     c_variogram_function = get_variogram_model(pars['variogram_function'].__name__)
 
     cdef double [::1] variogram_model_parameters = np.asarray(pars['variogram_model_parameters'])
 
-
-
     for i in range(npt):
         if mask[i]:
             continue
 
         bd = bd_all[i, :]
 
         bd_idx_sel = bd_idx[i, :]
 
-
         for k in range(n):
             p_i = bd_idx_sel[k]
             for j in range(n):
                 p_j = bd_idx_sel[j]
                 a_selection[k + nb*j] = a_all[p_i, p_j]
 
         for k in range(nb):
@@ -163,16 +155,16 @@
         if pars['exact_values']:
             check_b_vect(n, bd, b, eps)
 
         for k in range(nb):
             x[k] = b[k]
 
         # higher level (and slower) call to do the same thing as dgesv below
-        #a2D = a_selection.base[:nb*nb].reshape((nb, nb))
-        #x =  scipy.linalg.solve(a2D, b.base[:nb])
+        # a2D = a_selection.base[:nb*nb].reshape((nb, nb))
+        # x = scipy.linalg.solve(a2D, b.base[:nb])
 
         dgesv(
                 &nb,
                 &nrhs,
                 &(a_selection[0]),
                 &nb,
                 &(ipiv[0]),
@@ -182,15 +174,14 @@
                 )
 
         if info > 0:
             raise ValueError('Singular matrix')
         elif info < 0:
             raise ValueError('Wrong arguments')
 
-
         z_tmp = 0.0
         ss_tmp = 0.0
         for k in range(n):
             j = bd_idx_sel[k]
             z_tmp += x[k]*Z[j]
 
         for k in range(nb):
```

### Comparing `PyKrige-1.7.1/src/pykrige/lib/variogram_models.pyx` & `pykrige-1.7.2/src/pykrige/lib/variogram_models.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-#cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
-# -*- coding: utf-8 -*-
-import numpy as np
-cimport numpy as np
+# cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
 from libc.math cimport exp
 
-# copied from variogram_model.py
-
-
 
+# copied from variogram_model.py
 cdef variogram_model_t get_variogram_model(name):
     cdef variogram_model_t c_func
 
     if name == 'linear_variogram_model':
         c_func = &_c_linear_variogram_model
     elif name == 'power_variogram_model':
         c_func = &_c_power_variogram_model
@@ -23,54 +18,64 @@
         c_func = &_c_spherical_variogram_model
     else:
         raise NotImplementedError
 
     return c_func
 
 
-cdef void _c_linear_variogram_model(double [::1] params, long n, double [::1]  dist, double[::1] out) nogil:
+cdef void _c_linear_variogram_model(
+    double [::1] params, long n, double [::1]  dist, double[::1] out
+) noexcept nogil:
     cdef long k
     cdef double a, b
     a = params[0]
     b = params[1]
     for k in range(n):
         out[k] = a*dist[k] + b
 
 
-cdef void _c_power_variogram_model(double [::1] params, long n, double [::1] dist, double[::1] out) nogil:
+cdef void _c_power_variogram_model(
+    double [::1] params, long n, double [::1] dist, double[::1] out
+) noexcept nogil:
     cdef long k
     cdef double a, b, c
     a = params[0]
     b = params[1]
     c = params[2]
     for k in range(n):
-        out[k] =  a*(dist[k]**b) + c
+        out[k] = a*(dist[k]**b) + c
 
 
-cdef void _c_gaussian_variogram_model(double [::1] params, long n, double [::1]  dist, double [::1] out) nogil:
+cdef void _c_gaussian_variogram_model(
+    double [::1] params, long n, double [::1]  dist, double [::1] out
+) noexcept nogil:
     cdef long k
     cdef double a, b, c
     a = params[0]
     b = params[1]
     c = params[2]
     for k in range(n):
         out[k] = a*(1 - exp(-(dist[k]/(b*4.0/7.0))**2)) + c
 
 
-cdef void _c_exponential_variogram_model(double [::1] params, long n, double[::1] dist, double[::1] out) nogil:
+cdef void _c_exponential_variogram_model(
+    double [::1] params, long n, double[::1] dist, double[::1] out
+) noexcept nogil:
     cdef long k
     cdef double a, b, c
     a = params[0]
     b = params[1]
     c = params[2]
     for k in range(n):
         out[k] = a*(1 - exp(-dist[k]/(b/3.0))) + c
 
 
-cdef void _c_spherical_variogram_model(double [::1] params, long n, double[::1] dist, double[::1] out) nogil:
+cdef void _c_spherical_variogram_model(
+    double [::1] params, long n, double[::1] dist, double[::1] out
+) noexcept nogil:
     cdef long k
     cdef double a, b, c
     a = params[0]
     b = params[1]
     c = params[2]
     for k in range(n):
         if dist[k] < b:
```

### Comparing `PyKrige-1.7.1/src/pykrige/ok.py` & `pykrige-1.7.2/src/pykrige/ok.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
             if backend == "loop":
                 zvalues, sigmasq = self._exec_loop_moving_window(a, bd, mask, bd_idx)
             elif backend == "C":
                 zvalues, sigmasq = _c_exec_loop_moving_window(
                     a,
                     bd,
                     mask.astype("int8"),
-                    bd_idx.astype(int),
+                    bd_idx.astype("long"),
                     self.X_ADJUSTED.shape[0],
                     c_pars,
                 )
             else:
                 raise ValueError(
                     "Specified backend {} for a moving window "
                     "is not supported.".format(backend)
```

### Comparing `PyKrige-1.7.1/src/pykrige/ok3d.py` & `pykrige-1.7.2/src/pykrige/ok3d.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/rk.py` & `pykrige-1.7.2/src/pykrige/rk.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/uk.py` & `pykrige-1.7.2/src/pykrige/uk.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/uk3d.py` & `pykrige-1.7.2/src/pykrige/uk3d.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/src/pykrige/variogram_models.py` & `pykrige-1.7.2/src/pykrige/variogram_models.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_api.py` & `pykrige-1.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_classification_krige.py` & `pykrige-1.7.2/tests/test_classification_krige.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_core.py` & `pykrige-1.7.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_data/test1_answer.asc` & `pykrige-1.7.2/tests/test_data/test1_answer.asc`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_data/test2_answer.asc` & `pykrige-1.7.2/tests/test_data/test2_answer.asc`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_data/test3_answer.asc` & `pykrige-1.7.2/tests/test_data/test3_answer.asc`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_data/test3_dem.asc` & `pykrige-1.7.2/tests/test_data/test3_dem.asc`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_data/test3d_answer.txt` & `pykrige-1.7.2/tests/test_data/test3d_answer.txt`

 * *Files identical despite different names*

### Comparing `PyKrige-1.7.1/tests/test_regression_krige.py` & `pykrige-1.7.2/tests/test_regression_krige.py`

 * *Files identical despite different names*

