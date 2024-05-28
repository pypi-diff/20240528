# Comparing `tmp/earthkit_geo-0.1.0.tar.gz` & `tmp/earthkit_geo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit_geo-0.1.0.tar", last modified: Fri Apr 26 10:48:05 2024, max compression
+gzip compressed data, was "earthkit_geo-0.2.0.tar", last modified: Tue May 28 12:14:17 2024, max compression
```

## Comparing `earthkit_geo-0.1.0.tar` & `earthkit_geo-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,69 @@
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.795639 earthkit_geo-0.1.0/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.756049 earthkit_geo-0.1.0/.github/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.766875 earthkit_geo-0.1.0/.github/workflows/
--rw-r--r--   0 cgr        (501) staff       (20)     3667 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/ci_other.yml
--rw-r--r--   0 cgr        (501) staff       (20)      235 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/label-public-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)      275 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 cgr        (501) staff       (20)      279 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)     7224 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.gitignore
--rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 cgr        (501) staff       (20)      137 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.readthedocs.yml
--rw-r--r--   0 cgr        (501) staff       (20)    11382 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/LICENSE
--rw-r--r--   0 cgr        (501) staff       (20)      753 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/Makefile
--rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-04-26 10:48:05.795473 earthkit_geo-0.1.0/PKG-INFO
--rw-r--r--   0 cgr        (501) staff       (20)     2030 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/README.md
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.776152 earthkit_geo-0.1.0/docs/
--rw-r--r--   0 cgr        (501) staff       (20)      634 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/Makefile
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.777799 earthkit_geo-0.1.0/docs/_static/
--rw-r--r--   0 cgr        (501) staff       (20)        0 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/_static/.gitkeep
--rw-r--r--   0 cgr        (501) staff       (20)      832 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/_static/style.css
--rw-r--r--   0 cgr        (501) staff       (20)     2610 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/conf.py
--rw-r--r--   0 cgr        (501) staff       (20)     1514 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/development.rst
--rw-r--r--   0 cgr        (501) staff       (20)      818 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)      337 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/install.rst
--rw-r--r--   0 cgr        (501) staff       (20)      813 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/licence.rst
--rw-r--r--   0 cgr        (501) staff       (20)      224 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/references.rst
--rw-r--r--   0 cgr        (501) staff       (20)      129 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.756756 earthkit_geo-0.1.0/earthkit/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.787150 earthkit_geo-0.1.0/earthkit/geo/
--rw-r--r--   0 cgr        (501) staff       (20)     1028 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/__init__.py
--rw-r--r--   0 cgr        (501) staff       (20)      482 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/constants.py
--rw-r--r--   0 cgr        (501) staff       (20)     9817 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/distance.py
--rw-r--r--   0 cgr        (501) staff       (20)     1444 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/figure.py
--rw-r--r--   0 cgr        (501) staff       (20)       72 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit/geo/version.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.794685 earthkit_geo-0.1.0/earthkit_geo.egg-info/
--rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/PKG-INFO
--rw-r--r--   0 cgr        (501) staff       (20)      884 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/SOURCES.txt
--rw-r--r--   0 cgr        (501) staff       (20)        1 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/dependency_links.txt
--rw-r--r--   0 cgr        (501) staff       (20)       80 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/requires.txt
--rw-r--r--   0 cgr        (501) staff       (20)        9 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/top_level.txt
--rw-r--r--   0 cgr        (501) staff       (20)      232 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/environment.yml
--rw-r--r--   0 cgr        (501) staff       (20)      405 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/pyproject.toml
--rw-r--r--   0 cgr        (501) staff       (20)       48 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/pytest.ini
--rw-r--r--   0 cgr        (501) staff       (20)     1064 2024-04-26 10:48:05.796331 earthkit_geo-0.1.0/setup.cfg
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.793886 earthkit_geo-0.1.0/tests/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.794276 earthkit_geo-0.1.0/tests/distance/
--rw-r--r--   0 cgr        (501) staff       (20)     6069 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/distance/test_distance.py
--rw-r--r--   0 cgr        (501) staff       (20)       38 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/downstream-ci-requirements.txt
--rw-r--r--   0 cgr        (501) staff       (20)      258 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/environment-unit-tests.yml
--rw-r--r--   0 cgr        (501) staff       (20)      491 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/test_version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.744707 earthkit_geo-0.2.0/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.702817 earthkit_geo-0.2.0/.github/
+-rw-r--r--   0 cgr        (501) staff       (20)       36 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/.github/ci-hpc-config.yml
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.709480 earthkit_geo-0.2.0/.github/workflows/
+-rw-r--r--   0 cgr        (501) staff       (20)      155 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/.github/workflows/cd-pypi.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     1316 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      235 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     1637 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/.github/workflows/legacy-ci.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      275 2024-05-02 14:07:01.000000 earthkit_geo-0.2.0/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      279 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     7236 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/.gitignore
+-rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 cgr        (501) staff       (20)      137 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/.readthedocs.yml
+-rw-r--r--   0 cgr        (501) staff       (20)    11382 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/LICENSE
+-rw-r--r--   0 cgr        (501) staff       (20)      753 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/Makefile
+-rw-r--r--   0 cgr        (501) staff       (20)     3341 2024-05-28 12:14:17.744392 earthkit_geo-0.2.0/PKG-INFO
+-rw-------   0 cgr        (501) staff       (20)     2030 2024-05-28 12:03:59.000000 earthkit_geo-0.2.0/README.md
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.719129 earthkit_geo-0.2.0/docs/
+-rw-r--r--   0 cgr        (501) staff       (20)      634 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/Makefile
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.719849 earthkit_geo-0.2.0/docs/_static/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0 cgr        (501) staff       (20)      832 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/_static/style.css
+-rw-r--r--   0 cgr        (501) staff       (20)     2606 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/conf.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1514 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/development.rst
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.722087 earthkit_geo-0.2.0/docs/examples/
+-rw-r--r--   0 cgr        (501) staff       (20)      162 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/examples/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)   699593 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/examples/rotate.ipynb
+-rw-r--r--   0 cgr        (501) staff       (20)      942 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      337 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/install.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      813 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/docs/licence.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      653 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/references.rst
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.723843 earthkit_geo-0.2.0/docs/release_notes/
+-rw-r--r--   0 cgr        (501) staff       (20)      109 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/release_notes/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      316 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/release_notes/version_0.1_updates.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      685 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/release_notes/version_0.2_updates.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      145 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/docs/requirements.txt
+-rw-r--r--   0 cgr        (501) staff       (20)      252 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/environment.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     1568 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/pyproject.toml
+-rw-r--r--   0 cgr        (501) staff       (20)       48 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/pytest.ini
+-rw-r--r--   0 cgr        (501) staff       (20)       97 2024-05-28 12:14:17.746913 earthkit_geo-0.2.0/setup.cfg
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.690483 earthkit_geo-0.2.0/src/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.690130 earthkit_geo-0.2.0/src/earthkit/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.728543 earthkit_geo-0.2.0/src/earthkit/geo/
+-rw-r--r--   0 cgr        (501) staff       (20)     1029 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/__init__.py
+-rw-r--r--   0 cgr        (501) staff       (20)      411 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit/geo/_version.py
+-rw-r--r--   0 cgr        (501) staff       (20)      660 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/constants.py
+-rw-r--r--   0 cgr        (501) staff       (20)     2234 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/coord.py
+-rw-r--r--   0 cgr        (501) staff       (20)     9579 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/distance.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1444 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/figure.py
+-rw-r--r--   0 cgr        (501) staff       (20)     9619 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/src/earthkit/geo/rotate.py
+-rw-r--r--   0 cgr        (501) staff       (20)       72 2024-04-26 10:48:05.000000 earthkit_geo-0.2.0/src/earthkit/geo/version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.743363 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/
+-rw-r--r--   0 cgr        (501) staff       (20)     3341 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/PKG-INFO
+-rw-r--r--   0 cgr        (501) staff       (20)     1399 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        1 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 cgr        (501) staff       (20)       39 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/requires.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        9 2024-05-28 12:14:17.000000 earthkit_geo-0.2.0/src/earthkit_geo.egg-info/top_level.txt
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.741362 earthkit_geo-0.2.0/tests/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/__init__.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-28 12:14:17.742790 earthkit_geo-0.2.0/tests/data/
+-rw-r--r--   0 cgr        (501) staff       (20)     4577 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/data/rotated_wind_20x20_input.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     2964 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/data/rotated_wind_20x20_ref.npz
+-rw-r--r--   0 cgr        (501) staff       (20)       45 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/downstream-ci-requirements.txt
+-rw-r--r--   0 cgr        (501) staff       (20)      285 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/environment-unit-tests.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     1790 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/test_coord.py
+-rw-r--r--   0 cgr        (501) staff       (20)     6069 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/test_distance.py
+-rw-r--r--   0 cgr        (501) staff       (20)     6605 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/test_rotate.py
+-rw-r--r--   0 cgr        (501) staff       (20)      491 2024-04-26 10:46:05.000000 earthkit_geo-0.2.0/tests/test_version.py
+-rw-r--r--   0 cgr        (501) staff       (20)      929 2024-05-28 12:13:13.000000 earthkit_geo-0.2.0/tests/testing.py
```

### Comparing `earthkit_geo-0.1.0/.gitignore` & `earthkit_geo-0.2.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # setuptools-scm
 version.py
