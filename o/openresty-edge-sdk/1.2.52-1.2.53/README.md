# Comparing `tmp/openresty-edge-sdk-1.2.52.tar.gz` & `tmp/openresty_edge_sdk-1.2.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/root/orinc/edge-sdk/python-client/buildroot/dist/.tmp-6e1uk34w/openresty-edge-sdk-1.2.52.tar", last modified: Mon Mar 11 09:45:30 2024, max compression
+gzip compressed data, was "/root/orinc/edge-sdk/python-client/buildroot/dist/.tmp-kg4hocwj/openresty_edge_sdk-1.2.53.tar", last modified: Tue May 28 03:16:58 2024, max compression
```

## Comparing `openresty-edge-sdk-1.2.52.tar` & `openresty_edge_sdk-1.2.53.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 09:45:30.775070 openresty-edge-sdk-1.2.52/
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1171 2024-03-11 09:45:30.775070 openresty-edge-sdk-1.2.52/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 09:45:30.767070 openresty-edge-sdk-1.2.52/edge2client/
--rw-r--r--   0 root         (0) root         (0)      348 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      834 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/constants.py
--rw-r--r--   0 root         (0) root         (0)   130952 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/edge2client.py
--rw-r--r--   0 root         (0) root         (0)    16200 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/edge_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 09:45:30.767070 openresty-edge-sdk-1.2.52/edge2client/utils/
--rw-r--r--   0 root         (0) root         (0)      596 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/batch_release.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/copy_app.py
--rw-r--r--   0 root         (0) root         (0)     1026 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/create_app.py
--rw-r--r--   0 root         (0) root         (0)     1437 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/create_apps.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/delete_all_apps.py
--rw-r--r--   0 root         (0) root         (0)     1540 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/export_apps.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/get_app_id_by_global_rule.py
--rw-r--r--   0 root         (0) root         (0)     6963 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/global_ini.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/ngx_emer_conf.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/py_client.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/query_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/release_app.py
--rw-r--r--   0 root         (0) root         (0)      685 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/remove_useless_conf.py
--rw-r--r--   0 root         (0) root         (0)     5358 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/sync_eureka.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/update_dns.py
--rw-r--r--   0 root         (0) root         (0)     3214 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/update_proxy_timeout.py
--rw-r--r--   0 root         (0) root         (0)     3321 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/update_src_ip.py
--rw-r--r--   0 root         (0) root         (0)     8027 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/update_upstream_group_weight.py
--rw-r--r--   0 root         (0) root         (0)     3803 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/update_upstream_weight.py
--rw-r--r--   0 root         (0) root         (0)     4802 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils/utils_common.py
--rw-r--r--   0 root         (0) root         (0)     4790 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/utils_common.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/edge2client/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 09:45:30.775070 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-03-11 09:45:30.000000 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1905 2024-03-11 09:45:30.000000 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 09:45:30.000000 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-11 09:45:30.000000 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-11 09:45:30.000000 openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 09:45:30.775070 openresty-edge-sdk-1.2.52/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1302 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 09:45:30.775070 openresty-edge-sdk-1.2.52/tests/
--rw-r--r--   0 root         (0) root         (0)      548 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test.py
--rw-r--r--   0 root         (0) root         (0)     3075 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_app.py
--rw-r--r--   0 root         (0) root         (0)     3589 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_app_basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_app_dymetrics.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_app_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2138 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_approve.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_cache_purge.py
--rw-r--r--   0 root         (0) root         (0)      871 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5600 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_dns.py
--rw-r--r--   0 root         (0) root         (0)     6203 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_dos_logs.py
--rw-r--r--   0 root         (0) root         (0)      692 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1201 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_global_dymetrics.py
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_global_k8s.py
--rw-r--r--   0 root         (0) root         (0)     1804 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_global_k8s_domain.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_global_page_template.py
--rw-r--r--   0 root         (0) root         (0)    26759 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_global_rule.py
--rw-r--r--   0 root         (0) root         (0)     1552 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_ip_list.py
--rw-r--r--   0 root         (0) root         (0)     9521 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_k8s_upstream.py
--rw-r--r--   0 root         (0) root         (0)      299 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_lmdb.py
--rw-r--r--   0 root         (0) root         (0)      946 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_login.py
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_node_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2163 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_partition_lua_module.py
--rw-r--r--   0 root         (0) root         (0)      275 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_referenced.py
--rw-r--r--   0 root         (0) root         (0)    24695 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)     2183 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_rule_reorder.py
--rw-r--r--   0 root         (0) root         (0)     6703 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     3133 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_status.py
--rw-r--r--   0 root         (0) root         (0)     8432 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_upstream_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_variable.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_version.py
--rw-r--r--   0 root         (0) root         (0)     4675 2024-03-11 09:45:20.000000 openresty-edge-sdk-1.2.52/tests/test_waf_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:16:58.111968 openresty_edge_sdk-1.2.53/
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-28 03:16:58.111968 openresty_edge_sdk-1.2.53/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:16:58.103968 openresty_edge_sdk-1.2.53/edge2client/
+-rw-r--r--   0 root         (0) root         (0)      348 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      834 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/constants.py
+-rw-r--r--   0 root         (0) root         (0)   132834 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/edge2client.py
+-rw-r--r--   0 root         (0) root         (0)    16200 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/edge_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:16:58.107967 openresty_edge_sdk-1.2.53/edge2client/utils/
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/batch_release.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/copy_app.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/create_app.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/create_apps.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/delete_all_apps.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/export_apps.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/get_app_id_by_global_rule.py
+-rw-r--r--   0 root         (0) root         (0)     6963 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/global_ini.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/ngx_emer_conf.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/py_client.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/query_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/release_app.py
+-rw-r--r--   0 root         (0) root         (0)      685 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/remove_useless_conf.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/sync_eureka.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/update_dns.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/update_proxy_timeout.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/update_src_ip.py
+-rw-r--r--   0 root         (0) root         (0)     8027 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/update_upstream_group_weight.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/update_upstream_weight.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils/utils_common.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/utils_common.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/edge2client/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:16:58.111968 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-28 03:16:58.000000 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-05-28 03:16:58.000000 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 03:16:58.000000 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-28 03:16:58.000000 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-28 03:16:58.000000 openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 03:16:58.111968 openresty_edge_sdk-1.2.53/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:16:58.111968 openresty_edge_sdk-1.2.53/tests/
+-rw-r--r--   0 root         (0) root         (0)      548 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_app.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_app_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_app_dymetrics.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_app_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_approve.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_cache_purge.py
+-rw-r--r--   0 root         (0) root         (0)      871 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_dns.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_dos_logs.py
+-rw-r--r--   0 root         (0) root         (0)      692 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_global_dymetrics.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_global_k8s.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_global_k8s_domain.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_global_page_template.py
+-rw-r--r--   0 root         (0) root         (0)    26759 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_global_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_ip_list.py
+-rw-r--r--   0 root         (0) root         (0)     9521 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_k8s_upstream.py
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_lmdb.py
+-rw-r--r--   0 root         (0) root         (0)      946 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_login.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_node_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_partition_lua_module.py
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_referenced.py
+-rw-r--r--   0 root         (0) root         (0)    24695 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_rule_reorder.py
+-rw-r--r--   0 root         (0) root         (0)     6703 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_status.py
+-rw-r--r--   0 root         (0) root         (0)     8432 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_upstream_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_variable.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-05-28 03:16:47.000000 openresty_edge_sdk-1.2.53/tests/test_waf_logs.py
```

### Comparing `openresty-edge-sdk-1.2.52/LICENSE` & `openresty_edge_sdk-1.2.53/LICENSE`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/PKG-INFO` & `openresty_edge_sdk-1.2.53/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openresty-edge-sdk
-Version: 1.2.52
+Version: 1.2.53
 Summary: OpenResty Edge Python SDK
 Home-page: https://www.openresty.com
 Author: OpenResty Inc.
 Author-email: support@openresty.com
 Keywords: openresty-edge-sdk,edge2client,python,sdk
 Platform: Platform Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openresty-edge-sdk-1.2.52/edge2client/constants.py` & `openresty_edge_sdk-1.2.53/edge2client/constants.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/edge2client.py` & `openresty_edge_sdk-1.2.53/edge2client/edge2client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,28 @@
 GlobalRewriteRuleUrl = 'global/1/rewrite/rules?detail=1'
 GlobalWafRuleUrl = 'global/1/waf/rule_sets'
 GlobalUpstreamUrl = 'global/1/upstreams/'
 GlobalK8sUpstreamUrl = 'global/1/k8s_upstreams'
 GlobalDymetricsUrl = 'global/1/dymetrics'
 GlobalK8sUrl = 'global/1/k8s'
 GlobalIPListUrl = 'global/1/ip_list'
+ModGlobalIPListUrl = 'ip_list/{}/{}'
 K8sUrl = 'k8s'
 ApplicationUrl = 'applications'
 AppUpstreamUrl = 'applications/http/{}/clusters'
 AppK8sUpstreamUrl = 'applications/http/{}/k8s_upstreams'
 AppRewriteRuleUrl = 'applications/http/{}/phases/rewrite/rules'
 AppRewriteRuleDetailUrl = 'applications/http/{}/phases/rewrite/rules/?detail=1'
 APPRewriteRuleReorder = '_reorder/applications/http/{}/phases/rewrite/rules'
 AppSslCertUrl = 'applications/http/{}/phases/ssl_cert/certs/'
 AppAcmeCertUrl = 'acme_cert/info/'
 AppCachePurgeUrl = 'applications/http/{}/purge?detail=1'
 AppWafWhiteListUrl = 'applications/http/{}/waf_whitelist?detail=1'
 AppIPListUrl = 'applications/http/{}/ip_list'
+ModAppIPListUrl = 'app_ip_list/{}/{}/{}'
 PartitionsUrl = 'partitions/?detail=1'
 GatewayUrl = 'gateway'
 GatewayTagUrl = 'gatewaytag'
 VersionUrl = 'version'
 DymetricsDataUrl = 'log_server/dymetrics/list_data'
 AppMetricsUrl = 'log_server/metrics_http'
 AppDymetricsUrl = 'applications/http/{}/dymetrics'
@@ -2884,14 +2886,36 @@
 
     def del_global_ip_list(self, rule_id=None):
         if not rule_id:
             raise Exception('no active ip list selected')
 
         return self.do_api('DELETE', '{}/{}'.format(GlobalIPListUrl, rule_id))
 
+    def mod_global_ip_list(self, rule_id=None, http_verb='PUT',
+                           items=None, action=None):
+        body = {'items': items}
+
+        url = ModGlobalIPListUrl.format(rule_id, action)
+
+        return self.do_api(http_verb, url, body)
+
+    def append_to_global_ip_list(self, rule_id=None, items=None):
+        if not rule_id:
+            raise Exception('no active ip list selected')
+
+        return self.mod_global_ip_list(rule_id=rule_id, items=items,
+                                       action='append')
+
+    def remove_from_global_ip_list(self, rule_id=None, items=None):
+        if not rule_id:
+            raise Exception('no active ip list selected')
+
+        return self.mod_global_ip_list(rule_id=rule_id, items=items,
+                                       action='remove')
+
     def new_waf_whitelist(self, **kwargs):
         if not self.app_id:
             raise Exception('no active application selected')
 
         kwargs['http_verb'] = 'POST'
         data = self.put_waf_whitelist(**kwargs)
 
@@ -3301,14 +3325,40 @@
 
         if not rule_id:
             raise Exception('no active IP List selected')
 
         return self.do_api('DELETE', AppIPListUrl.format(self.app_id) + '/' +
                            str(rule_id))
 
+    def mod_ip_list(self, app_id=None, rule_id=None, http_verb='PUT',
+                    items=None, action=None):
+        body = {'items': items}
+
+        url = ModAppIPListUrl.format(app_id, action, rule_id)
+
+        return self.do_api(http_verb, url, body)
+
+    def append_to_ip_list(self, rule_id=None, items=None):
+        if not self.app_id:
+            raise Exception('no active application selected')
+        if not rule_id:
+            raise Exception('no active IP List selected');
+
+        return self.mod_ip_list(app_id=self.app_id, rule_id=rule_id,
+                                items=items, action='append')
+
+    def remove_from_ip_list(self, rule_id=None, items=None):
+        if not self.app_id:
+            raise Exception('no active application selected')
+        if not rule_id:
+            raise Exception('no active IP List selected');
+
+        return self.mod_ip_list(app_id=self.app_id, rule_id=rule_id,
+                                items=items, action='remove')
+
     def get_version(self):
         return self.do_api('GET', VersionUrl)
 
     def node_monitor(self, node_id, start_time=None, end_time=None, step=60):
         if not isinstance(node_id, int) or node_id <= 0:
             raise Exception('invalid node id')
```

