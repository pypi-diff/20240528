# Comparing `tmp/ritas-0.2.0.tar.gz` & `tmp/ritas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritas-0.2.0.tar", last modified: Fri Feb 23 15:26:13 2024, max compression
+gzip compressed data, was "ritas-0.3.0.tar", last modified: Tue May 28 13:04:24 2024, max compression
```

## Comparing `ritas-0.2.0.tar` & `ritas-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.388325 ritas-0.2.0/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       65 2023-12-14 14:52:38.000000 ritas-0.2.0/.gitattributes
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.381325 ritas-0.2.0/.github/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.383325 ritas-0.2.0/.github/workflows/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1197 2024-02-19 20:09:56.000000 ritas-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2765 2024-02-19 16:14:39.000000 ritas-0.2.0/.gitignore
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1143 2024-02-19 21:36:54.000000 ritas-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      509 2024-02-23 15:25:57.000000 ritas-0.2.0/CHANGELOG.md
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1068 2023-12-14 14:52:38.000000 ritas-0.2.0/LICENSE
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       28 2024-02-19 20:09:56.000000 ritas-0.2.0/MANIFEST.in
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1829 2024-02-23 15:26:13.388325 ritas-0.2.0/PKG-INFO
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1061 2024-02-22 16:35:56.000000 ritas-0.2.0/README.md
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      187 2024-02-19 20:09:56.000000 ritas-0.2.0/environment.yml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2346 2024-02-21 16:09:28.000000 ritas-0.2.0/pyproject.toml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       38 2024-02-23 15:26:13.388325 ritas-0.2.0/setup.cfg
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       80 2024-02-19 20:09:56.000000 ritas-0.2.0/setup.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.381325 ritas-0.2.0/src/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.385325 ritas-0.2.0/src/ritas/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      374 2024-02-19 20:09:56.000000 ritas-0.2.0/src/ritas/__init__.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.386325 ritas-0.2.0/src/ritas/app/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.386325 ritas-0.2.0/src/ritas/app/.streamlit/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      102 2023-12-14 14:52:38.000000 ritas-0.2.0/src/ritas/app/.streamlit/config.toml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        0 2023-12-14 14:52:38.000000 ritas-0.2.0/src/ritas/app/__init__.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2867 2024-02-21 16:09:28.000000 ritas-0.2.0/src/ritas/app/app.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      636 2024-02-22 16:35:56.000000 ritas-0.2.0/src/ritas/cli.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      295 2024-02-22 16:35:56.000000 ritas-0.2.0/src/ritas/io.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1757 2024-02-21 16:09:28.000000 ritas-0.2.0/src/ritas/main.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    21740 2024-02-21 16:09:28.000000 ritas-0.2.0/src/ritas/polygons.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4568 2024-02-21 16:09:28.000000 ritas-0.2.0/src/ritas/utils.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3542 2024-02-21 16:09:28.000000 ritas-0.2.0/src/ritas/viz.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      732 2024-02-22 16:35:56.000000 ritas-0.2.0/src/ritas/workflows.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.387325 ritas-0.2.0/src/ritas.egg-info/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1829 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/PKG-INFO
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      681 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/SOURCES.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        1 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/dependency_links.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       41 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/entry_points.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       80 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/requires.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        6 2024-02-23 15:26:13.000000 ritas-0.2.0/src/ritas.egg-info/top_level.txt
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.387325 ritas-0.2.0/tests/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        0 2023-12-14 14:52:38.000000 ritas-0.2.0/tests/__init__.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-02-23 15:26:13.387325 ritas-0.2.0/tests/data/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2417 2024-02-22 16:35:56.000000 ritas-0.2.0/tests/data/square_100m.csv
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      399 2024-02-22 16:35:56.000000 ritas-0.2.0/tests/test_cli.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3705 2024-02-21 16:09:28.000000 ritas-0.2.0/tests/test_polygons.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.147187 ritas-0.3.0/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       65 2024-03-22 15:13:46.000000 ritas-0.3.0/.gitattributes
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.138187 ritas-0.3.0/.github/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.140187 ritas-0.3.0/.github/workflows/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1770 2024-03-25 16:32:39.000000 ritas-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      740 2024-03-28 17:01:23.000000 ritas-0.3.0/.gitignore
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1142 2024-05-28 13:03:25.000000 ritas-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      947 2024-05-28 13:03:25.000000 ritas-0.3.0/CHANGELOG.md
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1068 2024-03-22 15:13:46.000000 ritas-0.3.0/LICENSE
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       28 2024-03-22 15:13:46.000000 ritas-0.3.0/MANIFEST.in
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1853 2024-05-28 13:04:24.147187 ritas-0.3.0/PKG-INFO
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1061 2024-03-22 15:13:46.000000 ritas-0.3.0/README.md
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.141187 ritas-0.3.0/docs/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      638 2024-03-25 16:18:18.000000 ritas-0.3.0/docs/Makefile
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      769 2024-03-25 16:18:18.000000 ritas-0.3.0/docs/make.bat
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.141187 ritas-0.3.0/docs/source/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      906 2024-03-25 16:18:18.000000 ritas-0.3.0/docs/source/conf.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      437 2024-03-25 16:18:18.000000 ritas-0.3.0/docs/source/index.rst
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      224 2024-03-26 16:06:18.000000 ritas-0.3.0/environment.yml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2403 2024-03-26 16:06:18.000000 ritas-0.3.0/pyproject.toml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       38 2024-05-28 13:04:24.147187 ritas-0.3.0/setup.cfg
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       81 2024-03-22 15:13:46.000000 ritas-0.3.0/setup.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.139187 ritas-0.3.0/src/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.144187 ritas-0.3.0/src/ritas/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      750 2024-03-29 16:49:48.000000 ritas-0.3.0/src/ritas/__init__.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.145187 ritas-0.3.0/src/ritas/app/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.145187 ritas-0.3.0/src/ritas/app/.streamlit/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      102 2024-03-22 15:13:46.000000 ritas-0.3.0/src/ritas/app/.streamlit/config.toml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        0 2024-03-22 15:13:46.000000 ritas-0.3.0/src/ritas/app/__init__.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2917 2024-05-28 13:03:25.000000 ritas-0.3.0/src/ritas/app/app.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1047 2024-03-28 17:01:23.000000 ritas-0.3.0/src/ritas/cli.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2137 2024-03-29 16:49:48.000000 ritas-0.3.0/src/ritas/io.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1565 2024-03-28 17:01:23.000000 ritas-0.3.0/src/ritas/main.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    21087 2024-03-29 16:49:48.000000 ritas-0.3.0/src/ritas/polygons.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4573 2024-03-28 17:01:23.000000 ritas-0.3.0/src/ritas/utils.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3542 2024-03-28 17:01:23.000000 ritas-0.3.0/src/ritas/viz.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1180 2024-03-28 17:01:23.000000 ritas-0.3.0/src/ritas/workflows.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.147187 ritas-0.3.0/src/ritas.egg-info/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1853 2024-05-28 13:04:23.000000 ritas-0.3.0/src/ritas.egg-info/PKG-INFO
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      751 2024-05-28 13:04:24.000000 ritas-0.3.0/src/ritas.egg-info/SOURCES.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        1 2024-05-28 13:04:23.000000 ritas-0.3.0/src/ritas.egg-info/dependency_links.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       41 2024-05-28 13:04:23.000000 ritas-0.3.0/src/ritas.egg-info/entry_points.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       89 2024-05-28 13:04:23.000000 ritas-0.3.0/src/ritas.egg-info/requires.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        6 2024-05-28 13:04:23.000000 ritas-0.3.0/src/ritas.egg-info/top_level.txt
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.146187 ritas-0.3.0/tests/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        0 2024-03-22 15:13:46.000000 ritas-0.3.0/tests/__init__.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-28 13:04:24.146187 ritas-0.3.0/tests/data/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2417 2024-03-26 15:17:31.000000 ritas-0.3.0/tests/data/square_100m.csv
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      789 2024-03-26 16:06:18.000000 ritas-0.3.0/tests/test_cli.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2693 2024-03-28 17:01:23.000000 ritas-0.3.0/tests/test_polygons.py
```

### Comparing `ritas-0.2.0/.github/workflows/ci.yml` & `ritas-0.3.0/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 name: CI
 on: [push, pull_request]
 
