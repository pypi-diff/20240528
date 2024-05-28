# Comparing `tmp/lymph-model-1.2.0.tar.gz` & `tmp/lymph_model-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lymph-model-1.2.0.tar", last modified: Fri Mar 29 12:57:58 2024, max compression
+gzip compressed data, was "lymph_model-1.2.1.tar", last modified: Tue May 28 13:41:21 2024, max compression
```

## Comparing `lymph-model-1.2.0.tar` & `lymph_model-1.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.593921 lymph-model-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.581921 lymph-model-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.581921 lymph-model-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-29 12:57:48.000000 lymph-model-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    28361 2024-03-29 12:57:48.000000 lymph-model-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-29 12:57:48.000000 lymph-model-1.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-29 12:57:48.000000 lymph-model-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-29 12:57:48.000000 lymph-model-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-29 12:57:58.593921 lymph-model-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-03-29 12:57:48.000000 lymph-model-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:48.000000 lymph-model-1.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.581921 lymph-model-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.585921 lymph-model-1.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.585921 lymph-model-1.2.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.585921 lymph-model-1.2.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    71634 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/_static/github-social-card.png
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/badges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/components.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/explanation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/graph.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/quickstart_bilateral.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/quickstart_unilateral.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/refs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-29 12:57:48.000000 lymph-model-1.2.0/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.589921 lymph-model-1.2.0/lymph/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/diagnosis_times.py
--rw-r--r--   0 runner    (1001) docker     (127)    29292 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/modalities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.589921 lymph-model-1.2.0/lymph/models/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28799 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/models/bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)    37972 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/models/midline.py
--rw-r--r--   0 runner    (1001) docker     (127)    40249 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/models/unilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-03-29 12:57:48.000000 lymph-model-1.2.0/lymph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.593921 lymph-model-1.2.0/lymph_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 12:57:58.000000 lymph-model-1.2.0/lymph_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-29 12:57:48.000000 lymph-model-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:57:58.593921 lymph-model-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.589921 lymph-model-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/bayesian_unilateral_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/binary_bilateral_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/binary_midline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/binary_unilateral_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:57:58.593921 lymph-model-1.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    92742 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/data/2021-clb-oropharynx.csv
--rw-r--r--   0 runner    (1001) docker     (127)   166960 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/data/2021-usz-oropharynx.csv
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/data/trans_mat_timings_897b495.csv
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/data/trans_mat_timings_v0.4.3.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/doc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/edge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/emcee_intergration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/graph_representation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/trinary_midline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-03-29 12:57:48.000000 lymph-model-1.2.0/tests/trinary_unilateral_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.195665 lymph_model-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.179665 lymph_model-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.183665 lymph_model-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 13:41:10.000000 lymph_model-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-28 13:41:10.000000 lymph_model-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-28 13:41:10.000000 lymph_model-1.2.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-28 13:41:10.000000 lymph_model-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 13:41:10.000000 lymph_model-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-05-28 13:41:21.195665 lymph_model-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 13:41:10.000000 lymph_model-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:10.000000 lymph_model-1.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.183665 lymph_model-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.187666 lymph_model-1.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.187666 lymph_model-1.2.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.187666 lymph_model-1.2.1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    71634 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/_static/github-social-card.png
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/explanation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/quickstart_bilateral.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/quickstart_unilateral.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/refs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 13:41:10.000000 lymph_model-1.2.1/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.187666 lymph_model-1.2.1/lymph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/diagnosis_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29555 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/modalities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.187666 lymph_model-1.2.1/lymph/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28806 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/models/bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37996 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/models/midline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40499 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/models/unilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-28 13:41:10.000000 lymph_model-1.2.1/lymph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.191666 lymph_model-1.2.1/lymph_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 13:41:21.000000 lymph_model-1.2.1/lymph_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-28 13:41:10.000000 lymph_model-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:41:21.195665 lymph_model-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.191666 lymph_model-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/bayesian_unilateral_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/binary_bilateral_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/binary_midline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/binary_unilateral_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:21.191666 lymph_model-1.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    92742 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/data/2021-clb-oropharynx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   166960 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/data/2021-usz-oropharynx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/data/trans_mat_timings_897b495.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/data/trans_mat_timings_v0.4.3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/distribution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/doc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/edge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/emcee_intergration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/graph_representation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/trinary_midline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-28 13:41:10.000000 lymph_model-1.2.1/tests/trinary_unilateral_test.py
```

### Comparing `lymph-model-1.2.0/.github/workflows/build.yml` & `lymph_model-1.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/.github/workflows/tests.yml` & `lymph_model-1.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/.gitignore` & `lymph_model-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/.pre-commit-config.yaml` & `lymph_model-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/.readthedocs.yml` & `lymph_model-1.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/CHANGELOG.md` & `lymph_model-1.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+
+<a name="1.2.1"></a>
+## [1.2.1] - 2024-05-28
+
+### Bug Fixes
+
+- (**uni**) `load_patient_data` should accept `None`.
+- (**mid**) Correct type hint of `marginalize`.
+- (**graph**) Wrong dict when trinary.\
+  The `to_dict()` method returned a wrong graph dictionary when trinary
+  due to growth edges. This is fixed now.
+- Skip `marginalize` only when safe.\
+  The marginalization should only be skipped (and 1 returned), when the
+  entire disease state of interest is `None`. In the midline case, this
+  disease state includes the midline extension.\
+  Previously, only the involvement pattern was checked. Now, the model is
+  more careful about when to take shortcuts.
+
+
+### Features
+
+- (**graph**) Modify mermaid graph.\
+  The `get_mermaid()` and `get_mermaid_url()` methods now accept arguments
+  that allow some modifications of the output.
+- (**uni**) Add `__repr__()`.
+
+### Refactor
+
+- (**uni**) Use pandas `map` instead of `apply`.\
+  This saves us a couple of lines in the `load_patient_data` method and is
+  more readable.
+
+
+### Merge
+
+- Branch 'main' into 'dev'.
+
+### Remove
+
+- Remains of callbacks.\
+  Some callback functionality that was tested in a pre-release has been
+  forgotten in the code base and is now deleted.
+
+
 <a name="1.2.0"></a>
 ## [1.2.0] - 2024-03-29
 
 ### Bug Fixes
 
 - (**mid**) `obs_dist` may return 3D array.
 
