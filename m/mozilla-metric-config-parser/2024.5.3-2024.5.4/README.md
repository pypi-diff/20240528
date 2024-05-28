# Comparing `tmp/mozilla_metric_config_parser-2024.5.3.tar.gz` & `tmp/mozilla_metric_config_parser-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_metric_config_parser-2024.5.3.tar", last modified: Fri May 24 22:33:09 2024, max compression
+gzip compressed data, was "mozilla_metric_config_parser-2024.5.4.tar", last modified: Tue May 28 20:45:47 2024, max compression
```

## Comparing `mozilla_metric_config_parser-2024.5.3.tar` & `mozilla_metric_config_parser-2024.5.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/
--rw-r--r--   0 root         (0) root         (0)    16725 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1590 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.710303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7185 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    28357 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)    10973 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)    10032 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    16178 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3374 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     5529 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.710303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_macros.j2
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     7147 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    26303 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    25837 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    13765 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2866 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    12162 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     4528 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:33:09.714303 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1590 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 22:33:09.000000 mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 22:33:09.718303 mozilla_metric_config_parser-2024.5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1574 2024-05-24 22:33:00.000000 mozilla_metric_config_parser-2024.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.613955 mozilla_metric_config_parser-2024.5.4/
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-28 20:45:47.613955 mozilla_metric_config_parser-2024.5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.609955 mozilla_metric_config_parser-2024.5.4/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7185 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    28357 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     5529 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.609955 mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/data_source_macros.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.609955 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.609955 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     7147 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    26303 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    13765 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 20:45:47.613955 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 20:45:47.000000 mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-28 20:45:47.613955 mozilla_metric_config_parser-2024.5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-05-28 20:45:39.000000 mozilla_metric_config_parser-2024.5.4/setup.py
```

### Comparing `mozilla_metric_config_parser-2024.5.3/LICENSE` & `mozilla_metric_config_parser-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/PKG-INFO` & `mozilla_metric_config_parser-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/alert.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/analysis.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/cli.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/config.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/config.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/data_source.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/definition.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/dimension.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/errors.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/experiment.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/exposure_signal.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/function.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/metric_group.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/monitoring.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/outcome.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/parameter.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/population.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/project.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/segment.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/sql.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/data_source_macros.j2` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/data_source_macros.j2`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,18 @@
             FROM
                 {{ data_source.from_expression }}
             {% if where -%}
             WHERE
                 {{ where }}
             {% endif -%}
         ) AS {{ data_source.name }}
-        {% if data_source.joins and data_source.client_id_column != 'NULL' -%}
+        {% if data_source.joins -%}
             {% for joined_data_source_slug, joined_data_source in data_source.joins.items() -%}
-                {{ join(data_source, joined_data_source_slug, joined_data_source) }}
+                {% if data_source.client_id_column != 'NULL' or joined_data_source.get('on_expression') -%}
+                    {{ join(data_source, joined_data_source_slug, joined_data_source) }}
+                {% endif -%}
             {% endfor -%}
         {% endif -%}
 {% if select_fields -%}
 )
 {% endif -%}
 {%- endmacro -%}
```

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/templates/metrics_query.sql` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/conftest.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_alert.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_analysis.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_config.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_experiment.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_function.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_metric.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_monitoring.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_outcomes.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_population.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_project.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/tests/test_sql.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/metric_config_parser/util.py` & `mozilla_metric_config_parser-2024.5.4/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla_metric_config_parser-2024.5.3/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla_metric_config_parser-2024.5.4/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla_metric_config_parser-2024.5.3/setup.py` & `mozilla_metric_config_parser-2024.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2024.5.3",
+    version="2024.5.4",
 )
```