### Comparing `openresty-edge-sdk-1.2.52/edge2client/edge_common.py` & `openresty_edge_sdk-1.2.53/edge2client/edge_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/batch_release.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/batch_release.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/copy_app.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/copy_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/create_app.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/create_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/create_apps.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/create_apps.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/export_apps.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/export_apps.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/get_app_id_by_global_rule.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/get_app_id_by_global_rule.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/global_ini.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/global_ini.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/ngx_emer_conf.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/ngx_emer_conf.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/py_client.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/py_client.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/query_rule_id.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/query_rule_id.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/release_app.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/release_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/remove_useless_conf.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/remove_useless_conf.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/sync_eureka.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/sync_eureka.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/update_dns.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/update_dns.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/update_proxy_timeout.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/update_proxy_timeout.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/update_src_ip.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/update_src_ip.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/update_upstream_group_weight.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/update_upstream_group_weight.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/update_upstream_weight.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/update_upstream_weight.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils/utils_common.py` & `openresty_edge_sdk-1.2.53/edge2client/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/edge2client/utils_common.py` & `openresty_edge_sdk-1.2.53/edge2client/utils_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/PKG-INFO` & `openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openresty-edge-sdk
-Version: 1.2.52
+Version: 1.2.53
 Summary: OpenResty Edge Python SDK
 Home-page: https://www.openresty.com
 Author: OpenResty Inc.
 Author-email: support@openresty.com
 Keywords: openresty-edge-sdk,edge2client,python,sdk
 Platform: Platform Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openresty-edge-sdk-1.2.52/openresty_edge_sdk.egg-info/SOURCES.txt` & `openresty_edge_sdk-1.2.53/openresty_edge_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/setup.py` & `openresty_edge_sdk-1.2.53/setup.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test.py` & `openresty_edge_sdk-1.2.53/tests/test.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_app.py` & `openresty_edge_sdk-1.2.53/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_app_basic_auth.py` & `openresty_edge_sdk-1.2.53/tests/test_app_basic_auth.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_app_dymetrics.py` & `openresty_edge_sdk-1.2.53/tests/test_app_dymetrics.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_approve.py` & `openresty_edge_sdk-1.2.53/tests/test_approve.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_cache_purge.py` & `openresty_edge_sdk-1.2.53/tests/test_cache_purge.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_cluster.py` & `openresty_edge_sdk-1.2.53/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_dns.py` & `openresty_edge_sdk-1.2.53/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_dos_logs.py` & `openresty_edge_sdk-1.2.53/tests/test_dos_logs.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_gateway.py` & `openresty_edge_sdk-1.2.53/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_global_dymetrics.py` & `openresty_edge_sdk-1.2.53/tests/test_global_dymetrics.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_global_k8s.py` & `openresty_edge_sdk-1.2.53/tests/test_global_k8s.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_global_k8s_domain.py` & `openresty_edge_sdk-1.2.53/tests/test_global_k8s_domain.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_global_page_template.py` & `openresty_edge_sdk-1.2.53/tests/test_global_page_template.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_global_rule.py` & `openresty_edge_sdk-1.2.53/tests/test_global_rule.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_ip_list.py` & `openresty_edge_sdk-1.2.53/tests/test_ip_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,26 @@
         self.assertEqual(ip_list_1.get('name'), 'ip_list_1')
 
         # modify
         self.client.put_ip_list(rule_id=rule_id, items=[{'ip': '192.168.1.1'}])
         ip_list_1 = self.client.get_ip_list(rule_id)
         self.assertEqual(ip_list_1.get('items')[0].get('ip'), '192.168.1.1')
 