@@ -664,15 +708,16 @@
 - delete unnecessary utils
 
 ### Maintenance
 - fix pyproject.toml typo
 - add pre-commit hook to check commit msg
 
 
-[Unreleased]: https://github.com/rmnldwg/lymph/compare/1.2.0...HEAD
+[Unreleased]: https://github.com/rmnldwg/lymph/compare/1.2.1...HEAD
+[1.2.1]: https://github.com/rmnldwg/lymph/compare/1.1.0...1.2.1
 [1.2.0]: https://github.com/rmnldwg/lymph/compare/1.1.0...1.2.0
 [1.1.0]: https://github.com/rmnldwg/lymph/compare/1.0.0...1.1.0
 [1.0.0]: https://github.com/rmnldwg/lymph/compare/1.0.0.rc2...1.0.0
 [1.0.0.rc2]: https://github.com/rmnldwg/lymph/compare/1.0.0.rc1...1.0.0.rc2
 [1.0.0.rc1]: https://github.com/rmnldwg/lymph/compare/1.0.0.a6...1.0.0.rc1
 [1.0.0.a6]: https://github.com/rmnldwg/lymph/compare/1.0.0.a5...1.0.0.a6
 [1.0.0.a5]: https://github.com/rmnldwg/lymph/compare/1.0.0.a4...1.0.0.a5
