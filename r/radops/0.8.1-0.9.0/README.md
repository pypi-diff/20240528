# Comparing `tmp/radops-0.8.1.tar.gz` & `tmp/radops-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radops-0.8.1.tar", last modified: Wed Nov  8 23:03:16 2023, max compression
+gzip compressed data, was "radops-0.9.0.tar", last modified: Tue Nov 14 19:28:26 2023, max compression
```

## Comparing `radops-0.8.1.tar` & `radops-0.9.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.963168 radops-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.943168 radops-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.947168 radops-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-08 23:03:02.000000 radops-0.8.1/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-08 23:03:02.000000 radops-0.8.1/.github/workflows/mlflow-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-08 23:03:03.000000 radops-0.8.1/.github/workflows/publish-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-11-08 23:03:03.000000 radops-0.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-08 23:03:03.000000 radops-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-08 23:03:03.000000 radops-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-11-08 23:03:03.000000 radops-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-11-08 23:03:16.963168 radops-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-08 23:03:03.000000 radops-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.947168 radops-0.8.1/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-11-08 23:03:03.000000 radops-0.8.1/demos/iris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.947168 radops-0.8.1/demos/remote_execution/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-08 23:03:03.000000 radops-0.8.1/demos/remote_execution/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-08 23:03:03.000000 radops-0.8.1/demos/remote_execution/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-08 23:03:03.000000 radops-0.8.1/demos/remote_execution/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.951168 radops-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2023-11-08 23:03:03.000000 radops-0.8.1/docs/data_lake.md
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-08 23:03:03.000000 radops-0.8.1/docs/experiment_tracking.md
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-08 23:03:03.000000 radops-0.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-11-08 23:03:03.000000 radops-0.8.1/docs/remote_job_execution.md
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-11-08 23:03:03.000000 radops-0.8.1/docs/serialization.md
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-08 23:03:03.000000 radops-0.8.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.951168 radops-0.8.1/mlflow-auth-docker/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/entry-point.sh
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/mlflow.sh
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/nginx.conf.template
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/supervisord.conf
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-08 23:03:03.000000 radops-0.8.1/mlflow-auth-docker/webserver.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-08 23:03:03.000000 radops-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.951168 radops-0.8.1/radops/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-08 23:03:03.000000 radops-0.8.1/radops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.955168 radops-0.8.1/radops/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-08 23:03:03.000000 radops-0.8.1/radops/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-08 23:03:03.000000 radops-0.8.1/radops/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-11-08 23:03:03.000000 radops-0.8.1/radops/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2023-11-08 23:03:03.000000 radops-0.8.1/radops/cli/data_lake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-11-08 23:03:03.000000 radops-0.8.1/radops/cli/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.955168 radops-0.8.1/radops/data_lake/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-11-08 23:03:03.000000 radops-0.8.1/radops/data_lake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2023-11-08 23:03:03.000000 radops-0.8.1/radops/data_lake/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2023-11-08 23:03:03.000000 radops-0.8.1/radops/data_lake/_file_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2023-11-08 23:03:03.000000 radops-0.8.1/radops/data_lake/cloud_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.955168 radops-0.8.1/radops/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:03.000000 radops-0.8.1/radops/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2023-11-08 23:03:03.000000 radops-0.8.1/radops/jobs/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-11-08 23:03:03.000000 radops-0.8.1/radops/jobs/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-11-08 23:03:03.000000 radops-0.8.1/radops/jobs/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.959168 radops-0.8.1/radops/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-08 23:03:03.000000 radops-0.8.1/radops/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17975 2023-11-08 23:03:03.000000 radops-0.8.1/radops/serialization/_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-11-08 23:03:03.000000 radops-0.8.1/radops/serialization/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2023-11-08 23:03:03.000000 radops-0.8.1/radops/serialization/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-11-08 23:03:03.000000 radops-0.8.1/radops/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.959168 radops-0.8.1/radops/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:03.000000 radops-0.8.1/radops/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-11-08 23:03:03.000000 radops-0.8.1/radops/tracking/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-11-08 23:03:03.000000 radops-0.8.1/radops/tracking/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-08 23:03:03.000000 radops-0.8.1/radops/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.955168 radops-0.8.1/radops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-08 23:03:16.000000 radops-0.8.1/radops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 23:03:16.963168 radops-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.947168 radops-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.959168 radops-0.8.1/tests/functional-tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2023-11-08 23:03:03.000000 radops-0.8.1/tests/functional-tests/test_data_lake.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-08 23:03:03.000000 radops-0.8.1/tests/functional-tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-11-08 23:03:03.000000 radops-0.8.1/tests/functional-tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-11-08 23:03:03.000000 radops-0.8.1/tests/functional-tests/test_mlflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 23:03:16.959168 radops-0.8.1/tests/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-11-08 23:03:03.000000 radops-0.8.1/tests/unit-tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2023-11-08 23:03:03.000000 radops-0.8.1/tests/unit-tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-11-08 23:03:03.000000 radops-0.8.1/tests/unit-tests/test_data_lake.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-11-08 23:03:03.000000 radops-0.8.1/tests/unit-tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-08 23:03:03.000000 radops-0.8.1/tests/unit-tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.011494 radops-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:25.999493 radops-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.003494 radops-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-14 19:28:16.000000 radops-0.9.0/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-14 19:28:16.000000 radops-0.9.0/.github/workflows/mlflow-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-14 19:28:16.000000 radops-0.9.0/.github/workflows/publish-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-11-14 19:28:16.000000 radops-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-14 19:28:16.000000 radops-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-14 19:28:16.000000 radops-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-11-14 19:28:16.000000 radops-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-11-14 19:28:26.011494 radops-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-14 19:28:16.000000 radops-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.003494 radops-0.9.0/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-11-14 19:28:16.000000 radops-0.9.0/demos/iris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.003494 radops-0.9.0/demos/remote_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-14 19:28:16.000000 radops-0.9.0/demos/remote_execution/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-14 19:28:16.000000 radops-0.9.0/demos/remote_execution/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-14 19:28:16.000000 radops-0.9.0/demos/remote_execution/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.003494 radops-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2023-11-14 19:28:16.000000 radops-0.9.0/docs/data_lake.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-14 19:28:16.000000 radops-0.9.0/docs/experiment_tracking.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-14 19:28:16.000000 radops-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-11-14 19:28:16.000000 radops-0.9.0/docs/remote_job_execution.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-11-14 19:28:16.000000 radops-0.9.0/docs/serialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-14 19:28:16.000000 radops-0.9.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/mlflow-auth-docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/entry-point.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/mlflow.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/nginx.conf.template
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/supervisord.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-14 19:28:16.000000 radops-0.9.0/mlflow-auth-docker/webserver.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-14 19:28:16.000000 radops-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/radops/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-14 19:28:16.000000 radops-0.9.0/radops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/radops/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-14 19:28:16.000000 radops-0.9.0/radops/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-14 19:28:16.000000 radops-0.9.0/radops/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-11-14 19:28:16.000000 radops-0.9.0/radops/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-11-14 19:28:16.000000 radops-0.9.0/radops/cli/data_lake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-11-14 19:28:16.000000 radops-0.9.0/radops/cli/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/radops/data_lake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-11-14 19:28:16.000000 radops-0.9.0/radops/data_lake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2023-11-14 19:28:16.000000 radops-0.9.0/radops/data_lake/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2023-11-14 19:28:16.000000 radops-0.9.0/radops/data_lake/_file_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2023-11-14 19:28:16.000000 radops-0.9.0/radops/data_lake/cloud_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/radops/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:16.000000 radops-0.9.0/radops/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2023-11-14 19:28:16.000000 radops-0.9.0/radops/jobs/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-11-14 19:28:16.000000 radops-0.9.0/radops/jobs/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-11-14 19:28:16.000000 radops-0.9.0/radops/jobs/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.011494 radops-0.9.0/radops/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-14 19:28:16.000000 radops-0.9.0/radops/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17975 2023-11-14 19:28:16.000000 radops-0.9.0/radops/serialization/_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-11-14 19:28:16.000000 radops-0.9.0/radops/serialization/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2023-11-14 19:28:16.000000 radops-0.9.0/radops/serialization/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-11-14 19:28:16.000000 radops-0.9.0/radops/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.011494 radops-0.9.0/radops/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:16.000000 radops-0.9.0/radops/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-11-14 19:28:16.000000 radops-0.9.0/radops/tracking/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-11-14 19:28:16.000000 radops-0.9.0/radops/tracking/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-14 19:28:16.000000 radops-0.9.0/radops/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.007494 radops-0.9.0/radops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 19:28:25.000000 radops-0.9.0/radops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 19:28:26.011494 radops-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.003494 radops-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.011494 radops-0.9.0/tests/functional-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2023-11-14 19:28:16.000000 radops-0.9.0/tests/functional-tests/test_data_lake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-14 19:28:16.000000 radops-0.9.0/tests/functional-tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-11-14 19:28:16.000000 radops-0.9.0/tests/functional-tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-11-14 19:28:16.000000 radops-0.9.0/tests/functional-tests/test_mlflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 19:28:26.011494 radops-0.9.0/tests/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2023-11-14 19:28:16.000000 radops-0.9.0/tests/unit-tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2023-11-14 19:28:16.000000 radops-0.9.0/tests/unit-tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-11-14 19:28:16.000000 radops-0.9.0/tests/unit-tests/test_data_lake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2023-11-14 19:28:16.000000 radops-0.9.0/tests/unit-tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-14 19:28:16.000000 radops-0.9.0/tests/unit-tests/test_serialization.py
```

### Comparing `radops-0.8.1/.github/workflows/mlflow-docker.yml` & `radops-0.9.0/.github/workflows/mlflow-docker.yml`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/.github/workflows/tests.yml` & `radops-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/.pre-commit-config.yaml` & `radops-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/Makefile` & `radops-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/PKG-INFO` & `radops-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radops
-Version: 0.8.1
+Version: 0.9.0
 Summary: ops tooling for Striveworks's R&D team
 Project-URL: homepage, https://www.striveworks.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: numpy
 Requires-Dist: pydantic-settings
```

