# Comparing `tmp/dynamicio-5.0.0rc5.tar.gz` & `tmp/dynamicio-5.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicio-5.0.0rc5.tar", last modified: Fri May 24 15:01:27 2024, max compression
+gzip compressed data, was "dynamicio-5.0.0rc6.tar", last modified: Fri May 24 21:11:34 2024, max compression
```

## Comparing `dynamicio-5.0.0rc5.tar` & `dynamicio-5.0.0rc6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.234807 dynamicio-5.0.0rc5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 15:01:27.234807 dynamicio-5.0.0rc5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.222807 dynamicio-5.0.0rc5/demo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.222807 dynamicio-5.0.0rc5/demo/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/environment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.222807 dynamicio-5.0.0rc5/demo/src/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/runners/staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/src/runners/transform.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.222807 dynamicio-5.0.0rc5/demo/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.226807 dynamicio-5.0.0rc5/demo/tests/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/runners/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/runners/test_staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/runners/test_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/test_pipeline.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/demo/tests/test_runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.226807 dynamicio-5.0.0rc5/dynamicio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3711 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.226807 dynamicio-5.0.0rc5/dynamicio/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/io_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.226807 dynamicio-5.0.0rc5/dynamicio/config/pydantic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/pydantic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/pydantic/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9290 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/pydantic/io_resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/config/pydantic/table_schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5841 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/metrics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.230807 dynamicio-5.0.0rc5/dynamicio/mixins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13786 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/with_kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/with_local.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8015 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/with_postgres.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18850 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/mixins/with_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13239 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/dynamicio/validations.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.226807 dynamicio-5.0.0rc5/dynamicio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      326 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-24 15:01:27.000000 dynamicio-5.0.0rc5/dynamicio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-24 15:01:27.234807 dynamicio-5.0.0rc5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.230807 dynamicio-5.0.0rc5/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34498 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.230807 dynamicio-5.0.0rc5/tests/mocking/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/mocking/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5068 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/mocking/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/mocking/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6425 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43997 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_metrics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:27.234807 dynamicio-5.0.0rc5/tests/test_mixins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16703 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/test_kafka_mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33927 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/test_local_mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5526 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/test_mixin_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8795 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/test_postgres_mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35816 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_mixins/test_s3_mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_table_schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17759 2024-05-24 15:01:14.000000 dynamicio-5.0.0rc5/tests/test_validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/demo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/demo/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/environment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/demo/src/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/runners/staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/src/runners/transform.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/demo/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/demo/tests/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/runners/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/runners/test_staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/runners/test_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/test_pipeline.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/demo/tests/test_runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/dynamicio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3711 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/dynamicio/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/io_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/dynamicio/config/pydantic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/pydantic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/pydantic/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9290 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/pydantic/io_resources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/config/pydantic/table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5841 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/metrics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/dynamicio/mixins/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13765 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/with_kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/with_local.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8015 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/with_postgres.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18850 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/mixins/with_s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/py.typed
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13239 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/dynamicio/validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.657251 dynamicio-5.0.0rc6/dynamicio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      326 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-24 21:11:34.000000 dynamicio-5.0.0rc6/dynamicio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34498 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/tests/mocking/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/mocking/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5068 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/mocking/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/mocking/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6425 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43997 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_metrics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:34.661250 dynamicio-5.0.0rc6/tests/test_mixins/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18416 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/test_kafka_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33927 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/test_local_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5526 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/test_mixin_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8795 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/test_postgres_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35816 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_mixins/test_s3_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17759 2024-05-24 21:11:23.000000 dynamicio-5.0.0rc6/tests/test_validations.py
```

### Comparing `dynamicio-5.0.0rc5/LICENSE` & `dynamicio-5.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/PKG-INFO` & `dynamicio-5.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc5
+Version: 5.0.0rc6
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc5/README.md` & `dynamicio-5.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/__init__.py` & `dynamicio-5.0.0rc6/demo/src/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/__main__.py` & `dynamicio-5.0.0rc6/demo/src/__main__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/io.py` & `dynamicio-5.0.0rc6/demo/src/io.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/runner_selection.py` & `dynamicio-5.0.0rc6/demo/src/runner_selection.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/runners/staging.py` & `dynamicio-5.0.0rc6/demo/src/runners/staging.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/src/runners/transform.py` & `dynamicio-5.0.0rc6/demo/src/runners/transform.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/tests/conftest.py` & `dynamicio-5.0.0rc6/demo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/tests/test_pipeline.py` & `dynamicio-5.0.0rc6/demo/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/demo/tests/test_runner_selection.py` & `dynamicio-5.0.0rc6/demo/tests/test_runner_selection.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/__init__.py` & `dynamicio-5.0.0rc6/dynamicio/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/cli.py` & `dynamicio-5.0.0rc6/dynamicio/cli.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/config/io_config.py` & `dynamicio-5.0.0rc6/dynamicio/config/io_config.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/config/pydantic/config.py` & `dynamicio-5.0.0rc6/dynamicio/config/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/config/pydantic/io_resources.py` & `dynamicio-5.0.0rc6/dynamicio/config/pydantic/io_resources.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/config/pydantic/table_schema.py` & `dynamicio-5.0.0rc6/dynamicio/config/pydantic/table_schema.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/core.py` & `dynamicio-5.0.0rc6/dynamicio/core.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/errors.py` & `dynamicio-5.0.0rc6/dynamicio/errors.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/metrics.py` & `dynamicio-5.0.0rc6/dynamicio/metrics.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/mixins/utils.py` & `dynamicio-5.0.0rc6/dynamicio/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/mixins/with_kafka.py` & `dynamicio-5.0.0rc6/dynamicio/mixins/with_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         "background_event_cb",
         "batch.size",
         "batch.num.messages",
         "bootstrap.servers",
         "broker.address.family",
         "broker.address.ttl",
         "broker.version.fallback",
