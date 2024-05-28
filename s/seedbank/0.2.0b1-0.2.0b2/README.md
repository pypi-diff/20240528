# Comparing `tmp/seedbank-0.2.0b1.tar.gz` & `tmp/seedbank-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedbank-0.2.0b1.tar", last modified: Fri May 24 07:53:34 2024, max compression
+gzip compressed data, was "seedbank-0.2.0b2.tar", last modified: Tue May 28 20:45:57 2024, max compression
```

## Comparing `seedbank-0.2.0b1.tar` & `seedbank-0.2.0b2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.376944 seedbank-0.2.0b1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.376944 seedbank-0.2.0b1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/patterns.rst
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.380944 seedbank-0.2.0b1/seedbank/
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.384944 seedbank-0.2.0b1/seedbank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.384944 seedbank-0.2.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_cupy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_derive.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_init_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_process_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_randomstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.859967 seedbank-0.2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-28 20:45:57.855967 seedbank-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.847967 seedbank-0.2.0b2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.847967 seedbank-0.2.0b2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/docs/patterns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.851967 seedbank-0.2.0b2/seedbank/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/seedbank/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.855967 seedbank-0.2.0b2/seedbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-28 20:45:57.000000 seedbank-0.2.0b2/seedbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 20:45:57.000000 seedbank-0.2.0b2/seedbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:45:57.000000 seedbank-0.2.0b2/seedbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 20:45:57.000000 seedbank-0.2.0b2/seedbank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 20:45:57.000000 seedbank-0.2.0b2/seedbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:45:57.859967 seedbank-0.2.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:45:57.855967 seedbank-0.2.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/init_seed.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/init_seed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/init_seed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_cupy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_derive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_init_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_process_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_randomstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-28 20:45:52.000000 seedbank-0.2.0b2/tests/test_stdlib.py
```

### Comparing `seedbank-0.2.0b1/.gitignore` & `seedbank-0.2.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/CITATION.cff` & `seedbank-0.2.0b2/CITATION.cff`

 * *Files 15% similar despite different names*

```diff
@@ -7,12 +7,16 @@
 authors:
     - given-names: Michael D.
       family-names: Ekstrand
       email: ekstrand@acm.org
       orcid: "https://orcid.org/0000-0003-2467-0108"
 repository-code: "https://github.com/lenskit/seedbank"
 url: "https://seedbank.lenskit.org"
+identifiers:
+    - type: doi
+      value: "10.5281/zenodo.11276060"
+      description: All versions
 keywords:
     - random numbers
 license: MIT
 version: 0.1.3
 date-released: "2023-09-28"
```

### Comparing `seedbank-0.2.0b1/LICENSE.md` & `seedbank-0.2.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/PKG-INFO` & `seedbank-0.2.0b2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
         Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -100,29 +100,23 @@
 
 In addition, it will initialize a root seed for constructing new-style NumPy `Generator` instances.
 
 If SeedBank doesn’t support your RNG yet, please submit a pull request!
 
 ## Developing SeedBank
 
-SeedBank uses Flit for managing dependencies.  To set up in a fresh
-virtual environment:
+The easiest way to set up your environment to develop seedbank is to install
+`uv` and `just`, and run:
 
-    python -m pip install flit
-    flit install --pth-file
+    uv venv create
+    just install-dev
 
-[conda-lock][] can help you set up a Conda environment (replace `linux-64` with your platform):
+You can also set up dev dependencies with `pip`:
 
-    # install conda-lock in base environment
-    # alternatively: pip install conda-lock
-    conda install -c conda-forge conda-lock
-    # create the lock file
-    conda-lock -p linux-64 -f pyproject.toml
-    # create the environment
-    conda env create -n seedbank -f conda-linux-64.lock
+    pip install -e '.[dev,test,doc]
 
 ## Acknowledgements
 
 This material is based upon work supported by the National Science Foundation
 under Grant No. IIS 17-51278. Any opinions, findings, and conclusions or
 recommendations expressed in this material are those of the author(s) and do not
 necessarily reflect the views of the National Science Foundation.
```

### Comparing `seedbank-0.2.0b1/README.md` & `seedbank-0.2.0b2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -27,29 +27,23 @@
 
 In addition, it will initialize a root seed for constructing new-style NumPy `Generator` instances.
 
 If SeedBank doesn’t support your RNG yet, please submit a pull request!
 
 ## Developing SeedBank
 
-SeedBank uses Flit for managing dependencies.  To set up in a fresh
-virtual environment:
+The easiest way to set up your environment to develop seedbank is to install
+`uv` and `just`, and run:
 
-    python -m pip install flit
-    flit install --pth-file
+    uv venv create
+    just install-dev
 
-[conda-lock][] can help you set up a Conda environment (replace `linux-64` with your platform):
+You can also set up dev dependencies with `pip`:
 
-    # install conda-lock in base environment
-    # alternatively: pip install conda-lock
-    conda install -c conda-forge conda-lock
-    # create the lock file
-    conda-lock -p linux-64 -f pyproject.toml
-    # create the environment
-    conda env create -n seedbank -f conda-linux-64.lock
+    pip install -e '.[dev,test,doc]
 
 ## Acknowledgements
 
 This material is based upon work supported by the National Science Foundation
 under Grant No. IIS 17-51278. Any opinions, findings, and conclusions or
 recommendations expressed in this material are those of the author(s) and do not
 necessarily reflect the views of the National Science Foundation.