### Comparing `radops-0.8.1/README.md` & `radops-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/demos/iris.py` & `radops-0.9.0/demos/iris.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/docs/data_lake.md` & `radops-0.9.0/docs/data_lake.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/docs/experiment_tracking.md` & `radops-0.9.0/docs/experiment_tracking.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/docs/index.md` & `radops-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/docs/remote_job_execution.md` & `radops-0.9.0/docs/remote_job_execution.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/docs/serialization.md` & `radops-0.9.0/docs/serialization.md`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/mlflow-auth-docker/Dockerfile` & `radops-0.9.0/mlflow-auth-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/mlflow-auth-docker/LICENSE` & `radops-0.9.0/mlflow-auth-docker/LICENSE`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/mlflow-auth-docker/nginx.conf.template` & `radops-0.9.0/mlflow-auth-docker/nginx.conf.template`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/pyproject.toml` & `radops-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/__init__.py` & `radops-0.9.0/radops/__init__.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/cli/__init__.py` & `radops-0.9.0/radops/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/cli/config.py` & `radops-0.9.0/radops/cli/config.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/cli/data_lake.py` & `radops-0.9.0/radops/cli/data_lake.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     add_from_url,
     add_local_file,
     get_local_path,
     get_unsynced_files,
     list_local_files,
 )
 from radops.data_lake.cloud_ops import (
+    create_presigned_url,
     file_exists_in_s3,
     list_files_and_folders,
 )
 
 from .common import _y_n_prompt_loop
 
 app = typer.Typer()
