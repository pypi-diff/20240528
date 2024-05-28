# Comparing `tmp/civis-2.1.0.tar.gz` & `tmp/civis-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civis-2.1.0.tar", last modified: Thu May 23 19:59:07 2024, max compression
+gzip compressed data, was "civis-2.2.0.tar", last modified: Tue May 28 20:45:36 2024, max compression
```

## Comparing `civis-2.1.0.tar` & `civis-2.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.068907 civis-2.1.0/
--rw-r--r--   0 jlee       (503) staff       (20)     1501 2023-06-28 16:43:32.000000 civis-2.1.0/LICENSE.md
--rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-23 19:59:07.067432 civis-2.1.0/PKG-INFO
--rw-r--r--   0 jlee       (503) staff       (20)     7512 2024-05-20 21:42:07.000000 civis-2.1.0/README.rst
--rw-r--r--   0 jlee       (503) staff       (20)     1990 2024-05-23 19:58:03.000000 civis-2.1.0/pyproject.toml
--rw-r--r--   0 jlee       (503) staff       (20)       38 2024-05-23 19:59:07.069164 civis-2.1.0/setup.cfg
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:06.957888 civis-2.1.0/src/
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:06.984487 civis-2.1.0/src/civis/
--rw-r--r--   0 jlee       (503) staff       (20)      446 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)     3171 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/_deprecation.py
--rw-r--r--   0 jlee       (503) staff       (20)     5387 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/_utils.py
--rw-r--r--   0 jlee       (503) staff       (20)    10829 2024-05-20 02:15:26.000000 civis-2.1.0/src/civis/base.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:06.996032 civis-2.1.0/src/civis/cli/
--rw-r--r--   0 jlee       (503) staff       (20)       73 2024-05-13 18:11:55.000000 civis-2.1.0/src/civis/cli/__init__.py
--rwxr-xr-x   0 jlee       (503) staff       (20)    11639 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/cli/__main__.py
--rw-r--r--   0 jlee       (503) staff       (20)    11849 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/cli/_cli_commands.py
--rw-r--r--   0 jlee       (503) staff       (20)    10665 2024-05-20 13:20:42.000000 civis-2.1.0/src/civis/client.py
--rw-r--r--   0 jlee       (503) staff       (20)  2209678 2024-05-23 19:58:03.000000 civis-2.1.0/src/civis/client.pyi
--rw-r--r--   0 jlee       (503) staff       (20)    27130 2024-05-20 21:42:07.000000 civis-2.1.0/src/civis/futures.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.003111 civis-2.1.0/src/civis/io/
--rw-r--r--   0 jlee       (503) staff       (20)      145 2024-05-13 18:11:55.000000 civis-2.1.0/src/civis/io/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)     5229 2024-05-20 21:42:07.000000 civis-2.1.0/src/civis/io/_databases.py
--rw-r--r--   0 jlee       (503) staff       (20)    21558 2024-05-20 21:42:07.000000 civis-2.1.0/src/civis/io/_files.py
--rw-r--r--   0 jlee       (503) staff       (20)    55786 2024-05-20 21:42:07.000000 civis-2.1.0/src/civis/io/_tables.py
--rw-r--r--   0 jlee       (503) staff       (20)     3223 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/loggers.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.007731 civis-2.1.0/src/civis/ml/
--rw-r--r--   0 jlee       (503) staff       (20)      110 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/ml/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)    12005 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/ml/_helper.py
--rw-r--r--   0 jlee       (503) staff       (20)    63734 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/ml/_model.py
--rw-r--r--   0 jlee       (503) staff       (20)    41253 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/parallel.py
--rw-r--r--   0 jlee       (503) staff       (20)     8573 2024-05-16 14:28:12.000000 civis-2.1.0/src/civis/polling.py
--rw-r--r--   0 jlee       (503) staff       (20)        0 2024-05-13 18:11:55.000000 civis-2.1.0/src/civis/py.typed
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.013728 civis-2.1.0/src/civis/resources/
--rw-r--r--   0 jlee       (503) staff       (20)      357 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/resources/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)     3686 2024-05-23 19:58:03.000000 civis-2.1.0/src/civis/resources/_client_pyi.py
--rw-r--r--   0 jlee       (503) staff       (20)    22167 2024-05-20 13:20:42.000000 civis-2.1.0/src/civis/resources/_resources.py
--rw-r--r--   0 jlee       (503) staff       (20)  2297577 2024-05-23 19:58:03.000000 civis-2.1.0/src/civis/resources/civis_api_spec.json
--rw-r--r--   0 jlee       (503) staff       (20)    11904 2024-05-23 19:58:03.000000 civis-2.1.0/src/civis/response.py
--rwxr-xr-x   0 jlee       (503) staff       (20)     5054 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/run_joblib_func.py
--rw-r--r--   0 jlee       (503) staff       (20)     7684 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/service_client.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.020784 civis-2.1.0/src/civis/tests/
--rw-r--r--   0 jlee       (503) staff       (20)      165 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/tests/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)     3414 2024-05-20 21:42:07.000000 civis-2.1.0/src/civis/tests/mocks.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.023627 civis-2.1.0/src/civis/utils/
--rw-r--r--   0 jlee       (503) staff       (20)       91 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/utils/__init__.py
--rw-r--r--   0 jlee       (503) staff       (20)     3272 2024-05-15 13:36:23.000000 civis-2.1.0/src/civis/utils/_jobs.py
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.060994 civis-2.1.0/src/civis.egg-info/
--rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/PKG-INFO
--rw-r--r--   0 jlee       (503) staff       (20)     1422 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/SOURCES.txt
--rw-r--r--   0 jlee       (503) staff       (20)        1 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/dependency_links.txt
--rw-r--r--   0 jlee       (503) staff       (20)       99 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/entry_points.txt
--rw-r--r--   0 jlee       (503) staff       (20)      381 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/requires.txt
--rw-r--r--   0 jlee       (503) staff       (20)        6 2024-05-23 19:59:06.000000 civis-2.1.0/src/civis.egg-info/top_level.txt
-drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-23 19:59:07.058467 civis-2.1.0/tests/
--rw-r--r--   0 jlee       (503) staff       (20)     1494 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_base.py
--rw-r--r--   0 jlee       (503) staff       (20)     6635 2024-05-20 21:42:07.000000 civis-2.1.0/tests/test_cli.py
--rw-r--r--   0 jlee       (503) staff       (20)     2341 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_client.py
--rw-r--r--   0 jlee       (503) staff       (20)     4101 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_deprecate.py
--rw-r--r--   0 jlee       (503) staff       (20)    15467 2024-05-16 15:37:34.000000 civis-2.1.0/tests/test_futures.py
--rw-r--r--   0 jlee       (503) staff       (20)    52275 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_io.py
--rw-r--r--   0 jlee       (503) staff       (20)     4599 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_jobs.py
--rw-r--r--   0 jlee       (503) staff       (20)     2999 2024-05-13 18:11:55.000000 civis-2.1.0/tests/test_loggers.py
--rw-r--r--   0 jlee       (503) staff       (20)      487 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_mocks.py
--rw-r--r--   0 jlee       (503) staff       (20)    22269 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_parallel.py
--rw-r--r--   0 jlee       (503) staff       (20)     3590 2024-05-16 14:28:12.000000 civis-2.1.0/tests/test_polling.py
--rw-r--r--   0 jlee       (503) staff       (20)    30059 2024-05-23 19:58:03.000000 civis-2.1.0/tests/test_resources.py
--rw-r--r--   0 jlee       (503) staff       (20)    12589 2024-05-23 19:58:03.000000 civis-2.1.0/tests/test_response.py
--rw-r--r--   0 jlee       (503) staff       (20)      181 2024-05-20 21:42:07.000000 civis-2.1.0/tests/test_run_joblib_func.py
--rw-r--r--   0 jlee       (503) staff       (20)    10238 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_service_client.py
--rw-r--r--   0 jlee       (503) staff       (20)    11118 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_utils.py
--rw-r--r--   0 jlee       (503) staff       (20)      560 2024-05-15 13:36:23.000000 civis-2.1.0/tests/test_version.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.821678 civis-2.2.0/
+-rw-r--r--   0 jlee       (503) staff       (20)     1501 2023-06-28 16:43:32.000000 civis-2.2.0/LICENSE.md
+-rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-28 20:45:36.820618 civis-2.2.0/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)     7512 2024-05-20 21:42:07.000000 civis-2.2.0/README.rst
+-rw-r--r--   0 jlee       (503) staff       (20)     1990 2024-05-28 20:00:34.000000 civis-2.2.0/pyproject.toml
+-rw-r--r--   0 jlee       (503) staff       (20)       38 2024-05-28 20:45:36.821926 civis-2.2.0/setup.cfg
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.708469 civis-2.2.0/src/
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.740576 civis-2.2.0/src/civis/
+-rw-r--r--   0 jlee       (503) staff       (20)      446 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3171 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/_deprecation.py
+-rw-r--r--   0 jlee       (503) staff       (20)     5387 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/_utils.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10829 2024-05-20 02:15:26.000000 civis-2.2.0/src/civis/base.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.751222 civis-2.2.0/src/civis/cli/
+-rw-r--r--   0 jlee       (503) staff       (20)       73 2024-05-13 18:11:55.000000 civis-2.2.0/src/civis/cli/__init__.py
+-rwxr-xr-x   0 jlee       (503) staff       (20)    11738 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/cli/__main__.py
+-rw-r--r--   0 jlee       (503) staff       (20)    11849 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/cli/_cli_commands.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10665 2024-05-20 13:20:42.000000 civis-2.2.0/src/civis/client.py
+-rw-r--r--   0 jlee       (503) staff       (20)  2209678 2024-05-28 18:57:02.000000 civis-2.2.0/src/civis/client.pyi
+-rw-r--r--   0 jlee       (503) staff       (20)    27130 2024-05-20 21:42:07.000000 civis-2.2.0/src/civis/futures.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.756836 civis-2.2.0/src/civis/io/
+-rw-r--r--   0 jlee       (503) staff       (20)      145 2024-05-13 18:11:55.000000 civis-2.2.0/src/civis/io/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     5229 2024-05-20 21:42:07.000000 civis-2.2.0/src/civis/io/_databases.py
+-rw-r--r--   0 jlee       (503) staff       (20)    21553 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/io/_files.py
+-rw-r--r--   0 jlee       (503) staff       (20)    55786 2024-05-20 21:42:07.000000 civis-2.2.0/src/civis/io/_tables.py
+-rw-r--r--   0 jlee       (503) staff       (20)     2914 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/loggers.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.761906 civis-2.2.0/src/civis/ml/
+-rw-r--r--   0 jlee       (503) staff       (20)      110 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/ml/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)    12005 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/ml/_helper.py
+-rw-r--r--   0 jlee       (503) staff       (20)    63734 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/ml/_model.py
+-rw-r--r--   0 jlee       (503) staff       (20)    41316 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/parallel.py
+-rw-r--r--   0 jlee       (503) staff       (20)     8573 2024-05-16 14:28:12.000000 civis-2.2.0/src/civis/polling.py
+-rw-r--r--   0 jlee       (503) staff       (20)        0 2024-05-13 18:11:55.000000 civis-2.2.0/src/civis/py.typed
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.769007 civis-2.2.0/src/civis/resources/
+-rw-r--r--   0 jlee       (503) staff       (20)      357 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/resources/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3686 2024-05-23 19:58:03.000000 civis-2.2.0/src/civis/resources/_client_pyi.py
+-rw-r--r--   0 jlee       (503) staff       (20)    22167 2024-05-20 13:20:42.000000 civis-2.2.0/src/civis/resources/_resources.py
+-rw-r--r--   0 jlee       (503) staff       (20)  2297577 2024-05-28 18:57:02.000000 civis-2.2.0/src/civis/resources/civis_api_spec.json
+-rw-r--r--   0 jlee       (503) staff       (20)    13608 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/response.py
+-rwxr-xr-x   0 jlee       (503) staff       (20)     5054 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/run_joblib_func.py
+-rw-r--r--   0 jlee       (503) staff       (20)     7684 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/service_client.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.781149 civis-2.2.0/src/civis/tests/
+-rw-r--r--   0 jlee       (503) staff       (20)      165 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/tests/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3523 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/tests/mocks.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.783788 civis-2.2.0/src/civis/utils/
+-rw-r--r--   0 jlee       (503) staff       (20)       91 2024-05-15 13:36:23.000000 civis-2.2.0/src/civis/utils/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3267 2024-05-28 20:00:34.000000 civis-2.2.0/src/civis/utils/_jobs.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.814427 civis-2.2.0/src/civis.egg-info/
+-rw-r--r--   0 jlee       (503) staff       (20)     9387 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)     1422 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/SOURCES.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        1 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/dependency_links.txt
+-rw-r--r--   0 jlee       (503) staff       (20)       99 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/entry_points.txt
+-rw-r--r--   0 jlee       (503) staff       (20)      381 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/requires.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        6 2024-05-28 20:45:36.000000 civis-2.2.0/src/civis.egg-info/top_level.txt
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2024-05-28 20:45:36.812714 civis-2.2.0/tests/
+-rw-r--r--   0 jlee       (503) staff       (20)     1494 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_base.py
+-rw-r--r--   0 jlee       (503) staff       (20)     6635 2024-05-20 21:42:07.000000 civis-2.2.0/tests/test_cli.py
+-rw-r--r--   0 jlee       (503) staff       (20)     2341 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_client.py
+-rw-r--r--   0 jlee       (503) staff       (20)     4101 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_deprecate.py
+-rw-r--r--   0 jlee       (503) staff       (20)    15895 2024-05-28 20:00:34.000000 civis-2.2.0/tests/test_futures.py
+-rw-r--r--   0 jlee       (503) staff       (20)    52275 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_io.py
+-rw-r--r--   0 jlee       (503) staff       (20)     4599 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_jobs.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3140 2024-05-28 20:00:34.000000 civis-2.2.0/tests/test_loggers.py
+-rw-r--r--   0 jlee       (503) staff       (20)      487 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_mocks.py
+-rw-r--r--   0 jlee       (503) staff       (20)    22269 2024-05-28 20:00:34.000000 civis-2.2.0/tests/test_parallel.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3590 2024-05-16 14:28:12.000000 civis-2.2.0/tests/test_polling.py
+-rw-r--r--   0 jlee       (503) staff       (20)    30059 2024-05-23 19:58:03.000000 civis-2.2.0/tests/test_resources.py
+-rw-r--r--   0 jlee       (503) staff       (20)    15273 2024-05-28 20:00:34.000000 civis-2.2.0/tests/test_response.py
+-rw-r--r--   0 jlee       (503) staff       (20)      181 2024-05-20 21:42:07.000000 civis-2.2.0/tests/test_run_joblib_func.py
+-rw-r--r--   0 jlee       (503) staff       (20)    10238 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_service_client.py
+-rw-r--r--   0 jlee       (503) staff       (20)    11118 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_utils.py
+-rw-r--r--   0 jlee       (503) staff       (20)      560 2024-05-15 13:36:23.000000 civis-2.2.0/tests/test_version.py
```

### Comparing `civis-2.1.0/LICENSE.md` & `civis-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/PKG-INFO` & `civis-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Civis API Python Client
 Author-email: Civis Analytics <opensource@civisanalytics.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://www.civisanalytics.com
 Project-URL: Source, https://github.com/civisanalytics/civis-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `civis-2.1.0/README.rst` & `civis-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/pyproject.toml` & `civis-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "civis"