+_version.py
 
 # Sphinx automatic generation of API
 docs/_api/
 
 # Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm
```

### Comparing `earthkit_geo-0.1.0/.pre-commit-config.yaml` & `earthkit_geo-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/LICENSE` & `earthkit_geo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/Makefile` & `earthkit_geo-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/PKG-INFO` & `earthkit_geo-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: earthkit-geo
-Version: 0.1.0
-Summary: A format-agnostic Python interface for geospatial data
-License: Apache License 2.0
+Version: 0.2.0
+Summary: Geospatial computations
+Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
+License: Apache License Version 2.0
+Project-URL: Documentation, https://earthkit-geo.readthedocs.io/
+Project-URL: Homepage, https://github.com/ecmwf/earthkit-geo/
+Project-URL: Issues, https://github.com/ecmwf/earthkit-geo/issues
+Project-URL: Repository, https://github.com/ecmwf/earthkit-geo/
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyproj
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-forked; extra == "test"
-Requires-Dist: pytest-timeout; extra == "test"
-Requires-Dist: nbformat; extra == "test"
-Requires-Dist: nbconvert; extra == "test"
 
 # earthkit-geo
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit-geo.svg)](https://pypi.python.org/pypi/earthkit-geo/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-geo.svg)](https://pypi.python.org/pypi/earthkit-geo/)
 
 **DISCLAIMER**
```

### Comparing `earthkit_geo-0.1.0/README.md` & `earthkit_geo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/docs/Makefile` & `earthkit_geo-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/docs/_static/style.css` & `earthkit_geo-0.2.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/docs/conf.py` & `earthkit_geo-0.2.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx_rtd_theme",
+    "nbsphinx",
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "autoapi.extension",
 ]
 
 # autodoc configuration
 autodoc_typehints = "none"
 
 # autoapi configuration