@@ -172,7 +173,25 @@
     if not f.exists_in_cloud():
         rich.print(f"[yellow]File [blue]{uid}[/blue] is not in the datalake.")
         raise typer.Exit()
     elif f.exists_locally():
         rich.print(f"[yellow]File [blue]{uid}[/blue] already exists locally.")
         raise typer.Exit()
     return File(uid).download_from_cloud()
+
+
+@app.command(name="presigned-url")
+def presigned_url(
+    uid: str,
+    expiration: Annotated[
+        int,
+        typer.Argument(
+            help="the expiration time in seconds. defaults to 3600 (1 hour)"
+        ),
+    ] = 60
+    * 60,
+):
+    """create a presigned url for a file. this allows sharing a file with someone
+    who does not have access to the data lake.
+    """
+    url = create_presigned_url(uid, expiration)
+    rich.print(f"Presigned url: {url}, set to expire in {expiration} seconds.")
```

### Comparing `radops-0.8.1/radops/cli/jobs.py` & `radops-0.9.0/radops/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/data_lake/__init__.py` & `radops-0.9.0/radops/data_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/data_lake/_file.py` & `radops-0.9.0/radops/data_lake/_file.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/data_lake/_file_creator.py` & `radops-0.9.0/radops/data_lake/_file_creator.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/data_lake/cloud_ops.py` & `radops-0.9.0/radops/data_lake/cloud_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,7 +178,24 @@
     def _make_relative(paths):
         return [os.path.relpath(p, base_folder) for p in paths]
 
     file_paths = _make_relative(file_paths)
     folders = _make_relative(folders)
 
     return file_paths, folders