```

### Comparing `lymph-model-1.2.0/CITATION.cff` & `lymph_model-1.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/CONTRIBUTING.md` & `lymph_model-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/LICENSE` & `lymph_model-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/PKG-INFO` & `lymph_model-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lymph-model
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package for statistical modelling of lymphatic metastatic spread.
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lymph
 Project-URL: documentation, https://lymph-model.readthedocs.io
 Keywords: cancer,metastasis,lymphatic progression,model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lymph-model-1.2.0/README.rst` & `lymph_model-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/Makefile` & `lymph_model-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/make.bat` & `lymph_model-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/_static/github-social-card.png` & `lymph_model-1.2.1/docs/source/_static/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/components.rst` & `lymph_model-1.2.1/docs/source/components.rst`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/conf.py` & `lymph_model-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/install.rst` & `lymph_model-1.2.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/license.rst` & `lymph_model-1.2.1/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/quickstart_bilateral.ipynb` & `lymph_model-1.2.1/docs/source/quickstart_bilateral.ipynb`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/docs/source/quickstart_unilateral.ipynb` & `lymph_model-1.2.1/docs/source/quickstart_unilateral.ipynb`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/__init__.py` & `lymph_model-1.2.1/lymph/__init__.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/diagnosis_times.py` & `lymph_model-1.2.1/lymph/diagnosis_times.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/graph.py` & `lymph_model-1.2.1/lymph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 compute e.g. the transition matrix of the model.
 """
 from __future__ import annotations
 
 import base64
 import warnings
 from itertools import product
+from typing import Literal
 
 import numpy as np
 
+from lymph import types
 from lymph.utils import (
     check_unique_names,
     comp_transition_tensor,
     flatten,
     popfirst,
     set_params_for,
-    trigger,
 )
 
 
 class AbstractNode:
     """Abstract base class for nodes in the graph reprsenting the lymphatic system."""
     def __init__(
         self,
@@ -220,29 +221,24 @@
     """This class represents an arc in the graph representation of the lymph system."""
     def __init__(
         self,
         parent: Tumor | LymphNodeLevel,
         child: LymphNodeLevel,
         spread_prob: float = 0.,
         micro_mod: float = 1.,
-        callbacks: list[callable] | None = None,
     ) -> None:
         """Create a new edge between two nodes.
 
         The ``parent`` node must be a :py:class:`Tumor` or a :py:class:`LymphNodeLevel`,
         and the ``child`` node must be a :py:class:`LymphNodeLevel`.
 
         The ``spread_prob`` parameter is the probability of a tumor or involved LNL to
         spread to the next LNL. The ``micro_mod`` parameter is a modifier for the spread
         probability in case of only a microscopic node involvement.
         """
-        self.trigger_callbacks = []
-        if callbacks is not None:
-            self.trigger_callbacks += callbacks
-
         self.parent: Tumor | LymphNodeLevel = parent
         self.child: LymphNodeLevel = child
 
         if (
             not isinstance(self.parent, Tumor)
             and self.parent.is_trinary
             and not self.is_growth
@@ -349,15 +345,14 @@
             not hasattr(self, "_micro_mod")
             or isinstance(self.parent, Tumor)
             or self.parent.is_binary
         ):
             self._micro_mod = 1.
         return self._micro_mod
 
-    @trigger
     def set_micro_mod(self, new_micro_mod: float | None) -> None:
         """Set the spread modifier for LNLs with microscopic involvement."""
         if new_micro_mod is None:
             return
 
         if isinstance(self.parent, Tumor) or self.parent.is_binary:
             warnings.warn("Microscopic spread modifier is not used for binary nodes!")
@@ -376,15 +371,14 @@
 
     def get_spread_prob(self) -> float:
         """Return the spread probability."""
         if not hasattr(self, "_spread_prob"):
             self._spread_prob = 0.
         return self._spread_prob
 
-    @trigger
     def set_spread_prob(self, new_spread_prob: float | None) -> None:
         """Set the spread probability of the edge."""
         if new_spread_prob is None:
             return
 
         if not 0. <= new_spread_prob <= 1.:
             raise ValueError("Spread probability must be between 0 and 1!")
@@ -489,15 +483,14 @@
     :py:class:`LymphNodeLevel`) and edges (:py:class:`Edge`) of the :py:mod:`models`.
     """
     def __init__(
         self,
         graph_dict: dict[tuple[str], list[str]],
         tumor_state: int | None = None,
         allowed_states: list[int] | None = None,
-        on_edge_change: list[callable] | None = None,
     ) -> None:
         """Create a new graph representation of nodes and edges.
 
         The ``graph_dict`` is a dictionary that defines which nodes are created and
         with what edges they are connected. The keys of the dictionary are tuples of
         the form ``(node_type, node_name)``. The ``node_type`` can be either ``"tumor"``
         or ``"lnl"``. The ``node_name`` is a string that uniquely identifies the node.
@@ -508,15 +501,15 @@
             allowed_states = [0, 1]
 
         if tumor_state is None:
             tumor_state = allowed_states[-1]
 
         check_unique_names(graph_dict)
         self._init_nodes(graph_dict, tumor_state, allowed_states)
-        self._init_edges(graph_dict, on_edge_change)
+        self._init_edges(graph_dict)
 
 
     def _init_nodes(self, graph, tumor_state, allowed_lnl_states):
         """Initialize the nodes of the graph."""
         self._nodes: dict[str, Tumor | LymphNodeLevel] = {}
 
         for node_type, node_name in graph:
@@ -581,15 +574,14 @@
 
         return res.pop()
 
 
     def _init_edges(
         self,
         graph: dict[tuple[str, str], list[str]],
-        on_edge_change: list[callable]
     ) -> None:
         """Initialize the edges of the ``graph``.
 
         Every one of the provided ``on_edge_change`` list of callback functions is
         called whenever a parameter of an edge is changed. Typically, this is used to
         update the transition tensor of the edge or the transition matrix of the
         :py:class:`lymph.models`.
@@ -598,20 +590,20 @@
         a growth edge.
         """
         self._edges: dict[str, Edge] = {}
 
         for (_, start_name), end_names in graph.items():
             start = self.nodes[start_name]
             if isinstance(start, LymphNodeLevel) and start.is_trinary:
-                growth_edge = Edge(parent=start, child=start, callbacks=on_edge_change)
+                growth_edge = Edge(parent=start, child=start)
                 self._edges[growth_edge.get_name()] = growth_edge
 
             for end_name in end_names:
                 end = self.nodes[end_name]
-                new_edge = Edge(parent=start, child=end, callbacks=on_edge_change)
+                new_edge = Edge(parent=start, child=end)
                 self._edges[new_edge.get_name()] = new_edge
 
 
     @property
     def edges(self) -> dict[str, Edge]:
         """Iterable of all edges in the graph."""
         return self._edges
@@ -665,19 +657,27 @@
         >>> graph = Representation(graph_dict)
         >>> graph.to_dict() == graph_dict
         True
         """
         res = {}
         for node in self.nodes.values():
             node_type = "tumor" if isinstance(node, Tumor) else "lnl"
-            res[(node_type, node.name)] = [o.child.name for o in node.out]
+            res[(node_type, node.name)] = [
+                o.child.name
+                for o in node.out
+                if not o.is_growth
+            ]
         return res
 
 
-    def get_mermaid(self) -> str:
+    def get_mermaid(
+        self,
+        with_params: bool = True,
+        direction: Literal["TD", "LR"] = "TD",
+    ) -> str:
         """Prints the graph in mermaid format.
 
         >>> graph_dict = {
         ...    ('tumor', 'T'): ['II', 'III'],
         ...    ('lnl', 'II'): ['III'],
         ...    ('lnl', 'III'): [],
         ... }
@@ -687,27 +687,37 @@
         >>> graph.edges["IItoIII"].spread_prob = 0.3
         >>> print(graph.get_mermaid())  # doctest: +NORMALIZE_WHITESPACE
         flowchart TD
             T-->|10%| II
             T-->|20%| III
             II-->|30%| III
         <BLANKLINE>
+        >>> print(graph.get_mermaid(with_params=False)) # doctest: +NORMALIZE_WHITESPACE
+        flowchart TD
+            T--> II
+            T--> III
+            II--> III
+        <BLANKLINE>
         """
-        mermaid_graph = "flowchart TD\n"
+        mermaid_graph = f"flowchart {direction}\n"
 
         for node in self.nodes.values():
             for edge in node.out:
-                mermaid_graph += f"\t{node.name}-->|{edge.spread_prob:.0%}| {edge.child.name}\n"
+                param_str = f"|{edge.spread_prob:.0%}|" if with_params else ""
+                mermaid_graph += f"\t{node.name}-->{param_str} {edge.child.name}\n"
 
         return mermaid_graph
 
 
-    def get_mermaid_url(self) -> str:
-        """Returns the URL to the rendered graph."""
-        mermaid_graph = self.get_mermaid()
+    def get_mermaid_url(self, **mermaid_kwargs) -> str:
+        """Returns the URL to the rendered graph.
+
+        Keyword arguments are passed to :py:meth:`~Representation.get_mermaid`.
+        """
+        mermaid_graph = self.get_mermaid(**mermaid_kwargs)
         graphbytes = mermaid_graph.encode("ascii")
         base64_bytes = base64.b64encode(graphbytes)
         base64_string = base64_bytes.decode("ascii")
         url="https://mermaid.ink/img/" + base64_string
         return url
```

