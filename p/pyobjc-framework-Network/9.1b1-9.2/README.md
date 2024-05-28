# Comparing `tmp/pyobjc-framework-Network-9.1b1.tar.gz` & `tmp/pyobjc-framework-Network-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Network-9.1b1.tar", last modified: Sun Mar 26 11:31:42 2023, max compression
+gzip compressed data, was "pyobjc-framework-Network-9.2.tar", last modified: Wed Jun  7 00:21:58 2023, max compression
```

## Comparing `pyobjc-framework-Network-9.1b1.tar` & `pyobjc-framework-Network-9.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:42.037629 pyobjc-framework-Network-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.896242 pyobjc-framework-Network-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.905914 pyobjc-framework-Network-9.1b1/Lib/Network/
--rw-r--r--   0 ronald     (501) staff       (20)      830 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/Lib/Network/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    62844 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.1b1/Lib/Network/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.912011 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-03-26 11:31:41.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1845 2023-03-26 11:31:41.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:31:41.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:39.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:31:41.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:31:41.000000 pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Network-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.914645 pyobjc-framework-Network-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     2753 2021-10-18 19:38:40.000000 pyobjc-framework-Network-9.1b1/Modules/_Network.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Network-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2023-03-26 11:31:42.037273 pyobjc-framework-Network-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.963105 pyobjc-framework-Network-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2605 2022-06-25 10:29:20.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_advertise_descriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1783 2023-03-03 17:21:59.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_browse_descriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1261 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_browse_result.py
--rw-r--r--   0 ronald     (501) staff       (20)     1297 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_browser.py
--rw-r--r--   0 ronald     (501) staff       (20)     4087 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection.py
--rw-r--r--   0 ronald     (501) staff       (20)     2918 2021-08-01 10:31:49.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection_group.py
--rw-r--r--   0 ronald     (501) staff       (20)     4552 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection_report.py
--rw-r--r--   0 ronald     (501) staff       (20)     1164 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_content_context.py
--rw-r--r--   0 ronald     (501) staff       (20)     2678 2022-06-23 11:03:28.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_endpoint.py
--rw-r--r--   0 ronald     (501) staff       (20)      727 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_error.py
--rw-r--r--   0 ronald     (501) staff       (20)     1713 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_ethernet_channel.py
--rw-r--r--   0 ronald     (501) staff       (20)     4843 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_framer_options.py
--rw-r--r--   0 ronald     (501) staff       (20)      907 2021-08-14 10:34:11.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_group_descriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1853 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_interface.py
--rw-r--r--   0 ronald     (501) staff       (20)     1629 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_ip_options.py
--rw-r--r--   0 ronald     (501) staff       (20)     1953 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_listener.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_network.py
--rw-r--r--   0 ronald     (501) staff       (20)      236 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_nw_object.py
--rw-r--r--   0 ronald     (501) staff       (20)     5644 2022-06-23 11:03:28.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_parameters.py
--rw-r--r--   0 ronald     (501) staff       (20)     1735 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_path.py
--rw-r--r--   0 ronald     (501) staff       (20)     1074 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_path_monitor.py
--rw-r--r--   0 ronald     (501) staff       (20)      711 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_privacy_context.py
--rw-r--r--   0 ronald     (501) staff       (20)      343 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_protocol_options.py
--rw-r--r--   0 ronald     (501) staff       (20)     3097 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_quic_options.py
--rw-r--r--   0 ronald     (501) staff       (20)      380 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_resolver_config.py
--rw-r--r--   0 ronald     (501) staff       (20)     1557 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_tcp_options.py
--rw-r--r--   0 ronald     (501) staff       (20)      445 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_tls_options.py
--rw-r--r--   0 ronald     (501) staff       (20)     2222 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_txt_record.py
--rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_udp_options.py
--rw-r--r--   0 ronald     (501) staff       (20)     4225 2021-04-09 10:15:21.000000 pyobjc-framework-Network-9.1b1/PyObjCTest/test_ws_options.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:41.975024 pyobjc-framework-Network-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    36528 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.1b1/metadata/Network.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:42.035576 pyobjc-framework-Network-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    96705 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97644 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   109368 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   109406 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    40930 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    74276 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    84426 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    96706 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    97645 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   109369 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   109407 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Network-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:31:42.037728 pyobjc-framework-Network-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      935 2023-03-25 14:20:32.000000 pyobjc-framework-Network-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.168209 pyobjc-framework-Network-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.074206 pyobjc-framework-Network-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.079665 pyobjc-framework-Network-9.2/Lib/Network/
+-rw-r--r--   0 ronald     (501) staff       (20)      830 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/Lib/Network/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    62916 2023-05-27 09:46:33.000000 pyobjc-framework-Network-9.2/Lib/Network/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.094778 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-06-07 00:21:58.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1860 2023-06-07 00:21:58.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:58.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:39.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:21:58.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:21:58.000000 pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Network-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.097223 pyobjc-framework-Network-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     2753 2021-10-18 19:38:40.000000 pyobjc-framework-Network-9.2/Modules/_Network.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Network-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:21:58.167562 pyobjc-framework-Network-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.130972 pyobjc-framework-Network-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2605 2022-06-25 10:29:20.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_advertise_descriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1783 2023-03-03 17:21:59.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_browse_descriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1261 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_browse_result.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1297 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_browser.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4087 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_connection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2918 2021-08-01 10:31:49.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_connection_group.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4552 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_connection_report.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1164 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_content_context.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2678 2022-06-23 11:03:28.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_endpoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      727 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_error.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1713 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_ethernet_channel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4843 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_framer_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)      907 2021-08-14 10:34:11.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_group_descriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1853 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_interface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1629 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_ip_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1953 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_listener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_network.py
+-rw-r--r--   0 ronald     (501) staff       (20)      236 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_nw_object.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5644 2022-06-23 11:03:28.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_parameters.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1735 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_path.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1074 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_path_monitor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      711 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_privacy_context.py
+-rw-r--r--   0 ronald     (501) staff       (20)      343 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_protocol_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3097 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_quic_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)      380 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_resolver_config.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1557 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_tcp_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)      445 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_tls_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2222 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_txt_record.py
+-rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_udp_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4225 2021-04-09 10:15:21.000000 pyobjc-framework-Network-9.2/PyObjCTest/test_ws_options.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.132832 pyobjc-framework-Network-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    36578 2023-05-27 09:46:33.000000 pyobjc-framework-Network-9.2/metadata/Network.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:58.166327 pyobjc-framework-Network-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    96705 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97644 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   109368 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   109406 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    40930 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    74276 2020-11-30 18:45:15.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    84426 2021-03-21 10:08:23.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    96706 2021-07-30 09:00:38.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    97645 2022-02-24 08:47:16.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   109369 2022-07-08 16:02:54.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   109407 2023-02-19 10:50:35.000000 pyobjc-framework-Network-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Network-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Network-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:58.168314 pyobjc-framework-Network-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1016 2023-05-29 10:07:46.000000 pyobjc-framework-Network-9.2/setup.py
```

### Comparing `pyobjc-framework-Network-9.1b1/Lib/Network/__init__.py` & `pyobjc-framework-Network-9.2/Lib/Network/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/Lib/Network/_metadata.py` & `pyobjc-framework-Network-9.2/Lib/Network/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Feb 18 13:11:33 2023
+# Last update: Sat May 20 12:16:56 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -1598,20 +1598,21 @@
     "nw_parameters_set_prohibit_expensive": (b"v@B",),
     "nw_parameters_set_fast_open_enabled": (b"v@B",),
     "nw_ethernet_channel_send": (
         b"v@@S^C@?",
         "",
         {
             "arguments": {
+                3: {"c_array_of_fixed_size": 6, "type_modifier": "n"},
                 4: {
                     "callable": {
                         "retval": {"type": b"v"},
                         "arguments": {0: {"type": "^v"}, 1: {"type": "@"}},
                     }
-                }
+                },
             }
         },
     ),
     "nw_data_transfer_report_get_transport_smoothed_rtt_milliseconds": (b"Q@I",),
     "nw_ws_metadata_get_close_code": (b"I@",),
     "nw_tcp_options_set_keepalive_interval": (b"v@I",),
     "nw_path_get_status": (b"I@",),
