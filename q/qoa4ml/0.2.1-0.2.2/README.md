# Comparing `tmp/qoa4ml-0.2.1.tar.gz` & `tmp/qoa4ml-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.2.1.tar", last modified: Mon May 27 14:41:33 2024, max compression
+gzip compressed data, was "qoa4ml-0.2.2.tar", last modified: Tue May 28 06:26:02 2024, max compression
```

## Comparing `qoa4ml-0.2.1.tar` & `qoa4ml-0.2.2.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.572306 qoa4ml-0.2.1/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      641 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.2.1/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.2.1/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-27 14:41:33.571965 qoa4ml-0.2.1/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10605 2024-05-27 07:40:24.000000 qoa4ml-0.2.1/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2024-05-27 14:39:15.000000 qoa4ml-0.2.1/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       35 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/dev_requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      165 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/ml_requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      176 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.553587 qoa4ml-0.2.1/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      281 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.557201 qoa4ml-0.2.1/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.2.1/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2616 2024-05-27 08:06:35.000000 qoa4ml-0.2.1/qoa4ml/collector/amqp_collector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      129 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/collector/base_collector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      153 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/collector/host_object.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1126 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/collector/socket_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.557646 qoa4ml-0.2.1/qoa4ml/config/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2872 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/config/configs.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.560210 qoa4ml-0.2.1/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.2.1/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2590 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      143 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/connector/base_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1410 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2396 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2499 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1040 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/connector/socket_connector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.561521 qoa4ml-0.2.1/qoa4ml/lang/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      655 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/qoa4ml/lang/common_models.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     3535 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/lang/datamodel_enum.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2242 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/lang/ml_contract.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4161 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/metric.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4046 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/metric_mananger.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.561940 qoa4ml-0.2.1/qoa4ml/observability/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/observability/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.563612 qoa4ml-0.2.1/qoa4ml/observability/odop_obs/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/observability/odop_obs/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      673 2024-05-21 11:39:02.000000 qoa4ml-0.2.1/qoa4ml/observability/odop_obs/embedded_database.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1138 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/observability/odop_obs/exporter.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     8440 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/observability/odop_obs/node_aggregator.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.566427 qoa4ml-0.2.1/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.2.1/qoa4ml/probes/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7859 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6060 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2248 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/probes/probe.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     3717 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/probes/process_monitoring_probe.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     3801 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/probes/system_monitoring_probe.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    14377 2024-05-27 11:28:12.000000 qoa4ml-0.2.1/qoa4ml/qoa_client.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.568896 qoa4ml-0.2.1/qoa4ml/reports/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/qoa4ml/reports/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      780 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/qoa4ml/reports/abstract_report.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      770 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/qoa4ml/reports/general_application_report.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1851 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/qoa4ml/reports/ml_report_model.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      610 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/reports/resources_report_model.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10220 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/qoa4ml/reports/rohe_reports.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.570959 qoa4ml-0.2.1/qoa4ml/utils/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1528 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/utils/gpu_utils.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    55920 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/utils/pynvml_forked.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    17074 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/utils/qoa_utils.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      805 2024-05-27 07:29:49.000000 qoa4ml-0.2.1/qoa4ml/utils/repeated_timer.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.555227 qoa4ml-0.2.1/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-27 14:41:33.000000 qoa4ml-0.2.1/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1645 2024-05-27 14:41:33.000000 qoa4ml-0.2.1/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2024-05-27 14:41:33.000000 qoa4ml-0.2.1/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      483 2024-05-27 14:41:33.000000 qoa4ml-0.2.1/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2024-05-27 14:41:33.000000 qoa4ml-0.2.1/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      291 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2024-05-27 14:41:33.572386 qoa4ml-0.2.1/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      788 2024-05-21 06:42:14.000000 qoa4ml-0.2.1/setup.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.548071 qoa4ml-0.2.1/tests/
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 14:41:33.571319 qoa4ml-0.2.1/tests/test_reportv1/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     5484 2024-05-27 11:09:59.000000 qoa4ml-0.2.1/tests/test_reportv1/test.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.741523 qoa4ml-0.2.2/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      641 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.2.2/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.2.2/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-28 06:26:02.741185 qoa4ml-0.2.2/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    10605 2024-05-27 07:40:24.000000 qoa4ml-0.2.2/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2024-05-28 06:25:58.000000 qoa4ml-0.2.2/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       35 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/dev_requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      165 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/ml_requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      176 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.722086 qoa4ml-0.2.2/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      281 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.725696 qoa4ml-0.2.2/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.2.2/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2616 2024-05-27 08:06:35.000000 qoa4ml-0.2.2/qoa4ml/collector/amqp_collector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      129 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/collector/base_collector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      153 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/collector/host_object.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1126 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/collector/socket_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.726489 qoa4ml-0.2.2/qoa4ml/config/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:24:22.000000 qoa4ml-0.2.2/qoa4ml/config/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2872 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/config/configs.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.729739 qoa4ml-0.2.2/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.2.2/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2590 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      143 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/connector/base_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1410 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2396 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2499 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1040 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/connector/socket_connector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.731440 qoa4ml-0.2.2/qoa4ml/lang/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:24:19.000000 qoa4ml-0.2.2/qoa4ml/lang/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      655 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/qoa4ml/lang/common_models.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3535 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/lang/datamodel_enum.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2242 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/lang/ml_contract.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4161 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/metric.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4046 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/metric_mananger.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.731907 qoa4ml-0.2.2/qoa4ml/observability/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/observability/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.733687 qoa4ml-0.2.2/qoa4ml/observability/odop_obs/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/observability/odop_obs/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      673 2024-05-21 11:39:02.000000 qoa4ml-0.2.2/qoa4ml/observability/odop_obs/embedded_database.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1138 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/observability/odop_obs/exporter.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     8440 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/observability/odop_obs/node_aggregator.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.736251 qoa4ml-0.2.2/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.2.2/qoa4ml/probes/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7859 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6060 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2248 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/probes/probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3717 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/probes/process_monitoring_probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3801 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/probes/system_monitoring_probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    14377 2024-05-27 11:28:12.000000 qoa4ml-0.2.2/qoa4ml/qoa_client.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.738594 qoa4ml-0.2.2/qoa4ml/reports/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/qoa4ml/reports/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      780 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/qoa4ml/reports/abstract_report.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      770 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/qoa4ml/reports/general_application_report.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1851 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/qoa4ml/reports/ml_report_model.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      610 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/reports/resources_report_model.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    10220 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/qoa4ml/reports/rohe_reports.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.740511 qoa4ml-0.2.2/qoa4ml/utils/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:24:26.000000 qoa4ml-0.2.2/qoa4ml/utils/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1528 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/utils/gpu_utils.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    55920 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/utils/pynvml_forked.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    17074 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/utils/qoa_utils.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      805 2024-05-27 07:29:49.000000 qoa4ml-0.2.2/qoa4ml/utils/repeated_timer.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.723927 qoa4ml-0.2.2/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-28 06:26:02.000000 qoa4ml-0.2.2/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1720 2024-05-28 06:26:02.000000 qoa4ml-0.2.2/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2024-05-28 06:26:02.000000 qoa4ml-0.2.2/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      483 2024-05-28 06:26:02.000000 qoa4ml-0.2.2/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2024-05-28 06:26:02.000000 qoa4ml-0.2.2/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      291 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2024-05-28 06:26:02.741607 qoa4ml-0.2.2/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      788 2024-05-21 06:42:14.000000 qoa4ml-0.2.2/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.717838 qoa4ml-0.2.2/tests/
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-28 06:26:02.740780 qoa4ml-0.2.2/tests/test_reportv1/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     5484 2024-05-27 11:09:59.000000 qoa4ml-0.2.2/tests/test_reportv1/test.py
```

### Comparing `qoa4ml-0.2.1/CHANGELOG.txt` & `qoa4ml-0.2.2/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/LICENCE.txt` & `qoa4ml-0.2.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/PKG-INFO` & `qoa4ml-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: dev
```

### Comparing `qoa4ml-0.2.1/README.md` & `qoa4ml-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.2.2/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/collector/socket_collector.py` & `qoa4ml-0.2.2/qoa4ml/collector/socket_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/config/configs.py` & `qoa4ml-0.2.2/qoa4ml/config/configs.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.2.2/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.2.2/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.2.2/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.2.2/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/connector/socket_connector.py` & `qoa4ml-0.2.2/qoa4ml/connector/socket_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/lang/common_models.py` & `qoa4ml-0.2.2/qoa4ml/lang/common_models.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/lang/datamodel_enum.py` & `qoa4ml-0.2.2/qoa4ml/lang/datamodel_enum.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/lang/ml_contract.py` & `qoa4ml-0.2.2/qoa4ml/lang/ml_contract.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/metric.py` & `qoa4ml-0.2.2/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/metric_mananger.py` & `qoa4ml-0.2.2/qoa4ml/metric_mananger.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/observability/odop_obs/embedded_database.py` & `qoa4ml-0.2.2/qoa4ml/observability/odop_obs/embedded_database.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/observability/odop_obs/exporter.py` & `qoa4ml-0.2.2/qoa4ml/observability/odop_obs/exporter.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/observability/odop_obs/node_aggregator.py` & `qoa4ml-0.2.2/qoa4ml/observability/odop_obs/node_aggregator.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/probes/dataquality.py` & `qoa4ml-0.2.2/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/probes/mlquality.py` & `qoa4ml-0.2.2/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/probes/probe.py` & `qoa4ml-0.2.2/qoa4ml/probes/probe.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/probes/process_monitoring_probe.py` & `qoa4ml-0.2.2/qoa4ml/probes/process_monitoring_probe.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/probes/system_monitoring_probe.py` & `qoa4ml-0.2.2/qoa4ml/probes/system_monitoring_probe.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/qoa_client.py` & `qoa4ml-0.2.2/qoa4ml/qoa_client.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/reports/abstract_report.py` & `qoa4ml-0.2.2/qoa4ml/reports/abstract_report.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/reports/general_application_report.py` & `qoa4ml-0.2.2/qoa4ml/reports/general_application_report.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/reports/ml_report_model.py` & `qoa4ml-0.2.2/qoa4ml/reports/ml_report_model.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/reports/resources_report_model.py` & `qoa4ml-0.2.2/qoa4ml/reports/resources_report_model.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/reports/rohe_reports.py` & `qoa4ml-0.2.2/qoa4ml/reports/rohe_reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/utils/gpu_utils.py` & `qoa4ml-0.2.2/qoa4ml/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/utils/pynvml_forked.py` & `qoa4ml-0.2.2/qoa4ml/utils/pynvml_forked.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/utils/qoa_utils.py` & `qoa4ml-0.2.2/qoa4ml/utils/qoa_utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml/utils/repeated_timer.py` & `qoa4ml-0.2.2/qoa4ml/utils/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.2.2/qoa4ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: dev
```

### Comparing `qoa4ml-0.2.1/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.2.2/qoa4ml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 qoa4ml.egg-info/requires.txt
 qoa4ml.egg-info/top_level.txt
 qoa4ml/collector/__init__.py
 qoa4ml/collector/amqp_collector.py
 qoa4ml/collector/base_collector.py
 qoa4ml/collector/host_object.py
 qoa4ml/collector/socket_collector.py