### Comparing `lymph-model-1.2.0/lymph/matrix.py` & `lymph_model-1.2.1/lymph/matrix.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/modalities.py` & `lymph_model-1.2.1/lymph/modalities.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/models/bilateral.py` & `lymph_model-1.2.1/lymph/models/bilateral.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,15 +622,15 @@
         over. For this, the :py:func:`.matrix.compute_encoding` function is used.
 
         If ``given_state_dist`` is ``None``, it will be computed by calling
         :py:meth:`.state_dist` with the given ``t_stage`` and ``mode``. These arguments
         are ignored if ``given_state_dist`` is provided.
         """
         if involvement is None:
-            return 1.
+            involvement = {}
 
         if given_state_dist is None:
             given_state_dist = self.state_dist(t_stage=t_stage, mode=mode)
 
         marginalize_over_states = {}
         for side in ["ipsi", "contra"]:
             side_graph = getattr(self, side).graph
```

### Comparing `lymph-model-1.2.0/lymph/models/midline.py` & `lymph_model-1.2.1/lymph/models/midline.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,15 +749,15 @@
             given_state_dist=given_state_dist,
             given_diagnosis=given_diagnosis,
         )
 
 
     def marginalize(
         self,
-        involvement: types.PatternType | None = None,
+        involvement: dict[str, types.PatternType] | None = None,
         given_state_dist: np.ndarray | None = None,
         t_stage: str = "early",
         mode: Literal["HMM", "BN"] = "HMM",
         midext: bool | None = None,
         central: bool = False,
     ) -> float:
         """Marginalize ``given_state_dist`` over matching ``involvement`` patterns.