+        # append
+        self.client.append_to_ip_list(rule_id=rule_id, items=[{'ip': '192.168.1.2'}])
+        ip_list_2 = self.client.get_ip_list(rule_id)
+        self.assertEqual(ip_list_2.get('items')[0].get('ip'), '192.168.1.1')
+        self.assertEqual(ip_list_2.get('items')[1].get('ip'), '192.168.1.2')
+
+        # remove
+        self.client.remove_from_ip_list(rule_id=rule_id, items=[{'ip': '192.168.1.2'}])
+        ip_list_3 = self.client.get_ip_list(rule_id)
+        self.assertEqual(ip_list_3.get('items')[0].get('ip'), '192.168.1.1')
+        self.assertEqual(1, len(ip_list_3.get('items', [])))
+
         # delete
         ok = self.client.del_ip_list(rule_id=rule_id)
         self.assertTrue(ok)
 
     def test_global_ip_list(self):
         # create
         global_rule_id = self.client.new_global_ip_list(name='g_ip_list_1',
@@ -34,10 +46,23 @@
 
         # modify
         self.client.put_global_ip_list(rule_id=global_rule_id,
                                        items=[{'ip': '192.168.1.2'}])
         g_ip_list_1 = self.client.get_global_ip_list(global_rule_id)
         self.assertEqual(g_ip_list_1.get('items')[0].get('ip'), '192.168.1.2')
 
+        # append
+        self.client.append_to_global_ip_list(rule_id=global_rule_id, items=[{'ip': '192.168.1.3'}])
+        g_ip_list_2 = self.client.get_global_ip_list(global_rule_id)
+        self.assertEqual(g_ip_list_2.get('items')[0].get('ip'), '192.168.1.2')
+        self.assertEqual(g_ip_list_2.get('items')[1].get('ip'), '192.168.1.3')
+
+        # remove
+        self.client.remove_from_global_ip_list(rule_id=global_rule_id,
+                                        items=[{'ip': '192.168.1.2'}])
+        g_ip_list_3 = self.client.get_global_ip_list(global_rule_id)
+        self.assertEqual(g_ip_list_3.get('items')[0].get('ip'), '192.168.1.3')
+        self.assertEqual(1, len(g_ip_list_3.get('items', [])))
+
         # delete
         ok = self.client.del_global_ip_list(rule_id=global_rule_id)
         self.assertTrue(ok)
```

### Comparing `openresty-edge-sdk-1.2.52/tests/test_k8s_upstream.py` & `openresty_edge_sdk-1.2.53/tests/test_k8s_upstream.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_login.py` & `openresty_edge_sdk-1.2.53/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_node_monitor.py` & `openresty_edge_sdk-1.2.53/tests/test_node_monitor.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_nodes.py` & `openresty_edge_sdk-1.2.53/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_partition_lua_module.py` & `openresty_edge_sdk-1.2.53/tests/test_partition_lua_module.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_rule.py` & `openresty_edge_sdk-1.2.53/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_rule_reorder.py` & `openresty_edge_sdk-1.2.53/tests/test_rule_reorder.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_search.py` & `openresty_edge_sdk-1.2.53/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_status.py` & `openresty_edge_sdk-1.2.53/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_upstream_proxy.py` & `openresty_edge_sdk-1.2.53/tests/test_upstream_proxy.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_variable.py` & `openresty_edge_sdk-1.2.53/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.52/tests/test_waf_logs.py` & `openresty_edge_sdk-1.2.53/tests/test_waf_logs.py`

 * *Files identical despite different names*