-autoapi_dirs = ["../earthkit/geo"]
+autoapi_dirs = ["../src/earthkit/geo"]
 autoapi_ignore = ["*/version.py", "sphinxext/*"]
 autoapi_options = [
     "members",
     "undoc-members",
     "show-inheritance",
     "show-module-summary",
-    "imported-members",
     "inherited-members",
 ]
 autoapi_root = "_api"
 autoapi_member_order = "alphabetical"
 autoapi_add_toctree_entry = False
 
 # napoleon configuration
```

### Comparing `earthkit_geo-0.1.0/docs/development.rst` & `earthkit_geo-0.2.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/docs/index.rst` & `earthkit_geo-0.2.0/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -9,32 +9,40 @@
 
     This documentation is still work in progress and can only be regarded as a **DRAFT**.
 
 
 .. toctree::
    :maxdepth: 1
    :caption: Examples
-   :titlesonly:
 
-   examples
+   examples/index
+
 
 .. toctree::
    :maxdepth: 1
    :caption: Documentation
 
    _api/geo/index
 
 .. toctree::
    :maxdepth: 1
    :caption: Installation
 
    install
+   release_notes/index
    development
    licence
 
+.. toctree::
+   :maxdepth: 1
+   :caption: Projects
+
+   earthkit <https://earthkit.readthedocs.io/en/latest>
+
+
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 
 .. * :ref:`modindex`