@@ -766,15 +766,15 @@
         over. For this, the :py:func:`.matrix.compute_encoding` function is used.
 
         The arguments ``t_stage``, ``mode``, and ``central`` are only used if
         ``given_state_dist`` is ``None``. In this case they are passed to the
         :py:meth:`.state_dist` method.
         """
         if involvement is None:
-            return 1.
+            involvement = {}
 
         if given_state_dist is None:
             given_state_dist = self.state_dist(t_stage=t_stage, mode=mode, central=central)
 
         if given_state_dist.ndim == 2:
             return self.ext.marginalize(
                 involvement=involvement,
@@ -783,15 +783,15 @@
 
         if midext is None:
             given_state_dist = np.sum(given_state_dist, axis=0)
         else:
             given_state_dist = given_state_dist[int(midext)]
             # I think I don't need to normalize here, since I am not computing a
             # probability of something *given* midext, but only sum up all states that
-            # match the involvement pattern (which includes the midext status).
+            # match the disease state of interest (which includes the midext status).
 
         return self.ext.marginalize(
             involvement=involvement,
             given_state_dist=given_state_dist,
         )
```

### Comparing `lymph-model-1.2.0/lymph/models/unilateral.py` & `lymph_model-1.2.1/lymph/models/unilateral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import warnings
 from itertools import product
-from typing import Any, Iterable, Literal
+from typing import Any, Callable, Iterable, Literal
 
 import numpy as np
 import pandas as pd
 from cachetools import LRUCache
 
 from lymph import diagnosis_times, graph, matrix, modalities, types, utils
 
@@ -113,14 +113,25 @@
 
     @classmethod
     def trinary(cls, graph_dict: types.GraphDictType, **kwargs) -> Unilateral:
         """Create an instance of the :py:class:`~Unilateral` class with trinary LNLs."""
         return cls(graph_dict, allowed_states=[0, 1, 2], **kwargs)
 
 
+    def __repr__(self) -> str:
+        """Return a string representation of the instance."""
+        return (
+            f"{type(self).__name__}("
+            f"graph_dict={self.graph.to_dict()}, "
+            f"tumor_state={list(self.graph.tumors.values())[0].state}, "
+            f"allowed_states={self.graph.allowed_states}, "
+            f"max_time={self.max_time})"
+        )
+
+
     def __str__(self) -> str:
         """Print info about the instance."""
         return f"Unilateral with {len(self.graph.tumors)} tumors and {len(self.graph.lnls)} LNLs"
 
 
     @property
     def is_trinary(self) -> bool:
@@ -485,15 +496,15 @@
         return self._diagnosis_matrix_cache[_hash].T
 
 
     def load_patient_data(
         self,
         patient_data: pd.DataFrame,
         side: str = "ipsi",
-        mapping: callable | dict[int, Any] | None = None,
+        mapping: Callable[[int], Any] | dict[int, Any] | None = None,
     ) -> None:
         """Load patient data in `LyProX`_ format into the model.
 
         Since the `LyProX`_ data format contains information on both sides (i.e.,
         ipsi- and contralateral) of the neck, the ``side`` parameter is used to select
         the for which of the two to store the involvement data.
 