```

### Comparing `seedbank-0.2.0b1/docs/_templates/footer.html` & `seedbank-0.2.0b2/docs/_templates/footer.html`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/docs/api.rst` & `seedbank-0.2.0b2/docs/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -61,10 +61,11 @@
 
 SeedBank provides functions for obtaining RNGs of various types.  These functions take seeds that
 override the global seed to support seed-specifying APIs.
 
 Packages that expect their client code to use SeedBank to seed the random number ecosystem should
 use these functions to obtain random number generators.
 
+.. autofunction:: std_rng
 .. autofunction:: numpy_rng
 .. autofunction:: numpy_random_state
 .. autofunction:: cupy_rng
```

### Comparing `seedbank-0.2.0b1/docs/conf.py` & `seedbank-0.2.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/docs/extending.rst` & `seedbank-0.2.0b2/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/docs/index.rst` & `seedbank-0.2.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/docs/patterns.rst` & `seedbank-0.2.0b2/docs/patterns.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/justfile` & `seedbank-0.2.0b2/justfile`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/pyproject.toml` & `seedbank-0.2.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/__init__.py` & `seedbank-0.2.0b2/seedbank/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 _root_state = SeedState()
 
 __all__ = [
     "make_seed",
     "initialize",
     "init_file",
     "derive_seed",
+    "std_rng",
     "numpy_rng",
     "numpy_random_state",
     "cupy_rng",
     "SeedLike",
 ]
 
 # This list contains the modules that initialize seeds.
@@ -132,7 +133,8 @@
     else:
         return seed.generate_state(words)
 
 
 from seedbank._config import init_file  # noqa: E402
 from seedbank.cupy import cupy_rng  # noqa: E402
 from seedbank.numpy import numpy_random_state, numpy_rng  # noqa: E402
+from seedbank.stdlib import std_rng  # noqa: E402
```

### Comparing `seedbank-0.2.0b1/seedbank/_config.py` & `seedbank-0.2.0b2/seedbank/_config.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/_keys.py` & `seedbank-0.2.0b2/seedbank/_keys.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/_state.py` & `seedbank-0.2.0b2/seedbank/_state.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/cupy.py` & `seedbank-0.2.0b2/seedbank/cupy.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/numba.py` & `seedbank-0.2.0b2/seedbank/numba.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/numpy.py` & `seedbank-0.2.0b2/seedbank/numpy.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank/tensorflow.py` & `seedbank-0.2.0b2/seedbank/tensorflow.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/seedbank.egg-info/PKG-INFO` & `seedbank-0.2.0b2/seedbank.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
         Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -100,29 +100,23 @@
 
 In addition, it will initialize a root seed for constructing new-style NumPy `Generator` instances.
 
 If SeedBank doesn’t support your RNG yet, please submit a pull request!
 
 ## Developing SeedBank
 
-SeedBank uses Flit for managing dependencies.  To set up in a fresh
-virtual environment:
+The easiest way to set up your environment to develop seedbank is to install
+`uv` and `just`, and run:
 
-    python -m pip install flit
-    flit install --pth-file
+    uv venv create
+    just install-dev
 
-[conda-lock][] can help you set up a Conda environment (replace `linux-64` with your platform):
+You can also set up dev dependencies with `pip`:
 
-    # install conda-lock in base environment
-    # alternatively: pip install conda-lock
-    conda install -c conda-forge conda-lock
-    # create the lock file
-    conda-lock -p linux-64 -f pyproject.toml
-    # create the environment
-    conda env create -n seedbank -f conda-linux-64.lock
+    pip install -e '.[dev,test,doc]
 
 ## Acknowledgements
 
 This material is based upon work supported by the National Science Foundation
 under Grant No. IIS 17-51278. Any opinions, findings, and conclusions or
 recommendations expressed in this material are those of the author(s) and do not
 necessarily reflect the views of the National Science Foundation.
```

### Comparing `seedbank-0.2.0b1/seedbank.egg-info/SOURCES.txt` & `seedbank-0.2.0b2/seedbank.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 tests/test_cupy_generator.py
 tests/test_derive.py
 tests/test_generator.py
 tests/test_init.py
 tests/test_init_file.py
 tests/test_numba.py
 tests/test_process_seed.py
-tests/test_randomstate.py
+tests/test_randomstate.py
+tests/test_stdlib.py
```

### Comparing `seedbank-0.2.0b1/tests/test_cupy_generator.py` & `seedbank-0.2.0b2/tests/test_cupy_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_derive.py` & `seedbank-0.2.0b2/tests/test_derive.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_generator.py` & `seedbank-0.2.0b2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_init.py` & `seedbank-0.2.0b2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_init_file.py` & `seedbank-0.2.0b2/tests/test_init_file.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_process_seed.py` & `seedbank-0.2.0b2/tests/test_process_seed.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0b1/tests/test_randomstate.py` & `seedbank-0.2.0b2/tests/test_randomstate.py`

 * *Files identical despite different names*