```

### Comparing `earthkit_geo-0.1.0/docs/licence.rst` & `earthkit_geo-0.2.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/earthkit/geo/__init__.py` & `earthkit_geo-0.2.0/src/earthkit/geo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 try:
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
-    from .version import __version__
+    from ._version import __version__
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
     __version__ = "999"
 
 
 from earthkit.geo.distance import (
     GeoKDTree,
```

### Comparing `earthkit_geo-0.1.0/earthkit/geo/distance.py` & `earthkit_geo-0.2.0/src/earthkit/geo/distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import numpy as np
 
 from . import constants
+from .coord import latlon_to_xyz
 from .figure import IFS_SPHERE, UNIT_SPHERE
 
 
 def _regulate_lat(lat):
-    return np.where(np.abs(lat) > constants.north, np.nan, lat)
+    return np.where(np.abs(lat) > constants.NORTH_POLE_LAT, np.nan, lat)
 
 
 def haversine_distance(p1, p2, figure=IFS_SPHERE):
     """Compute haversine distance between two (sets of) points on a spheroid.
 
     Parameters
     ----------
@@ -148,27 +149,14 @@
         index = np.nanargmin(distance)
         index = index[0] if isinstance(index, np.ndarray) else index
         res_index.append(index)
         res_distance.append(distance[index])
     return (np.array(res_index), figure.scale(np.array(res_distance)))
 
 
-def _latlon_to_xyz(lat, lon):
-    """Works on the unit sphere."""
-    lat = np.asarray(lat)
-    lon = np.asarray(lon)
-    lat = np.radians(lat)
-    lon = np.radians(lon)
-    x = np.cos(lat) * np.cos(lon)
-    y = np.cos(lat) * np.sin(lon)
-    z = np.sin(lat)
-
-    return x, y, z
-
-
 def _chordlength_to_arclength(chord_length):
     """
     Convert 3D (Euclidean) distance to great circle arc length
     https://en.wikipedia.org/wiki/Great-circle_distance
     Works on the unit sphere.
     """
     central_angle = 2.0 * np.arcsin(chord_length / 2.0)
@@ -183,27 +171,27 @@
     """
     central_angle = arc_length
     return np.sin(central_angle / 2) * 2.0
 
 
 class GeoKDTree:
     def __init__(self, lats, lons):
-        """KDTree built from ``lats`` and ``lons``."""
+        """Build a KDTree from ``lats`` and ``lons``."""
         from scipy.spatial import KDTree
 
         lats = np.asarray(lats).flatten()
         lons = np.asarray(lons).flatten()
 
         # kdtree cannot contain nans
         if np.isnan(lats.max()) or np.isnan(lons.max()):
             mask = ~np.isnan(lats) & ~np.isnan(lons)
             lats = lats[mask]
             lons = lons[mask]
 
-        x, y, z = _latlon_to_xyz(lats, lons)
+        x, y, z = latlon_to_xyz(lats, lons)
         v = np.column_stack((x, y, z))
         self.tree = KDTree(v)
 
         # TODO: allow user to specify max distance
         self.max_distance_arc = np.pi / 4
         if self.max_distance_arc <= np.pi:
             self.max_distance_chord = _arclength_to_chordlength(self.max_distance_arc)
@@ -228,15 +216,15 @@
         ndarray
             The distance (m) between the ``ref_points`` and the corresponding nearest
             point in ``points``. Computed on the surface of the spheroid defined
             by ``figure``.
 
         """
         lat, lon = ref_points
-        x, y, z = _latlon_to_xyz(lat, lon)
+        x, y, z = latlon_to_xyz(lat, lon)
         points = np.column_stack((x, y, z))
 
         # find the nearest point
         distance, index = self.tree.query(
             points, distance_upper_bound=self.max_distance_arc
         )
```

### Comparing `earthkit_geo-0.1.0/earthkit/geo/figure.py` & `earthkit_geo-0.2.0/src/earthkit/geo/figure.py`

 * *Files identical despite different names*

### Comparing `earthkit_geo-0.1.0/earthkit_geo.egg-info/PKG-INFO` & `earthkit_geo-0.2.0/src/earthkit_geo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: earthkit-geo
-Version: 0.1.0
-Summary: A format-agnostic Python interface for geospatial data
-License: Apache License 2.0
+Version: 0.2.0
+Summary: Geospatial computations
+Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
+License: Apache License Version 2.0
+Project-URL: Documentation, https://earthkit-geo.readthedocs.io/
+Project-URL: Homepage, https://github.com/ecmwf/earthkit-geo/
+Project-URL: Issues, https://github.com/ecmwf/earthkit-geo/issues
+Project-URL: Repository, https://github.com/ecmwf/earthkit-geo/
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyproj
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-forked; extra == "test"
-Requires-Dist: pytest-timeout; extra == "test"
-Requires-Dist: nbformat; extra == "test"
-Requires-Dist: nbconvert; extra == "test"
 
 # earthkit-geo
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit-geo.svg)](https://pypi.python.org/pypi/earthkit-geo/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-geo.svg)](https://pypi.python.org/pypi/earthkit-geo/)
 
 **DISCLAIMER**
```

### Comparing `earthkit_geo-0.1.0/tests/distance/test_distance.py` & `earthkit_geo-0.2.0/tests/test_distance.py`

 * *Files identical despite different names*