@@ -508,15 +519,14 @@
         information necessary to compute the observation and diagnosis matrices.
 
         .. _LyProX: https://lyprox.org/
         """
         if mapping is None:
             mapping = early_late_mapping
 
-        # pylint: disable=unnecessary-lambda-assignment
         patient_data = (
             patient_data
             .copy()
             .drop(columns="_model", errors="ignore")
             .reset_index(drop=True)
         )
 
@@ -541,23 +551,15 @@
                     )
                     column = None
                 else:
                     column = patient_data[modality, side, lnl]
 
                 patient_data["_model", modality, lnl] = column
 
-        if len(patient_data) == 0:
-            patient_data[MAP_T_COL] = None
-        else:
-            mapping = dict_to_func(mapping) if isinstance(mapping, dict) else mapping
-            patient_data[MAP_T_COL] = patient_data.apply(
-                lambda row: mapping(row[RAW_T_COL]),
-                axis=1,
-            )
-
+        patient_data[MAP_T_COL] = patient_data[RAW_T_COL].map(mapping)
         self._patient_data = patient_data
         self._cache_version += 1
 
         for t_stage in self.get_t_stages("distributions"):
             if t_stage not in patient_data[MAP_T_COL].values:
                 warnings.warn(
                     message=f"No data for T-stage {t_stage} found.",
@@ -829,15 +831,19 @@
         Any state that matches the provided ``involvement`` pattern is marginalized
         over. For this, the :py:func:`.matrix.compute_encoding` function is used.
 
         If ``given_state_dist`` is ``None``, it will be computed by calling
         :py:meth:`.state_dist` with the given ``t_stage`` and ``mode``. These arguments
         are ignored if ``given_state_dist`` is provided.
         """