+
+
+def create_presigned_url(object_name: str, expiration: int) -> str:
+    """Create a pre-signed url
+
+    Parameters
+    ----------
+    object_name
+        object to generate a pre-signed url for
+    expiration
+        number of seconds until the url expires
+    """
+    return get_s3_client().generate_presigned_url(
+        ClientMethod="get_object",
+        Params={"Bucket": settings.bucket_name, "Key": object_name},
+        ExpiresIn=expiration,
+    )
```

### Comparing `radops-0.8.1/radops/jobs/docker.py` & `radops-0.9.0/radops/jobs/docker.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/jobs/executor.py` & `radops-0.9.0/radops/jobs/executor.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/jobs/gcp.py` & `radops-0.9.0/radops/jobs/gcp.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/serialization/_deserialization.py` & `radops-0.9.0/radops/serialization/_deserialization.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/serialization/_math.py` & `radops-0.9.0/radops/serialization/_math.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/serialization/_serialization.py` & `radops-0.9.0/radops/serialization/_serialization.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/settings.py` & `radops-0.9.0/radops/settings.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/tracking/base.py` & `radops-0.9.0/radops/tracking/base.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/tracking/mlflow.py` & `radops-0.9.0/radops/tracking/mlflow.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops/utils.py` & `radops-0.9.0/radops/utils.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/radops.egg-info/PKG-INFO` & `radops-0.9.0/radops.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radops
-Version: 0.8.1
+Version: 0.9.0
 Summary: ops tooling for Striveworks's R&D team
 Project-URL: homepage, https://www.striveworks.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: numpy
 Requires-Dist: pydantic-settings
```

### Comparing `radops-0.8.1/radops.egg-info/SOURCES.txt` & `radops-0.9.0/radops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/functional-tests/test_data_lake.py` & `radops-0.9.0/tests/functional-tests/test_data_lake.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/functional-tests/test_gcp.py` & `radops-0.9.0/tests/functional-tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/functional-tests/test_jobs.py` & `radops-0.9.0/tests/functional-tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/functional-tests/test_mlflow.py` & `radops-0.9.0/tests/functional-tests/test_mlflow.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/unit-tests/conftest.py` & `radops-0.9.0/tests/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/unit-tests/test_cli.py` & `radops-0.9.0/tests/unit-tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/unit-tests/test_data_lake.py` & `radops-0.9.0/tests/unit-tests/test_data_lake.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/unit-tests/test_jobs.py` & `radops-0.9.0/tests/unit-tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `radops-0.8.1/tests/unit-tests/test_serialization.py` & `radops-0.9.0/tests/unit-tests/test_serialization.py`

 * *Files identical despite different names*

