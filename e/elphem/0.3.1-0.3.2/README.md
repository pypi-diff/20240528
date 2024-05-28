# Comparing `tmp/elphem-0.3.1.tar.gz` & `tmp/elphem-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphem-0.3.1.tar", last modified: Fri May 17 14:54:33 2024, max compression
+gzip compressed data, was "elphem-0.3.2.tar", last modified: Tue May 28 06:53:03 2024, max compression
```

## Comparing `elphem-0.3.1.tar` & `elphem-0.3.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 14:54:28.000000 elphem-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-17 14:54:33.215528 elphem-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-17 14:54:28.000000 elphem-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.207527 elphem-0.3.1/elphem/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/common/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/electron/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/electron/electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/elph/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/electron_phonon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/green_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/lattice_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/primitive_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/reciprocal_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/phonon/phonon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/elphem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:54:33.215528 elphem-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-17 14:54:28.000000 elphem-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/electron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/electron/test_electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/elph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/elph/test_self_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/lattice/test_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/phonon/test_phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.624229 elphem-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 06:52:59.000000 elphem-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-28 06:53:03.620229 elphem-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-05-28 06:52:59.000000 elphem-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/electron/electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/electron_phonon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/green_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/lattice_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/primitive_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/reciprocal_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/phonon/phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:53:03.624229 elphem-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-28 06:52:59.000000 elphem-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/electron/test_electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/elph/test_self_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/lattice/test_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/phonon/test_phonon.py
```

### Comparing `elphem-0.3.1/LICENSE` & `elphem-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/PKG-INFO` & `elphem-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: elphem
-Version: 0.3.1
-Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
-Home-page: https://github.com/cohsh/elphem
-Download-URL: https://github.com/cohsh/elphem
-Author: Kohei Ishii
-Author-email: 
-Maintainer: Kohei Ishii
-Maintainer-email: 
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-
 # elphem
 [![Upload Python Package](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/cohsh/elphem/actions/workflows/python-package.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-package.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/elphem)
 ![PyPI - Version](https://img.shields.io/pypi/v/elphem)
 [![Downloads](https://static.pepy.tech/badge/elphem/month)](https://pepy.tech/project/elphem)
 ![GitHub](https://img.shields.io/github/license/cohsh/elphem)
@@ -45,15 +24,18 @@
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - direct and reciprocal lattice vectors from lattice constants with optimization.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
-- first-order electron-phonon couplings.
+- first-order electron-phonon interactions with
+    - Bloch coupling constants.
+    - Nordheim coupling constants.
+    - Bardeen coupling constants.
 - one-electron self-energies.
 - spectral functions.
 
 ## Examples
 ### Calculation of spectral functions (`examples/spectrum.py`)
 ![spectrum](images/spectrum.png)
 
@@ -76,15 +58,15 @@
     n_q = [6, 6, 6]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
-    temperature = 0.8 * debye_temperature
+    temperature = 300.0
     n_bands_elph = 4
 
     # Generate a lattice
     lattice = Lattice3D('bcc', 'Li', a)
 
     # Get k-path
     k_path = lattice.get_k_path(k_names, n_split)
@@ -92,15 +74,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
 
     # Set frequencies
     n_omega = 200
     range_omega = [-6 * Energy.EV["->"], 20 * Energy.EV["->"]]
     omega_array = np.linspace(range_omega[0] , range_omega[1], n_omega)
     
     # Calculate a spectral function
@@ -119,15 +101,15 @@
     ax.set_xticks(k_path.major_scales)
     ax.set_xticklabels(k_names)
     
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
     ax.set_title("Spectral function of bcc-Li (Normalized)")
     
     fig.colorbar(mappable, ax=ax)
-    mappable.set_clim(0.00, 0.03)
+    mappable.set_clim(0.00, 0.02)
 
     fig.savefig("spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
 
@@ -284,8 +266,8 @@
 
 ## License
 MIT
 
 ## Author
 Kohei Ishii (The University of Tokyo, Japan)
 
-https://cohsh.github.io
+https://cohsh.github.io
```

### Comparing `elphem-0.3.1/README.md` & `elphem-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: elphem
+Version: 0.3.2
+Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
+Home-page: https://github.com/cohsh/elphem
+Download-URL: https://github.com/cohsh/elphem
+Author: Kohei Ishii
+Author-email: 
+Maintainer: Kohei Ishii
+Maintainer-email: 
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+
 # elphem
 [![Upload Python Package](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/cohsh/elphem/actions/workflows/python-package.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-package.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/elphem)
 ![PyPI - Version](https://img.shields.io/pypi/v/elphem)
 [![Downloads](https://static.pepy.tech/badge/elphem/month)](https://pepy.tech/project/elphem)
 ![GitHub](https://img.shields.io/github/license/cohsh/elphem)
@@ -24,15 +45,18 @@
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - direct and reciprocal lattice vectors from lattice constants with optimization.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
-- first-order electron-phonon couplings.
+- first-order electron-phonon interactions with
+    - Bloch coupling constants.
+    - Nordheim coupling constants.
+    - Bardeen coupling constants.
 - one-electron self-energies.
 - spectral functions.
 
 ## Examples
 ### Calculation of spectral functions (`examples/spectrum.py`)
 ![spectrum](images/spectrum.png)
 
@@ -55,15 +79,15 @@
     n_q = [6, 6, 6]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
-    temperature = 0.8 * debye_temperature
+    temperature = 300.0
     n_bands_elph = 4
 
     # Generate a lattice
     lattice = Lattice3D('bcc', 'Li', a)
 
     # Get k-path
     k_path = lattice.get_k_path(k_names, n_split)
@@ -71,15 +95,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
 
     # Set frequencies
     n_omega = 200
     range_omega = [-6 * Energy.EV["->"], 20 * Energy.EV["->"]]
     omega_array = np.linspace(range_omega[0] , range_omega[1], n_omega)
     
     # Calculate a spectral function
@@ -98,15 +122,15 @@
     ax.set_xticks(k_path.major_scales)
     ax.set_xticklabels(k_names)
     
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
     ax.set_title("Spectral function of bcc-Li (Normalized)")
     
     fig.colorbar(mappable, ax=ax)
-    mappable.set_clim(0.00, 0.03)
+    mappable.set_clim(0.00, 0.02)
 
     fig.savefig("spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
 
@@ -263,8 +287,8 @@
 
 ## License
 MIT
 
 ## Author
 Kohei Ishii (The University of Tokyo, Japan)
 
-https://cohsh.github.io
+https://cohsh.github.io
```

### Comparing `elphem-0.3.1/elphem/common/atomic_weight.py` & `elphem-0.3.2/elphem/common/atomic_weight.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/common/brillouin.py` & `elphem-0.3.2/elphem/common/brillouin.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/common/distribution.py` & `elphem-0.3.2/elphem/common/distribution.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/common/function.py` & `elphem-0.3.2/elphem/common/function.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/common/stdout.py` & `elphem-0.3.2/elphem/common/stdout.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/common/unit.py` & `elphem-0.3.2/elphem/common/unit.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/electron/electron.py` & `elphem-0.3.2/elphem/electron/electron.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         n_electrons (int): Number of electrons per unit cell.
         n_bands (int): Number of energy bands considered.
         n_k (int): Number of k_points.
         g (np.ndarray): Reciprocal lattice vectors.
         k (np.ndarray): Vectors in the reciprocal space.
         eigenenergies (np.ndarray): Eigenenergies of free electron model.
         fermi_energy (float): Fermi energy
+        fermi_wave_number (float): Fermi wave-number
+        thomas_fermi_wave_number (float): Thomas-Fermi wave-number
     """
     
     def __init__(self, lattice: Lattice, n_electrons: int):
         """
         Args:
             lattice (Lattice): Lattice on which the free electron model is applied.
             n_electrons (int): Number of electrons per unit cell.
@@ -30,14 +32,16 @@
         self.n_bands = None
         self.n_k = None
         self.g = None
         self.k = None
         self.eigenenergies = None
 
         self.fermi_energy = self.calculate_fermi_energy()
+        self.fermi_wave_number = self.calculate_fermi_wave_number()
+        self.thomas_fermi_wave_number = self.calculate_thomas_fermi_wave_number()
         
     @classmethod
     def create_from_n(cls, lattice: Lattice, n_electrons: int, n_bands: int, n_k_array: np.ndarray) -> 'Electron':
         """Create free electrons from the number of the number of k (array-type).
 
         Args:
             lattice (Lattice): Lattice on which the free electron model is applied
@@ -213,10 +217,29 @@
         Returns:
             float: The Fermi energy.
         """
         gamma = math.gamma(self.lattice.n_dim / 2.0 + 1.0)
         coefficient = 2.0 * np.pi
         electron_density = self.n_electrons / self.lattice.primitive.volume
         
-        fermi_energy = coefficient * (0.5 * gamma * electron_density) ** (2.0 / self.lattice.n_dim)
+        return coefficient * (0.5 * gamma * electron_density) ** (2.0 / self.lattice.n_dim)
+    
+    def calculate_fermi_wave_number(self) -> float:
+        """Calculate the Fermi wave-number from Fermi energy.
+
+        Returns:
+            float: The Fermi wave-number
+        """
+        
+        return np.sqrt(2.0 * self.fermi_energy)
+    
+    def calculate_thomas_fermi_wave_number(self) -> float:
+        """Calculate the Thomas-Fermi wave-number from Fermi wave-number
+
+        Returns:
+            float: The Thomas-Fermi wave-number
+        """
+        
+        coefficient = 4.0 / np.pi * (4.0 / (9.0 * np.pi)) ** (1.0 / 3.0)
+        r = (self.lattice.primitive.volume * math.gamma(self.lattice.n_dim / 2.0 + 1.0) / (self.n_electrons * np.pi ** (self.lattice.n_dim / 2.0))) ** (1.0 / self.lattice.n_dim)
         
-        return fermi_energy
+        return coefficient * r * self.fermi_wave_number ** 2
```

### Comparing `elphem-0.3.1/elphem/elph/electron_phonon.py` & `elphem-0.3.2/elphem/elph/electron_phonon.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,17 @@
         electron (Electron): Free electron for initial and final states
         electron_inter (Electron): Free electron for intermediate states
         phonon (Phonon): Debye Phonon
         green_function (GreenFunction): Green function
         couplings (np.ndarray): electron-phonon coupling constants squared
     """
     def __init__(self, electron: Electron, phonon: Phonon, temperature: float, n_bands: int,
-                sigma: float = 0.001, eta: float = 0.0005,
-                effective_potential: float = 0.0625):
+                sigma: float = 0.001, eta: float = 0.0005, coupling_type: str = "bardeen"):
         self.n_dim = electron.lattice.n_dim
         self.temperature = temperature
-        self.effective_potential = effective_potential
         if n_bands > electron.n_bands:
             self.n_bands = electron.n_bands
         else:
             self.n_bands = n_bands
 
         self.eigenenergies = electron.eigenenergies[0:self.n_bands, :]
         
@@ -43,15 +41,15 @@
         self.electron_inter = electron.clone_with_gk_grid(g2, k + q)
         self.phonon = phonon.clone_with_q_grid(q)
         
         # set Green function
         self.green_function = GreenFunction(self.electron_inter, self.phonon, self.temperature, sigma, eta)
 
         # set electron-phonon coupling constants squared
-        self.coupling2 = np.abs(self.calculate_couplings()) ** 2
+        self.coupling2 = np.abs(self.calculate_couplings(coupling_type)) ** 2
 
     def create_ggkq_grid(self, electron: Electron, phonon: Phonon) -> tuple:
         """Create (G_!, G_2, k, q) combined grids
 
         Args:
             electron (Electron): Free electron
             phonon (Phonon): Debye phonon
@@ -64,21 +62,60 @@
         g1 = np.broadcast_to(electron.g[:self.n_bands, np.newaxis, np.newaxis, np.newaxis, :], shape)
         g2 = np.broadcast_to(electron.g[np.newaxis, :, np.newaxis, np.newaxis, :], shape)
         k = np.broadcast_to(electron.k[np.newaxis, np.newaxis, :, np.newaxis, :], shape)
         q = np.broadcast_to(phonon.q[np.newaxis, np.newaxis, np.newaxis, :, :], shape)
         
         return g1, g2, k, q
 
-    def calculate_couplings(self) -> np.ndarray:
-        """Calculate the lowest-order electron-phonon coupling constants.
+    def calculate_couplings(self, coupling_type: str) -> np.ndarray:
+        if coupling_type == "bloch":
+            return self.calculate_couplings_bloch()
+        elif coupling_type == "nordheim":
+            return self.calculate_couplings_nordheim()
+        elif coupling_type == "bardeen":
+            return self.calculate_couplings_bardeen()
+        else:
+            raise ValueError("coupling_type is invalid.")
+
+    def calculate_couplings_bloch(self) -> np.ndarray:
+        """Calculate the Bloch (1929) electron-phonon coupling constants.
+
+        Returns:
+            np.ndarray: The lowest-order electron-phonon coupling constants
+        """
+        potential = 1.0 / 16.0
+        
+        return -1.0j * potential * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+
+    def calculate_couplings_nordheim(self) -> np.ndarray:
+        """Calculate the Nordheim (1931) electron-phonon coupling constants.
 
         Returns:
             np.ndarray: The lowest-order electron-phonon coupling constants
         """
-        return -1.0j * self.effective_potential * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+        potential = 4.0 / self.electron.lattice.primitive.volume * self.electron.n_electrons * np.pi / ( np.nansum(self.phonon.q + self.electron.g - self.electron_inter.g, axis=-1) ** 2)
+        
+        return -1.0j * potential * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+
+    def calculate_couplings_bardeen(self) -> np.ndarray:
+        """Calculate the Bardeen (1937) electron-phonon coupling constants.
+
+        Returns:
+            np.ndarray: The lowest-order electron-phonon coupling constants
+        """
+        wave_number = np.nansum(self.phonon.q + self.electron.g - self.electron_inter.g, axis=-1)
+
+        numerator = 4.0 * self.electron.n_electrons * np.pi
+        denominator = wave_number ** 2 + self.electron.thomas_fermi_wave_number ** 2 * self.calculate_lindhard_function(wave_number / (2.0 * self.electron.fermi_wave_number))
+        
+        return -1.0j / self.electron.lattice.primitive.volume * numerator / denominator * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+    
+    @staticmethod
+    def calculate_lindhard_function(x: np.ndarray) -> np.ndarray:
+        return 0.5 + (1.0 - x ** 2) / (4.0 * x) * np.log(np.abs(1.0 + x) / np.abs(1.0 - x))
 
     def calculate_self_energies(self, omega: float) -> np.ndarray:
         """Calculate Fan self-energies.
 
         Args:
             omega (float): a frequency.
```

### Comparing `elphem-0.3.1/elphem/elph/green_function.py` & `elphem-0.3.2/elphem/elph/green_function.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/cell.py` & `elphem-0.3.2/elphem/lattice/cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/lattice.py` & `elphem-0.3.2/elphem/lattice/lattice.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/lattice_constant.py` & `elphem-0.3.2/elphem/lattice/lattice_constant.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/primitive_cell.py` & `elphem-0.3.2/elphem/lattice/primitive_cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/reciprocal_cell.py` & `elphem-0.3.2/elphem/lattice/reciprocal_cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/lattice/rotation.py` & `elphem-0.3.2/elphem/lattice/rotation.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem/phonon/phonon.py` & `elphem-0.3.2/elphem/phonon/phonon.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/elphem.egg-info/PKG-INFO` & `elphem-0.3.2/elphem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elphem
-Version: 0.3.1
+Version: 0.3.2
 Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
 Home-page: https://github.com/cohsh/elphem
 Download-URL: https://github.com/cohsh/elphem
 Author: Kohei Ishii
 Author-email: 
 Maintainer: Kohei Ishii
 Maintainer-email: 
@@ -45,15 +45,18 @@
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - direct and reciprocal lattice vectors from lattice constants with optimization.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
-- first-order electron-phonon couplings.
+- first-order electron-phonon interactions with
+    - Bloch coupling constants.
+    - Nordheim coupling constants.
+    - Bardeen coupling constants.
 - one-electron self-energies.
 - spectral functions.
 
 ## Examples
 ### Calculation of spectral functions (`examples/spectrum.py`)
 ![spectrum](images/spectrum.png)
 
@@ -76,15 +79,15 @@
     n_q = [6, 6, 6]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
-    temperature = 0.8 * debye_temperature
+    temperature = 300.0
     n_bands_elph = 4
 
     # Generate a lattice
     lattice = Lattice3D('bcc', 'Li', a)
 
     # Get k-path
     k_path = lattice.get_k_path(k_names, n_split)
@@ -92,15 +95,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
 
     # Set frequencies
     n_omega = 200
     range_omega = [-6 * Energy.EV["->"], 20 * Energy.EV["->"]]
     omega_array = np.linspace(range_omega[0] , range_omega[1], n_omega)
     
     # Calculate a spectral function
@@ -119,15 +122,15 @@
     ax.set_xticks(k_path.major_scales)
     ax.set_xticklabels(k_names)
     
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
     ax.set_title("Spectral function of bcc-Li (Normalized)")
     
     fig.colorbar(mappable, ax=ax)
-    mappable.set_clim(0.00, 0.03)
+    mappable.set_clim(0.00, 0.02)
 
     fig.savefig("spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `elphem-0.3.1/elphem.egg-info/SOURCES.txt` & `elphem-0.3.2/elphem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/setup.py` & `elphem-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = 'Elphem: Calculating electron-phonon interactions with the empty lattice.'
 NAME = 'elphem'
 AUTHOR = 'Kohei Ishii'
 AUTHOR_EMAIL = ''
 URL = 'https://github.com/cohsh/elphem'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = ['numpy', 'scipy']
 
 CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.10',
```

### Comparing `elphem-0.3.1/tests/common/test_brillouin.py` & `elphem-0.3.2/tests/common/test_brillouin.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/tests/common/test_unit.py` & `elphem-0.3.2/tests/common/test_unit.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/tests/electron/test_electron.py` & `elphem-0.3.2/tests/electron/test_electron.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/tests/elph/test_self_energy.py` & `elphem-0.3.2/tests/elph/test_self_energy.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/tests/lattice/test_lattice.py` & `elphem-0.3.2/tests/lattice/test_lattice.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.1/tests/phonon/test_phonon.py` & `elphem-0.3.2/tests/phonon/test_phonon.py`

 * *Files identical despite different names*