```

### Comparing `pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/PKG-INFO` & `pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Network
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Network on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Network
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-Network-9.1b1/Lib/pyobjc_framework_Network.egg-info/SOURCES.txt` & `pyobjc-framework-Network-9.2/Lib/pyobjc_framework_Network.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Network/__init__.py
 Lib/Network/_metadata.py
 Lib/pyobjc_framework_Network.egg-info/PKG-INFO
 Lib/pyobjc_framework_Network.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Network.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Network.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Network-9.1b1/License.txt` & `pyobjc-framework-Network-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/Modules/_Network.m` & `pyobjc-framework-Network-9.2/Modules/_Network.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Network-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Network-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-Network-9.1b1/PKG-INFO` & `pyobjc-framework-Network-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Network
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Network on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Network
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_advertise_descriptor.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_advertise_descriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_browse_descriptor.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_browse_descriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_browse_result.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_browse_result.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_browser.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_browser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_connection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection_group.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_connection_group.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_connection_report.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_connection_report.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_content_context.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_content_context.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_endpoint.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_error.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_error.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_ethernet_channel.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_ethernet_channel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_framer_options.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_framer_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_group_descriptor.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_group_descriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_interface.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_interface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_ip_options.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_ip_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_listener.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_listener.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_parameters.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_path.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_path.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_path_monitor.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_path_monitor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_privacy_context.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_privacy_context.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_quic_options.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_quic_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_tcp_options.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_tcp_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_txt_record.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_txt_record.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/PyObjCTest/test_ws_options.py` & `pyobjc-framework-Network-9.2/PyObjCTest/test_ws_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/Network.fwinfo` & `pyobjc-framework-Network-9.2/metadata/Network.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -801,15 +801,15 @@
    "nw_ethernet_channel_create": {
     "retval": {
      "already_retained": true
     }
    },
    "nw_ethernet_channel_send": {
     "args": {
-     "3": {},
+     "3": { "type_modifier": "n", "c_array_of_fixed_size": 6 },
      "4": {
       "callable": {
        "arguments": {
         "0": { "type": "^v" },
         "1": { "type": "@" }
        },
        "retval": { "type": "v" }
```

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-Network-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Network-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Network-9.1b1/setup.py` & `pyobjc-framework-Network-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-from pyobjc_setup import Extension, setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-Network",
     description="Wrappers for the framework Network on macOS",
     min_os_level="10.14",
     packages=["Network"],
     ext_modules=[
```

