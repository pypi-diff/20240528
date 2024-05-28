# Comparing `tmp/sdc_dp_helpers-1.4.0.tar.gz` & `tmp/sdc_dp_helpers-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_dp_helpers-1.4.0.tar", last modified: Fri May 17 09:41:09 2024, max compression
+gzip compressed data, was "sdc_dp_helpers-1.4.1.tar", last modified: Tue May 28 08:05:48 2024, max compression
```

## Comparing `sdc_dp_helpers-1.4.0.tar` & `sdc_dp_helpers-1.4.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.389600 sdc_dp_helpers-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-17 09:41:09.389600 sdc_dp_helpers-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.369601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.373601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/__init_.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/data_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20801 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/date_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/file_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/retry_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/tracking_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.373601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.373601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.373601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/falcon_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.373601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.377601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/generate_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.377601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.377601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.377601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.377601 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.381600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.381600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.381600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.381600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/onesignal_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.381600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.385600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/config_magagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.385600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.385600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.385600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/xero_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.385600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.389600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/records_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/users_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.389600 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-17 09:41:04.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:09.369601 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-17 09:41:08.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-17 09:41:09.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:41:08.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 09:41:08.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 09:41:08.000000 sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 09:41:09.389600 sdc_dp_helpers-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-17 09:41:06.000000 sdc_dp_helpers-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/__init_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/data_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/date_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/file_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/retry_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/tracking_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/falcon_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/generate_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/onesignal_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/config_magagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/xero_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/records_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/users_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-28 08:05:46.000000 sdc_dp_helpers-1.4.1/setup.py
```

### Comparing `sdc_dp_helpers-1.4.0/README.md` & `sdc_dp_helpers-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/data_managers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/data_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/date_managers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/date_managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """UTILITIES TO HANDLE DATE VALUES"""
 