+# Allow actions to write to the repository
+permissions:
+  contents: write
+
 jobs:
   build-and-test:
     defaults:
       run:
         # Ensure environment gets sourced between steps
         shell: bash -l {0}
     name: Python (${{ matrix.python-version }})
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.9", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v4
 
-          # setup conda-forge with micromamba
+    # setup conda-forge with micromamba
     - name: Setup Python
       uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: environment.yml
         condarc: |
           channels:
             - conda-forge
@@ -43,7 +47,21 @@
     - name: Upload coverage
       if: ${{ matrix.python-version == '3.12' }}
       uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: true
         token: ${{ secrets.CODECOV_TOKEN }}
         files: coverage.xml
+
+    - name: Build docs
+      run: |
+        set -e
+        cd docs
+        make html
+
+    # This is somewhat suboptimal
+    - name: Deploy docs
+      if: ${{ matrix.python-version == '3.12' && github.event_name == 'push' && github.ref == 'refs/heads/main'}}
+      uses: JamesIves/github-pages-deploy-action@v4
+      with:
+        branch: gh-pages # The branch the action should deploy to.
+        folder: docs/build/html # The folder the action should deploy. This example folder is generated by Sphinx
```

### Comparing `ritas-0.2.0/.pre-commit-config.yaml` & `ritas-0.3.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-executables-have-shebangs
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
         types: [python]
       - id: trailing-whitespace
       - id: requirements-txt-fixer
 
   - repo: https://github.com/MarcoGorelli/auto-walrus