+qoa4ml/config/__init__.py
 qoa4ml/config/configs.py
 qoa4ml/connector/__init__.py
 qoa4ml/connector/amqp_connector.py
 qoa4ml/connector/base_connector.py
 qoa4ml/connector/mess_logging.py
 qoa4ml/connector/mqtt_connector.py
 qoa4ml/connector/prom_connector.py
 qoa4ml/connector/socket_connector.py
+qoa4ml/lang/__init__.py
 qoa4ml/lang/common_models.py
 qoa4ml/lang/datamodel_enum.py
 qoa4ml/lang/ml_contract.py
 qoa4ml/observability/__init__.py
 qoa4ml/observability/odop_obs/__init__.py
 qoa4ml/observability/odop_obs/embedded_database.py
 qoa4ml/observability/odop_obs/exporter.py
@@ -46,12 +48,13 @@
 qoa4ml/probes/system_monitoring_probe.py
 qoa4ml/reports/__init__.py
 qoa4ml/reports/abstract_report.py
 qoa4ml/reports/general_application_report.py
 qoa4ml/reports/ml_report_model.py
 qoa4ml/reports/resources_report_model.py
 qoa4ml/reports/rohe_reports.py
+qoa4ml/utils/__init__.py
 qoa4ml/utils/gpu_utils.py
 qoa4ml/utils/pynvml_forked.py
 qoa4ml/utils/qoa_utils.py
 qoa4ml/utils/repeated_timer.py
 tests/test_reportv1/test.py
```

### Comparing `qoa4ml-0.2.1/setup.py` & `qoa4ml-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.2.1/tests/test_reportv1/test.py` & `qoa4ml-0.2.2/tests/test_reportv1/test.py`

 * *Files identical despite different names*