-        "buffer.memory",
         "builtin.features",
         "check.crcs",
         "client.dns.lookup",
         "client.id",
         "client.rack",
         "closesocket_cb",
         "compression.codec",
@@ -304,29 +303,30 @@
         }
         return Producer(**self.__kafka_config)
 
     def _send_messages(self, df: pd.DataFrame, topic: str) -> None:
         logger.info(f"Sending {len(df)} messages to Kafka topic: {topic}.")
 
         messages = df.reset_index(drop=True).to_dict("records")
+
         for idx, message in zip(df.index.values, messages):
             key = self.__key_generator(idx, message)
             transformed_message = self.__document_transformer(message)
             serialized_key = self.__key_serializer(key)
             serialized_value = self.__value_serializer(transformed_message)
 
             self.__producer.produce(topic=topic, key=serialized_key, value=serialized_value, on_delivery=self._on_delivery)
 
         self.__producer.flush()
 
     @staticmethod
     def _on_delivery(err, msg):
         """Callback for message delivery."""
         if err is not None:
-            logger.error(f"Message delivery failed: {err}, for message: {msg}")
+            raise Exception(f"Message delivery failed: {err}, for message: {msg}")
 
     @staticmethod
     def _default_key_serializer(key: Optional[Any]) -> Optional[bytes]:
         if key is not None:
             return str(key).encode("utf-8")
         return None