-    rev: v0.2.2
+    rev: 0.3.4
     hooks:
       - id: auto-walrus
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.4.5
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
 
   #- repo: https://github.com/codespell-project/codespell
   #  rev: v2.2.6
   #  hooks:
   #    - id: codespell
   #      additional_dependencies:
   #        - tomli
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: '1.7.0'
+    rev: '2.1.3'
     hooks:
       - id: pyproject-fmt
 
   #- repo: https://github.com/pre-commit/mirrors-mypy
   #  rev: v1.6.0
   #  hooks:
   #    - id: mypy
```

### Comparing `ritas-0.2.0/LICENSE` & `ritas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ritas-0.2.0/PKG-INFO` & `ritas-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritas
-Version: 0.2.0
+Version: 0.3.0
 License: MIT License
         
         Copyright (c) 2023 Jarad Niemi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,10 +33,11 @@
 Requires-Dist: click
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pykrige
 Requires-Dist: pyproj
+Requires-Dist: rasterio
 Requires-Dist: shapely
 Requires-Dist: streamlit
 Requires-Dist: tqdm
```

### Comparing `ritas-0.2.0/README.md` & `ritas-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ritas-0.2.0/pyproject.toml` & `ritas-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   "click",
   "geopandas",
   "matplotlib",
   "pandas",
   "pyarrow",
   "pykrige",
   "pyproj",
+  "rasterio",
   "shapely",
   "streamlit",
   "tqdm",
 ]
 dynamic = [
   "version",
 ]
@@ -96,14 +97,15 @@
 
 [tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 
 [tool.ruff.lint.per-file-ignores]
+'docs/source/conf.py' = ['INP001', 'A001']
 'tests/*' = ['ARG', 'PT011', 'S101', 'PLR2004',]
 
 
 [tool.ruff.lint.pylint]
 max-args = 15
 max-branches = 20
 max-returns = 10
```

### Comparing `ritas-0.2.0/src/ritas/app/app.py` & `ritas-0.3.0/src/ritas/app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import geopandas as gpd
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 import streamlit as st
 
 from ritas.polygons import (
     chop_polygons,
     make_grid,
     make_vehicle_polygons,
     reshape_polygons,
 )
 from ritas.viz import plot_coordinates, plot_map
 
 
 def main() -> None:
     st.title("RITAS")
-
+    reshaped_geodf = None
+    aggregate_polygons = None
     with st.form("upload_form"):
         st.header("Upload Data File")
         data_file = st.file_uploader("Choose a CSV file", type="csv")
         proj4 = st.text_input("Enter the proj4 string")
         submit = st.form_submit_button("Submit")
 
         if submit:
```

### Comparing `ritas-0.2.0/src/ritas/main.py` & `ritas-0.3.0/src/ritas/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 import argparse
-import logging
 from typing import Any
 
 import matplotlib.pyplot as plt
 import pandas as pd
 
+from ritas import LOG
 from ritas.polygons import make_vehicle_polygons, reshape_polygons
 from ritas.viz import plot_coordinates, plot_map
 
 
-def setup_logging() -> None:
-    logging.basicConfig(
-        level=logging.INFO,
-        format="%(asctime)s - %(levelname)s - %(message)s",
-    )
-
-
 def main(args: Any) -> None:
-    logging.info("Reading CSV file from %s", args.input_csv)
+    LOG.info("Reading CSV file from %s", args.input_csv)
     df = pd.read_csv(args.input_csv)
 
-    logging.info("Using Proj4 string: %s", args.proj4string)
+    LOG.info("Using Proj4 string: %s", args.proj4string)
     proj4string = args.proj4string
 
-    logging.info("Plotting coordinates.")
+    LOG.info("Plotting coordinates.")
     plot_coordinates(df)
 
-    logging.info("Creating vehicle polygons.")
+    LOG.info("Creating vehicle polygons.")
     geodf = make_vehicle_polygons(df, proj4string=proj4string)
 
-    logging.info("Reshaping polygons.")
+    LOG.info("Reshaping polygons.")
     reshaped_geodf = reshape_polygons(geodf)
 
-    logging.info("Creating plots.")
+    LOG.info("Creating plots.")
     # Start by creating a single figure and two axes
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(15, 5))  # 1 row, 2 columns
 
     # Plot on the first axes, ignore the returned figure
     _, ax1 = plot_map(geodf, ax=ax1, title="Original Polygons")
     # Plot on the second axes, ignore the returned figure
     _, ax2 = plot_map(reshaped_geodf, ax=ax2, title="Reshaped Polygons")
 
     plt.tight_layout()