-# pylint: disable=too-few-public-methods
+# pylint: disable=too-few-public-methods, line-too-long, too-many-arguments, import-error
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 import re
 from typing import Tuple, Generator, Union
 from dateutil.relativedelta import relativedelta
 import pandas as pd
 from sdc_dp_helpers.api_utilities.exceptions import (
@@ -381,22 +381,24 @@
 
 def date_range_iterator(
     start_date: str,
     end_date: str,
     interval: str,
     end_inclusive: bool = False,
     time_format: str = "%Y-%m-%d",
+    ytd: bool = False,
 ) -> Generator[Tuple[str, str], None, None]:
     """Processes the Date and Returns the date value to work with
     Args:
         start_date (str): date string (2022-11-14 or the allowed date string values)
         end_date (str): date string (2022-11-14 or the allowed date string values)
         interval (str): string 1_month, 1_day, yearly, monthly, weekly
         end_inclusive (bool): whether the yielded end for period/interval is inclusive or not.
         time_format (str, optional): The format of the returned date value. Defaults to "%Y-%m-%d".
+        ytd (bool, optional): (Year To Date) If true returns dates in ranges of time beginning the first day of the current calendar year upto the current date
     Yields:
         Generator[Tuple[str, str], None, None]: start and end (exclusive) for each time interval.
     """
     phrase_handler = IntervalDatePhraseHandler(date_value=interval)
     cadence, time_bucket = phrase_handler.phrase_to_date()
     handler = DateHandlerFactory().get_date_handler(
         time_bucket=time_bucket, cadence=cadence
@@ -408,17 +410,22 @@
     while startdate <= enddate:
         end = next_end
         if end_inclusive:
             end = next_end - timedelta(days=1)
             if time_bucket == "hour":
                 end = next_end - timedelta(hours=1)
             # end = next_end - timedelta(days=1)
-        yield datetime.strftime(startdate, time_format), datetime.strftime(
-            end, time_format
-        )
+        if ytd:
+            yield datetime.strftime(
+                startdate.replace(month=1, day=1), time_format
+            ), datetime.strftime(end, time_format)
+        else:
+            yield datetime.strftime(startdate, time_format), datetime.strftime(
+                end, time_format
+            )
         startdate = next_end
         next_end = handler.add_interval(date_value=startdate, cadence=cadence)
 
 
 def date_string_change_format(
     date_string: str, output_format="%Y-%m-%d", input_format="%Y-%m-%d"
 ) -> str:
```

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/exceptions.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/file_managers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/file_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/retry_managers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/retry_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/api_utilities/tracking_metadata.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/tracking_metadata.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/azure/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_writer.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writer.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/base_writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/facebook/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/falcon_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/falcon_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/falcon/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/ftp/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/generate_refresh_token.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/generate_refresh_token.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_ads/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/config_managers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/config_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/utils.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_analytics_v4/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_big_query/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_knowledge_graph_v1/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_postmaster_tools/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/google_search_console/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/onesignal_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/onesignal_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/onesignal/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/utils.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/pyspark/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/utils.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/sailthru/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/sftp/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/webvitalize/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,13 +67,13 @@
                 "Invalid date format for partitioning expected: 'YYYY-mm-dd'"
             )
         _data: list = payload["data"]
         _date: str = payload["date"].replace("-", "")
         _endpoint: str = payload["endpoint"]
         _trackingCategoryId = payload["trackingCategoryId"]
         _tenant_name = payload["tenant_name"]
-        _filter_by = payload["filterby"]
+        _filter_by = payload.get("filterby")
         if _trackingCategoryId:
             write_path = f"{self.folder_path}/{_endpoint}/{_tenant_name}/{_filter_by}/{_trackingCategoryId}/{_date}"
         else:
             write_path = f"{self.folder_path}/{_endpoint}/{_tenant_name}/{_date}"
         return write_path, _data
```

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/xero/xero_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/xero_sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# pylint: disable=too-few-public-methods, unused-import ,attribute-defined-outside-init,broad-exception-raise,trailing-whitespace,line-too-long,no-member,broad-exception-raised,bare-except,too-many-arguments,arguments-differ,wildcard-import,broad-exception-caught,unused-wildcard-import
+"""
+    XERO API SDK
+"""
+# pylint: disable=too-few-public-methods, unused-import ,attribute-defined-outside-init,trailing-whitespace,line-too-long,no-member,broad-exception-raised,bare-except,too-many-arguments,arguments-differ,wildcard-import,broad-exception-caught,unused-wildcard-import,no-else-return,missing-function-docstring,unspecified-encoding
 import os
 import json
 import ast
 from abc import abstractmethod
 import requests
 from oauth2 import *
 from xero.auth import OAuth2Credentials
@@ -21,14 +24,17 @@
     """
 
     def __init__(self, config, creds_filepath):
         self.creds_path: str = creds_filepath
         self.config: dict = config
 
     def token_isvalid(self, creds: OAuth2Credentials) -> bool:
+        """
+        Token validity
+        """
         if not isinstance(creds, OAuth2Credentials):
             raise TypeError("creds is not an object of type OAuth2Credentials")
 
         return creds.get_tenants()[0]["tenantId"] is not None
 
     def get_auth_token(self) -> OAuth2Credentials:
         """
@@ -99,76 +105,70 @@
 class XeroAPICall:
     "Class for making xero API call"
 
     def __init__(self, creds_path, config):
         self.creds_filepath = creds_path
         self.config = config
 
-    def get_reports(self, report_name):
-        results = []
+    def get_reports(
+        self,
+        report_name: str,
+        start_date: str,
+        end_date: str,
+        tracking_category: str,
+        filterby: str,
+    ):
+        """Get reports data"""
         get_data_methods = {
-            "filtered": ReportsByTrackingOption,
+            "bytrackingoption": ReportsByTrackingOption,
             "notfiltered": ReportsNotFiltered,
         }
-        for filterby in self.config["reports"][report_name]["filter"]:
-            method_ids_caller = get_data_methods[filterby](
-                config=self.config, creds_filepath=self.creds_filepath
-            )
-            data = method_ids_caller.make_api_call(
-                report_name, self.config["reports"][report_name]["params"], filterby
-            )
-            results.append(data)
-        return results
+        method_ids_caller = get_data_methods[filterby](
+            config=self.config, creds_filepath=self.creds_filepath
+        )
+        data = method_ids_caller.make_api_call(
+            report_name, start_date,end_date, tracking_category
+        )
+        return data
 
-    def get_modules(self, module):
+    def get_modules(self, module, start_date, end_date):
+        """Get modules data"""
         module_ = Modules(config=self.config, creds_filepath=self.creds_filepath)
-        results = module_.make_api_call(module)
+        results = module_.make_api_call(module, start_date, end_date)
+        return results
+
+    def get_tracking_categories(self):
+        """Get tracking categories data"""
+        categories = GetTrackingCategories(
+            config=self.config, creds_filepath=self.creds_filepath
+        )
+        results = categories.make_api_call()
         return results
 
 
 class ReportsNotFiltered(RequestHandler):
     "Class for not Filtered reports"
-    def make_api_call(self, report_name, request_params, filterby):
-        data_set = {}
+
+    def make_api_call(self, report_name, start_date, end_date, tracking_category):
+        request_params = {}
         auth_token = self.authenticator.get_auth_token()
-        trackingcategories = GetTrackingCategories(
-            config=self.config, creds_filepath=self.creds_path
-        ).make_api_call()
-        params = {}
         option_id = None
-        for tracking_category in trackingcategories:
-            file_name = (
-                report_name
-                + "_"
-                + filterby
-                + "_"
-                + tracking_category["TrackingCategoryID"]
-            )
-            params.update(
-                {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
-            )
-            report = get_report(
-                auth_token,
-                params,
-                option_id,
-                self.config["tenant_id"],
-                report_name,
-                request_params,
-            )
-            result = {
-                "endpoint": report_name,
-                "tenant_name": self.config["tenant_name"],
-                "trackingCategoryId": tracking_category["TrackingCategoryID"],
-                "data": [report],
-                "date": request_params.get("date", request_params.get("end_date")),
-                "filterby": filterby,
-            }
-            if result and result is not None:
-                data_set.update({file_name: result})
-        return data_set
+        request_params.update(
+            {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
+        )
+        report = get_report(
+            self.config,
+            auth_token,
+            start_date,
+            end_date,
+            option_id,
+            report_name,
+            request_params,
+        )
+        return [report]
 
 
 class GetTrackingCategories(RequestHandler):
     "class to get Reports filtered by Tracking categories"
 
     def make_api_call(self):
         auth_token = self.authenticator.get_auth_token()
@@ -179,56 +179,34 @@
         )
         return trackingcategories
 
 
 class ReportsByTrackingOption(RequestHandler):
     "class to get Reports filtered by TrackingOptionID"
 
-    def make_api_call(self, report_name, request_params, filterby):
-        data_set = {}
-        trackingcategories = GetTrackingCategories(
-            config=self.config, creds_filepath=self.creds_path
-        ).make_api_call()
+    def make_api_call(self, report_name, start_date, end_date, tracking_category):
+        request_params = {}
         auth_token = self.authenticator.get_auth_token()
-        params = {}
-
-        for tracking_category in trackingcategories:
-            option_data = []
-            for option_id in tracking_category["Options"]:
-                file_name = (
-                    report_name
-                    + "_"
-                    + filterby
-                    + "_"
-                    + tracking_category["TrackingCategoryID"]
-                )
-                params.update(
-                    {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
-                )
-                params.update({"TrackingOptionID": option_id["TrackingOptionID"]})
-                report = get_report(
-                    auth_token,
-                    params,
-                    option_id,
-                    self.config["tenant_id"],
-                    report_name,
-                    request_params,
-                )
-                option_data.append(report)
-            result = {
-                "endpoint": report_name,
-                "tenant_name": self.config["tenant_name"],
-                "trackingCategoryId": tracking_category["TrackingCategoryID"],
-                "data": option_data,
-                "date": request_params.get("date", request_params.get("end_date")),
-                "filterby": filterby,
-            }
-            if option_data and option_data is not None:
-                data_set.update({file_name: result})
-        return data_set
+        option_data = []
+        for option_id in tracking_category["Options"]:
+            request_params.update(
+                {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
+            )
+            request_params.update({"TrackingOptionID": option_id["TrackingOptionID"]})
+            report = get_report(
+                self.config,
+                auth_token,
+                start_date,
+                end_date,
+                option_id,
+                report_name,
+                request_params,
+            )
+            option_data.append(report)
+        return option_data
 
 
 class Modules(RequestHandler):
     "class to get Modules"
 
     @request_handler(
         wait=int(os.environ.get("REQUEST_WAIT_TIME", 0.1)),
@@ -238,107 +216,112 @@
     def run_request(self, xero_client, api_object, request):
         """
         Run the API request that consumes a request payload and site url.
         This separates the request with the request handler from the rest of the logic.
         """
         # To Do Handle API Errors
         api_call = getattr(xero_client, api_object)
+        if api_object in ["currencies", "trackingcategories"]:
+            return api_call.filter(page=request["page"])
         # XeroRateLimitExceeded
-        return api_call.filter(
-            raw=date_filter_helper(request["from_date"], request["to_date"]),
-            page=request["page"],
-        )
+        else:
+            return api_call.filter(
+                raw=date_filter_helper(request["from_date"], request["to_date"]),
+                page=request["page"],
+            )
 
-    def make_api_call(self, module):
+    def make_api_call(self, module, start_date, end_date):
+        """
+        API call to get module data
+        """
         auth_token = self.authenticator.get_auth_token()
         auth_token.tenant_id = self.config.get("tenant_id")
         xero = Xero(auth_token)
-        data_set = {}
-        if module not in [
-            "accounts",
-        ]:
+        data = []
+        if module not in ["accounts", "trackingcategories", "currencies"]:
             raise ValueError(module + " is not supported or does not exist.")
-        data_set[module] = []
         prev_response = None
         page = 1
         while True:
             response = self.run_request(
                 xero_client=xero,
                 api_object=module,
                 request={
-                    "from_date": self.config.get("start_date"),
-                    "to_date": self.config.get("end_date"),
+                    "from_date": start_date,
+                    "to_date": end_date,
                     "page": page,
                 },
             )
-            print(response)
             if len(response) < 1:
                 print("Request returned empty payload. breaking...")
                 break
             if response == prev_response:
                 print("Request returned copy of last payload. breaking...")
-            data_set[module] += [
+                break
+            data = [
                 json.loads(
                     json.dumps(response_obj, indent=4, sort_keys=True, default=str)
                 )
                 for response_obj in response
             ]
-            # ensure the token is still fresh
             auth_token = self.authenticator.get_auth_token()
             prev_response = response
             page += 1
-        return data_set
+        return data
 
 
 ############### helper functions
 
 
-
-@retry_handler(exceptions=XeroQuotaException, total_tries=5, initial_wait=5)
-def get_report(auth_token, params, option_id, tenant_id, report_name, request_params):
+@retry_handler(exceptions=XeroQuotaException, total_tries=5, initial_wait=1)
+def get_report(configs,
+    auth_token, start_date, end_date, option_id, report_name, request_params
+):
+    """Get single report data"""
     if report_name in ["ProfitAndLoss"]:
-        params = {
-            "fromDate": request_params["start_date"],
-            "toDate": request_params["end_date"],
-        }
+        request_params.update({"fromDate": start_date})
+        request_params.update({"toDate": end_date})
+
     if report_name in ["BalanceSheet"]:
-        params.update({"date": request_params.get("date")})
-        params.update({"timeframe": request_params.get("timeframe")})
-        params.update({"periods": request_params.get("periods")})
+        request_params.update({"date": end_date})
+        request_params.update({"timeframe": configs.get("timeframe")})
+        request_params.update({"periods": configs.get("periods")})
     headers = {
         "Authorization": "Bearer " + auth_token.token["access_token"],
-        "Xero-Tenant-Id": tenant_id,
+        "Xero-Tenant-Id": configs['tenant_id'],
         "Accept": "application/json",
     }
     try:
         response = requests.get(
             "https://api.xero.com/api.xro/2.0/Reports/" + report_name,
-            params=params,
+            params=request_params,
             headers=headers,
             timeout=30,
         )
         report = json.loads(
             response.text.replace("\r", "").replace("\n", "").strip("'<>() ")
         )
-        report = format_values(report, tenant_id, option_id=option_id)
+        report = normalize(report, configs['tenant_id'], option_id=option_id)
     except Exception as err:
         if err.code == 429:
             raise XeroQuotaException(
                 f"Xero Quota Reached" f"Status code: {err.code}, Reason: {err.reason}. "
             ) from err
     return report
 
 
-def format_values(report, tenant_id, option_id=None):
+def normalize(report, tenant_id, option_id=None):
     for row in range(len(report["Reports"][0]["Rows"])):
         period = report["Reports"][0]["Rows"][0]["Cells"]
         try:
             for report_ in report["Reports"][0]["Rows"][row]["Rows"]:
                 for idx, cells in enumerate(report_["Cells"]):
-                    cells["Attributes"][0].update({"type": report_["Cells"][0]["Value"]})
+                    cells["Attributes"][0].update(
+                        {"type": report_["Cells"][0]["Value"]}
+                    )
                     cells["Attributes"][0].update({"period": period[idx]["Value"]})
         except:
             pass
     if option_id:
         report["TrackingOptionID"] = option_id["TrackingOptionID"]
         report["TrackingOptionName"] = option_id["Name"]
     report["tenantId"] = tenant_id
```

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/xml/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/bulk_endpoint.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/bulk_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/records_endpoint.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/records_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/users_endpoint.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/users_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/readers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/writers.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/sdc_dp_helpers.egg-info/SOURCES.txt` & `sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.0/setup.py` & `sdc_dp_helpers-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,19 +71,19 @@
         "paramiko",
         "google-cloud-enterpriseknowledgegraph>=0.3.3",
     ],
     extras_require={"pyspark": ["pyspark"]},
     cmdclass={"sdist_zip": sdistzip},
     description="A module for developing data pipelines from external api's and on ETL like services",
 
-    version="1.4.0",
+    version="1.4.1",
 
     url="http://github.com/RingierIMU/sdc-dataPipeline-helpers",
     author="Ringier South Africa",
     author_email="tools@ringier.co.za",
     keywords=[
         "pip",
         "datapipeline",
         "helpers",
     ],
-    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.4.0.zip",
+    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.4.1.zip",
 )
```