```

### Comparing `dynamicio-5.0.0rc5/dynamicio/mixins/with_local.py` & `dynamicio-5.0.0rc6/dynamicio/mixins/with_local.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/mixins/with_postgres.py` & `dynamicio-5.0.0rc6/dynamicio/mixins/with_postgres.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/mixins/with_s3.py` & `dynamicio-5.0.0rc6/dynamicio/mixins/with_s3.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio/validations.py` & `dynamicio-5.0.0rc6/dynamicio/validations.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/dynamicio.egg-info/PKG-INFO` & `dynamicio-5.0.0rc6/dynamicio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc5
+Version: 5.0.0rc6
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc5/dynamicio.egg-info/SOURCES.txt` & `dynamicio-5.0.0rc6/dynamicio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/pyproject.toml` & `dynamicio-5.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/setup.py` & `dynamicio-5.0.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/conftest.py` & `dynamicio-5.0.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/mocking/io.py` & `dynamicio-5.0.0rc6/tests/mocking/io.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/mocking/models.py` & `dynamicio-5.0.0rc6/tests/mocking/models.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_cli.py` & `dynamicio-5.0.0rc6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_config.py` & `dynamicio-5.0.0rc6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_core.py` & `dynamicio-5.0.0rc6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_metrics.py` & `dynamicio-5.0.0rc6/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_mixins/test_kafka_mixins.py` & `dynamicio-5.0.0rc6/tests/test_mixins/test_kafka_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,15 +205,14 @@
         kafka_config.pop("value_serializer", None)  # Use .pop with default value to avoid KeyError
         kafka_config.pop("key_serializer", None)  # Use .pop with default value to avoid KeyError
 
         # Check that user options are correctly set
         assert kafka_config == {
             "batch.size": 20000000,
             "bootstrap.servers": "mock-kafka-server",
-            "buffer.memory": 134217728,
             "compression.type": "gzip",
             "linger.ms": 3000,
             "max.in.flight.requests.per.connection": 10,
             "message.send.max.retries": 3,
             "request.timeout.ms": 60000,
             "retry.backoff.ms": 100,
         }
@@ -363,7 +362,45 @@
         # When
         with patch("dynamicio.mixins.with_kafka.Producer", return_value=mock_kafka_producer_instance):
             write_kafka_io.write(keyed_test_df)
 
         # Then
         assert write_kafka_io._WithKafka__key_generator("idx", "value") == "xxx"
         assert write_kafka_io._WithKafka__document_transformer("value") == "xxx"
+
+    @pytest.mark.unit
+    def test_raise_exception_on_single_message_failure(self, input_messages_df):
+        # Given
+        def rows_generator(_df, chunk_size):
+            _chunk = []
+            for _, row in _df.iterrows():
+                _chunk.append(row.to_dict())
+                if len(_chunk) == chunk_size:
+                    yield pd.DataFrame(_chunk)
+                    _chunk.clear()
+
+        df = input_messages_df
+
+        kafka_cloud_config = IOConfig(
+            path_to_source_yaml=(os.path.join(constants.TEST_RESOURCES, "definitions/processed.yaml")),
+            env_identifier="CLOUD",
+            dynamic_vars=constants,
+        ).get(source_key="WRITE_TO_KAFKA_JSON")
+
+        # Create the MockKafkaProducer instance before patching
+        mock_kafka_producer_instance = MockKafkaProducer()
+
+        def mock_produce(*args, **kwargs):  # pylint: disable=unused-argument
+            if mock_kafka_producer_instance.produce_call_count == 1:
+                raise Exception("Mock message delivery failure")
+            mock_kafka_producer_instance.produce_call_count += 1
+
+        # When
+        with patch("dynamicio.mixins.with_kafka.Producer", return_value=mock_kafka_producer_instance):
+            with patch.object(mock_kafka_producer_instance, "produce", side_effect=mock_produce):
+                write_kafka_io = WriteKafkaIO(kafka_cloud_config)
+                with pytest.raises(Exception, match="Mock message delivery failure"):
+                    for chunk in rows_generator(_df=df, chunk_size=2):
+                        write_kafka_io.write(chunk)
+
+                # Ensure only one message is sent successfully before the failure
+                assert mock_kafka_producer_instance.produce_call_count == 1
```

### Comparing `dynamicio-5.0.0rc5/tests/test_mixins/test_local_mixins.py` & `dynamicio-5.0.0rc6/tests/test_mixins/test_local_mixins.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_mixins/test_mixin_utils.py` & `dynamicio-5.0.0rc6/tests/test_mixins/test_mixin_utils.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_mixins/test_postgres_mixins.py` & `dynamicio-5.0.0rc6/tests/test_mixins/test_postgres_mixins.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_mixins/test_s3_mixins.py` & `dynamicio-5.0.0rc6/tests/test_mixins/test_s3_mixins.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc5/tests/test_validations.py` & `dynamicio-5.0.0rc6/tests/test_validations.py`

 * *Files identical despite different names*