-    logging.info("Displaying plots.")
+    LOG.info("Displaying plots.")
     plt.show()
 
 
 if __name__ == "__main__":
-    setup_logging()
-
     parser = argparse.ArgumentParser(
         description="Process and visualize vehicle polygons."
     )
     parser.add_argument("input_csv", help="Path to the input CSV file.")
     parser.add_argument(
         "proj4string",
         help="Proj4 string for the coordinate reference system",
```

### Comparing `ritas-0.2.0/src/ritas/polygons.py` & `ritas-0.3.0/src/ritas/polygons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import warnings
 from typing import Callable, Optional, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from pykrige.ok import OrdinaryKriging
@@ -11,25 +10,22 @@
 from shapely.geometry import (
     MultiPolygon,
     Polygon,
     box,
 )
 from tqdm import tqdm
 
+from ritas import LOG, ColNames
 from ritas.utils import (
-    convert_to_utm,
-    is_in_utm_range,
     lognormal_to_normal,
     yield_equation_mgha,
 )
 
 warnings.filterwarnings("ignore")
 
-logging.basicConfig(level=logging.INFO)
-
 
 def make_bounding_box(
     x: np.ndarray,
     y: np.ndarray,
     w: np.ndarray,
     d: np.ndarray,
 ) -> pd.DataFrame:
@@ -53,15 +49,15 @@
 
     Note:
         `w` MUST BE IN METERS.
     """
     if not (len(x) == len(y) == len(w) == len(d)):
         raise ValueError("All input arrays must be of the same length.")
 
-    logging.info("Running make_bounding_box...")
+    LOG.info("Running make_bounding_box...")
 
     # prepare the input arrays
     x0, x1 = np.r_[np.nan, x[:-1]], x
     y0, y1 = np.r_[np.nan, y[:-1]], y
 
     # Compute distance of the vertices to the centroid
     h = 0.5 * w  # half width
@@ -114,17 +110,16 @@
             "x12",
             "y12",
         ],
     )
 
 
 def make_vehicle_polygons(
-    df: pd.DataFrame,
+    geodf: gpd.GeoDataFrame,
     proj4string: str,
-    is_utm: bool = True,
 ) -> gpd.GeoDataFrame:
     """
     Create a gpd.GeoDataFrame object from the dataframe given as an input.
     For each row in the input dataframe, a rectangle is constructed using
     the current and next positions as well as the swath width.
 
     Args:
@@ -132,52 +127,31 @@
             The swath represents the box width and must be in meters.
             Optional column `d` can represent box diagonal length in meters.
         proj4string: The proj4string associated with the system of coordinates
 
     Returns:
         A gpd.GeoDataFrame with one rectangle per row.
     """
-
-    if not isinstance(df, pd.DataFrame):
-        raise TypeError("Input must be a DataFrame.")
-
-    for column in ["x", "y", "swath"]:
-        if column not in df.columns:
-            raise ValueError(
-                f"Missing required column '{column}' in the dataframe."
-            )
-
     if not isinstance(proj4string, str):
         raise ValueError("The proj4string must be a string.")
 
-    if "d" not in df.columns:
-        df["d"] = np.nan
-
     try:
         CRS(proj4string)
     except CRSError as e:
         raise ValueError(f"Invalid proj4string: {e}") from e
 
-    if not is_in_utm_range(df["x"].values, df["y"].values):
-        raise ValueError("Coordinates are not in UTM range.")
-
-    if not is_utm:
-        df["x"], df["y"] = convert_to_utm(
-            df["x"].values, df["y"].values, proj4string
-        )
-
     # Compute vertices of the rectangles for each coordinate
     bounding_box = make_bounding_box(
-        df["x"].values,
-        df["y"].values,
-        df["swath"].values,
-        df["d"].values,
+        geodf.geometry.x,
+        geodf.geometry.y,
+        geodf[ColNames.SWATH].values,
+        geodf[ColNames.DISTANCE].values,
     )
 
-    df = pd.concat([df, bounding_box], axis=1)
+    df = pd.concat([geodf, bounding_box], axis=1)
 
     df = df.dropna(
         subset=["x01", "y01", "x02", "y02", "x11", "y11", "x12", "y12"]
     )
 
     polygons = [
         Polygon(
@@ -273,15 +247,15 @@
             overlapping_geometry = spdf.at[idx, "geometry"]
 
             try:
                 cropped = crop_polygon(overlapping_geometry, current_geometry)
                 if cropped:
                     spdf.at[idx, "geometry"] = cropped
             except (ValueError, AttributeError) as e:
-                logging.error(
+                LOG.error(
                     "Error processing geometry at index %s with exception: %s",
                     idx,
                     e,
                 )
                 continue
 
     # Merge adjacent and overlapping polygons
@@ -473,17 +447,17 @@
                             for col in col_weight
                         }
                     )
                     data["originalPolyID"] = poly_row["record"]
                     data["gridPolyID"] = grid_row["id"]
                     data["areaWeight"] = weight
                     data["geometry"] = intersection
-                    data[
-                        "outID"
-                    ] = f"{data['originalPolyID']}-{data['gridPolyID']}"
+                    data["outID"] = (
+                        f"{data['originalPolyID']}-{data['gridPolyID']}"
+                    )
 
                     results.append(data)
 
     chopped_gdf = gpd.GeoDataFrame(
         results,
         columns=list(results[0].keys())
         if results
```

### Comparing `ritas-0.2.0/src/ritas/utils.py` & `ritas-0.3.0/src/ritas/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tbd."""
-import logging
+
 from typing import Union
 
 import numpy as np
 import pyproj
 from pyproj import CRS
 
+from ritas import LOG
+
 Number = Union[int, float]
 ArrayLike = Union[list[Number], np.ndarray]
 
 MIN_LONGITUDE = -180
 MAX_LONGITUDE = 180
 
 
@@ -93,15 +95,15 @@
     kg_to_mg = 0.001  # 1 kilogram = 0.001 megagram
     m2_to_ha = 0.0001  # 1 square meter = 0.0001 hectare
     yield_values = 10 * (mass_kg * kg_to_mg) / (area_m2 * m2_to_ha)
     too_high_yields = (
         yield_values > MAX_YIELD_THRESHOLD
     )  # or some threshold that is considered too high
     if too_high_yields.any():
-        logging.warning(
+        LOG.warning(
             "High yields calculated at indices: %s",
             too_high_yields[too_high_yields].index.tolist(),
         )
 
     return yield_values
```

### Comparing `ritas-0.2.0/src/ritas/viz.py` & `ritas-0.3.0/src/ritas/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import logging
 from pathlib import Path
 from typing import Optional
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import pandas as pd
 from matplotlib.colors import LinearSegmentedColormap
 
+from ritas import LOG
+
 project_dir = Path(__file__).resolve().parents[0].parents[0].parents[0]
 
 green_cm = LinearSegmentedColormap.from_list(
     "green_cm", ["lightgreen", "green", "darkgreen"], N=256
 )
 
 
@@ -36,15 +37,15 @@
     - ... [other parameters are unchanged]
     """
     # Ensure the input is a GeoDataFrame
     if not isinstance(gdf, gpd.GeoDataFrame):
         raise TypeError("gdf must be a GeoDataFrame.")
 
     # Log the beginning of the plotting process
-    logging.info("Creating plot...")
+    LOG.info("Creating plot...")
 
     # Create the plot if no Axes is passed
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
         fig_created = True
     else:
         fig = ax.figure
@@ -82,15 +83,15 @@
     if axis_off:
         ax.set_axis_off()
 
     # Save the figure if a filename is provided and a new figure was created
     if fname is not None and fig_created:
         fig_path = project_dir / "plots" / fname
         fig.savefig(fig_path, dpi=dpi)
-        logging.info("Plot saved to %s", fig_path)
+        LOG.info("Plot saved to %s", fig_path)
 
     return fig, ax
 
 
 def plot_coordinates(data: pd.DataFrame) -> plt:
     """
     Plots latitude and longitude coordinates.
```

### Comparing `ritas-0.2.0/src/ritas.egg-info/PKG-INFO` & `ritas-0.3.0/src/ritas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritas
-Version: 0.2.0
+Version: 0.3.0
 License: MIT License
         
         Copyright (c) 2023 Jarad Niemi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,10 +33,11 @@
 Requires-Dist: click
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pykrige
 Requires-Dist: pyproj
+Requires-Dist: rasterio
 Requires-Dist: shapely
 Requires-Dist: streamlit
 Requires-Dist: tqdm
```

### Comparing `ritas-0.2.0/src/ritas.egg-info/SOURCES.txt` & `ritas-0.3.0/src/ritas.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 pyproject.toml
 setup.py
 .github/workflows/ci.yml
+docs/Makefile
+docs/make.bat
+docs/source/conf.py
+docs/source/index.rst
 src/ritas/__init__.py
 src/ritas/cli.py
 src/ritas/io.py
 src/ritas/main.py
 src/ritas/polygons.py
 src/ritas/utils.py
 src/ritas/viz.py
```

### Comparing `ritas-0.2.0/tests/data/square_100m.csv` & `ritas-0.3.0/tests/data/square_100m.csv`

 * *Files identical despite different names*

### Comparing `ritas-0.2.0/tests/test_polygons.py` & `ritas-0.3.0/tests/test_polygons.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Tests for the polygons module."""
+
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pytest
 from ritas.polygons import make_bounding_box, make_vehicle_polygons
 from shapely.geometry import Polygon
 
 
@@ -54,71 +57,41 @@
 
 
 def test_make_bounding_box_zero_width() -> None:
     x = np.array([1, 2])
     y = np.array([1, 2])
     w = np.array([0, 0])
     d = np.array([np.nan, 3])
-    df = make_bounding_box(x, y, w, d)
+    make_bounding_box(x, y, w, d)
     # Further assertions can be added here
 
 
 # Test cases for make_vehicle_polygons
 def test_make_vehicle_polygons_basic() -> None:
     df = pd.DataFrame(
         {
             "x": [500000, 500010, 500020],  # UTM coordinates
             "y": [4640000, 4640010, 4640020],
             "swath": [2, 2, 2],
             "d": [1, 3, 3],
         },
     )
     proj4string = "+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs"
+    df = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df["x"], df["y"]))
 
     gdf = make_vehicle_polygons(df, proj4string)
     assert len(gdf) == len(df) - 1
     assert all(isinstance(geom, Polygon) for geom in gdf.geometry)
 
 
-def test_make_vehicle_polygons_missing_columns() -> None:
-    df = pd.DataFrame({"x": [1, 3, 5], "y": [1, 2, 1]})
-    proj4string = "+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs"
-    with pytest.raises(ValueError):
-        make_vehicle_polygons(df, proj4string)
-
-
 def test_make_vehicle_polygons_invalid_proj4string() -> None:
     df = pd.DataFrame(
         {
             "x": [1, 3, 5],
             "y": [1, 2, 1],
             "swath": [2, 2, 2],
             "d": [np.nan, 3, 3],
         },
     )
     proj4string = "invalid_proj4string"
     with pytest.raises(ValueError):
         make_vehicle_polygons(df, proj4string)
-
-
-def test_make_vehicle_polygons_invalid_dataframe_type() -> None:
-    with pytest.raises(TypeError):
-        make_vehicle_polygons(
-            "not_a_dataframe",
-            "+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs",
-        )
-
-
-def test_make_vehicle_polygons_coordinates_outside_utm_range() -> None:
-    df = pd.DataFrame({"x": [1e10], "y": [1e10], "swath": [2], "d": [np.nan]})
-    proj4string = (
-        "+proj=utm +zone=33 +ellps=WGS84 +datum=WGS84 +units=m +no_defs"
-    )
-    with pytest.raises(ValueError):
-        make_vehicle_polygons(df, proj4string)
-
-
-def test_make_vehicle_polygons_non_utm_coordinates() -> None:
-    df = pd.DataFrame({"x": [10], "y": [10], "swath": [2], "d": [np.nan]})
-    proj4string = "+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs"
-    with pytest.raises(ValueError):
-        make_vehicle_polygons(df, proj4string, is_utm=False)
```