-        if involvement is None:
+        if (
+            involvement is None
+            or not involvement     # empty dict is falsey
+            or all(value is None for value in involvement.values())
+        ):
             return 1.
 
         if given_state_dist is None:
             given_state_dist = self.state_dist(t_stage=t_stage, mode=mode)
 
         marginalize_over_states = matrix.compute_encoding(
             lnls=self.graph.lnls.keys(),
```

### Comparing `lymph-model-1.2.0/lymph/types.py` & `lymph_model-1.2.1/lymph/types.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph/utils.py` & `lymph_model-1.2.1/lymph/utils.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/lymph_model.egg-info/PKG-INFO` & `lymph_model-1.2.1/lymph_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lymph-model
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package for statistical modelling of lymphatic metastatic spread.
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lymph
 Project-URL: documentation, https://lymph-model.readthedocs.io
 Keywords: cancer,metastasis,lymphatic progression,model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lymph-model-1.2.0/lymph_model.egg-info/SOURCES.txt` & `lymph_model-1.2.1/lymph_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/pyproject.toml` & `lymph_model-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/bayesian_unilateral_test.py` & `lymph_model-1.2.1/tests/bayesian_unilateral_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/binary_bilateral_test.py` & `lymph_model-1.2.1/tests/binary_bilateral_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/binary_midline_test.py` & `lymph_model-1.2.1/tests/binary_midline_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/binary_unilateral_test.py` & `lymph_model-1.2.1/tests/binary_unilateral_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/data/2021-clb-oropharynx.csv` & `lymph_model-1.2.1/tests/data/2021-clb-oropharynx.csv`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/data/2021-usz-oropharynx.csv` & `lymph_model-1.2.1/tests/data/2021-usz-oropharynx.csv`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/distribution_test.py` & `lymph_model-1.2.1/tests/distribution_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/doc_test.py` & `lymph_model-1.2.1/tests/doc_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/edge_test.py` & `lymph_model-1.2.1/tests/edge_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 class BinaryEdgeTestCase(fixtures.IgnoreWarningsTestCase):
     """Tests for the Edge class."""
 
     def setUp(self) -> None:
         super().setUp()
         parent = graph.LymphNodeLevel("parent")
         child = graph.LymphNodeLevel("child")
-        self.was_called = False
-        self.edge = graph.Edge(parent, child, callbacks=[self.callback])
-
-    def callback(self) -> None:
-        """Callback function for the edge."""
-        self.was_called = True
+        self.edge = graph.Edge(parent, child)
 
     def test_str(self) -> None:
         """Test the string representation of the edge."""
         self.assertEqual(str(self.edge), "Edge parent to child")
 
     def test_repr(self) -> None:
         """Test if the edge can be recreated from repr."""
@@ -37,25 +32,19 @@
         )
         self.assertEqual(self.edge.get_name(), recreated_edge.get_name())
         self.assertEqual(self.edge.parent.name, recreated_edge.parent.name)
         self.assertEqual(self.edge.child.name, recreated_edge.child.name)
         self.assertEqual(self.edge.spread_prob, recreated_edge.spread_prob)
         self.assertEqual(self.edge.micro_mod, recreated_edge.micro_mod)
 
-    def test_callback_on_param_change(self) -> None:
-        """Test if the callback function is called."""
-        self.edge.spread_prob = 0.5
-        self.assertTrue(self.was_called)
-
     def test_graph_change(self) -> None:
         """Check if the callback also works when parent/child nodes are changed."""
         old_child = self.edge.child
         new_child = graph.LymphNodeLevel("new_child")
         self.edge.child = new_child
-        self.assertTrue(self.was_called)
         self.assertNotIn(self.edge, old_child.inc)
 
     def test_transition_tensor_row_sums(self) -> None:
         """Testing the transition tensor."""
         row_sum = self.edge.transition_tensor.sum(axis=2)
         self.assertTrue(np.allclose(row_sum, 1.0))
```

### Comparing `lymph-model-1.2.0/tests/emcee_intergration_test.py` & `lymph_model-1.2.1/tests/emcee_intergration_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/fixtures.py` & `lymph_model-1.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/graph_representation_test.py` & `lymph_model-1.2.1/tests/graph_representation_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,18 @@
             ("lnl", "II"): ["III"],
             ("lnl", "III"): [],
         }
         self.graph_dict = large_graph
         self.graph_repr = graph.Representation(
             graph_dict=self.graph_dict,
             allowed_states=[0, 1],
-            on_edge_change=[self.callback],
         )
         self.was_called = False
         self.rng = np.random.default_rng(42)
 
-    def callback(self) -> None:
-        """Callback function for the graph."""
-        self.was_called = True
-
     def test_nodes(self) -> None:
         """Test the number of nodes."""
         self.assertEqual(len(self.graph_repr.nodes), len(self.graph_dict))
         node_names = {tpl[1] for tpl in self.graph_dict.keys()}
 
         for name, node in self.graph_repr.nodes.items():
             self.assertIn(name, node_names)
```

### Comparing `lymph-model-1.2.0/tests/integration_test.py` & `lymph_model-1.2.1/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/node_test.py` & `lymph_model-1.2.1/tests/node_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/trinary_midline_test.py` & `lymph_model-1.2.1/tests/trinary_midline_test.py`

 * *Files identical despite different names*

### Comparing `lymph-model-1.2.0/tests/trinary_unilateral_test.py` & `lymph_model-1.2.1/tests/trinary_unilateral_test.py`

 * *Files identical despite different names*