-version = "2.1.0"
+version = "2.2.0"
 description = "Civis API Python Client"
 readme = "README.rst"
 requires-python = ">= 3.9"
 authors = [ { name = "Civis Analytics", email = "opensource@civisanalytics.com" } ]
 license = { text = "BSD-3-Clause" }
 dependencies = [
     "PyYAML >= 3.0",
```

### Comparing `civis-2.1.0/src/civis/_deprecation.py` & `civis-2.2.0/src/civis/_deprecation.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/_utils.py` & `civis-2.2.0/src/civis/_utils.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/base.py` & `civis-2.2.0/src/civis/base.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/cli/__main__.py` & `civis-2.2.0/src/civis/cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import time
 from warnings import warn
 
 import click
 from jsonref import JsonRef
 import yaml
 from requests import Request
+
+import civis
 from civis.cli._cli_commands import (
     civis_ascii_art,
     files_download_cmd,
     files_upload_cmd,
     jobs_follow_log,
     jobs_follow_run_log,
     notebooks_download_cmd,
@@ -256,14 +258,15 @@
     spec = retrieve_spec_dict()
 
     # Replace references in the spec so that we don't have to worry about them
     # when making the CLI.
     spec = JsonRef.replace_refs(spec)
 
     cli = click.Group()
+    cli = click.version_option(version=civis.__version__, package_name="civis")(cli)
 
     # Iterate through top-level resources (e.g., Scripts, Files, Models).
     groups = {}
     for path, path_dict in spec["paths"].items():
         resource = path.strip("/").split("/")[0]
         grp = groups.get(resource)
         if grp is None:
```

### Comparing `civis-2.1.0/src/civis/cli/_cli_commands.py` & `civis-2.2.0/src/civis/cli/_cli_commands.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/client.py` & `civis-2.2.0/src/civis/client.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/client.pyi` & `civis-2.2.0/src/civis/client.pyi`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/futures.py` & `civis-2.2.0/src/civis/futures.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/io/_databases.py` & `civis-2.2.0/src/civis/io/_databases.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/io/_files.py` & `civis-2.2.0/src/civis/io/_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     file_response = client.files.post(name, **kwargs)
 
     # Platform has given us a URL to which we can upload a file.
     # The file must be uploaded with a POST formatted as per
     # http://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-post-example.html
     # Note that the payload must have "key" first and "file" last.
     url = file_response.upload_url
-    form = file_response.upload_fields._data_snake
+    form = file_response.upload_fields.json()
     form_key = OrderedDict(key=form.pop("key"))
     form_key.update(form)
 
     # Store the current buffer position in case we need to retry below.
     buf_orig_position = buf.tell()
 
     @retry(RETRY_EXCEPTIONS)
```

### Comparing `civis-2.1.0/src/civis/io/_tables.py` & `civis-2.2.0/src/civis/io/_tables.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/loggers.py` & `civis-2.2.0/src/civis/loggers.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,20 +56,15 @@
         logger.setLevel(os.getenv("CIVIS_LOG_LEVEL") or logging.INFO)
     else:
         logger.setLevel(level)
 
     # When running on Civis Platform (as opposed to unit tests in CI),
     # we don't want to propagate log records to the root logger
     # in order to avoid duplicate logs.
-    # But in running unit tests we do want to leave `propagate` as `True`,
-    # or else all the logging/caplog tests would fail.
-    # The user can set the `propagate` attribute of the resulting logger
-    # back to True if they so choose.
-    if os.getenv("CIVIS_JOB_ID") and os.getenv("CIVIS_RUN_ID"):
-        logger.propagate = False
+    logger.propagate = False
 
     if isinstance(fmt, logging.Formatter):
         platform_fmt = fmt
     else:
         platform_fmt = logging.Formatter(fmt)
 
     at_or_below_info_hdlr = logging.StreamHandler(sys.stdout)
```

### Comparing `civis-2.1.0/src/civis/ml/_helper.py` & `civis-2.2.0/src/civis/ml/_helper.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/ml/_model.py` & `civis-2.2.0/src/civis/ml/_model.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/parallel.py` & `civis-2.2.0/src/civis/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,68 +190,70 @@
     """
     if client is None:
         client = civis.APIClient()
 
     if not os.environ.get("CIVIS_JOB_ID"):
         raise RuntimeError("This function must be run " "inside a container job.")
     state = client.scripts.get_containers(os.environ["CIVIS_JOB_ID"])
+    state_json = state.json()
     if state.from_template_id:
         # If this is a Custom Script from a template, we need the
         # backing script. Make sure to save the arguments from
         # the Custom Script: those are the only user-settable parts.
         template = client.templates.get_scripts(state.from_template_id)
         try:
-            custom_args = state.arguments
+            custom_args = state_json["arguments"]
             state = client.scripts.get_containers(template.script_id)
-            state._replace("arguments", custom_args)
+            state_json = state.json()
+            state_json["arguments"] = custom_args
         except civis.base.CivisAPIError as err:
             if err.status_code == 404:
                 raise RuntimeError(
                     "Unable to introspect environment from "
                     "your template's backing script. "
                     "You may not have permission to view "
                     "script ID {}.".format(template.script_id)
                 )
             else:
                 raise
 
     # Default to this container's resource requests, but
     # allow users to override it.
-    state.required_resources._data_snake.update(required_resources or {})
+    state_json["required_resources"].update(required_resources or {})
 
     # Update parameters with user input
     params = params or []
     for input_param in params:
-        for i, param in enumerate(list(state.params)):
+        for param in state_json["params"]:
             if param["name"] == input_param["name"]:
-                param._data_snake.update(input_param)
+                param.update(input_param)
                 break
         else:
-            state._data_snake["params"].append(input_param)
+            state_json["params"].append(input_param)
 
     # Update arguments with input
-    state.arguments._data_snake.update(arguments or {})
+    state_json["arguments"].update(arguments or {})
 
     # Set defaults on other keyword arguments with
     # values from the current script
     for key in KEYS_TO_INFER:
-        kwargs.setdefault(key, state[key])
+        kwargs.setdefault(key, state_json[key])
 
     # Don't include parent job params since they're added automatically
     # in _ContainerShellExecutor.__init__.
     filtered_params = [
         p
-        for p in state.params
+        for p in state_json["params"]
         if p["name"].upper() not in ("CIVIS_PARENT_JOB_ID", "CIVIS_PARENT_RUN_ID")
     ]
 
     return make_backend_factory(
-        required_resources=state.required_resources,
+        required_resources=state_json["required_resources"],
         params=filtered_params,
-        arguments=state.arguments,
+        arguments=state_json["arguments"],
         client=client,
         polling_interval=polling_interval,
         setup_cmd=setup_cmd,
         max_submit_retries=max_submit_retries,
         max_job_retries=max_job_retries,
         hidden=hidden,
         remote_backend=remote_backend,
```

### Comparing `civis-2.1.0/src/civis/polling.py` & `civis-2.2.0/src/civis/polling.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/resources/_client_pyi.py` & `civis-2.2.0/src/civis/resources/_client_pyi.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/resources/_resources.py` & `civis-2.2.0/src/civis/resources/_resources.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/resources/civis_api_spec.json` & `civis-2.2.0/src/civis/resources/civis_api_spec.json`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/response.py` & `civis-2.2.0/src/civis/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import dataclasses
+import json
+import pprint
+
 import requests
 
 from civis._utils import camel_to_snake
 
 
 _RETURN_TYPES = frozenset({"snake", "raw"})
 
@@ -96,15 +100,15 @@
 class Response:
     """Custom Civis response object.
 
     Attributes
     ----------
     json_data : dict | None
         This is `json_data` as it is originally returned to the user without
-        the key names being changed. See Notes. None is used if the original
+        the key names being changed. None is used if the original
         response returned a 204 No Content response.
     headers : dict
         This is the header for the API call without changing the key names.
     calls_remaining : int
         Number of API calls remaining before rate limit is reached.
     rate_limit : int
         Total number of calls per API rate limit period.
@@ -116,29 +120,36 @@
         self.calls_remaining = (
             int(x) if (x := (headers or {}).get("X-RateLimit-Remaining")) else x
         )
         self.rate_limit = (
             int(x) if (x := (headers or {}).get("X-RateLimit-Limit")) else x
         )
 
+        # Note that these two dicts can have Response objects as values.
         self._data_camel = {}
         self._data_snake = {}
 
+        self._inner_response = False
+
         if json_data is not None:
             for key, v in json_data.items():
 
                 if isinstance(v, dict):
                     # Script arguments are often environment variables in
                     # ALL_CAPS that we don't want to convert to snake_case.
                     if key == "arguments":
                         val = Response(v, snake_case=False)
                     else:
                         val = Response(v)
+                    val._inner_response = True
                 elif isinstance(v, list):
                     val = [Response(o) if isinstance(o, dict) else o for o in v]
+                    for r in val:
+                        if isinstance(r, Response):
+                            r._inner_response = True
                 else:
                     val = v
 
                 key_snake = camel_to_snake(key) if snake_case else key
 
                 self._data_camel[key] = val
                 self._data_snake[key_snake] = val
@@ -162,15 +173,20 @@
             return self._to_dict_with_snake_case_keys()
         else:
             return self.json_data.copy()
 
     def _to_dict_with_snake_case_keys(self):
         result = {}
         for k, v in self._data_snake.items():
-            if isinstance(v, Response):
+            if isinstance(v, list):
+                result[k] = [
+                    o._to_dict_with_snake_case_keys() if isinstance(o, Response) else o
+                    for o in v
+                ]
+            elif isinstance(v, Response):
                 result[k] = v._to_dict_with_snake_case_keys()
             else:
                 result[k] = v
         return result
 
     def __setattr__(self, key, value):
         if key == "__dict__":
@@ -178,14 +194,15 @@
         elif key in (
             "json_data",
             "headers",
             "calls_remaining",
             "rate_limit",
             "_data_camel",
             "_data_snake",
+            "_inner_response",
         ):
             self.__dict__[key] = value
         else:
             _raise_response_immutable_error()
 
     def __setitem__(self, key, value):
         _raise_response_immutable_error()
@@ -202,15 +219,35 @@
         except KeyError as e:
             raise AttributeError(f"Response object has no attribute {str(e)}")
 
     def __len__(self):
         return len(self._data_snake)
 
     def __repr__(self):
-        return repr(self._data_snake)
+        return repr(self._to_dataclass_repr_pprint())
+
+    def __hash__(self):
+        return hash(json.dumps(self.json_data))
+
+    def _to_dataclass_repr_pprint(self):
+        """Convert the response to a dataclass for repr and pprint purposes."""
+        # Only show the "Response" class name at the outermost level.
+        class_name = "" if self._inner_response else "Response"
+        klass = dataclasses.make_dataclass(class_name, self._data_snake.keys())
+        return klass(**self._data_snake)
+
+    def _repr_pretty_(self, p, cycle):
+        """Pretty-print the response object in IPython and Jupyter.
+
+        https://ipython.readthedocs.io/en/stable/api/generated/IPython.lib.pretty.html#extending
+        """
+        if cycle:
+            p.text("Response(...)")
+        else:
+            p.text(pprint.pformat(self._to_dataclass_repr_pprint()))
 
     def get(self, key, default=None):
         """Get the value for the given key."""
         try:
             return self.__getitem__(key)
         except KeyError:
             return default
@@ -227,17 +264,28 @@
         else:
             raise TypeError(f"Response and {type(other)} can't be compared")
 
     def __setstate__(self, state):
         """Set the state when unpickling, to avoid RecursionError."""
         self.__dict__ = state
 
-    def _replace(self, key, value):
-        """Only used within this repo; `key` assumed to be in snake_case."""
-        self._data_snake[key] = value
+
+class _ResponsePrettyPrinter(pprint.PrettyPrinter):
+    """Override pprint.PrettyPrinter so that pprint.pprint(response) works nicely.
+
+    https://stackoverflow.com/a/15417704
+    """
+
+    def _format(self, obj, stream, indent, allowance, context, level):
+        if isinstance(obj, Response):
+            obj = obj._to_dataclass_repr_pprint()
+        super()._format(obj, stream, indent, allowance, context, level)
+
+
+pprint.PrettyPrinter = _ResponsePrettyPrinter
 
 
 class PaginatedResponse:
     """A response object which is an iterator
 
     Parameters
     ----------
```

### Comparing `civis-2.1.0/src/civis/run_joblib_func.py` & `civis-2.2.0/src/civis/run_joblib_func.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/service_client.py` & `civis-2.2.0/src/civis/service_client.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/src/civis/tests/mocks.py` & `civis-2.2.0/src/civis/tests/mocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,28 +68,28 @@
     c = create_client_mock()
 
     mock_container = Response({"id": script_id})
     c.scripts.post_containers.return_value = mock_container
     mock_container_run_start = Response(
         {"id": run_id, "container_id": script_id, "state": "queued"}
     )
-    mock_container_run = Response(
-        {"id": run_id, "container_id": script_id, "state": state}
-    )
+    mock_container_run_json = {"id": run_id, "container_id": script_id, "state": state}
     if state == "failed":
-        mock_container_run._replace("error", "None")
+        mock_container_run_json["error"] = "None"
+    mock_container_run = Response(mock_container_run_json)
     c.scripts.post_containers_runs.return_value = mock_container_run_start
     c.scripts.get_containers_runs.return_value = mock_container_run
     c.scripts.list_containers_runs_outputs.return_value = run_outputs or []
     c.jobs.list_runs_outputs.return_value = run_outputs or []
     c.jobs.list_runs_logs.return_value = log_outputs or []
 
     def change_state_to_cancelled(script_id):
-        mock_container_run._replace("state", "cancelled")
-        return mock_container_run
+        mock_container_run_json = mock_container_run.json()
+        mock_container_run_json["state"] = "cancelled"
+        return Response(mock_container_run_json)
 
     c.scripts.post_cancel.side_effect = change_state_to_cancelled
 
     return c
 
 
 @lru_cache(maxsize=1)
```

### Comparing `civis-2.1.0/src/civis/utils/_jobs.py` & `civis-2.2.0/src/civis/utils/_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,11 +88,11 @@
         if len(json_output) > 1:
             log.warning(
                 "More than 1 JSON output for template {}"
                 " -- returning only the first one.".format(id)
             )
         # Note that the cast to a dict is to convert
         # an expected Response object.
-        return json_output[0]._data_snake
+        return json_output[0].json()
     else:
         file_ids = {o.name: o.object_id for o in outputs}
         return file_ids
```

### Comparing `civis-2.1.0/src/civis.egg-info/PKG-INFO` & `civis-2.2.0/src/civis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Civis API Python Client
 Author-email: Civis Analytics <opensource@civisanalytics.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://www.civisanalytics.com
 Project-URL: Source, https://github.com/civisanalytics/civis-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `civis-2.1.0/src/civis.egg-info/SOURCES.txt` & `civis-2.2.0/src/civis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_base.py` & `civis-2.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_cli.py` & `civis-2.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_client.py` & `civis-2.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_deprecate.py` & `civis-2.2.0/tests/test_deprecate.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_futures.py` & `civis-2.2.0/tests/test_futures.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,31 +108,37 @@
         )
         future = bpe.submit(my_param="spam")
     else:
         bpe = _ContainerShellExecutor(client=c, polling_interval=0.01)
         future = bpe.submit("foo")
 
     # Mock and test running, future.job_id, and done()
-    mock_run._replace("state", "running")
+    mock_run_json = mock_run.json()
+    mock_run_json["state"] = "running"
+    mock_run = response.Response(mock_run_json)
     assert future.running(), "future is incorrectly marked as not running"
     assert future.job_id == job_id, "job_id not stored properly"
     assert not future.done(), "future is incorrectly marked as done"
 
     future.cancel()
 
     # Mock and test cancelled()
     assert future.cancelled(), "cancelled() did not return True as expected"
     assert not future.running(), "running() did not return False as expected"
 
     # Mock and test done()
-    mock_run._replace("state", "succeeded")
+    mock_run_json = mock_run.json()
+    mock_run_json["state"] = "succeeded"
+    mock_run = response.Response(mock_run_json)
     assert future.done(), "done() did not return True as expected"
 
     # Test cancelling all jobs.
-    mock_run._replace("state", "running")
+    mock_run_json = mock_run.json()
+    mock_run_json["state"] = "running"
+    mock_run = response.Response(mock_run_json)
     bpe.cancel_all()
     assert future.cancelled(), "cancel_all() failed"
 
     # Test shutdown method.
     bpe.shutdown(wait=True)
     assert future.done(), "shutdown() failed"
 
@@ -294,16 +300,17 @@
     c.scripts.post_containers_runs.return_value = mock_container_run
     c.jobs.post_runs.return_value = mock_container_run
     c.scripts.get_containers_runs.side_effect = _make_error_func(
         n_failures, failure_is_error
     )
 
     def change_state_to_cancelled(job_id):
-        mock_container_run._replace("state", "cancelled")
-        return mock_container_run
+        mock_container_run_json = mock_container_run.json()
+        mock_container_run_json["state"] = "cancelled"
+        return response.Response(mock_container_run_json)
 
     c.scripts.post_cancel.side_effect = change_state_to_cancelled
 
     return c
 
 
 def test_cancel_finished_job():
@@ -321,15 +328,17 @@
             "status_code": status_code,
             "error": "not_found",
             "errorDescription": "The requested resource could not be found.",
             "content": True,
         }
     ).encode()
     c.scripts.post_cancel.side_effect = CivisAPIError(err_resp)
-    c.scripts.post_containers_runs.return_value._replace("state", "running")
+    resp_json = c.scripts.post_containers_runs.return_value.json()
+    resp_json["state"] = "running"
+    c.scripts.post_containers_runs.return_value = response.Response(resp_json)
     fut = ContainerFuture(
         -10, 100, polling_interval=1, client=c, poll_on_creation=False
     )
     assert not fut.done()
     with warnings.catch_warnings():
         # Check that no warnings are raised.
         warnings.simplefilter("error")
```

### Comparing `civis-2.1.0/tests/test_io.py` & `civis-2.2.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_jobs.py` & `civis-2.2.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_loggers.py` & `civis-2.2.0/tests/test_loggers.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from civis import civis_logger
 
 
 def _get_test_logger(*args, **kwargs):
     # Need to use a logger of a different name in each test function,
     # or else we'd hit this issue:
     # https://github.com/pytest-dev/pytest/issues/5577
-    return civis_logger(name=str(uuid4()), *args, **kwargs)
+    logger = civis_logger(name=str(uuid4()), *args, **kwargs)
+    # Set `propagate` back to `True`,
+    # or else all the logging/caplog tests would fail.
+    logger.propagate = True
+    return logger
 
 
 def test_civis_logger_base_case(caplog, capsys):
     log = _get_test_logger()
     caplog.set_level(log.level)
 
     log.debug("debug level")
```

### Comparing `civis-2.1.0/tests/test_parallel.py` & `civis-2.2.0/tests/test_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     mock_client = create_client_mock()
     mock_client.scripts.get_containers.return_value = mock_job
     with mock.patch.dict(
         "os.environ", {"CIVIS_JOB_ID": "test_job", "CIVIS_RUN_ID": "test_run"}
     ):
         civis.parallel.infer_backend_factory(client=mock_client)
 
-    expected = mock_job._data_snake
+    expected = mock_job.json()
     del expected["from_template_id"]
     del expected["id"]
     mock_make_factory.assert_called_once_with(
         client=mock_client,
         setup_cmd=None,
         polling_interval=None,
         max_submit_retries=0,
@@ -456,15 +456,15 @@
     fut = ContainerFuture(1, 2, client=mock_client)
     res = civis.parallel._CivisBackendResult(fut, callback)
     fut._set_api_exception(CivisJobFailure(Response({"state": "failed"})))
 
     with pytest.raises(TransportableException) as exc:
         res.get()
 
-    assert "{'state': 'failed'}" in str(exc.value)
+    assert "Response(state='failed')" in str(exc.value)
     assert callback.call_count == 0
 
 
 @mock.patch.object(civis.parallel, "civis")
 def test_result_callback_exception(mock_civis):
     # An error in the result retrieval should be raised by .get
     callback = mock.MagicMock()
```

### Comparing `civis-2.1.0/tests/test_polling.py` & `civis-2.2.0/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_resources.py` & `civis-2.2.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_response.py` & `civis-2.2.0/tests/test_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import io
 import pickle
+import pprint
+import sys
+from string import ascii_lowercase
 from unittest import mock
 
 import pytest
 import requests
 
 from civis.response import (
     CivisClientError,
@@ -267,14 +270,19 @@
     "source, as_snake_case",
     [
         ({"foo": {"barBar": 1}}, {"foo": {"bar_bar": 1}}),
         (
             {"fooBar": 1, "arguments": {"FOO": 2, "FOO_BAR": 3}},
             {"foo_bar": 1, "arguments": {"FOO": 2, "FOO_BAR": 3}},
         ),
+        (
+            {"fooBar": [{"name": "a", "type": "b"}, {"name": "c", "type": "d"}]},
+            {"foo_bar": [{"name": "a", "type": "b"}, {"name": "c", "type": "d"}]},
+        ),
+        ({"fooBar": ["a", "b", "c"]}, {"foo_bar": ["a", "b", "c"]}),
     ],
 )
 def test_json(source, as_snake_case):
     response = Response(source)
     assert response.json() == as_snake_case
     assert response.json(snake_case=False) == source
 
@@ -310,25 +318,94 @@
     assert response.json_data == json_data
     assert len(response) == expected_length
 
 
 @pytest.mark.parametrize(
     "json_data, expected_repr",
     [
-        ({}, "{}"),
-        ({"foo": 123}, "{'foo': 123}"),
-        ({"foo": {"barBaz": 456}}, "{'foo': {'bar_baz': 456}}"),
+        (None, "Response()"),
+        ({}, "Response()"),
+        ({"foo": 123}, "Response(foo=123)"),
+        ({"foo": {"barBaz": 456}}, "Response(foo=(bar_baz=456))"),
+        # repr() call doesn't wrap long lines.
+        (
+            {
+                "foo": {ascii_lowercase[i]: i for i in range(3)},
+                "fooBar": {ascii_lowercase[i]: i for i in range(15)},
+            },
+            "Response(foo=(a=0, b=1, c=2), foo_bar=(a=0, b=1, c=2, d=3, e=4, f=5, g=6, h=7, i=8, j=9, k=10, l=11, m=12, n=13, o=14))",  # noqa: E501
+        ),
     ],
 )
 def test_repr(json_data, expected_repr):
     response = Response(json_data)
     assert response.json_data == json_data
     assert repr(response) == expected_repr
 
 
+@pytest.mark.skipif(
+    sys.version_info < (3, 10),
+    reason=(
+        "pprint for dataclasses is only available since 3.10+, "
+        "https://bugs.python.org/issue43080"
+    ),
+)
+@pytest.mark.parametrize(
+    "json_data, expected",
+    [
+        # A "short" response's pprint looks the same as its repr.
+        ({"foo": {"barBaz": 456}}, "Response(foo=(bar_baz=456))"),
+        # A "long" response's pprint triggers line wrapping in pretty-printing.
+        (
+            {ascii_lowercase[i]: i for i in range(15)},
+            "Response(a=0,\n"
+            "         b=1,\n"
+            "         c=2,\n"
+            "         d=3,\n"
+            "         e=4,\n"
+            "         f=5,\n"
+            "         g=6,\n"
+            "         h=7,\n"
+            "         i=8,\n"
+            "         j=9,\n"
+            "         k=10,\n"
+            "         l=11,\n"
+            "         m=12,\n"
+            "         n=13,\n"
+            "         o=14)",
+        ),
+        (
+            {
+                "foo": {ascii_lowercase[i]: i for i in range(3)},
+                "fooBar": {ascii_lowercase[i]: i for i in range(15)},
+            },
+            "Response(foo=(a=0, b=1, c=2),\n"
+            "         foo_bar=(a=0,\n"
+            "                  b=1,\n"
+            "                  c=2,\n"
+            "                  d=3,\n"
+            "                  e=4,\n"
+            "                  f=5,\n"
+            "                  g=6,\n"
+            "                  h=7,\n"
+            "                  i=8,\n"
+            "                  j=9,\n"
+            "                  k=10,\n"
+            "                  l=11,\n"
+            "                  m=12,\n"
+            "                  n=13,\n"
+            "                  o=14))",
+        ),
+    ],
+)
+def test_pprint(json_data, expected):
+    response = Response(json_data)
+    assert pprint.pformat(response) == expected
+
+
 def test_get():
     # JSON data from the Civis API is in camelCase.
     json_data = {"foo": 123, "bar": {"bazQux": 456}}
     response = Response(json_data)
     assert response.json_data == json_data
     assert response.get("foo") == 123
     assert response.bar.get("baz_qux") == response.bar.get("bazQux") == 456
```

### Comparing `civis-2.1.0/tests/test_service_client.py` & `civis-2.2.0/tests/test_service_client.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_utils.py` & `civis-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `civis-2.1.0/tests/test_version.py` & `civis-2.2.0/tests/test_version.py`

 * *Files identical despite different names*

