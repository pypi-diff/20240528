# Comparing `tmp/opensearch-py-2.5.0.tar.gz` & `tmp/opensearch_py-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-py-2.5.0.tar", last modified: Mon Mar 25 16:41:28 2024, max compression
+gzip compressed data, was "opensearch_py-2.6.0.tar", last modified: Tue May 28 16:58:33 2024, max compression
```

## Comparing `opensearch-py-2.5.0.tar` & `opensearch_py-2.6.0.tar`

### file list

```diff
@@ -1,123 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.595121 opensearch-py-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-25 16:41:28.595121 opensearch-py-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.591121 opensearch-py-2.5.0/opensearch_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 16:41:28.000000 opensearch-py-2.5.0/opensearch_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.575121 opensearch-py-2.5.0/opensearchpy/
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.575121 opensearch-py-2.5.0/opensearchpy/_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/_extra_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.579121 opensearch-py-2.5.0/opensearchpy/_async/client/
--rw-r--r--   0 runner    (1001) docker     (127)    88280 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    36619 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/dangling_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    69794 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/remote_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.583121 opensearch-py-2.5.0/opensearchpy/_async/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/faceted_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    17498 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/helpers/update_by_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/http_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.583121 opensearch-py-2.5.0/opensearchpy/_async/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/plugins/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/plugins/index_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/plugins/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18839 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.587121 opensearch-py-2.5.0/opensearchpy/client/
--rw-r--r--   0 runner    (1001) docker     (127)    87713 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    36331 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22926 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/dangling_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    69218 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/remote_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26125 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.587121 opensearch-py-2.5.0/opensearchpy/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/async_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/http_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/http_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.591121 opensearch-py-2.5.0/opensearchpy/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/aggs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/asyncsigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    19449 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/faceted_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    24664 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.591121 opensearch-py-2.5.0/opensearchpy/helpers/response/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/response/aggs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/response/hit.py
--rw-r--r--   0 runner    (1001) docker     (127)    27319 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/signer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/update_by_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    20342 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/helpers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:41:28.591121 opensearch-py-2.5.0/opensearchpy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/plugins/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/plugins/index_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/plugins/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/opensearchpy/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-25 16:41:28.595121 opensearch-py-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-03-25 16:30:01.000000 opensearch-py-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.121106 opensearch_py-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-28 16:58:33.121106 opensearch_py-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.117106 opensearch_py-2.6.0/opensearch_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-28 16:58:33.000000 opensearch_py-2.6.0/opensearch_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-28 16:58:33.000000 opensearch_py-2.6.0/opensearch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:58:33.000000 opensearch_py-2.6.0/opensearch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:58:32.000000 opensearch_py-2.6.0/opensearch_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 16:58:33.000000 opensearch_py-2.6.0/opensearch_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 16:58:33.000000 opensearch_py-2.6.0/opensearch_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.097105 opensearch_py-2.6.0/opensearchpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.101105 opensearch_py-2.6.0/opensearchpy/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/_extra_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.105105 opensearch_py-2.6.0/opensearchpy/_async/client/
+-rw-r--r--   0 runner    (1001) docker     (127)   128817 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52655 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40409 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/dangling_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114334 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/remote_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/search_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84139 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.105105 opensearch_py-2.6.0/opensearchpy/_async/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/faceted_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17498 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/helpers/update_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/http_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.109105 opensearch_py-2.6.0/opensearchpy/_async/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/index_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15502 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/rollups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18592 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.109105 opensearch_py-2.6.0/opensearchpy/client/
+-rw-r--r--   0 runner    (1001) docker     (127)   128250 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52367 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40157 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/dangling_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113758 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/remote_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/search_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83239 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22211 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.113106 opensearch_py-2.6.0/opensearchpy/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/async_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/http_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/http_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/http_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.117106 opensearch_py-2.6.0/opensearchpy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/aggs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/asyncsigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19449 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/faceted_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24664 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.117106 opensearch_py-2.6.0/opensearchpy/helpers/response/
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/response/aggs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/response/hit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27319 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/update_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20342 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/helpers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.117106 opensearch_py-2.6.0/opensearchpy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/metrics/metrics_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/metrics/metrics_none.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:58:33.117106 opensearch_py-2.6.0/opensearchpy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/index_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15430 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/rollups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20620 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/opensearchpy/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 16:58:33.121106 opensearch_py-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-28 16:20:40.000000 opensearch_py-2.6.0/setup.py
```

### Comparing `opensearch-py-2.5.0/CONTRIBUTING.md` & `opensearch_py-2.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/LICENSE.txt` & `opensearch_py-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/PKG-INFO` & `opensearch_py-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-py
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
@@ -12,54 +12,57 @@
 Project-URL: Source Code, https://github.com/opensearch-project/opensearch-py
 Project-URL: Issue Tracker, https://github.com/opensearch-project/opensearch-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS
-Requires-Dist: urllib3<2,>=1.26.18
+Requires-Dist: urllib3<1.27,>=1.26.18; python_version < "3.10"
+Requires-Dist: urllib3!=2.2.0,<3,>=1.26.18; python_version >= "3.10"
 Requires-Dist: requests<3.0.0,>=2.4.0
 Requires-Dist: six
 Requires-Dist: python-dateutil
 Requires-Dist: certifi>=2022.12.07
+Requires-Dist: Events
 Provides-Extra: develop
 Requires-Dist: requests<3.0.0,>=2.0.0; extra == "develop"
 Requires-Dist: coverage<8.0.0; extra == "develop"
 Requires-Dist: mock; extra == "develop"
 Requires-Dist: pyyaml; extra == "develop"
 Requires-Dist: pytest>=3.0.0; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytz; extra == "develop"
 Requires-Dist: botocore; extra == "develop"
 Requires-Dist: pytest-mock<4.0.0; extra == "develop"
 Requires-Dist: sphinx; extra == "develop"
 Requires-Dist: sphinx_rtd_theme; extra == "develop"
 Requires-Dist: myst_parser; extra == "develop"
 Requires-Dist: sphinx_copybutton; extra == "develop"
-Requires-Dist: black; extra == "develop"
+Requires-Dist: black>=24.3.0; extra == "develop"
 Requires-Dist: jinja2; extra == "develop"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
-Requires-Dist: aiohttp<4,>=3; extra == "docs"
+Requires-Dist: aiohttp<4,>=3.9.4; extra == "docs"
 Provides-Extra: async
-Requires-Dist: aiohttp<4,>=3; extra == "async"
+Requires-Dist: aiohttp<4,>=3.9.4; extra == "async"
 Provides-Extra: kerberos
 Requires-Dist: requests_kerberos; extra == "kerberos"
 
 [![Release](https://github.com/opensearch-project/opensearch-py/actions/workflows/unified-release.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/unified-release.yml)
 [![CI](https://github.com/opensearch-project/opensearch-py/actions/workflows/ci.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/ci.yml)
 [![Integration](https://github.com/opensearch-project/opensearch-py/actions/workflows/integration.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/integration.yml)
 [![Chat](https://img.shields.io/badge/chat-on%20forums-blue)](https://discuss.opendistrocommunity.dev/c/clients/)
```

### Comparing `opensearch-py-2.5.0/README.md` & `opensearch_py-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearch_py.egg-info/PKG-INFO` & `opensearch_py-2.6.0/opensearch_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-py
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
@@ -12,54 +12,57 @@
 Project-URL: Source Code, https://github.com/opensearch-project/opensearch-py
 Project-URL: Issue Tracker, https://github.com/opensearch-project/opensearch-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS
-Requires-Dist: urllib3<2,>=1.26.18
+Requires-Dist: urllib3<1.27,>=1.26.18; python_version < "3.10"
+Requires-Dist: urllib3!=2.2.0,<3,>=1.26.18; python_version >= "3.10"
 Requires-Dist: requests<3.0.0,>=2.4.0
 Requires-Dist: six
 Requires-Dist: python-dateutil
 Requires-Dist: certifi>=2022.12.07
+Requires-Dist: Events
 Provides-Extra: develop
 Requires-Dist: requests<3.0.0,>=2.0.0; extra == "develop"
 Requires-Dist: coverage<8.0.0; extra == "develop"
 Requires-Dist: mock; extra == "develop"
 Requires-Dist: pyyaml; extra == "develop"
 Requires-Dist: pytest>=3.0.0; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytz; extra == "develop"
 Requires-Dist: botocore; extra == "develop"
 Requires-Dist: pytest-mock<4.0.0; extra == "develop"
 Requires-Dist: sphinx; extra == "develop"
 Requires-Dist: sphinx_rtd_theme; extra == "develop"
 Requires-Dist: myst_parser; extra == "develop"
 Requires-Dist: sphinx_copybutton; extra == "develop"
-Requires-Dist: black; extra == "develop"
+Requires-Dist: black>=24.3.0; extra == "develop"
 Requires-Dist: jinja2; extra == "develop"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
-Requires-Dist: aiohttp<4,>=3; extra == "docs"
+Requires-Dist: aiohttp<4,>=3.9.4; extra == "docs"
 Provides-Extra: async
-Requires-Dist: aiohttp<4,>=3; extra == "async"
+Requires-Dist: aiohttp<4,>=3.9.4; extra == "async"
 Provides-Extra: kerberos
 Requires-Dist: requests_kerberos; extra == "kerberos"
 
 [![Release](https://github.com/opensearch-project/opensearch-py/actions/workflows/unified-release.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/unified-release.yml)
 [![CI](https://github.com/opensearch-project/opensearch-py/actions/workflows/ci.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/ci.yml)
 [![Integration](https://github.com/opensearch-project/opensearch-py/actions/workflows/integration.yml/badge.svg)](https://github.com/opensearch-project/opensearch-py/actions/workflows/integration.yml)
 [![Chat](https://img.shields.io/badge/chat-on%20forums-blue)](https://discuss.opendistrocommunity.dev/c/clients/)
```

### Comparing `opensearch-py-2.5.0/opensearch_py.egg-info/SOURCES.txt` & `opensearch_py-2.6.0/opensearch_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 opensearchpy/_async/client/http.py
 opensearchpy/_async/client/indices.py
 opensearchpy/_async/client/ingest.py
 opensearchpy/_async/client/nodes.py
 opensearchpy/_async/client/plugins.py
 opensearchpy/_async/client/remote.py
 opensearchpy/_async/client/remote_store.py
+opensearchpy/_async/client/search_pipeline.py
 opensearchpy/_async/client/security.py
 opensearchpy/_async/client/snapshot.py
 opensearchpy/_async/client/tasks.py
 opensearchpy/_async/client/utils.py
 opensearchpy/_async/helpers/__init__.py
 opensearchpy/_async/helpers/actions.py
 opensearchpy/_async/helpers/document.py
@@ -52,28 +53,32 @@
 opensearchpy/_async/helpers/search.py
 opensearchpy/_async/helpers/test.py
 opensearchpy/_async/helpers/update_by_query.py
 opensearchpy/_async/plugins/__init__.py
 opensearchpy/_async/plugins/alerting.py
 opensearchpy/_async/plugins/index_management.py
 opensearchpy/_async/plugins/knn.py
+opensearchpy/_async/plugins/notifications.py
+opensearchpy/_async/plugins/rollups.py
+opensearchpy/_async/plugins/transforms.py
 opensearchpy/client/__init__.py
 opensearchpy/client/_patch.py
 opensearchpy/client/cat.py
 opensearchpy/client/client.py
 opensearchpy/client/cluster.py
 opensearchpy/client/dangling_indices.py
 opensearchpy/client/features.py
 opensearchpy/client/http.py
 opensearchpy/client/indices.py
 opensearchpy/client/ingest.py
 opensearchpy/client/nodes.py
 opensearchpy/client/plugins.py
 opensearchpy/client/remote.py
 opensearchpy/client/remote_store.py
+opensearchpy/client/search_pipeline.py
 opensearchpy/client/security.py
 opensearchpy/client/snapshot.py
 opensearchpy/client/tasks.py
 opensearchpy/client/utils.py
 opensearchpy/connection/__init__.py
 opensearchpy/connection/async_connections.py
 opensearchpy/connection/base.py
@@ -100,11 +105,18 @@
 opensearchpy/helpers/test.py
 opensearchpy/helpers/update_by_query.py
 opensearchpy/helpers/utils.py
 opensearchpy/helpers/wrappers.py
 opensearchpy/helpers/response/__init__.py
 opensearchpy/helpers/response/aggs.py
 opensearchpy/helpers/response/hit.py
+opensearchpy/metrics/__init__.py
+opensearchpy/metrics/metrics.py
+opensearchpy/metrics/metrics_events.py
+opensearchpy/metrics/metrics_none.py
 opensearchpy/plugins/__init__.py
 opensearchpy/plugins/alerting.py
 opensearchpy/plugins/index_management.py
-opensearchpy/plugins/knn.py
+opensearchpy/plugins/knn.py
+opensearchpy/plugins/notifications.py
+opensearchpy/plugins/rollups.py
+opensearchpy/plugins/transforms.py
```

### Comparing `opensearch-py-2.5.0/opensearchpy/__init__.py` & `opensearch_py-2.6.0/opensearchpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 from .helpers.index import Index, IndexTemplate
 from .helpers.mapping import Mapping
 from .helpers.query import Q
 from .helpers.search import MultiSearch, Search
 from .helpers.update_by_query import UpdateByQuery
 from .helpers.utils import AttrDict, AttrList, DslBase
 from .helpers.wrappers import Range
+from .metrics import Metrics, MetricsEvents, MetricsNone
 from .serializer import JSONSerializer
 from .transport import Transport
 
 # Only raise one warning per deprecation message so as not
 # to spam up the user if the same action is done multiple times.
 warnings.simplefilter("default", category=OpenSearchDeprecationWarning, append=True)
 
@@ -236,14 +237,17 @@
     "char_filter",
     "connections",
     "construct_field",
     "normalizer",
     "token_filter",
     "tokenizer",
     "__versionstr__",
+    "Metrics",
+    "MetricsEvents",
+    "MetricsNone",
 ]
 
 try:
     from ._async.client import AsyncOpenSearch
     from ._async.http_aiohttp import AIOHttpConnection, AsyncConnection
     from ._async.transport import AsyncTransport
     from .connection import AsyncHttpConnection
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/__init__.py` & `opensearch_py-2.6.0/opensearchpy/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/_extra_imports.py` & `opensearch_py-2.6.0/opensearchpy/_async/_extra_imports.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/__init__.py` & `opensearch_py-2.6.0/opensearchpy/client/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,36 +35,37 @@
 
 
 from __future__ import unicode_literals
 
 import logging
 from typing import Any, Type
 
-from ..transport import AsyncTransport, TransportError
+from ..transport import Transport, TransportError
 from .cat import CatClient
 from .client import Client
 from .cluster import ClusterClient
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .http import HttpClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .plugins import PluginsClient
 from .remote import RemoteClient
 from .remote_store import RemoteStoreClient
+from .search_pipeline import SearchPipelineClient
 from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 from .utils import SKIP_IN_PATH, _bulk_body, _make_path, query_params
 
 logger = logging.getLogger("opensearch")
 
 
-class AsyncOpenSearch(Client):
+class OpenSearch(Client):
     """
     OpenSearch client. Provides a straightforward mapping from
     Python to OpenSearch REST endpoints.
 
     The instance has attributes ``cat``, ``cluster``, ``indices``, ``ingest``,
     ``nodes``, ``snapshot`` and ``tasks`` that provide access to instances of
     :class:`~opensearchpy.client.CatClient`,
@@ -191,15 +192,15 @@
         delete_point_in_time,
         list_all_point_in_time,
     )
 
     def __init__(
         self,
         hosts: Any = None,
-        transport_class: Type[AsyncTransport] = AsyncTransport,
+        transport_class: Type[Transport] = Transport,
         **kwargs: Any
     ) -> None:
         """
         :arg hosts: list of nodes, or a single node, we should connect to.
             Node should be a dictionary ({"host": "localhost", "port": 9200}),
             the entire dictionary will be passed to the :class:`~opensearchpy.Connection`
             class as kwargs, or a string in the format of ``host[:port]`` which will be
@@ -211,14 +212,15 @@
         :arg kwargs: any additional arguments will be passed on to the
             :class:`~opensearchpy.Transport` class and, subsequently, to the
             :class:`~opensearchpy.Connection` instances.
         """
         super().__init__(hosts, transport_class, **kwargs)
 
         # namespaced clients for compatibility with API names
+        self.search_pipeline = SearchPipelineClient(self)
         self.cat = CatClient(self)
         self.cluster = ClusterClient(self)
         self.dangling_indices = DanglingIndicesClient(self)
         self.indices = IndicesClient(self)
         self.ingest = IngestClient(self)
         self.nodes = NodesClient(self)
         self.remote = RemoteClient(self)
@@ -237,1353 +239,1874 @@
             cons: Any = self.transport.hosts
             # truncate to 5 if there are too many
             if len(cons) > 5:
                 cons = cons[:5] + ["..."]
             return "<{cls}({cons})>".format(cls=self.__class__.__name__, cons=cons)
         except Exception:
             # probably operating on custom transport and connection_pool, ignore
-            return super(AsyncOpenSearch, self).__repr__()
+            return super(OpenSearch, self).__repr__()
 
-    async def __aenter__(self) -> Any:
+    def __enter__(self) -> Any:
         if hasattr(self.transport, "_async_call"):
-            await self.transport._async_call()
+            self.transport._async_call()
         return self
 
-    async def __aexit__(self, *_: Any) -> None:
-        await self.close()
+    def __exit__(self, *_: Any) -> None:
+        self.close()
 
-    async def close(self) -> None:
+    def close(self) -> None:
         """Closes the Transport and all internal connections"""
-        await self.transport.close()
+        self.transport.close()
 
     # AUTO-GENERATED-API-DEFINITIONS #
-    @query_params()
-    async def ping(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def ping(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns whether the cluster is running.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         try:
-            return await self.transport.perform_request(
+            return self.transport.perform_request(
                 "HEAD", "/", params=params, headers=headers
             )
         except TransportError:
             return False
 
-    @query_params()
-    async def info(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def info(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns basic information about the cluster.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", "/", params=params, headers=headers
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "pipeline",
+        "pretty",
         "refresh",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    async def create(
+    def create(
         self,
         index: Any,
         id: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates a new document in the index.  Returns a 409 response when a document
         with a same ID already exists in the index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the data stream or index to target. If the
+            target doesn’t exist and matches the name or wildcard (`*`) pattern of
+            an index template with a `data_stream` definition, this request creates
+            the data stream. If the target doesn’t exist and doesn’t match a data
+            stream template, this request creates the index.
+        :arg id: Unique identifier for the document.
         :arg body: The document
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period the request waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_create", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "PUT", path, params=params, headers=headers, body=body
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
         "op_type",
         "pipeline",
+        "pretty",
         "refresh",
         "require_alias",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    async def index(
+    def index(
         self,
         index: Any,
         body: Any,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates or updates a document in an index.
 
 
-        :arg index: Index name.
+        :arg index: Name of the data stream or index to target.
         :arg body: The document
-        :arg id: Document ID.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
-        :arg op_type: Explicit operation type. Defaults to `index` for
-            requests with an explicit document ID, and to `create` for requests
-            without an explicit document ID. Valid choices are index, create.
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: When true, requires destination to be an
+        :arg id: Unique identifier for the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
+        :arg op_type: Set to create to only index the document if it
+            does not already exist (put if absent).If a document with the specified
+            `_id` already exists, the indexing operation will fail.Same as using the
+            `<index>/_create` endpoint.Valid values: `index`, `create`.If document
+            id is specified, it defaults to `index`.Otherwise, it defaults to
+            `create`.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg require_alias: If `true`, the destination must be an index
             alias. Default is false.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period the request waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST" if id in SKIP_IN_PATH else "PUT",
             _make_path(index, "_doc", id),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "pipeline",
+        "pretty",
         "refresh",
         "require_alias",
         "routing",
+        "source",
         "timeout",
         "wait_for_active_shards",
     )
-    async def bulk(
+    def bulk(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to perform multiple index/update/delete operations in a single request.
 
 
         :arg body: The operation definition and data (action-data
             pairs), separated by newlines
-        :arg index: Default index for items which don't provide one.
-        :arg _source: True or false to return the _source field or not,
-            or default list of fields to return, can be overridden on each sub-
-            request.
-        :arg _source_excludes: Default list of fields to exclude from
-            the returned _source field, can be overridden on each sub-request.
-        :arg _source_includes: Default list of fields to extract and
-            return from the _source field, can be overridden on each sub-request.
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: Sets require_alias for all incoming
-            documents. Default is false.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg index: Name of the data stream, index, or index alias to
+            perform bulk actions on.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg require_alias: If `true`, the request’s actions must target
+            an index alias. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period each action waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_bulk"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    async def clear_scroll(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def clear_scroll(
         self,
         body: Any = None,
         scroll_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Explicitly clears the search context for a scroll.
 
 
         :arg body: Comma-separated list of scroll IDs to clear if none
             was specified via the scroll_id parameter
-        :arg scroll_id: Comma-separated list of scroll IDs to clear.
+        :arg scroll_id: Comma-separated list of scroll IDs to clear. To
+            clear all scroll IDs, use `_all`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if scroll_id in SKIP_IN_PATH and body in SKIP_IN_PATH:
             raise ValueError("You need to supply scroll_id or body.")
         elif scroll_id and not body:
             body = {"scroll_id": [scroll_id]}
         elif scroll_id:
             params["scroll_id"] = scroll_id
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "DELETE", "/_search/scroll", params=params, headers=headers, body=body
         )
 
     @query_params(
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "lenient",
         "min_score",
         "preference",
+        "pretty",
         "q",
         "routing",
+        "source",
         "terminate_after",
     )
-    async def count(
+    def count(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns number of documents matching a query.
 
 
         :arg body: Query to restrict the results specified with the
             Query DSL (optional)
-        :arg index: Comma-separated list of indices to restrict the
-            results.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*` or `_all`.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed.This parameter can only be used when the `q` query string
+            parameter is specified. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the `q` query string parameter is
+            specified.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg min_score: Include only documents with a specific `_score`
-            value in the result.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+            query: `AND` or `OR`.This parameter can only be used when the `q` query
+            string parameter is specified. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.This parameter can only be used when the `q` query
+            string parameter is specified.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, concrete, expanded or aliased
+            indices are ignored when frozen.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg min_score: Sets the minimum `_score` value that documents
+            must have to be included in the result.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_count"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
+        "pretty",
         "refresh",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    async def delete(
+    def delete(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Removes a document from the index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg index: Name of the target index.
+        :arg id: Unique identifier for the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "DELETE", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "conflicts",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
         "from_",
+        "human",
         "ignore_unavailable",
         "lenient",
         "max_docs",
         "preference",
+        "pretty",
         "q",
         "refresh",
         "request_cache",
         "requests_per_second",
         "routing",
         "scroll",
         "scroll_size",
         "search_timeout",
         "search_type",
         "size",
         "slices",
         "sort",
+        "source",
         "stats",
         "terminate_after",
         "timeout",
         "version",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    async def delete_by_query(
+    def delete_by_query(
         self,
         index: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes documents matching the provided query.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            or indices, omit this parameter or use `*` or `_all`.
         :arg body: The search definition using the Query DSL
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
         :arg _source_excludes: List of fields to exclude from the
             returned _source field.
         :arg _source_includes: List of fields to extract and return from
             the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
-        :arg conflicts: What to do when the operation encounters version
-            conflicts?. Valid choices are abort, proceed.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.
+        :arg conflicts: What to do if delete by query hits version
+            conflicts: `abort` or `proceed`. Valid choices are abort, proceed.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid values are: `all`,
+            `open`, `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg max_docs: Maximum number of documents to process.Defaults
+            to all documents.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg request_cache: If `true`, the request cache is used for
+            this request.Defaults to the index-level setting.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg scroll_size: Size on the scroll request powering the
+            requests per second. Default is 0.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg scroll_size: Size of the scroll request that powers the
             operation. Default is 100.
-        :arg search_timeout: Explicit timeout for each search request.
-            Defaults to no timeout.
-        :arg search_type: Search operation type. Valid choices are
+        :arg search_timeout: Explicit timeout for each search
+            request.Defaults to no timeout.
+        :arg search_type: The type of the search operation.Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg size: Deprecated, please use `max_docs` instead.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+            into. Valid choices are auto.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg version: Whether to return document version as part of a
-            hit.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.
+        :arg timeout: Period each deletion request waits for active
+            shards.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
         for param in (index, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_delete_by_query"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("requests_per_second")
-    async def delete_by_query_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    def delete_by_query_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Delete By Query
         operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: The ID for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path("_delete_by_query", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    async def delete_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def delete_script(
         self,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
         """
         if id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "DELETE", _make_path("_scripts", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
         "version",
         "version_type",
     )
-    async def exists(
+    def exists(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about whether a document exists in an index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases. Supports wildcards (`*`).
+        :arg id: Identifier of the document.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: List of stored fields to return as part of a
+            hit.If no fields are specified, no stored fields are included in the
+            response.If this field is specified, the `_source` parameter defaults to
+            false.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "HEAD", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "version",
         "version_type",
     )
-    async def exists_source(
+    def exists_source(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about whether a document source exists in an index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases. Supports wildcards (`*`).
+        :arg id: Identifier of the document.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_source", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "HEAD", path, params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "analyze_wildcard",
         "analyzer",
         "default_operator",
         "df",
+        "error_trace",
+        "filter_path",
+        "human",
         "lenient",
         "preference",
+        "pretty",
         "q",
         "routing",
+        "source",
         "stored_fields",
     )
-    async def explain(
+    def explain(
         self,
         index: Any,
         id: Any,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about why a specific matches (or doesn't match) a query.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Index names used to limit the request. Only a single
+            index name can be provided to this parameter.
+        :arg id: Defines the document ID.
         :arg body: The query definition using the Query DSL
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg analyze_wildcard: Specify whether wildcards and prefix
-            queries in the query string query should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg _source: True or false to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the `q` query string parameter is
+            specified.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The default field for query string query. Default is
-            _all.
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string. Default is _all.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: A comma-separated list of stored fields to
+            return in the response.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_explain", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "allow_no_indices",
+        "error_trace",
         "expand_wildcards",
         "fields",
+        "filter_path",
+        "human",
         "ignore_unavailable",
         "include_unmapped",
+        "pretty",
+        "source",
     )
-    async def field_caps(
+    def field_caps(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns the information about the capabilities of fields among multiple
         indices.
 
 
         :arg body: An index filter specified with the Query DSL
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg fields: Comma-separated list of field names.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg include_unmapped: Indicates whether unmapped fields should
-            be included in the response. Default is false.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases used to limit the request. Supports wildcards (*). To target all
+            data streams and indices, omit this parameter or use * or _all.
+        :arg allow_no_indices: If false, the request returns an error if
+            any wildcard expression, index alias,or `_all` value targets only
+            missing or closed indices. This behavior applies even if the request
+            targets other open indices. For example, a requesttargeting `foo*,bar*`
+            returns an error if an index starts with foo but no index starts with
+            bar.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match. If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams. Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg fields: Comma-separated list of fields to retrieve
+            capabilities for. Wildcard (`*`) expressions are supported.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `true`, missing or closed indices
+            are not included in the response.
+        :arg include_unmapped: If true, unmapped fields are included in
+            the response. Default is false.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_field_caps"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
         "version",
         "version_type",
     )
-    async def get(
+    def get(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns a document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the index that contains the document.
+        :arg id: Unique identifier of the document.
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If true, Opensearch refreshes the affected shards
+            to make this operation visible to search. If false, do nothing with
+            refreshes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: List of stored fields to return as part of a
+            hit.If no fields are specified, no stored fields are included in the
+            response.If this field is specified, the `_source` parameter defaults to
+            false.
         :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+            The specified version must match the current version of the document for
+            the request to succeed.
+        :arg version_type: Specific version type: internal, external,
+            external_gte. Valid choices are internal, external, external_gte, force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout")
-    async def get_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    def get_script(
         self,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", _make_path("_scripts", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "version",
         "version_type",
     )
-    async def get_source(
+    def get_source(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns the source of a document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the index that contains the document.
+        :arg id: Unique identifier of the document.
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: Boolean) If true, the request is real-time as
+            opposed to near-real-time.
+        :arg refresh: If true, Opensearch refreshes the affected shards
+            to make this operation visible to search. If false, do nothing with
+            refreshes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+            The specified version must match the current version of the document for
+            the request to succeed.
+        :arg version_type: Specific version type: internal, external,
+            external_gte. Valid choices are internal, external, external_gte, force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_source", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", path, params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
     )
-    async def mget(
+    def mget(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to get multiple documents in one request.
 
 
         :arg body: Document identifiers; can be either `docs`
             (containing full document information) or `ids` (when index is provided
             in the URL.
-        :arg index: Index name.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg index: Name of the index to retrieve documents from when
+            `ids` are specified, or when a document in the `docs` array does not
+            specify an index.
+        :arg _source: True or false to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.You can also use this parameter to exclude
+            fields from the subset specified in `_source_includes` query parameter.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.If this parameter is specified, only these
+            source fields are returned. You can exclude fields from this subset
+            using the `_source_excludes` query parameter.If the `_source` parameter
+            is `false`, this parameter is ignored.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, the request refreshes relevant shards
+            before retrieving documents.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: If `true`, retrieves the document fields
+            stored in the index rather than the document `_source`.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_mget"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "ccs_minimize_roundtrips",
+        "error_trace",
+        "filter_path",
+        "human",
         "max_concurrent_searches",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
+        "pretty",
         "rest_total_hits_as_int",
         "search_type",
+        "source",
         "typed_keys",
     )
-    async def msearch(
+    def msearch(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to execute several search operations in one request.
 
 
         :arg body: The request definitions (metadata-search request
             definition pairs), separated by newlines
-        :arg index: Comma-separated list of indices to use as default.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg max_concurrent_searches: Controls the maximum number of
-            concurrent searches the multi search api will execute.
-        :arg max_concurrent_shard_requests: The number of concurrent
-            shard requests each sub search executes concurrently per node. This
-            value should be used to limit the impact of the search on the cluster in
-            order to limit the number of concurrent shard requests. Default is 5.
-        :arg pre_filter_shard_size: Threshold that enforces a pre-filter
-            round-trip to prefilter search shards based on query rewriting if the
-            number of shards the search request expands to exceeds the threshold.
-            This filter round-trip can limit the number of shards significantly if
-            for instance a shard can not match any documents based on its rewrite
-            method ie. if date filters are mandatory to match but the shard bounds
-            and the query are disjoint.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
+        :arg index: Comma-separated list of data streams, indices, and
+            index aliases to search.
+        :arg ccs_minimize_roundtrips: If true, network roundtrips
+            between the coordinating node and remote clusters are minimized for
+            cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_concurrent_searches: Maximum number of concurrent
+            searches the multi search API can execute.
+        :arg max_concurrent_shard_requests: Maximum number of concurrent
+            shard requests that each sub-search request executes per node. Default
+            is 5.
+        :arg pre_filter_shard_size: Defines a threshold that enforces a
+            pre-filter roundtrip to prefilter search shards based on query rewriting
+            if the number of shards the search request expands to exceeds the
+            threshold. This filter roundtrip can limit the number of shards
+            significantly if for instance a shard can not match any documents based
+            on its rewrite method i.e., if date filters are mandatory to match but
+            the shard bounds and the query are disjoint.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If true, hits.total are returned as
+            an integer in the response. Defaults to false, which returns an object.
             Default is false.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg search_type: Indicates whether global term and document
+            frequencies should be used when scoring returned documents. Valid
+            choices are query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: Specifies whether aggregation and suggester
+            names should be prefixed by their respective types in the response.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_msearch"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "ccs_minimize_roundtrips",
+        "error_trace",
+        "filter_path",
+        "human",
         "max_concurrent_searches",
+        "pretty",
         "rest_total_hits_as_int",
         "search_type",
+        "source",
         "typed_keys",
     )
-    async def msearch_template(
+    def msearch_template(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to execute several search template operations in one request.
 
 
         :arg body: The request definitions (metadata-search request
             definition pairs), separated by newlines
-        :arg index: Comma-separated list of indices to use as default.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg max_concurrent_searches: Controls the maximum number of
-            concurrent searches the multi search api will execute.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*`.
+        :arg ccs_minimize_roundtrips: If `true`, network round-trips are
+            minimized for cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_concurrent_searches: Maximum number of concurrent
+            searches the API can run.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If `true`, the response returns
+            `hits.total` as an integer.If `false`, it returns `hits.total` as an
+            object. Default is false.
+        :arg search_type: The type of the search operation.Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
+            query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: If `true`, the response prefixes aggregation
+            and suggester names with their respective types.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_msearch", "template"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
         "field_statistics",
         "fields",
+        "filter_path",
+        "human",
         "ids",
         "offsets",
         "payloads",
         "positions",
         "preference",
+        "pretty",
         "realtime",
         "routing",
+        "source",
         "term_statistics",
         "version",
         "version_type",
     )
-    async def mtermvectors(
+    def mtermvectors(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns multiple termvectors in one request.
 
 
         :arg body: Define ids, documents, parameters or a list of
             parameters per document here. You must at least provide a list of
             document ids. See documentation.
-        :arg index: The index in which the document resides.
-        :arg field_statistics: Specifies if document count, sum of
-            document frequencies and sum of total term frequencies should be
-            returned. Applies to all returned documents unless otherwise specified
-            in body 'params' or 'docs'. Default is True.
-        :arg fields: Comma-separated list of fields to return. Applies
-            to all returned documents unless otherwise specified in body 'params' or
-            'docs'.
-        :arg ids: Comma-separated list of documents ids. You must define
-            ids as parameter or set 'ids' or 'docs' in the request body.
-        :arg offsets: Specifies if term offsets should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg payloads: Specifies if term payloads should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg positions: Specifies if term positions should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Applies to all returned documents unless otherwise
-            specified in body 'params' or 'docs'. Default is random.
-        :arg realtime: Specifies if requests are real-time as opposed to
+        :arg index: Name of the index that contains the documents.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg field_statistics: If `true`, the response includes the
+            document count, sum of document frequencies, and sum of total term
+            frequencies. Default is True.
+        :arg fields: Comma-separated list or wildcard expressions of
+            fields to include in the statistics.Used as the default list unless a
+            specific field list is provided in the `completion_fields` or
+            `fielddata_fields` parameters.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ids: A comma-separated list of documents ids. You must
+            define ids as parameter or set "ids" or "docs" in the request body
+        :arg offsets: If `true`, the response includes term offsets.
+            Default is True.
+        :arg payloads: If `true`, the response includes term payloads.
+            Default is True.
+        :arg positions: If `true`, the response includes term positions.
+            Default is True.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
             near-real-time. Default is True.
-        :arg routing: Routing value. Applies to all returned documents
-            unless otherwise specified in body 'params' or 'docs'.
-        :arg term_statistics: Specifies if total term frequency and
-            document frequency should be returned. Applies to all returned documents
-            unless otherwise specified in body 'params' or 'docs'. Default is false.
-        :arg version: Explicit version number for concurrency control.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg term_statistics: If true, the response includes term
+            frequency and document frequency. Default is false.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
         :arg version_type: Specific version type. Valid choices are
             internal, external, external_gte, force.
         """
         path = _make_path(index, "_mtermvectors")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    async def put_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def put_script(
         self,
         id: Any,
         body: Any,
         context: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates or updates a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
+            Must be unique within the cluster.
         :arg body: The document
-        :arg context: Script context.
+        :arg context: Context in which the script or search template
+            should run. To prevent errors, the API immediately compiles the script
+            or template in this context.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
         """
         for param in (id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "PUT",
             _make_path("_scripts", id, context),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
-        "allow_no_indices", "expand_wildcards", "ignore_unavailable", "search_type"
+        "allow_no_indices",
+        "error_trace",
+        "expand_wildcards",
+        "filter_path",
+        "human",
+        "ignore_unavailable",
+        "pretty",
+        "search_type",
+        "source",
     )
-    async def rank_eval(
+    def rank_eval(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to evaluate the quality of ranked search results over a set of typical
         search queries.
 
 
         :arg body: The ranking evaluation search definition, including
             search requests, document ratings and ranking metric definition.
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
+        :arg index: Comma-separated list of data streams, indices, and
+            index aliases used to limit the request. Wildcard (`*`) expressions are
+            supported. To target all data streams and indices in a cluster, omit
+            this parameter or use `_all` or `*`.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices. This behavior applies even if the request
+            targets other open indices. For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, dfs_query_then_fetch.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `true`, missing or closed indices
+            are not included in the response.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg search_type: Search operation type
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_rank_eval"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "max_docs",
+        "pretty",
         "refresh",
         "requests_per_second",
         "scroll",
         "slices",
+        "source",
         "timeout",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    async def reindex(
+    def reindex(
         self,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to copy documents from one index to another, optionally filtering the
         source documents by a query, changing the destination index settings, or
         fetching the documents from a remote cluster.
 
 
         :arg body: The search definition using the Query DSL and the
             prototype for the index request.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg refresh: Should the affected indexes be refreshed?.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_docs: Maximum number of documents to process. By
+            default, all documents.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, the request refreshes affected shards
+            to make this operation visible to search.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg scroll: Specify how long a consistent view of the index
+            requests per second.Defaults to no throttle. Default is 0.
+        :arg scroll: Specifies how long a consistent view of the index
             should be maintained for scrolled search.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+            into.Defaults to 1 slice, meaning the task isn’t sliced into subtasks.
+            Valid choices are auto.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period each indexing waits for automatic index
+            creation, dynamic mapping updates, and waiting for active shards.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", "/_reindex", params=params, headers=headers, body=body
         )
 
-    @query_params("requests_per_second")
-    async def reindex_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    def reindex_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Reindex operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: Identifier for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path("_reindex", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    async def render_search_template(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def render_search_template(
         self,
         body: Any = None,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to use the Mustache language to pre-render a search definition.
 
 
         :arg body: The search definition template and its params
-        :arg id: The id of the stored search template.
+        :arg id: ID of the search template to render. If no `source` is
+            specified, this or the `id` request body parameter is required.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path("_render", "template", id),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    async def scripts_painless_execute(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def scripts_painless_execute(
         self,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows an arbitrary script to be executed and a result to be returned.
 
 
         :arg body: The script to execute
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             "/_scripts/painless/_execute",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("rest_total_hits_as_int", "scroll")
-    async def scroll(
+    @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "rest_total_hits_as_int",
+        "scroll",
+        "source",
+    )
+    def scroll(
         self,
         body: Any = None,
         scroll_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to retrieve a large numbers of results from a single search request.
 
 
         :arg body: The scroll ID if not passed by URL or query
             parameter.
-        :arg scroll_id: Scroll ID.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
+        :arg scroll_id: The scroll ID for scrolled search
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If true, the API response’s
+            hit.total property is returned as an integer. If false, the API
+            response’s hit.total property is returned as an object. Default is
+            false.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if scroll_id in SKIP_IN_PATH and body in SKIP_IN_PATH:
             raise ValueError("You need to supply scroll_id or body.")
         elif scroll_id and not body:
             body = {"scroll_id": scroll_id}
         elif scroll_id:
             params["scroll_id"] = scroll_id
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", "/_search/scroll", params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
@@ -1592,677 +2115,950 @@
         "analyze_wildcard",
         "analyzer",
         "batched_reduce_size",
         "ccs_minimize_roundtrips",
         "default_operator",
         "df",
         "docvalue_fields",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
         "from_",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "include_named_queries_score",
         "lenient",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
         "preference",
+        "pretty",
         "q",
         "request_cache",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_pipeline",
         "search_type",
         "seq_no_primary_term",
         "size",
         "sort",
+        "source",
         "stats",
         "stored_fields",
         "suggest_field",
         "suggest_mode",
         "suggest_size",
         "suggest_text",
         "terminate_after",
         "timeout",
         "track_scores",
         "track_total_hits",
         "typed_keys",
         "version",
     )
-    async def search(
+    def search(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns results matching a query.
 
 
         :arg body: The search definition using the Query DSL
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg allow_partial_search_results: Indicate if an error should
-            be returned if there is a partial search failure or timeout. Default is
-            True.
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*` or `_all`.
+        :arg _source: Indicates which source fields are returned for
+            matching documents.These fields are returned in the `hits._source`
+            property of the search response.Valid values are:`true` to return the
+            entire document source;`false` to not return the document
+            source;`<string>` to return the source fields that are specified as a
+            comma-separated list (supports wildcard (`*`) patterns).
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.You can also use this parameter to exclude
+            fields from the subset specified in `_source_includes` query
+            parameter.If the `_source` parameter is `false`, this parameter is
+            ignored.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.If this parameter is specified, only these
+            source fields are returned.You can exclude fields from this subset using
+            the `_source_excludes` query parameter.If the `_source` parameter is
+            `false`, this parameter is ignored.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg allow_partial_search_results: If true, returns partial
+            results if there are shard request timeouts or shard failures. If false,
+            returns an error with no partial results. Default is True.
+        :arg analyze_wildcard: If true, wildcard and prefix queries are
+            analyzed.This parameter can only be used when the q query string
+            parameter is specified. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the q query string parameter is
+            specified.
         :arg batched_reduce_size: The number of shard results that
-            should be reduced at once on the coordinating node. This value should be
+            should be reduced at once on the coordinating node.This value should be
             used as a protection mechanism to reduce the memory overhead per search
             request if the potential number of shards in the request can be large.
             Default is 512.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
+        :arg ccs_minimize_roundtrips: If true, network round-trips
+            between the coordinating node and the remote clusters are minimized when
+            executing cross-cluster search (CCS) requests. Default is True.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg docvalue_fields: Comma-separated list of fields to return
-            as the docvalue representation of a field for each hit.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg explain: Specify whether to return detailed information
-            about score computation as part of a hit.
-        :arg from_: Starting offset. Default is 0.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
+            query: AND or OR.This parameter can only be used when the `q` query
+            string parameter is specified. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.This parameter can only be used when the q query
+            string parameter is specified.
+        :arg docvalue_fields: A comma-separated list of fields to return
+            as the docvalue representation for each hit.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg explain: If `true`, returns detailed information about
+            score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg from_: Starting document offset.Needs to be non-negative.By
+            default, you cannot page through more than 10,000 hits using the `from`
+            and `size` parameters.To page through more hits, use the `search_after`
+            parameter. Default is 0.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, concrete, expanded or aliased
+            indices will be ignored when frozen.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
         :arg include_named_queries_score: Indicates whether
             hit.matched_queries should be rendered as a map that includes the name
             of the matched query associated with its score (true) or as an array
             containing the name of the matched queries (false) Default is false.
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_concurrent_shard_requests: The number of concurrent
-            shard requests per node this search executes concurrently. This value
-            should be used to limit the impact of the search on the cluster in order
-            to limit the number of concurrent shard requests. Default is 5.
-        :arg pre_filter_shard_size: Threshold that enforces a pre-filter
-            round-trip to prefilter search shards based on query rewriting if the
-            number of shards the search request expands to exceeds the threshold.
-            This filter round-trip can limit the number of shards significantly if
-            for instance a shard can not match any documents based on its rewrite
-            method ie. if date filters are mandatory to match but the shard bounds
-            and the query are disjoint.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg q: Query in the Lucene query string syntax.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be
+            ignored.This parameter can only be used when the `q` query string
+            parameter is specified.
+        :arg max_concurrent_shard_requests: Defines the number of
+            concurrent shard requests per node this search executes
+            concurrently.This value should be used to limit the impact of the search
+            on the cluster in order to limit the number of concurrent shard
+            requests. Default is 5.
+        :arg pre_filter_shard_size: Defines a threshold that enforces a
+            pre-filter roundtrip to prefilter search shards based on query rewriting
+            if the number of shards the search request expands to exceeds the
+            threshold.This filter roundtrip can limit the number of shards
+            significantly if for instance a shard can not match any documents based
+            on its rewrite method (if date filters are mandatory to match but the
+            shard bounds and the query are disjoint).When unspecified, the pre-
+            filter phase is executed if any of these conditions is met:the request
+            targets more than 128 shards;the request targets one or more read-only
+            index;the primary sort of the query targets an indexed field.
+        :arg preference: Nodes and shards used for the search.By
+            default, Opensearch selects from eligible nodes and shards using
+            adaptive replica selection, accounting for allocation awareness. Valid
+            values are:`_only_local` to run the search only on shards on the local
+            node;`_local` to, if possible, run the search on shards on the local
+            node, or if not, select shards using the default
+            method;`_only_nodes:<node-id>,<node-id>` to run the search on only the
+            specified nodes IDs, where, if suitable shards exist on more than one
+            selected node, use shards on those nodes using the default method, or if
+            none of the specified nodes are available, select shards from any
+            available node using the default method;`_prefer_nodes:<node-id>,<node-
+            id>` to if possible, run the search on the specified nodes IDs, or if
+            not, select shards using the default method;`_shards:<shard>,<shard>` to
+            run the search only on the specified shards;`<custom-string>` (any
+            string that does not start with `_`) to route searches with the same
+            `<custom-string>` to the same shards in the same order. Default is
+            random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg q: Query in the Lucene query string syntax using query
+            parameter search.Query parameter searches do not support the full
+            Opensearch Query DSL but are handy for testing.
+        :arg request_cache: If `true`, the caching of search results is
+            enabled for requests where `size` is `0`.Defaults to index level
+            settings.
+        :arg rest_total_hits_as_int: Indicates whether `hits.total`
+            should be rendered as an integer or an object in the rest search
+            response. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+            See Scroll search results.By default, this value cannot exceed `1d` (24
+            hours).You can change this limit using the `search.max_keep_alive`
+            cluster-level setting.
         :arg search_pipeline: Customizable sequence of processing stages
             applied to search queries.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, dfs_query_then_fetch.
-        :arg seq_no_primary_term: Specify whether to return sequence
-            number and primary term of the last modification of each hit.
-        :arg size: Number of hits to return. Default is 10.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+        :arg search_type: How distributed term frequencies are
+            calculated for relevance scoring. Valid choices are query_then_fetch,
+            dfs_query_then_fetch.
+        :arg seq_no_primary_term: If `true`, returns sequence number and
+            primary term of the last modification of each hit.
+        :arg size: Defines the number of hits to return.By default, you
+            cannot page through more than 10,000 hits using the `from` and `size`
+            parameters.To page through more hits, use the `search_after` parameter.
+            Default is 10.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
-        :arg suggest_field: Specify which field to use for suggestions.
-        :arg suggest_mode: Specify suggest mode. Valid choices are
-            missing, popular, always.
-        :arg suggest_size: How many suggestions to return in response.
+        :arg stored_fields: A comma-separated list of stored fields to
+            return as part of a hit.If no fields are specified, no stored fields are
+            included in the response.If this field is specified, the `_source`
+            parameter defaults to `false`.You can pass `_source: true` to return
+            both source fields and stored fields in the search response.
+        :arg suggest_field: Specifies which field to use for
+            suggestions.
+        :arg suggest_mode: Specifies the suggest mode.This parameter can
+            only be used when the `suggest_field` and `suggest_text` query string
+            parameters are specified. Valid choices are missing, popular, always.
+        :arg suggest_size: Number of suggestions to return.This
+            parameter can only be used when the `suggest_field` and `suggest_text`
+            query string parameters are specified.
         :arg suggest_text: The source text for which the suggestions
-            should be returned.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Operation timeout.
-        :arg track_scores: Whether to calculate and return scores even
-            if they are not used for sorting.
-        :arg track_total_hits: Indicate if the number of documents that
-            match the query should be tracked.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
-        :arg version: Whether to return document version as part of a
+            should be returned.This parameter can only be used when the
+            `suggest_field` and `suggest_text` query string parameters are
+            specified.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.If set to
+            `0` (default), the query does not terminate early.
+        :arg timeout: Specifies the period of time to wait for a
+            response from each shard.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg track_scores: If `true`, calculate and return document
+            scores, even if the scores are not used for sorting.
+        :arg track_total_hits: Number of hits matching the query to
+            count accurately.If `true`, the exact number of hits is returned at the
+            cost of some performance.If `false`, the response does not include the
+            total number of hits matching the query.
+        :arg typed_keys: If `true`, aggregation and suggester names are
+            be prefixed by their respective types in the response.
+        :arg version: If `true`, returns document version as part of a
             hit.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_search"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "allow_no_indices",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "ignore_unavailable",
         "local",
         "preference",
+        "pretty",
         "routing",
+        "source",
     )
-    async def search_shards(
+    def search_shards(
         self,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about the indices and shards that a search request would be
         executed against.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg routing: Routing value.
+        :arg index: Returns the indices and shards that a search request
+            would be executed against.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg local: If `true`, the request retrieves information from
+            the local node only. Default is false.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", _make_path(index, "_search_shards"), params=params, headers=headers
         )
 
     @query_params(
         "allow_no_indices",
         "ccs_minimize_roundtrips",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "preference",
+        "pretty",
         "profile",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_type",
+        "source",
         "typed_keys",
     )
-    async def search_template(
+    def search_template(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to use the Mustache language to pre-render a search definition.
 
 
         :arg body: The search definition template and its params
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg explain: Specify whether to return detailed information
-            about score computation as part of a hit.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg profile: Specify whether to profile the query execution.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (*).
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg ccs_minimize_roundtrips: If `true`, network round-trips are
+            minimized for cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg explain: If `true`, the response includes additional
+            details about score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, specified concrete, expanded,
+            or aliased indices are not included in the response when throttled.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg profile: If `true`, the query execution is profiled.
+        :arg rest_total_hits_as_int: If true, hits.total are rendered as
+            an integer in the response. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Specifies how long a consistent view of the
+            indexshould be maintained for scrolled search.
+        :arg search_type: The type of the search operation. Valid
+            choices are query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: If `true`, the response prefixes aggregation
+            and suggester names with their respective types.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_search", "template"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
         "field_statistics",
         "fields",
+        "filter_path",
+        "human",
         "offsets",
         "payloads",
         "positions",
         "preference",
+        "pretty",
         "realtime",
         "routing",
+        "source",
         "term_statistics",
         "version",
         "version_type",
     )
-    async def termvectors(
+    def termvectors(
         self,
         index: Any,
         body: Any = None,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information and statistics about terms in the fields of a particular
         document.
 
 
-        :arg index: The index in which the document resides.
+        :arg index: Name of the index that contains the document.
         :arg body: Define parameters and or supply a document to get
             termvectors for. See documentation.
-        :arg id: Document ID. When not specified a doc param should be
-            supplied.
-        :arg field_statistics: Specifies if document count, sum of
-            document frequencies and sum of total term frequencies should be
-            returned. Default is True.
-        :arg fields: Comma-separated list of fields to return.
-        :arg offsets: Specifies if term offsets should be returned.
+        :arg id: Unique identifier of the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg field_statistics: If `true`, the response includes the
+            document count, sum of document frequencies, and sum of total term
+            frequencies. Default is True.
+        :arg fields: Comma-separated list or wildcard expressions of
+            fields to include in the statistics.Used as the default list unless a
+            specific field list is provided in the `completion_fields` or
+            `fielddata_fields` parameters.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg offsets: If `true`, the response includes term offsets.
             Default is True.
-        :arg payloads: Specifies if term payloads should be returned.
+        :arg payloads: If `true`, the response includes term payloads.
             Default is True.
-        :arg positions: Specifies if term positions should be returned.
+        :arg positions: If `true`, the response includes term positions.
             Default is True.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specifies if request is real-time as opposed to
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
             near-real-time. Default is True.
-        :arg routing: Routing value.
-        :arg term_statistics: Specifies if total term frequency and
-            document frequency should be returned. Default is false.
-        :arg version: Explicit version number for concurrency control.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg term_statistics: If `true`, the response includes term
+            frequency and document frequency. Default is false.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
         :arg version_type: Specific version type. Valid choices are
             internal, external, external_gte, force.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
         path = _make_path(index, "_termvectors", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
         "lang",
+        "pretty",
         "refresh",
         "require_alias",
         "retry_on_conflict",
         "routing",
+        "source",
         "timeout",
         "wait_for_active_shards",
     )
-    async def update(
+    def update(
         self,
         index: Any,
         id: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Updates a document with a script or partial document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: The name of the index
+        :arg id: Document ID
         :arg body: The request definition requires either `script` or
             partial `doc`
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
+        :arg _source: Set to false to disable source retrieval. You can
+            also specify a comma-separatedlist of the fields you want to retrieve.
+        :arg _source_excludes: Specify the source fields you want to
+            exclude.
+        :arg _source_includes: Specify the source fields you want to
+            retrieve.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
         :arg lang: The script language. Default is painless.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: When true, requires destination to be an
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If 'true', Opensearch refreshes the affected
+            shards to make this operationvisible to search, if 'wait_for' then wait
+            for a refresh to make this operationvisible to search, if 'false' do
+            nothing with refreshes. Valid choices are true, false, wait_for.
+        :arg require_alias: If true, the destination must be an index
             alias. Default is false.
         :arg retry_on_conflict: Specify how many times should the
             operation be retried when a conflict occurs. Default is 0.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for dynamic mapping updates and
+            active shards.This guarantees Opensearch waits for at least the timeout
+            before failing.The actual wait time could be longer, particularly when
+            multiple waits occur.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operations.Set to 'all' or any
+            positive integer up to the total number of shards in the
+            index(number_of_replicas+1). Defaults to 1 meaning the primary shard.
+            Valid choices are all, index-setting.
         """
         for param in (index, id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_update", id)
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "conflicts",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
         "from_",
+        "human",
         "ignore_unavailable",
         "lenient",
         "max_docs",
         "pipeline",
         "preference",
+        "pretty",
         "q",
         "refresh",
         "request_cache",
         "requests_per_second",
         "routing",
         "scroll",
         "scroll_size",
         "search_timeout",
         "search_type",
         "size",
         "slices",
         "sort",
+        "source",
         "stats",
         "terminate_after",
         "timeout",
         "version",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    async def update_by_query(
+    def update_by_query(
         self,
         index: Any,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Performs an update on every document in the index without changing the source,
         for example to pick up a mapping change.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            or indices, omit this parameter or use `*` or `_all`.
         :arg body: The search definition using the Query DSL
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
         :arg _source_excludes: List of fields to exclude from the
             returned _source field.
         :arg _source_includes: List of fields to extract and return from
             the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
-        :arg conflicts: What to do when the operation encounters version
-            conflicts?. Valid choices are abort, proceed.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.
+        :arg conflicts: What to do if update by query hits version
+            conflicts: `abort` or `proceed`. Valid choices are abort, proceed.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg max_docs: Maximum number of documents to process.Defaults
+            to all documents.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg refresh: Should the affected indexes be refreshed?.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
+        :arg refresh: If `true`, Opensearch refreshes affected shards to
+            make the operation visible to search.
+        :arg request_cache: If `true`, the request cache is used for
+            this request.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg scroll_size: Size on the scroll request powering the
+            requests per second. Default is 0.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg scroll_size: Size of the scroll request that powers the
             operation. Default is 100.
         :arg search_timeout: Explicit timeout for each search request.
-            Defaults to no timeout.
-        :arg search_type: Search operation type. Valid choices are
+        :arg search_type: The type of the search operation. Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg size: Deprecated, please use `max_docs` instead.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+            into. Valid choices are auto.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg version: Whether to return document version as part of a
-            hit.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.
+        :arg timeout: Period each update request waits for the following
+            operations: dynamic mapping updates, waiting for active shards.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_update_by_query"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("requests_per_second")
-    async def update_by_query_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    def update_by_query_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Update By Query
         operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: The ID for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path("_update_by_query", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    async def get_script_context(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def get_script_context(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns all script contexts.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", "/_script_context", params=params, headers=headers
         )
 
-    @query_params()
-    async def get_script_languages(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def get_script_languages(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns available script types, languages and contexts.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", "/_script_language", params=params, headers=headers
         )
 
     @query_params(
         "allow_partial_pit_creation",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "keep_alive",
         "preference",
+        "pretty",
         "routing",
+        "source",
     )
-    async def create_pit(
+    def create_pit(
         self,
         index: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates point in time context.
 
 
         :arg index: Comma-separated list of indices; use `_all` or empty
             string to perform the operation on all indices.
         :arg allow_partial_pit_creation: Allow if point in time can be
             created with partial failures.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg keep_alive: Specify the keep alive for point in time.
         :arg preference: Specify the node or shard the operation should
             be performed on. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg routing: Comma-separated list of specific routing values.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "POST",
             _make_path(index, "_search", "point_in_time"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    async def delete_all_pits(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def delete_all_pits(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes all active point in time searches.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "DELETE", "/_search/point_in_time/_all", params=params, headers=headers
         )
 
-    @query_params()
-    async def delete_pit(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def delete_pit(
         self,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes one or more point in time searches based on the IDs passed.
 
 
         :arg body: The point-in-time ids to be deleted
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "DELETE",
             "/_search/point_in_time",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    async def get_all_pits(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def get_all_pits(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Lists all active point in time searches.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
+        return self.transport.perform_request(
             "GET", "/_search/point_in_time/_all", params=params, headers=headers
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/_patch.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/_patch.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/client.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/client.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/cluster.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/snapshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,626 +35,577 @@
 
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class ClusterClient(NamespacedClient):
+class SnapshotClient(NamespacedClient):
     @query_params(
-        "awareness_attribute",
         "cluster_manager_timeout",
-        "expand_wildcards",
-        "level",
-        "local",
+        "error_trace",
+        "filter_path",
+        "human",
         "master_timeout",
-        "timeout",
-        "wait_for_active_shards",
-        "wait_for_events",
-        "wait_for_no_initializing_shards",
-        "wait_for_no_relocating_shards",
-        "wait_for_nodes",
-        "wait_for_status",
+        "pretty",
+        "source",
+        "wait_for_completion",
     )
-    async def health(
+    async def create(
         self,
-        index: Any = None,
+        repository: Any,
+        snapshot: Any,
+        body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns basic information about the health of the cluster.
+        Creates a snapshot in a repository.
 
 
-        :arg index: Limit the information returned to specific indicies.
-        :arg awareness_attribute: The awareness attribute for which the
-            health is required.
+        :arg repository: Repository for the snapshot.
+        :arg snapshot: Name of the snapshot. Must be unique in the
+            repository.
+        :arg body: The snapshot definition
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg level: Specify the level of detail for returned
-            information. Valid choices are cluster, indices, shards,
-            awareness_attributes.
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
-        :arg wait_for_active_shards: Wait until the specified number of
-            shards is active.
-        :arg wait_for_events: Wait until all currently queued events
-            with the given priority are processed. Valid choices are immediate,
-            urgent, high, normal, low, languid.
-        :arg wait_for_no_initializing_shards: Whether to wait until
-            there are no initializing shards in the cluster.
-        :arg wait_for_no_relocating_shards: Whether to wait until there
-            are no relocating shards in the cluster.
-        :arg wait_for_nodes: Wait until the specified number of nodes is
-            available.
-        :arg wait_for_status: Wait until cluster is in a specific state.
-            Valid choices are green, yellow, red.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node. If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg wait_for_completion: If `true`, the request returns a
+            response when the snapshot is complete. If `false`, the request returns
+            a response when the snapshot initializes. Default is false.
         """
+        for param in (repository, snapshot):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
+
         return await self.transport.perform_request(
-            "GET",
-            _make_path("_cluster", "health", index),
+            "PUT",
+            _make_path("_snapshot", repository, snapshot),
             params=params,
             headers=headers,
+            body=body,
         )
 
-    @query_params("cluster_manager_timeout", "local", "master_timeout")
-    async def pending_tasks(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    async def delete(
         self,
+        repository: Any,
+        snapshot: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns a list of any cluster-level changes (e.g. create index, update mapping,
-        allocate or fail shard) which have not yet been executed.
+        Deletes a snapshot.
 
 
+        :arg repository: A repository name
+        :arg snapshot: A comma-separated list of snapshot names
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
+        for param in (repository, snapshot):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
+
         return await self.transport.perform_request(
-            "GET", "/_cluster/pending_tasks", params=params, headers=headers
+            "DELETE",
+            _make_path("_snapshot", repository, snapshot),
+            params=params,
+            headers=headers,
         )
 
     @query_params(
-        "allow_no_indices",
         "cluster_manager_timeout",
-        "expand_wildcards",
-        "flat_settings",
+        "error_trace",
+        "filter_path",
+        "human",
         "ignore_unavailable",
-        "local",
         "master_timeout",
-        "wait_for_metadata_version",
-        "wait_for_timeout",
+        "pretty",
+        "source",
+        "verbose",
     )
-    async def state(
+    async def get(
         self,
-        metric: Any = None,
-        index: Any = None,
+        repository: Any,
+        snapshot: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns a comprehensive information about the state of the cluster.
+        Returns information about a snapshot.
 
 
-        :arg metric: Limit the information returned to the specified
-            metrics. Valid choices are _all, blocks, metadata, nodes, routing_table,
-            routing_nodes, master_node, cluster_manager_node, version.
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
+        :arg repository: Comma-separated list of snapshot repository
+            names used to limit the request. Wildcard (*) expressions are supported.
+        :arg snapshot: Comma-separated list of snapshot names to
+            retrieve. Also accepts wildcards (*). - To get information about all
+            snapshots in a registered repository, use a wildcard (*) or _all. - To
+            get information about any snapshots that are currently running, use
+            _current.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If false, the request returns an error
+            for any snapshots that are unavailable. Default is false.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg wait_for_metadata_version: Wait for the metadata version to
-            be equal or greater than the specified metadata version.
-        :arg wait_for_timeout: The maximum time to wait for
-            wait_for_metadata_version before timing out.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node. If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg verbose: If true, returns additional information about each
+            snapshot such as the version of Opensearch which took the snapshot, the
+            start and end times of the snapshot, and the number of shards
+            snapshotted.
         """
-        if index and metric in SKIP_IN_PATH:
-            metric = "_all"
-
-        return await self.transport.perform_request(
-            "GET",
-            _make_path("_cluster", "state", metric, index),
-            params=params,
-            headers=headers,
-        )
-
-    @query_params("flat_settings", "timeout")
-    async def stats(
-        self,
-        node_id: Any = None,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Returns high-level overview of cluster statistics.
-
+        for param in (repository, snapshot):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
-        :arg timeout: Operation timeout.
-        """
         return await self.transport.perform_request(
             "GET",
-            "/_cluster/stats"
-            if node_id in SKIP_IN_PATH
-            else _make_path("_cluster", "stats", "nodes", node_id),
+            _make_path("_snapshot", repository, snapshot),
             params=params,
             headers=headers,
         )
 
     @query_params(
         "cluster_manager_timeout",
-        "dry_run",
-        "explain",
+        "error_trace",
+        "filter_path",
+        "human",
         "master_timeout",
-        "metric",
-        "retry_failed",
+        "pretty",
+        "source",
         "timeout",
     )
-    async def reroute(
+    async def delete_repository(
         self,
-        body: Any = None,
+        repository: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Allows to manually change the allocation of individual shards in the cluster.
+        Deletes a repository.
 
 
-        :arg body: The definition of `commands` to perform (`move`,
-            `cancel`, `allocate`)
+        :arg repository: Name of the snapshot repository to unregister.
+            Wildcard (`*`) patterns are supported.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg dry_run: Simulate the operation only and return the
-            resulting state.
-        :arg explain: Return an explanation of why the commands can or
-            cannot be executed.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg metric: Limit the information returned to the specified
-            metrics. Defaults to all but metadata.
-        :arg retry_failed: Retries allocation of shards that are blocked
-            due to too many subsequent allocation failures.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
+        if repository in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'repository'.")
+
         return await self.transport.perform_request(
-            "POST", "/_cluster/reroute", params=params, headers=headers, body=body
+            "DELETE",
+            _make_path("_snapshot", repository),
+            params=params,
+            headers=headers,
         )
 
     @query_params(
         "cluster_manager_timeout",
-        "flat_settings",
-        "include_defaults",
+        "error_trace",
+        "filter_path",
+        "human",
+        "local",
         "master_timeout",
-        "timeout",
+        "pretty",
+        "source",
     )
-    async def get_settings(
+    async def get_repository(
         self,
+        repository: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns cluster settings.
+        Returns information about a repository.
 
 
+        :arg repository: A comma-separated list of repository names
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
-        :arg include_defaults: Whether to return all default clusters
-            setting. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg local: Return local information, do not retrieve the state
+            from cluster-manager node. Default is false.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         return await self.transport.perform_request(
-            "GET", "/_cluster/settings", params=params, headers=headers
+            "GET", _make_path("_snapshot", repository), params=params, headers=headers
         )
 
     @query_params(
-        "cluster_manager_timeout", "flat_settings", "master_timeout", "timeout"
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+        "verify",
     )
-    async def put_settings(
+    async def create_repository(
         self,
+        repository: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Updates the cluster settings.
+        Creates a repository.
 
 
-        :arg body: The settings to be updated. Can be either `transient`
-            or `persistent` (survives cluster restart).
+        :arg repository: A repository name
+        :arg body: The repository definition
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
+        :arg verify: Whether to verify the repository after creation
         """
-        if body in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'body'.")
-
-        return await self.transport.perform_request(
-            "PUT", "/_cluster/settings", params=params, headers=headers, body=body
-        )
-
-    @query_params()
-    async def remote_info(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Returns the information about configured remote clusters.
-
-        """
-        return await self.transport.perform_request(
-            "GET", "/_remote/info", params=params, headers=headers
-        )
-
-    @query_params("include_disk_info", "include_yes_decisions")
-    async def allocation_explain(
-        self,
-        body: Any = None,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Provides explanations for shard allocations in the cluster.
-
+        for param in (repository, body):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
 
-        :arg body: The index, shard, and primary flag to explain. Empty
-            means 'explain the first unassigned shard'
-        :arg include_disk_info: Return information about disk usage and
-            shard sizes. Default is false.
-        :arg include_yes_decisions: Return 'YES' decisions in
-            explanation. Default is false.
-        """
         return await self.transport.perform_request(
-            "POST",
-            "/_cluster/allocation/explain",
+            "PUT",
+            _make_path("_snapshot", repository),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    async def delete_component_template(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "wait_for_completion",
+    )
+    async def restore(
         self,
-        name: Any,
+        repository: Any,
+        snapshot: Any,
+        body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Deletes a component template.
+        Restores a snapshot.
 
 
-        :arg name: The name of the template.
+        :arg repository: A repository name
+        :arg snapshot: A snapshot name
+        :arg body: Details of what to restore
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg wait_for_completion: Should this request wait until the
+            operation has completed before returning Default is false.
         """
-        if name in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'name'.")
+        for param in (repository, snapshot):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
 
         return await self.transport.perform_request(
-            "DELETE",
-            _make_path("_component_template", name),
+            "POST",
+            _make_path("_snapshot", repository, snapshot, "_restore"),
             params=params,
             headers=headers,
+            body=body,
         )
 
-    @query_params("cluster_manager_timeout", "local", "master_timeout")
-    async def get_component_template(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "ignore_unavailable",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    async def status(
         self,
-        name: Any = None,
+        repository: Any = None,
+        snapshot: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns one or more component templates.
+        Returns information about the status of a snapshot.
 
 
-        :arg name: The Comma-separated names of the component templates.
+        :arg repository: A repository name
+        :arg snapshot: A comma-separated list of snapshot names
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: Whether to ignore unavailable
+            snapshots, defaults to false which means a SnapshotMissingException is
+            thrown Default is false.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         return await self.transport.perform_request(
             "GET",
-            _make_path("_component_template", name),
+            _make_path("_snapshot", repository, snapshot, "_status"),
             params=params,
             headers=headers,
         )
 
-    @query_params("cluster_manager_timeout", "create", "master_timeout", "timeout")
-    async def put_component_template(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def verify_repository(
         self,
-        name: Any,
-        body: Any,
+        repository: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Creates or updates a component template.
+        Verifies a repository.
 
 
-        :arg name: The name of the template.
-        :arg body: The template definition
+        :arg repository: A repository name
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg create: Whether the index template should only be added if
-            new or can also replace an existing one. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
-        for param in (name, body):
-            if param in SKIP_IN_PATH:
-                raise ValueError("Empty value passed for a required argument.")
+        if repository in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'repository'.")
 
         return await self.transport.perform_request(
-            "PUT",
-            _make_path("_component_template", name),
+            "POST",
+            _make_path("_snapshot", repository, "_verify"),
             params=params,
             headers=headers,
-            body=body,
         )
 
-    @query_params("cluster_manager_timeout", "local", "master_timeout")
-    async def exists_component_template(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def cleanup_repository(
         self,
-        name: Any,
+        repository: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns information about whether a particular component template exist.
+        Removes stale data from repository.
 
 
-        :arg name: The name of the template.
+        :arg repository: Snapshot repository to clean up.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        """
-        if name in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'name'.")
-
-        return await self.transport.perform_request(
-            "HEAD",
-            _make_path("_component_template", name),
-            params=params,
-            headers=headers,
-        )
-
-    @query_params("wait_for_removal")
-    async def delete_voting_config_exclusions(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.
         """
-        Clears cluster voting config exclusions.
-
+        if repository in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'repository'.")
 
-        :arg wait_for_removal: Specifies whether to wait for all
-            excluded nodes to be removed from the cluster before clearing the voting
-            configuration exclusions list. Default is True.
-        """
         return await self.transport.perform_request(
-            "DELETE",
-            "/_cluster/voting_config_exclusions",
-            params=params,
-            headers=headers,
-        )
-
-    @query_params("node_ids", "node_names", "timeout")
-    async def post_voting_config_exclusions(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Updates the cluster voting config exclusions by node ids or node names.
-
-
-        :arg node_ids: Comma-separated list of the persistent ids of the
-            nodes to exclude from the voting configuration. If specified, you may
-            not also specify ?node_names.
-        :arg node_names: Comma-separated list of the names of the nodes
-            to exclude from the voting configuration. If specified, you may not also
-            specify ?node_ids.
-        :arg timeout: Operation timeout.
-        """
-        return await self.transport.perform_request(
-            "POST", "/_cluster/voting_config_exclusions", params=params, headers=headers
-        )
-
-    @query_params()
-    async def delete_decommission_awareness(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Delete any existing decommission.
-
-        """
-        return await self.transport.perform_request(
-            "DELETE", "/_cluster/decommission/awareness", params=params, headers=headers
-        )
-
-    @query_params()
-    async def delete_weighted_routing(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Delete weighted shard routing weights.
-
-        """
-        return await self.transport.perform_request(
-            "DELETE",
-            "/_cluster/routing/awareness/weights",
-            params=params,
-            headers=headers,
-        )
-
-    @query_params()
-    async def get_decommission_awareness(
-        self,
-        awareness_attribute_name: Any,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Get details and status of decommissioned attribute.
-
-
-        :arg awareness_attribute_name: Awareness attribute name.
-        """
-        if awareness_attribute_name in SKIP_IN_PATH:
-            raise ValueError(
-                "Empty value passed for a required argument 'awareness_attribute_name'."
-            )
-
-        return await self.transport.perform_request(
-            "GET",
-            _make_path(
-                "_cluster",
-                "decommission",
-                "awareness",
-                awareness_attribute_name,
-                "_status",
-            ),
-            params=params,
-            headers=headers,
-        )
-
-    @query_params()
-    async def get_weighted_routing(
-        self,
-        attribute: Any,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Fetches weighted shard routing weights.
-
-
-        :arg attribute: Awareness attribute name.
-        """
-        if attribute in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'attribute'.")
-
-        return await self.transport.perform_request(
-            "GET",
-            _make_path("_cluster", "routing", "awareness", attribute, "weights"),
+            "POST",
+            _make_path("_snapshot", repository, "_cleanup"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    async def put_decommission_awareness(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    async def clone(
         self,
-        awareness_attribute_name: Any,
-        awareness_attribute_value: Any,
+        repository: Any,
+        snapshot: Any,
+        target_snapshot: Any,
+        body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Decommissions an awareness attribute.
+        Clones indices from one snapshot into another snapshot in the same repository.
 
 
-        :arg awareness_attribute_name: Awareness attribute name.
-        :arg awareness_attribute_value: Awareness attribute value.
+        :arg repository: A repository name
+        :arg snapshot: The name of the snapshot to clone from
+        :arg target_snapshot: The name of the cloned snapshot to create
+        :arg body: The snapshot clone definition
+        :arg cluster_manager_timeout: Operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg master_timeout (Deprecated: To promote inclusive language,
+            use 'cluster_manager_timeout' instead.): Explicit operation timeout for
+            connection to master node
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        for param in (awareness_attribute_name, awareness_attribute_value):
+        for param in (repository, snapshot, target_snapshot, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         return await self.transport.perform_request(
             "PUT",
-            _make_path(
-                "_cluster",
-                "decommission",
-                "awareness",
-                awareness_attribute_name,
-                awareness_attribute_value,
-            ),
-            params=params,
-            headers=headers,
-        )
-
-    @query_params()
-    async def put_weighted_routing(
-        self,
-        attribute: Any,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Updates weighted shard routing weights.
-
-
-        :arg attribute: Awareness attribute name.
-        """
-        if attribute in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'attribute'.")
-
-        return await self.transport.perform_request(
-            "PUT",
-            _make_path("_cluster", "routing", "awareness", attribute, "weights"),
+            _make_path("_snapshot", repository, snapshot, "_clone", target_snapshot),
             params=params,
             headers=headers,
+            body=body,
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/dangling_indices.py` & `opensearch_py-2.6.0/opensearchpy/client/search_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,32 +2,14 @@
 #
 # The OpenSearch Contributors require contributions made to
 # this file be licensed under the Apache-2.0 license or a
 # compatible open source license.
 #
 # Modifications Copyright OpenSearch Contributors. See
 # GitHub history for details.
-#
-#  Licensed to Elasticsearch B.V. under one or more contributor
-#  license agreements. See the NOTICE file distributed with
-#  this work for additional information regarding copyright
-#  ownership. Elasticsearch B.V. licenses this file to you under
-#  the Apache License, Version 2.0 (the "License"); you may
-#  not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-# 	http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing,
-#  software distributed under the License is distributed on an
-#  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-#  KIND, either express or implied.  See the License for the
-#  specific language governing permissions and limitations
-#  under the License.
-
 
 # ------------------------------------------------------------------------------------------
 # THIS CODE IS AUTOMATICALLY GENERATED AND MANUAL EDITS WILL BE LOST
 #
 # To contribute, kindly make modifications in the opensearch-py client generator
 # or in the OpenSearch API specification, and run `nox -rs generate`. See DEVELOPER_GUIDE.md
 # and https://github.com/opensearch-project/opensearch-api-specification for details.
@@ -35,84 +17,135 @@
 
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class DanglingIndicesClient(NamespacedClient):
+class SearchPipelineClient(NamespacedClient):
     @query_params(
-        "accept_data_loss", "cluster_manager_timeout", "master_timeout", "timeout"
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
     )
-    async def delete_dangling_index(
+    def get(
         self,
-        index_uuid: Any,
+        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Deletes the specified dangling index.
+        Retrieves information about a specified search pipeline.
 
 
-        :arg index_uuid: The UUID of the dangling index.
-        :arg accept_data_loss: Must be set to true in order to delete
-            the dangling index.
-        :arg cluster_manager_timeout: Operation timeout for connection
+        :arg id: Comma-separated list of search pipeline ids. Wildcards
+            supported.
+        :arg cluster_manager_timeout: operation timeout for connection
             to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        if index_uuid in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
-
-        return await self.transport.perform_request(
-            "DELETE",
-            _make_path("_dangling", index_uuid),
-            params=params,
-            headers=headers,
+        return self.transport.perform_request(
+            "GET", _make_path("_search", "pipeline", id), params=params, headers=headers
         )
 
     @query_params(
-        "accept_data_loss", "cluster_manager_timeout", "master_timeout", "timeout"
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "timeout",
     )
-    async def import_dangling_index(
+    def delete(
         self,
-        index_uuid: Any,
+        id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Imports the specified dangling index.
+        Deletes the specified search pipeline.
 
 
-        :arg index_uuid: The UUID of the dangling index.
-        :arg accept_data_loss: Must be set to true in order to import
-            the dangling index.
+        :arg id: Pipeline ID.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg timeout: Operation timeout.
         """
-        if index_uuid in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
+        if id in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return await self.transport.perform_request(
-            "POST", _make_path("_dangling", index_uuid), params=params, headers=headers
+        return self.transport.perform_request(
+            "DELETE",
+            _make_path("_search", "pipeline", id),
+            params=params,
+            headers=headers,
         )
 
-    @query_params()
-    async def list_dangling_indices(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def put(
         self,
+        id: Any,
+        body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns all dangling indices.
+        Creates or replaces the specified search pipeline.
 
+
+        :arg id: Pipeline ID.
+        :arg cluster_manager_timeout: operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Operation timeout.
         """
-        return await self.transport.perform_request(
-            "GET", "/_dangling", params=params, headers=headers
+        for param in (id, body):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
+
+        return self.transport.perform_request(
+            "PUT",
+            _make_path("_search", "pipeline", id),
+            params=params,
+            headers=headers,
+            body=body,
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/features.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/features.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/http.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/http.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/ingest.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/dangling_indices.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,134 +35,131 @@
 
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class IngestClient(NamespacedClient):
-    @query_params("cluster_manager_timeout", "master_timeout")
-    async def get_pipeline(
+class DanglingIndicesClient(NamespacedClient):
+    @query_params(
+        "accept_data_loss",
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def delete_dangling_index(
         self,
-        id: Any = None,
+        index_uuid: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns a pipeline.
+        Deletes the specified dangling index.
 
 
-        :arg id: Comma-separated list of pipeline ids. Wildcards
-            supported.
+        :arg index_uuid: The UUID of the dangling index
+        :arg accept_data_loss: Must be set to true in order to delete
+            the dangling index
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
-        return await self.transport.perform_request(
-            "GET", _make_path("_ingest", "pipeline", id), params=params, headers=headers
-        )
-
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    async def put_pipeline(
-        self,
-        id: Any,
-        body: Any,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Creates or updates a pipeline.
-
-
-        :arg id: Pipeline ID.
-        :arg body: The ingest definition
-        :arg cluster_manager_timeout: Operation timeout for connection
-            to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
-        """
-        for param in (id, body):
-            if param in SKIP_IN_PATH:
-                raise ValueError("Empty value passed for a required argument.")
+        if index_uuid in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
 
         return await self.transport.perform_request(
-            "PUT",
-            _make_path("_ingest", "pipeline", id),
+            "DELETE",
+            _make_path("_dangling", index_uuid),
             params=params,
             headers=headers,
-            body=body,
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    async def delete_pipeline(
+    @query_params(
+        "accept_data_loss",
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def import_dangling_index(
         self,
-        id: Any,
+        index_uuid: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Deletes a pipeline.
+        Imports the specified dangling index.
 
 
-        :arg id: Pipeline ID.
+        :arg index_uuid: The UUID of the dangling index
+        :arg accept_data_loss: Must be set to true in order to import
+            the dangling index
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
-        if id in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'id'.")
+        if index_uuid in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
 
         return await self.transport.perform_request(
-            "DELETE",
-            _make_path("_ingest", "pipeline", id),
-            params=params,
-            headers=headers,
+            "POST", _make_path("_dangling", index_uuid), params=params, headers=headers
         )
 
-    @query_params("verbose")
-    async def simulate(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def list_dangling_indices(
         self,
-        body: Any,
-        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Allows to simulate a pipeline with example documents.
-
-
-        :arg body: The simulate definition
-        :arg id: Pipeline ID.
-        :arg verbose: Verbose mode. Display data output for each
-            processor in executed pipeline. Default is false.
-        """
-        if body in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'body'.")
+        Returns all dangling indices.
 
-        return await self.transport.perform_request(
-            "POST",
-            _make_path("_ingest", "pipeline", id, "_simulate"),
-            params=params,
-            headers=headers,
-            body=body,
-        )
-
-    @query_params()
-    async def processor_grok(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Returns a list of the built-in patterns.
 
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         return await self.transport.perform_request(
-            "GET", "/_ingest/processor/grok", params=params, headers=headers
+            "GET", "/_dangling", params=params, headers=headers
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/nodes.py` & `opensearch_py-2.6.0/opensearchpy/client/ingest.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,190 +32,225 @@
 # or in the OpenSearch API specification, and run `nox -rs generate`. See DEVELOPER_GUIDE.md
 # and https://github.com/opensearch-project/opensearch-api-specification for details.
 # -----------------------------------------------------------------------------------------+
 
 
 from typing import Any
 
-from .utils import NamespacedClient, _make_path, query_params
+from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class NodesClient(NamespacedClient):
-    @query_params("timeout")
-    async def reload_secure_settings(
+class IngestClient(NamespacedClient):
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    def get_pipeline(
         self,
-        body: Any = None,
-        node_id: Any = None,
+        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Reloads secure settings.
+        Returns a pipeline.
 
 
-        :arg body: An object containing the password for the opensearch
-            keystore
-        :arg node_id: Comma-separated list of node IDs to span the
-            reload/reinit call. Should stay empty because reloading usually involves
-            all cluster nodes.
-        :arg timeout: Operation timeout.
+        :arg id: Comma-separated list of pipeline IDs to retrieve.
+            Wildcard (`*`) expressions are supported. To get all ingest pipelines,
+            omit this parameter or use `*`.
+        :arg cluster_manager_timeout: Operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg master_timeout (Deprecated: To promote inclusive language,
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return await self.transport.perform_request(
-            "POST",
-            _make_path("_nodes", node_id, "reload_secure_settings"),
-            params=params,
-            headers=headers,
-            body=body,
+        return self.transport.perform_request(
+            "GET", _make_path("_ingest", "pipeline", id), params=params, headers=headers
         )
 
-    @query_params("flat_settings", "timeout")
-    async def info(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def put_pipeline(
         self,
-        node_id: Any = None,
-        metric: Any = None,
+        id: Any,
+        body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns information about nodes in the cluster.
+        Creates or updates a pipeline.
 
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg metric: Comma-separated list of metrics you wish returned.
-            Leave empty to return all. Valid choices are settings, os, process, jvm,
-            thread_pool, transport, http, plugins, ingest.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
-        :arg timeout: Operation timeout.
-        """
-        return await self.transport.perform_request(
-            "GET", _make_path("_nodes", node_id, metric), params=params, headers=headers
+        :arg id: ID of the ingest pipeline to create or update.
+        :arg body: The ingest definition
+        :arg cluster_manager_timeout: Operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg master_timeout (Deprecated: To promote inclusive language,
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node. If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response. If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
+        """
+        for param in (id, body):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
+
+        return self.transport.perform_request(
+            "PUT",
+            _make_path("_ingest", "pipeline", id),
+            params=params,
+            headers=headers,
+            body=body,
         )
 
     @query_params(
-        "completion_fields",
-        "fielddata_fields",
-        "fields",
-        "groups",
-        "include_segment_file_sizes",
-        "level",
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
         "timeout",
-        "types",
     )
-    async def stats(
+    def delete_pipeline(
         self,
-        node_id: Any = None,
-        metric: Any = None,
-        index_metric: Any = None,
+        id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns statistical information about nodes in the cluster.
+        Deletes a pipeline.
 
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg metric: Limit the information returned to the specified
-            metrics. Valid choices are _all, breaker, fs, http, indices, jvm, os,
-            process, thread_pool, transport, discovery, indexing_pressure,
-            search_pipeline.
-        :arg index_metric: Limit the information returned for `indices`
-            metric to the specific index metrics. Isn't used if `indices` (or `all`)
-            metric isn't specified. Valid choices are _all, store, indexing, get,
-            search, merge, flush, refresh, query_cache, fielddata, docs, warmer,
-            completion, segments, translog, suggest, request_cache, recovery.
-        :arg completion_fields: Comma-separated list of fields for
-            `fielddata` and `suggest` index metric (supports wildcards).
-        :arg fielddata_fields: Comma-separated list of fields for
-            `fielddata` index metric (supports wildcards).
-        :arg fields: Comma-separated list of fields for `fielddata` and
-            `completion` index metric (supports wildcards).
-        :arg groups: Comma-separated list of search groups for `search`
-            index metric.
-        :arg include_segment_file_sizes: Whether to report the
-            aggregated disk usage of each one of the Lucene index files (only
-            applies if segment stats are requested). Default is false.
-        :arg level: Return indices stats aggregated at index, node or
-            shard level. Valid choices are indices, node, shards.
-        :arg timeout: Operation timeout.
-        :arg types: Comma-separated list of document types for the
-            `indexing` index metric.
-        """
-        return await self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "stats", metric, index_metric),
+        :arg id: Pipeline ID or wildcard expression of pipeline IDs used
+            to limit the request. To delete all ingest pipelines in a cluster, use a
+            value of `*`.
+        :arg cluster_manager_timeout: Operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg master_timeout (Deprecated: To promote inclusive language,
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
+        """
+        if id in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'id'.")
+
+        return self.transport.perform_request(
+            "DELETE",
+            _make_path("_ingest", "pipeline", id),
             params=params,
             headers=headers,
         )
 
-    @query_params(
-        "doc_type", "ignore_idle_threads", "interval", "snapshots", "threads", "timeout"
-    )
-    async def hot_threads(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source", "verbose")
+    def simulate(
         self,
-        node_id: Any = None,
+        body: Any,
+        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns information about hot threads on each node in the cluster.
+        Allows to simulate a pipeline with example documents.
+
 
+        :arg body: The simulate definition
+        :arg id: Pipeline to test. If you don’t specify a `pipeline` in
+            the request body, this parameter is required.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg verbose: If `true`, the response includes output data for
+            each processor in the executed pipeline. Default is false.
+        """
+        if body in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'body'.")
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg doc_type: The type to sample. Valid choices are cpu, wait,
-            block.
-        :arg ignore_idle_threads: Don't show threads that are in known-
-            idle places, such as waiting on a socket select or pulling from an empty
-            task queue. Default is True.
-        :arg interval: The interval for the second sampling of threads.
-        :arg snapshots: Number of samples of thread stacktrace. Default
-            is 10.
-        :arg threads: Specify the number of threads to provide
-            information for. Default is 3.
-        :arg timeout: Operation timeout.
-        """
-        # type is a reserved word so it cannot be used, use doc_type instead
-        if "doc_type" in params:
-            params["type"] = params.pop("doc_type")
-
-        return await self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "hot_threads"),
+        return self.transport.perform_request(
+            "POST",
+            _make_path("_ingest", "pipeline", id, "_simulate"),
             params=params,
             headers=headers,
+            body=body,
         )
 
-    @query_params("timeout")
-    async def usage(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def processor_grok(
         self,
-        node_id: Any = None,
-        metric: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns low-level information about REST actions usage on nodes.
+        Returns a list of the built-in patterns.
 
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg metric: Limit the information returned to the specified
-            metrics. Valid choices are _all, rest_actions.
-        :arg timeout: Operation timeout.
-        """
-        return await self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "usage", metric),
-            params=params,
-            headers=headers,
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        """
+        return self.transport.perform_request(
+            "GET", "/_ingest/processor/grok", params=params, headers=headers
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/plugins.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 
 import warnings
 from typing import Any
 
 from ..plugins.alerting import AlertingClient
 from ..plugins.index_management import IndexManagementClient
 from ..plugins.knn import KnnClient
+from ..plugins.notifications import NotificationsClient
+from ..plugins.rollups import RollupsClient
+from ..plugins.transforms import TransformsClient
 from .client import Client
 from .utils import NamespacedClient
 
 
 class PluginsClient(NamespacedClient):
     alerting: Any
     index_management: Any
 
     def __init__(self, client: Client) -> None:
         super(PluginsClient, self).__init__(client)
+        self.transforms = TransformsClient(client)
+        self.rollups = RollupsClient(client)
+        self.notifications = NotificationsClient(client)
         self.knn = KnnClient(client)
         # self.query_workbench = QueryWorkbenchClient(client)
         # self.reporting = ReportingClient(client)
         # self.notebooks = NotebooksClient(client)
         self.alerting = AlertingClient(client)
         # self.anomaly_detection = AnomalyDetectionClient(client)
         # self.trace_analytics = TraceAnalyticsClient(client)
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/remote.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/remote.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/remote_store.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/remote_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,28 +18,46 @@
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, query_params
 
 
 class RemoteStoreClient(NamespacedClient):
-    @query_params("cluster_manager_timeout", "wait_for_completion")
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "wait_for_completion",
+    )
     async def restore(
         self,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Restores from remote store.
 
 
         :arg body: Comma-separated list of index IDs
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg wait_for_completion: Should this request wait until the
             operation has completed before returning. Default is false.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         return await self.transport.perform_request(
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/client/utils.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/compat.py` & `opensearch_py-2.6.0/opensearchpy/helpers/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,28 +21,25 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 
-import asyncio
+from typing import Any, List
 
-from ..compat import *  # noqa
+from ..exceptions import OpenSearchException
 
-# Hack supporting Python 3.6 asyncio which didn't have 'get_running_loop()'.
-# Essentially we want to get away from having users pass in a loop to us.
-# Instead we should call 'get_running_loop()' whenever we need
-# the currently running loop.
-# See: https://aiopg.readthedocs.io/en/stable/run_loop.html#implementation
-try:
-    from asyncio import get_running_loop
-except ImportError:
-
-    def get_running_loop() -> asyncio.AbstractEventLoop:
-        loop = asyncio.get_event_loop()
-        if not loop.is_running():
-            raise RuntimeError("no running event loop")
-        return loop
 
+class BulkIndexError(OpenSearchException):
+    @property
+    def errors(self) -> List[Any]:
+        """List of errors from execution of the last chunk."""
+        return self.args[1]  # type: ignore
 
-__all__ = ["get_running_loop"]
+
+class ScanError(OpenSearchException):
+    scroll_id: str
+
+    def __init__(self, scroll_id: str, *args: Any, **kwargs: Any) -> None:
+        super(ScanError, self).__init__(*args, **kwargs)
+        self.scroll_id = scroll_id
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/actions.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/document.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/document.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/faceted_search.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/index.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/mapping.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/search.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/search.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/test.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/test.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/helpers/update_by_query.py` & `opensearch_py-2.6.0/opensearchpy/_async/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/http_aiohttp.py` & `opensearch_py-2.6.0/opensearchpy/_async/http_aiohttp.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/plugins/alerting.py` & `opensearch_py-2.6.0/opensearchpy/_async/plugins/alerting.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,17 +143,19 @@
         """
         Returns the details of a specific destination.
 
         :arg destination_id: The id of the destination we are trying to fetch. If None, returns all destinations
         """
         return await self.transport.perform_request(
             "GET",
-            _make_path("_plugins", "_alerting", "destinations", destination_id)
-            if destination_id
-            else _make_path("_plugins", "_alerting", "destinations"),
+            (
+                _make_path("_plugins", "_alerting", "destinations", destination_id)
+                if destination_id
+                else _make_path("_plugins", "_alerting", "destinations")
+            ),
             params=params,
             headers=headers,
         )
 
     @query_params()
     async def create_destination(
         self,
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/plugins/index_management.py` & `opensearch_py-2.6.0/opensearchpy/_async/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/plugins/knn.py` & `opensearch_py-2.6.0/opensearchpy/_async/plugins/knn.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,49 +18,69 @@
 
 from typing import Any
 
 from ..client.utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
 class KnnClient(NamespacedClient):
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     async def delete_model(
         self,
         model_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Used to delete a particular model in the cluster.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if model_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'model_id'.")
 
         return await self.transport.perform_request(
             "DELETE",
             _make_path("_plugins", "_knn", "models", model_id),
             params=params,
             headers=headers,
         )
 
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     async def get_model(
         self,
         model_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Used to retrieve information about models present in the cluster.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if model_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'model_id'.")
 
         return await self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", "models", model_id),
@@ -77,32 +97,37 @@
         "analyze_wildcard",
         "analyzer",
         "batched_reduce_size",
         "ccs_minimize_roundtrips",
         "default_operator",
         "df",
         "docvalue_fields",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
         "from_",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "lenient",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
         "preference",
+        "pretty",
         "q",
         "request_cache",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_type",
         "seq_no_primary_term",
         "size",
         "sort",
+        "source",
         "stats",
         "stored_fields",
         "suggest_field",
         "suggest_mode",
         "suggest_size",
         "suggest_text",
         "terminate_after",
@@ -147,20 +172,26 @@
             execution. Default is True.
         :arg default_operator: The default operator for query string
             query (AND or OR). Valid choices are AND, OR.
         :arg df: The field to use as default where no field prefix is
             given in the query string.
         :arg docvalue_fields: Comma-separated list of fields to return
             as the docvalue representation of a field for each hit.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
         :arg explain: Specify whether to return detailed information
             about score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg ignore_throttled: Whether specified concrete, expanded or
             aliased indices should be ignored when throttled.
         :arg ignore_unavailable: Whether specified concrete indices
             should be ignored when unavailable (missing or closed).
         :arg lenient: Specify whether format-based query failures (such
             as providing text to a numeric field) should be ignored.
         :arg max_concurrent_shard_requests: The number of concurrent
@@ -172,14 +203,16 @@
             number of shards the search request expands to exceeds the threshold.
             This filter round-trip can limit the number of shards significantly if
             for instance a shard can not match any documents based on its rewrite
             method ie. if date filters are mandatory to match but the shard bounds
             and the query are disjoint.
         :arg preference: Specify the node or shard the operation should
             be performed on. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
         :arg request_cache: Specify if request cache should be used for
             this request or not, defaults to index level setting.
         :arg rest_total_hits_as_int: Indicates whether hits.total should
             be rendered as an integer or an object in the rest search response.
             Default is false.
         :arg routing: Comma-separated list of specific routing values.
@@ -187,14 +220,16 @@
             should be maintained for scrolled search.
         :arg search_type: Search operation type. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg seq_no_primary_term: Specify whether to return sequence
             number and primary term of the last modification of each hit.
         :arg size: Number of hits to return. Default is 10.
         :arg sort: Comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg stats: Specific 'tag' of the request for logging and
             statistical purposes.
         :arg stored_fields: Comma-separated list of stored fields to
             return.
         :arg suggest_field: Specify which field to use for suggestions.
         :arg suggest_mode: Specify suggest mode. Valid choices are
             missing, popular, always.
@@ -222,15 +257,15 @@
             "POST",
             "/_plugins/_knn/models/_search",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("timeout")
+    @query_params("error_trace", "filter_path", "human", "pretty", "source", "timeout")
     async def stats(
         self,
         node_id: Any = None,
         stat: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
@@ -239,75 +274,97 @@
 
 
         :arg node_id: Comma-separated list of node IDs or names to limit
             the returned information; use `_local` to return information from the
             node you're connecting to, leave empty to get information from all
             nodes.
         :arg stat: Comma-separated list of stats to retrieve; use `_all`
-            or empty string to retrieve all stats. Valid choices are
-            circuit_breaker_triggered, total_load_time, eviction_count, hit_count,
-            miss_count, graph_memory_usage, graph_memory_usage_percentage,
-            graph_index_requests, graph_index_errors, graph_query_requests,
-            graph_query_errors, knn_query_requests, cache_capacity_reached,
-            load_success_count, load_exception_count, indices_in_cache,
-            script_compilations, script_compilation_errors, script_query_requests,
-            script_query_errors, nmslib_initialized, faiss_initialized,
-            model_index_status, indexing_from_model_degraded, training_requests,
-            training_errors, training_memory_usage,
-            training_memory_usage_percentage.
+            or empty string to retrieve all stats.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg timeout: Operation timeout.
         """
         return await self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", node_id, "stats", stat),
             params=params,
             headers=headers,
         )
 
-    @query_params("preference")
+    @query_params(
+        "error_trace", "filter_path", "human", "preference", "pretty", "source"
+    )
     async def train_model(
         self,
         body: Any,
         model_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Create and train a model that can be used for initializing k-NN native library
         indexes during indexing.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg preference: Preferred node to execute training.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         return await self.transport.perform_request(
             "POST",
             _make_path("_plugins", "_knn", "models", model_id, "_train"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     async def warmup(
         self,
         index: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Preloads native library files into memory, reducing initial search latency for
-        specified indexes
+        specified indexes.
 
 
         :arg index: Comma-separated list of indices; use `_all` or empty
             string to perform the operation on all indices.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
         return await self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", "warmup", index),
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_async/transport.py` & `opensearch_py-2.6.0/opensearchpy/_async/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 
 import asyncio
 import logging
-import sys
 from itertools import chain
 from typing import Any, Collection, Mapping, Optional, Type, Union
 
 from opensearchpy.connection.base import Connection
 from opensearchpy.serializer import Serializer
 
 from ..connection_pool import ConnectionPool
@@ -247,21 +246,18 @@
             if conn in self.connection_pool.connections:
                 continue
             tasks.append(_sniff_request(conn))
 
         done: Any = ()
         try:
             while tasks:
-                # The 'loop' keyword is deprecated in 3.8+ so don't
-                # pass it to asyncio.wait() unless we're on <=3.7
-                wait_kwargs = {"loop": self.loop} if sys.version_info < (3, 8) else {}
 
                 # execute sniff requests in parallel, wait for first to return
                 done, tasks = await asyncio.wait(
-                    tasks, return_when=asyncio.FIRST_COMPLETED, **wait_kwargs
+                    tasks, return_when=asyncio.FIRST_COMPLETED
                 )
                 # go through all the finished tasks
                 for t in done:
                     try:
                         _, headers, node_info = t.result()
 
                         # Lowercase all the header names for consistency in accessing them.
```

### Comparing `opensearch-py-2.5.0/opensearchpy/_version.py` & `opensearch_py-2.6.0/opensearchpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-__versionstr__: str = "2.5.0"
+__versionstr__: str = "2.6.0"
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/__init__.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,36 +35,37 @@
 
 
 from __future__ import unicode_literals
 
 import logging
 from typing import Any, Type
 
-from ..transport import Transport, TransportError
+from ..transport import AsyncTransport, TransportError
 from .cat import CatClient
 from .client import Client
 from .cluster import ClusterClient
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .http import HttpClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .plugins import PluginsClient
 from .remote import RemoteClient
 from .remote_store import RemoteStoreClient
+from .search_pipeline import SearchPipelineClient
 from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 from .utils import SKIP_IN_PATH, _bulk_body, _make_path, query_params
 
 logger = logging.getLogger("opensearch")
 
 
-class OpenSearch(Client):
+class AsyncOpenSearch(Client):
     """
     OpenSearch client. Provides a straightforward mapping from
     Python to OpenSearch REST endpoints.
 
     The instance has attributes ``cat``, ``cluster``, ``indices``, ``ingest``,
     ``nodes``, ``snapshot`` and ``tasks`` that provide access to instances of
     :class:`~opensearchpy.client.CatClient`,
@@ -191,15 +192,15 @@
         delete_point_in_time,
         list_all_point_in_time,
     )
 
     def __init__(
         self,
         hosts: Any = None,
-        transport_class: Type[Transport] = Transport,
+        transport_class: Type[AsyncTransport] = AsyncTransport,
         **kwargs: Any
     ) -> None:
         """
         :arg hosts: list of nodes, or a single node, we should connect to.
             Node should be a dictionary ({"host": "localhost", "port": 9200}),
             the entire dictionary will be passed to the :class:`~opensearchpy.Connection`
             class as kwargs, or a string in the format of ``host[:port]`` which will be
@@ -211,14 +212,15 @@
         :arg kwargs: any additional arguments will be passed on to the
             :class:`~opensearchpy.Transport` class and, subsequently, to the
             :class:`~opensearchpy.Connection` instances.
         """
         super().__init__(hosts, transport_class, **kwargs)
 
         # namespaced clients for compatibility with API names
+        self.search_pipeline = SearchPipelineClient(self)
         self.cat = CatClient(self)
         self.cluster = ClusterClient(self)
         self.dangling_indices = DanglingIndicesClient(self)
         self.indices = IndicesClient(self)
         self.ingest = IngestClient(self)
         self.nodes = NodesClient(self)
         self.remote = RemoteClient(self)
@@ -237,1353 +239,1874 @@
             cons: Any = self.transport.hosts
             # truncate to 5 if there are too many
             if len(cons) > 5:
                 cons = cons[:5] + ["..."]
             return "<{cls}({cons})>".format(cls=self.__class__.__name__, cons=cons)
         except Exception:
             # probably operating on custom transport and connection_pool, ignore
-            return super(OpenSearch, self).__repr__()
+            return super(AsyncOpenSearch, self).__repr__()
 
-    def __enter__(self) -> Any:
+    async def __aenter__(self) -> Any:
         if hasattr(self.transport, "_async_call"):
-            self.transport._async_call()
+            await self.transport._async_call()
         return self
 
-    def __exit__(self, *_: Any) -> None:
-        self.close()
+    async def __aexit__(self, *_: Any) -> None:
+        await self.close()
 
-    def close(self) -> None:
+    async def close(self) -> None:
         """Closes the Transport and all internal connections"""
-        self.transport.close()
+        await self.transport.close()
 
     # AUTO-GENERATED-API-DEFINITIONS #
-    @query_params()
-    def ping(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def ping(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns whether the cluster is running.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         try:
-            return self.transport.perform_request(
+            return await self.transport.perform_request(
                 "HEAD", "/", params=params, headers=headers
             )
         except TransportError:
             return False
 
-    @query_params()
-    def info(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def info(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns basic information about the cluster.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", "/", params=params, headers=headers
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "pipeline",
+        "pretty",
         "refresh",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    def create(
+    async def create(
         self,
         index: Any,
         id: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates a new document in the index.  Returns a 409 response when a document
         with a same ID already exists in the index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the data stream or index to target. If the
+            target doesn’t exist and matches the name or wildcard (`*`) pattern of
+            an index template with a `data_stream` definition, this request creates
+            the data stream. If the target doesn’t exist and doesn’t match a data
+            stream template, this request creates the index.
+        :arg id: Unique identifier for the document.
         :arg body: The document
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period the request waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_create", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "PUT", path, params=params, headers=headers, body=body
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
         "op_type",
         "pipeline",
+        "pretty",
         "refresh",
         "require_alias",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    def index(
+    async def index(
         self,
         index: Any,
         body: Any,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates or updates a document in an index.
 
 
-        :arg index: Index name.
+        :arg index: Name of the data stream or index to target.
         :arg body: The document
-        :arg id: Document ID.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
-        :arg op_type: Explicit operation type. Defaults to `index` for
-            requests with an explicit document ID, and to `create` for requests
-            without an explicit document ID. Valid choices are index, create.
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: When true, requires destination to be an
+        :arg id: Unique identifier for the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
+        :arg op_type: Set to create to only index the document if it
+            does not already exist (put if absent).If a document with the specified
+            `_id` already exists, the indexing operation will fail.Same as using the
+            `<index>/_create` endpoint.Valid values: `index`, `create`.If document
+            id is specified, it defaults to `index`.Otherwise, it defaults to
+            `create`.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg require_alias: If `true`, the destination must be an index
             alias. Default is false.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period the request waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST" if id in SKIP_IN_PATH else "PUT",
             _make_path(index, "_doc", id),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "pipeline",
+        "pretty",
         "refresh",
         "require_alias",
         "routing",
+        "source",
         "timeout",
         "wait_for_active_shards",
     )
-    def bulk(
+    async def bulk(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to perform multiple index/update/delete operations in a single request.
 
 
         :arg body: The operation definition and data (action-data
             pairs), separated by newlines
-        :arg index: Default index for items which don't provide one.
-        :arg _source: True or false to return the _source field or not,
-            or default list of fields to return, can be overridden on each sub-
-            request.
-        :arg _source_excludes: Default list of fields to exclude from
-            the returned _source field, can be overridden on each sub-request.
-        :arg _source_includes: Default list of fields to extract and
-            return from the _source field, can be overridden on each sub-request.
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: Sets require_alias for all incoming
-            documents. Default is false.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg index: Name of the data stream, index, or index alias to
+            perform bulk actions on.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg require_alias: If `true`, the request’s actions must target
+            an index alias. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period each action waits for the following
+            operations: automatic index creation, dynamic mapping updates, waiting
+            for active shards.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_bulk"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    def clear_scroll(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def clear_scroll(
         self,
         body: Any = None,
         scroll_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Explicitly clears the search context for a scroll.
 
 
         :arg body: Comma-separated list of scroll IDs to clear if none
             was specified via the scroll_id parameter
-        :arg scroll_id: Comma-separated list of scroll IDs to clear.
+        :arg scroll_id: Comma-separated list of scroll IDs to clear. To
+            clear all scroll IDs, use `_all`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if scroll_id in SKIP_IN_PATH and body in SKIP_IN_PATH:
             raise ValueError("You need to supply scroll_id or body.")
         elif scroll_id and not body:
             body = {"scroll_id": [scroll_id]}
         elif scroll_id:
             params["scroll_id"] = scroll_id
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "DELETE", "/_search/scroll", params=params, headers=headers, body=body
         )
 
     @query_params(
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "lenient",
         "min_score",
         "preference",
+        "pretty",
         "q",
         "routing",
+        "source",
         "terminate_after",
     )
-    def count(
+    async def count(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns number of documents matching a query.
 
 
         :arg body: Query to restrict the results specified with the
             Query DSL (optional)
-        :arg index: Comma-separated list of indices to restrict the
-            results.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*` or `_all`.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed.This parameter can only be used when the `q` query string
+            parameter is specified. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the `q` query string parameter is
+            specified.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg min_score: Include only documents with a specific `_score`
-            value in the result.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+            query: `AND` or `OR`.This parameter can only be used when the `q` query
+            string parameter is specified. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.This parameter can only be used when the `q` query
+            string parameter is specified.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, concrete, expanded or aliased
+            indices are ignored when frozen.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg min_score: Sets the minimum `_score` value that documents
+            must have to be included in the result.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_count"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
+        "pretty",
         "refresh",
         "routing",
+        "source",
         "timeout",
         "version",
         "version_type",
         "wait_for_active_shards",
     )
-    def delete(
+    async def delete(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Removes a document from the index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg index: Name of the target index.
+        :arg id: Unique identifier for the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, Opensearch refreshes the affected
+            shards to make this operation visible to search, if `wait_for` then wait
+            for a refresh to make this operation visible to search, if `false` do
+            nothing with refreshes.Valid values: `true`, `false`, `wait_for`.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for active shards.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "DELETE", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "conflicts",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
         "from_",
+        "human",
         "ignore_unavailable",
         "lenient",
         "max_docs",
         "preference",
+        "pretty",
         "q",
         "refresh",
         "request_cache",
         "requests_per_second",
         "routing",
         "scroll",
         "scroll_size",
         "search_timeout",
         "search_type",
         "size",
         "slices",
         "sort",
+        "source",
         "stats",
         "terminate_after",
         "timeout",
         "version",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    def delete_by_query(
+    async def delete_by_query(
         self,
         index: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes documents matching the provided query.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            or indices, omit this parameter or use `*` or `_all`.
         :arg body: The search definition using the Query DSL
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
         :arg _source_excludes: List of fields to exclude from the
             returned _source field.
         :arg _source_includes: List of fields to extract and return from
             the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
-        :arg conflicts: What to do when the operation encounters version
-            conflicts?. Valid choices are abort, proceed.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.
+        :arg conflicts: What to do if delete by query hits version
+            conflicts: `abort` or `proceed`. Valid choices are abort, proceed.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid values are: `all`,
+            `open`, `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg max_docs: Maximum number of documents to process.Defaults
+            to all documents.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg request_cache: If `true`, the request cache is used for
+            this request.Defaults to the index-level setting.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg scroll_size: Size on the scroll request powering the
+            requests per second. Default is 0.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg scroll_size: Size of the scroll request that powers the
             operation. Default is 100.
-        :arg search_timeout: Explicit timeout for each search request.
-            Defaults to no timeout.
-        :arg search_type: Search operation type. Valid choices are
+        :arg search_timeout: Explicit timeout for each search
+            request.Defaults to no timeout.
+        :arg search_type: The type of the search operation.Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg size: Deprecated, please use `max_docs` instead.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+            into. Valid choices are auto.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg version: Whether to return document version as part of a
-            hit.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.
+        :arg timeout: Period each deletion request waits for active
+            shards.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to all or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
         for param in (index, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_delete_by_query"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("requests_per_second")
-    def delete_by_query_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    async def delete_by_query_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Delete By Query
         operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: The ID for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path("_delete_by_query", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    def delete_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def delete_script(
         self,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
         """
         if id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "DELETE", _make_path("_scripts", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
         "version",
         "version_type",
     )
-    def exists(
+    async def exists(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about whether a document exists in an index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases. Supports wildcards (`*`).
+        :arg id: Identifier of the document.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: List of stored fields to return as part of a
+            hit.If no fields are specified, no stored fields are included in the
+            response.If this field is specified, the `_source` parameter defaults to
+            false.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "HEAD", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "version",
         "version_type",
     )
-    def exists_source(
+    async def exists_source(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about whether a document source exists in an index.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases. Supports wildcards (`*`).
+        :arg id: Identifier of the document.
+        :arg _source: `true` or `false` to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, Opensearch refreshes all shards
+            involved in the delete by query after the request completes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg version: Explicit version number for concurrency
+            control.The specified version must match the current version of the
+            document for the request to succeed.
+        :arg version_type: Specific version type: `external`,
+            `external_gte`. Valid choices are internal, external, external_gte,
+            force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_source", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "HEAD", path, params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "analyze_wildcard",
         "analyzer",
         "default_operator",
         "df",
+        "error_trace",
+        "filter_path",
+        "human",
         "lenient",
         "preference",
+        "pretty",
         "q",
         "routing",
+        "source",
         "stored_fields",
     )
-    def explain(
+    async def explain(
         self,
         index: Any,
         id: Any,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about why a specific matches (or doesn't match) a query.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Index names used to limit the request. Only a single
+            index name can be provided to this parameter.
+        :arg id: Defines the document ID.
         :arg body: The query definition using the Query DSL
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg analyze_wildcard: Specify whether wildcards and prefix
-            queries in the query string query should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg _source: True or false to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the `q` query string parameter is
+            specified.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The default field for query string query. Default is
-            _all.
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string. Default is _all.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: A comma-separated list of stored fields to
+            return in the response.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_explain", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "allow_no_indices",
+        "error_trace",
         "expand_wildcards",
         "fields",
+        "filter_path",
+        "human",
         "ignore_unavailable",
         "include_unmapped",
+        "pretty",
+        "source",
     )
-    def field_caps(
+    async def field_caps(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns the information about the capabilities of fields among multiple
         indices.
 
 
         :arg body: An index filter specified with the Query DSL
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg fields: Comma-separated list of field names.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg include_unmapped: Indicates whether unmapped fields should
-            be included in the response. Default is false.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases used to limit the request. Supports wildcards (*). To target all
+            data streams and indices, omit this parameter or use * or _all.
+        :arg allow_no_indices: If false, the request returns an error if
+            any wildcard expression, index alias,or `_all` value targets only
+            missing or closed indices. This behavior applies even if the request
+            targets other open indices. For example, a requesttargeting `foo*,bar*`
+            returns an error if an index starts with foo but no index starts with
+            bar.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match. If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams. Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg fields: Comma-separated list of fields to retrieve
+            capabilities for. Wildcard (`*`) expressions are supported.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `true`, missing or closed indices
+            are not included in the response.
+        :arg include_unmapped: If true, unmapped fields are included in
+            the response. Default is false.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_field_caps"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
         "version",
         "version_type",
     )
-    def get(
+    async def get(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns a document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the index that contains the document.
+        :arg id: Unique identifier of the document.
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If true, Opensearch refreshes the affected shards
+            to make this operation visible to search. If false, do nothing with
+            refreshes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: List of stored fields to return as part of a
+            hit.If no fields are specified, no stored fields are included in the
+            response.If this field is specified, the `_source` parameter defaults to
+            false.
         :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+            The specified version must match the current version of the document for
+            the request to succeed.
+        :arg version_type: Specific version type: internal, external,
+            external_gte. Valid choices are internal, external, external_gte, force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", _make_path(index, "_doc", id), params=params, headers=headers
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout")
-    def get_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+    )
+    async def get_script(
         self,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", _make_path("_scripts", id), params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "version",
         "version_type",
     )
-    def get_source(
+    async def get_source(
         self,
         index: Any,
         id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns the source of a document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: Name of the index that contains the document.
+        :arg id: Unique identifier of the document.
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude in the response.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: Boolean) If true, the request is real-time as
+            opposed to near-real-time.
+        :arg refresh: If true, Opensearch refreshes the affected shards
+            to make this operation visible to search. If false, do nothing with
+            refreshes.
+        :arg routing: Target the specified primary shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg version: Explicit version number for concurrency control.
-        :arg version_type: Specific version type. Valid choices are
-            internal, external, external_gte, force.
+            The specified version must match the current version of the document for
+            the request to succeed.
+        :arg version_type: Specific version type: internal, external,
+            external_gte. Valid choices are internal, external, external_gte, force.
         """
         for param in (index, id):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_source", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", path, params=params, headers=headers
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "preference",
+        "pretty",
         "realtime",
         "refresh",
         "routing",
+        "source",
         "stored_fields",
     )
-    def mget(
+    async def mget(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to get multiple documents in one request.
 
 
         :arg body: Document identifiers; can be either `docs`
             (containing full document information) or `ids` (when index is provided
             in the URL.
-        :arg index: Index name.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specify whether to perform the operation in
-            realtime or search mode.
-        :arg refresh: Refresh the shard containing the document before
-            performing the operation.
-        :arg routing: Routing value.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
+        :arg index: Name of the index to retrieve documents from when
+            `ids` are specified, or when a document in the `docs` array does not
+            specify an index.
+        :arg _source: True or false to return the `_source` field or
+            not, or a list of fields to return.
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.You can also use this parameter to exclude
+            fields from the subset specified in `_source_includes` query parameter.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.If this parameter is specified, only these
+            source fields are returned. You can exclude fields from this subset
+            using the `_source_excludes` query parameter.If the `_source` parameter
+            is `false`, this parameter is ignored.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on. Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If `true`, the request is real-time as opposed to
+            near-real-time.
+        :arg refresh: If `true`, the request refreshes relevant shards
+            before retrieving documents.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stored_fields: If `true`, retrieves the document fields
+            stored in the index rather than the document `_source`.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_mget"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "ccs_minimize_roundtrips",
+        "error_trace",
+        "filter_path",
+        "human",
         "max_concurrent_searches",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
+        "pretty",
         "rest_total_hits_as_int",
         "search_type",
+        "source",
         "typed_keys",
     )
-    def msearch(
+    async def msearch(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to execute several search operations in one request.
 
 
         :arg body: The request definitions (metadata-search request
             definition pairs), separated by newlines
-        :arg index: Comma-separated list of indices to use as default.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg max_concurrent_searches: Controls the maximum number of
-            concurrent searches the multi search api will execute.
-        :arg max_concurrent_shard_requests: The number of concurrent
-            shard requests each sub search executes concurrently per node. This
-            value should be used to limit the impact of the search on the cluster in
-            order to limit the number of concurrent shard requests. Default is 5.
-        :arg pre_filter_shard_size: Threshold that enforces a pre-filter
-            round-trip to prefilter search shards based on query rewriting if the
-            number of shards the search request expands to exceeds the threshold.
-            This filter round-trip can limit the number of shards significantly if
-            for instance a shard can not match any documents based on its rewrite
-            method ie. if date filters are mandatory to match but the shard bounds
-            and the query are disjoint.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
+        :arg index: Comma-separated list of data streams, indices, and
+            index aliases to search.
+        :arg ccs_minimize_roundtrips: If true, network roundtrips
+            between the coordinating node and remote clusters are minimized for
+            cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_concurrent_searches: Maximum number of concurrent
+            searches the multi search API can execute.
+        :arg max_concurrent_shard_requests: Maximum number of concurrent
+            shard requests that each sub-search request executes per node. Default
+            is 5.
+        :arg pre_filter_shard_size: Defines a threshold that enforces a
+            pre-filter roundtrip to prefilter search shards based on query rewriting
+            if the number of shards the search request expands to exceeds the
+            threshold. This filter roundtrip can limit the number of shards
+            significantly if for instance a shard can not match any documents based
+            on its rewrite method i.e., if date filters are mandatory to match but
+            the shard bounds and the query are disjoint.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If true, hits.total are returned as
+            an integer in the response. Defaults to false, which returns an object.
             Default is false.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg search_type: Indicates whether global term and document
+            frequencies should be used when scoring returned documents. Valid
+            choices are query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: Specifies whether aggregation and suggester
+            names should be prefixed by their respective types in the response.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_msearch"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "ccs_minimize_roundtrips",
+        "error_trace",
+        "filter_path",
+        "human",
         "max_concurrent_searches",
+        "pretty",
         "rest_total_hits_as_int",
         "search_type",
+        "source",
         "typed_keys",
     )
-    def msearch_template(
+    async def msearch_template(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to execute several search template operations in one request.
 
 
         :arg body: The request definitions (metadata-search request
             definition pairs), separated by newlines
-        :arg index: Comma-separated list of indices to use as default.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg max_concurrent_searches: Controls the maximum number of
-            concurrent searches the multi search api will execute.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*`.
+        :arg ccs_minimize_roundtrips: If `true`, network round-trips are
+            minimized for cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_concurrent_searches: Maximum number of concurrent
+            searches the API can run.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If `true`, the response returns
+            `hits.total` as an integer.If `false`, it returns `hits.total` as an
+            object. Default is false.
+        :arg search_type: The type of the search operation.Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
+            query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: If `true`, the response prefixes aggregation
+            and suggester names with their respective types.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         body = _bulk_body(self.transport.serializer, body)
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_msearch", "template"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
         "field_statistics",
         "fields",
+        "filter_path",
+        "human",
         "ids",
         "offsets",
         "payloads",
         "positions",
         "preference",
+        "pretty",
         "realtime",
         "routing",
+        "source",
         "term_statistics",
         "version",
         "version_type",
     )
-    def mtermvectors(
+    async def mtermvectors(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns multiple termvectors in one request.
 
 
         :arg body: Define ids, documents, parameters or a list of
             parameters per document here. You must at least provide a list of
             document ids. See documentation.
-        :arg index: The index in which the document resides.
-        :arg field_statistics: Specifies if document count, sum of
-            document frequencies and sum of total term frequencies should be
-            returned. Applies to all returned documents unless otherwise specified
-            in body 'params' or 'docs'. Default is True.
-        :arg fields: Comma-separated list of fields to return. Applies
-            to all returned documents unless otherwise specified in body 'params' or
-            'docs'.
-        :arg ids: Comma-separated list of documents ids. You must define
-            ids as parameter or set 'ids' or 'docs' in the request body.
-        :arg offsets: Specifies if term offsets should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg payloads: Specifies if term payloads should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg positions: Specifies if term positions should be returned.
-            Applies to all returned documents unless otherwise specified in body
-            'params' or 'docs'. Default is True.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Applies to all returned documents unless otherwise
-            specified in body 'params' or 'docs'. Default is random.
-        :arg realtime: Specifies if requests are real-time as opposed to
+        :arg index: Name of the index that contains the documents.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg field_statistics: If `true`, the response includes the
+            document count, sum of document frequencies, and sum of total term
+            frequencies. Default is True.
+        :arg fields: Comma-separated list or wildcard expressions of
+            fields to include in the statistics.Used as the default list unless a
+            specific field list is provided in the `completion_fields` or
+            `fielddata_fields` parameters.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ids: A comma-separated list of documents ids. You must
+            define ids as parameter or set "ids" or "docs" in the request body
+        :arg offsets: If `true`, the response includes term offsets.
+            Default is True.
+        :arg payloads: If `true`, the response includes term payloads.
+            Default is True.
+        :arg positions: If `true`, the response includes term positions.
+            Default is True.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
             near-real-time. Default is True.
-        :arg routing: Routing value. Applies to all returned documents
-            unless otherwise specified in body 'params' or 'docs'.
-        :arg term_statistics: Specifies if total term frequency and
-            document frequency should be returned. Applies to all returned documents
-            unless otherwise specified in body 'params' or 'docs'. Default is false.
-        :arg version: Explicit version number for concurrency control.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg term_statistics: If true, the response includes term
+            frequency and document frequency. Default is false.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
         :arg version_type: Specific version type. Valid choices are
             internal, external, external_gte, force.
         """
         path = _make_path(index, "_mtermvectors")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    def put_script(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def put_script(
         self,
         id: Any,
         body: Any,
         context: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates or updates a script.
 
 
-        :arg id: Script ID.
+        :arg id: Identifier for the stored script or search template.
+            Must be unique within the cluster.
         :arg body: The document
-        :arg context: Script context.
+        :arg context: Context in which the script or search template
+            should run. To prevent errors, the API immediately compiles the script
+            or template in this context.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Period to wait for a connection
+            to the master node.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
         """
         for param in (id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "PUT",
             _make_path("_scripts", id, context),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
-        "allow_no_indices", "expand_wildcards", "ignore_unavailable", "search_type"
+        "allow_no_indices",
+        "error_trace",
+        "expand_wildcards",
+        "filter_path",
+        "human",
+        "ignore_unavailable",
+        "pretty",
+        "search_type",
+        "source",
     )
-    def rank_eval(
+    async def rank_eval(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to evaluate the quality of ranked search results over a set of typical
         search queries.
 
 
         :arg body: The ranking evaluation search definition, including
             search requests, document ratings and ranking metric definition.
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
+        :arg index: Comma-separated list of data streams, indices, and
+            index aliases used to limit the request. Wildcard (`*`) expressions are
+            supported. To target all data streams and indices in a cluster, omit
+            this parameter or use `_all` or `*`.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices. This behavior applies even if the request
+            targets other open indices. For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, dfs_query_then_fetch.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `true`, missing or closed indices
+            are not included in the response.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg search_type: Search operation type
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_rank_eval"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
         "max_docs",
+        "pretty",
         "refresh",
         "requests_per_second",
         "scroll",
         "slices",
+        "source",
         "timeout",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    def reindex(
+    async def reindex(
         self,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to copy documents from one index to another, optionally filtering the
         source documents by a query, changing the destination index settings, or
         fetching the documents from a remote cluster.
 
 
         :arg body: The search definition using the Query DSL and the
             prototype for the index request.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg refresh: Should the affected indexes be refreshed?.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg max_docs: Maximum number of documents to process. By
+            default, all documents.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If `true`, the request refreshes affected shards
+            to make this operation visible to search.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg scroll: Specify how long a consistent view of the index
+            requests per second.Defaults to no throttle. Default is 0.
+        :arg scroll: Specifies how long a consistent view of the index
             should be maintained for scrolled search.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+            into.Defaults to 1 slice, meaning the task isn’t sliced into subtasks.
+            Valid choices are auto.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period each indexing waits for automatic index
+            creation, dynamic mapping updates, and waiting for active shards.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", "/_reindex", params=params, headers=headers, body=body
         )
 
-    @query_params("requests_per_second")
-    def reindex_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    async def reindex_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Reindex operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: Identifier for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path("_reindex", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    def render_search_template(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def render_search_template(
         self,
         body: Any = None,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to use the Mustache language to pre-render a search definition.
 
 
         :arg body: The search definition template and its params
-        :arg id: The id of the stored search template.
+        :arg id: ID of the search template to render. If no `source` is
+            specified, this or the `id` request body parameter is required.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path("_render", "template", id),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    def scripts_painless_execute(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def scripts_painless_execute(
         self,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows an arbitrary script to be executed and a result to be returned.
 
 
         :arg body: The script to execute
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             "/_scripts/painless/_execute",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("rest_total_hits_as_int", "scroll")
-    def scroll(
+    @query_params(
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "rest_total_hits_as_int",
+        "scroll",
+        "source",
+    )
+    async def scroll(
         self,
         body: Any = None,
         scroll_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to retrieve a large numbers of results from a single search request.
 
 
         :arg body: The scroll ID if not passed by URL or query
             parameter.
-        :arg scroll_id: Scroll ID.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
+        :arg scroll_id: The scroll ID for scrolled search
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg rest_total_hits_as_int: If true, the API response’s
+            hit.total property is returned as an integer. If false, the API
+            response’s hit.total property is returned as an object. Default is
+            false.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if scroll_id in SKIP_IN_PATH and body in SKIP_IN_PATH:
             raise ValueError("You need to supply scroll_id or body.")
         elif scroll_id and not body:
             body = {"scroll_id": scroll_id}
         elif scroll_id:
             params["scroll_id"] = scroll_id
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", "/_search/scroll", params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
@@ -1592,677 +2115,950 @@
         "analyze_wildcard",
         "analyzer",
         "batched_reduce_size",
         "ccs_minimize_roundtrips",
         "default_operator",
         "df",
         "docvalue_fields",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
         "from_",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "include_named_queries_score",
         "lenient",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
         "preference",
+        "pretty",
         "q",
         "request_cache",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_pipeline",
         "search_type",
         "seq_no_primary_term",
         "size",
         "sort",
+        "source",
         "stats",
         "stored_fields",
         "suggest_field",
         "suggest_mode",
         "suggest_size",
         "suggest_text",
         "terminate_after",
         "timeout",
         "track_scores",
         "track_total_hits",
         "typed_keys",
         "version",
     )
-    def search(
+    async def search(
         self,
         body: Any = None,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns results matching a query.
 
 
         :arg body: The search definition using the Query DSL
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg allow_partial_search_results: Indicate if an error should
-            be returned if there is a partial search failure or timeout. Default is
-            True.
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            and indices, omit this parameter or use `*` or `_all`.
+        :arg _source: Indicates which source fields are returned for
+            matching documents.These fields are returned in the `hits._source`
+            property of the search response.Valid values are:`true` to return the
+            entire document source;`false` to not return the document
+            source;`<string>` to return the source fields that are specified as a
+            comma-separated list (supports wildcard (`*`) patterns).
+        :arg _source_excludes: A comma-separated list of source fields
+            to exclude from the response.You can also use this parameter to exclude
+            fields from the subset specified in `_source_includes` query
+            parameter.If the `_source` parameter is `false`, this parameter is
+            ignored.
+        :arg _source_includes: A comma-separated list of source fields
+            to include in the response.If this parameter is specified, only these
+            source fields are returned.You can exclude fields from this subset using
+            the `_source_excludes` query parameter.If the `_source` parameter is
+            `false`, this parameter is ignored.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg allow_partial_search_results: If true, returns partial
+            results if there are shard request timeouts or shard failures. If false,
+            returns an error with no partial results. Default is True.
+        :arg analyze_wildcard: If true, wildcard and prefix queries are
+            analyzed.This parameter can only be used when the q query string
+            parameter is specified. Default is false.
+        :arg analyzer: Analyzer to use for the query string.This
+            parameter can only be used when the q query string parameter is
+            specified.
         :arg batched_reduce_size: The number of shard results that
-            should be reduced at once on the coordinating node. This value should be
+            should be reduced at once on the coordinating node.This value should be
             used as a protection mechanism to reduce the memory overhead per search
             request if the potential number of shards in the request can be large.
             Default is 512.
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
+        :arg ccs_minimize_roundtrips: If true, network round-trips
+            between the coordinating node and the remote clusters are minimized when
+            executing cross-cluster search (CCS) requests. Default is True.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg docvalue_fields: Comma-separated list of fields to return
-            as the docvalue representation of a field for each hit.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg explain: Specify whether to return detailed information
-            about score computation as part of a hit.
-        :arg from_: Starting offset. Default is 0.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
+            query: AND or OR.This parameter can only be used when the `q` query
+            string parameter is specified. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.This parameter can only be used when the q query
+            string parameter is specified.
+        :arg docvalue_fields: A comma-separated list of fields to return
+            as the docvalue representation for each hit.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`. Valid choices are all, open,
+            closed, hidden, none.
+        :arg explain: If `true`, returns detailed information about
+            score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg from_: Starting document offset.Needs to be non-negative.By
+            default, you cannot page through more than 10,000 hits using the `from`
+            and `size` parameters.To page through more hits, use the `search_after`
+            parameter. Default is 0.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, concrete, expanded or aliased
+            indices will be ignored when frozen.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
         :arg include_named_queries_score: Indicates whether
             hit.matched_queries should be rendered as a map that includes the name
             of the matched query associated with its score (true) or as an array
             containing the name of the matched queries (false) Default is false.
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_concurrent_shard_requests: The number of concurrent
-            shard requests per node this search executes concurrently. This value
-            should be used to limit the impact of the search on the cluster in order
-            to limit the number of concurrent shard requests. Default is 5.
-        :arg pre_filter_shard_size: Threshold that enforces a pre-filter
-            round-trip to prefilter search shards based on query rewriting if the
-            number of shards the search request expands to exceeds the threshold.
-            This filter round-trip can limit the number of shards significantly if
-            for instance a shard can not match any documents based on its rewrite
-            method ie. if date filters are mandatory to match but the shard bounds
-            and the query are disjoint.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg q: Query in the Lucene query string syntax.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be
+            ignored.This parameter can only be used when the `q` query string
+            parameter is specified.
+        :arg max_concurrent_shard_requests: Defines the number of
+            concurrent shard requests per node this search executes
+            concurrently.This value should be used to limit the impact of the search
+            on the cluster in order to limit the number of concurrent shard
+            requests. Default is 5.
+        :arg pre_filter_shard_size: Defines a threshold that enforces a
+            pre-filter roundtrip to prefilter search shards based on query rewriting
+            if the number of shards the search request expands to exceeds the
+            threshold.This filter roundtrip can limit the number of shards
+            significantly if for instance a shard can not match any documents based
+            on its rewrite method (if date filters are mandatory to match but the
+            shard bounds and the query are disjoint).When unspecified, the pre-
+            filter phase is executed if any of these conditions is met:the request
+            targets more than 128 shards;the request targets one or more read-only
+            index;the primary sort of the query targets an indexed field.
+        :arg preference: Nodes and shards used for the search.By
+            default, Opensearch selects from eligible nodes and shards using
+            adaptive replica selection, accounting for allocation awareness. Valid
+            values are:`_only_local` to run the search only on shards on the local
+            node;`_local` to, if possible, run the search on shards on the local
+            node, or if not, select shards using the default
+            method;`_only_nodes:<node-id>,<node-id>` to run the search on only the
+            specified nodes IDs, where, if suitable shards exist on more than one
+            selected node, use shards on those nodes using the default method, or if
+            none of the specified nodes are available, select shards from any
+            available node using the default method;`_prefer_nodes:<node-id>,<node-
+            id>` to if possible, run the search on the specified nodes IDs, or if
+            not, select shards using the default method;`_shards:<shard>,<shard>` to
+            run the search only on the specified shards;`<custom-string>` (any
+            string that does not start with `_`) to route searches with the same
+            `<custom-string>` to the same shards in the same order. Default is
+            random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg q: Query in the Lucene query string syntax using query
+            parameter search.Query parameter searches do not support the full
+            Opensearch Query DSL but are handy for testing.
+        :arg request_cache: If `true`, the caching of search results is
+            enabled for requests where `size` is `0`.Defaults to index level
+            settings.
+        :arg rest_total_hits_as_int: Indicates whether `hits.total`
+            should be rendered as an integer or an object in the rest search
+            response. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+            See Scroll search results.By default, this value cannot exceed `1d` (24
+            hours).You can change this limit using the `search.max_keep_alive`
+            cluster-level setting.
         :arg search_pipeline: Customizable sequence of processing stages
             applied to search queries.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, dfs_query_then_fetch.
-        :arg seq_no_primary_term: Specify whether to return sequence
-            number and primary term of the last modification of each hit.
-        :arg size: Number of hits to return. Default is 10.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+        :arg search_type: How distributed term frequencies are
+            calculated for relevance scoring. Valid choices are query_then_fetch,
+            dfs_query_then_fetch.
+        :arg seq_no_primary_term: If `true`, returns sequence number and
+            primary term of the last modification of each hit.
+        :arg size: Defines the number of hits to return.By default, you
+            cannot page through more than 10,000 hits using the `from` and `size`
+            parameters.To page through more hits, use the `search_after` parameter.
+            Default is 10.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg stored_fields: Comma-separated list of stored fields to
-            return.
-        :arg suggest_field: Specify which field to use for suggestions.
-        :arg suggest_mode: Specify suggest mode. Valid choices are
-            missing, popular, always.
-        :arg suggest_size: How many suggestions to return in response.
+        :arg stored_fields: A comma-separated list of stored fields to
+            return as part of a hit.If no fields are specified, no stored fields are
+            included in the response.If this field is specified, the `_source`
+            parameter defaults to `false`.You can pass `_source: true` to return
+            both source fields and stored fields in the search response.
+        :arg suggest_field: Specifies which field to use for
+            suggestions.
+        :arg suggest_mode: Specifies the suggest mode.This parameter can
+            only be used when the `suggest_field` and `suggest_text` query string
+            parameters are specified. Valid choices are missing, popular, always.
+        :arg suggest_size: Number of suggestions to return.This
+            parameter can only be used when the `suggest_field` and `suggest_text`
+            query string parameters are specified.
         :arg suggest_text: The source text for which the suggestions
-            should be returned.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Operation timeout.
-        :arg track_scores: Whether to calculate and return scores even
-            if they are not used for sorting.
-        :arg track_total_hits: Indicate if the number of documents that
-            match the query should be tracked.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
-        :arg version: Whether to return document version as part of a
+            should be returned.This parameter can only be used when the
+            `suggest_field` and `suggest_text` query string parameters are
+            specified.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.If set to
+            `0` (default), the query does not terminate early.
+        :arg timeout: Specifies the period of time to wait for a
+            response from each shard.If no response is received before the timeout
+            expires, the request fails and returns an error.
+        :arg track_scores: If `true`, calculate and return document
+            scores, even if the scores are not used for sorting.
+        :arg track_total_hits: Number of hits matching the query to
+            count accurately.If `true`, the exact number of hits is returned at the
+            cost of some performance.If `false`, the response does not include the
+            total number of hits matching the query.
+        :arg typed_keys: If `true`, aggregation and suggester names are
+            be prefixed by their respective types in the response.
+        :arg version: If `true`, returns document version as part of a
             hit.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_search"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
         "allow_no_indices",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "ignore_unavailable",
         "local",
         "preference",
+        "pretty",
         "routing",
+        "source",
     )
-    def search_shards(
+    async def search_shards(
         self,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information about the indices and shards that a search request would be
         executed against.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg local: Return local information, do not retrieve the state
-            from cluster-manager node. Default is false.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg routing: Routing value.
+        :arg index: Returns the indices and shards that a search request
+            would be executed against.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg local: If `true`, the request retrieves information from
+            the local node only. Default is false.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", _make_path(index, "_search_shards"), params=params, headers=headers
         )
 
     @query_params(
         "allow_no_indices",
         "ccs_minimize_roundtrips",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "preference",
+        "pretty",
         "profile",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_type",
+        "source",
         "typed_keys",
     )
-    def search_template(
+    async def search_template(
         self,
         body: Any,
         index: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Allows to use the Mustache language to pre-render a search definition.
 
 
         :arg body: The search definition template and its params
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg ccs_minimize_roundtrips: Indicates whether network round-
-            trips should be minimized as part of cross-cluster search requests
-            execution. Default is True.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
-        :arg explain: Specify whether to return detailed information
-            about score computation as part of a hit.
-        :arg ignore_throttled: Whether specified concrete, expanded or
-            aliased indices should be ignored when throttled.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg profile: Specify whether to profile the query execution.
-        :arg rest_total_hits_as_int: Indicates whether hits.total should
-            be rendered as an integer or an object in the rest search response.
-            Default is false.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg search_type: Search operation type. Valid choices are
-            query_then_fetch, query_and_fetch, dfs_query_then_fetch,
-            dfs_query_and_fetch.
-        :arg typed_keys: Specify whether aggregation and suggester names
-            should be prefixed by their respective types in the response.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (*).
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg ccs_minimize_roundtrips: If `true`, network round-trips are
+            minimized for cross-cluster search requests. Default is True.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg explain: If `true`, the response includes additional
+            details about score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_throttled: If `true`, specified concrete, expanded,
+            or aliased indices are not included in the response when throttled.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg profile: If `true`, the query execution is profiled.
+        :arg rest_total_hits_as_int: If true, hits.total are rendered as
+            an integer in the response. Default is false.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Specifies how long a consistent view of the
+            indexshould be maintained for scrolled search.
+        :arg search_type: The type of the search operation. Valid
+            choices are query_then_fetch, dfs_query_then_fetch.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg typed_keys: If `true`, the response prefixes aggregation
+            and suggester names with their respective types.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_search", "template"),
             params=params,
             headers=headers,
             body=body,
         )
 
     @query_params(
+        "error_trace",
         "field_statistics",
         "fields",
+        "filter_path",
+        "human",
         "offsets",
         "payloads",
         "positions",
         "preference",
+        "pretty",
         "realtime",
         "routing",
+        "source",
         "term_statistics",
         "version",
         "version_type",
     )
-    def termvectors(
+    async def termvectors(
         self,
         index: Any,
         body: Any = None,
         id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns information and statistics about terms in the fields of a particular
         document.
 
 
-        :arg index: The index in which the document resides.
+        :arg index: Name of the index that contains the document.
         :arg body: Define parameters and or supply a document to get
             termvectors for. See documentation.
-        :arg id: Document ID. When not specified a doc param should be
-            supplied.
-        :arg field_statistics: Specifies if document count, sum of
-            document frequencies and sum of total term frequencies should be
-            returned. Default is True.
-        :arg fields: Comma-separated list of fields to return.
-        :arg offsets: Specifies if term offsets should be returned.
+        :arg id: Unique identifier of the document.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg field_statistics: If `true`, the response includes the
+            document count, sum of document frequencies, and sum of total term
+            frequencies. Default is True.
+        :arg fields: Comma-separated list or wildcard expressions of
+            fields to include in the statistics.Used as the default list unless a
+            specific field list is provided in the `completion_fields` or
+            `fielddata_fields` parameters.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg offsets: If `true`, the response includes term offsets.
             Default is True.
-        :arg payloads: Specifies if term payloads should be returned.
+        :arg payloads: If `true`, the response includes term payloads.
             Default is True.
-        :arg positions: Specifies if term positions should be returned.
+        :arg positions: If `true`, the response includes term positions.
             Default is True.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
-        :arg realtime: Specifies if request is real-time as opposed to
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg realtime: If true, the request is real-time as opposed to
             near-real-time. Default is True.
-        :arg routing: Routing value.
-        :arg term_statistics: Specifies if total term frequency and
-            document frequency should be returned. Default is false.
-        :arg version: Explicit version number for concurrency control.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg term_statistics: If `true`, the response includes term
+            frequency and document frequency. Default is false.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
         :arg version_type: Specific version type. Valid choices are
             internal, external, external_gte, force.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
         path = _make_path(index, "_termvectors", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
+        "error_trace",
+        "filter_path",
+        "human",
         "if_primary_term",
         "if_seq_no",
         "lang",
+        "pretty",
         "refresh",
         "require_alias",
         "retry_on_conflict",
         "routing",
+        "source",
         "timeout",
         "wait_for_active_shards",
     )
-    def update(
+    async def update(
         self,
         index: Any,
         id: Any,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Updates a document with a script or partial document.
 
 
-        :arg index: Index name.
-        :arg id: Document ID.
+        :arg index: The name of the index
+        :arg id: Document ID
         :arg body: The request definition requires either `script` or
             partial `doc`
-        :arg _source: True or false to return the _source field or not,
-            or a list of fields to return.
-        :arg _source_excludes: List of fields to exclude from the
-            returned _source field.
-        :arg _source_includes: List of fields to extract and return from
-            the _source field.
-        :arg if_primary_term: only perform the operation if the last
-            operation that has changed the document has the specified primary term.
-        :arg if_seq_no: only perform the operation if the last operation
-            that has changed the document has the specified sequence number.
+        :arg _source: Set to false to disable source retrieval. You can
+            also specify a comma-separatedlist of the fields you want to retrieve.
+        :arg _source_excludes: Specify the source fields you want to
+            exclude.
+        :arg _source_includes: Specify the source fields you want to
+            retrieve.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg if_primary_term: Only perform the operation if the document
+            has this primary term.
+        :arg if_seq_no: Only perform the operation if the document has
+            this sequence number.
         :arg lang: The script language. Default is painless.
-        :arg refresh: If `true` then refresh the affected shards to make
-            this operation visible to search, if `wait_for` then wait for a refresh
-            to make this operation visible to search, if `false` (the default) then
-            do nothing with refreshes. Valid choices are true, false, wait_for.
-        :arg require_alias: When true, requires destination to be an
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg refresh: If 'true', Opensearch refreshes the affected
+            shards to make this operationvisible to search, if 'wait_for' then wait
+            for a refresh to make this operationvisible to search, if 'false' do
+            nothing with refreshes. Valid choices are true, false, wait_for.
+        :arg require_alias: If true, the destination must be an index
             alias. Default is false.
         :arg retry_on_conflict: Specify how many times should the
             operation be retried when a conflict occurs. Default is 0.
-        :arg routing: Routing value.
-        :arg timeout: Operation timeout.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for dynamic mapping updates and
+            active shards.This guarantees Opensearch waits for at least the timeout
+            before failing.The actual wait time could be longer, particularly when
+            multiple waits occur.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operations.Set to 'all' or any
+            positive integer up to the total number of shards in the
+            index(number_of_replicas+1). Defaults to 1 meaning the primary shard.
+            Valid choices are all, index-setting.
         """
         for param in (index, id, body):
             if param in SKIP_IN_PATH:
                 raise ValueError("Empty value passed for a required argument.")
 
         path = _make_path(index, "_update", id)
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST", path, params=params, headers=headers, body=body
         )
 
     @query_params(
         "_source",
         "_source_excludes",
         "_source_includes",
         "allow_no_indices",
         "analyze_wildcard",
         "analyzer",
         "conflicts",
         "default_operator",
         "df",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
         "from_",
+        "human",
         "ignore_unavailable",
         "lenient",
         "max_docs",
         "pipeline",
         "preference",
+        "pretty",
         "q",
         "refresh",
         "request_cache",
         "requests_per_second",
         "routing",
         "scroll",
         "scroll_size",
         "search_timeout",
         "search_type",
         "size",
         "slices",
         "sort",
+        "source",
         "stats",
         "terminate_after",
         "timeout",
         "version",
         "wait_for_active_shards",
         "wait_for_completion",
     )
-    def update_by_query(
+    async def update_by_query(
         self,
         index: Any,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Performs an update on every document in the index without changing the source,
         for example to pick up a mapping change.
 
 
-        :arg index: Comma-separated list of indices; use `_all` or empty
-            string to perform the operation on all indices.
+        :arg index: Comma-separated list of data streams, indices, and
+            aliases to search. Supports wildcards (`*`). To search all data streams
+            or indices, omit this parameter or use `*` or `_all`.
         :arg body: The search definition using the Query DSL
         :arg _source: True or false to return the _source field or not,
             or a list of fields to return.
         :arg _source_excludes: List of fields to exclude from the
             returned _source field.
         :arg _source_includes: List of fields to extract and return from
             the _source field.
-        :arg allow_no_indices: Whether to ignore if a wildcard indices
-            expression resolves into no concrete indices. (This includes `_all`
-            string or when no indices have been specified).
-        :arg analyze_wildcard: Specify whether wildcard and prefix
-            queries should be analyzed. Default is false.
-        :arg analyzer: The analyzer to use for the query string.
-        :arg conflicts: What to do when the operation encounters version
-            conflicts?. Valid choices are abort, proceed.
+        :arg allow_no_indices: If `false`, the request returns an error
+            if any wildcard expression, index alias, or `_all` value targets only
+            missing or closed indices.This behavior applies even if the request
+            targets other open indices.For example, a request targeting `foo*,bar*`
+            returns an error if an index starts with `foo` but no index starts with
+            `bar`.
+        :arg analyze_wildcard: If `true`, wildcard and prefix queries
+            are analyzed. Default is false.
+        :arg analyzer: Analyzer to use for the query string.
+        :arg conflicts: What to do if update by query hits version
+            conflicts: `abort` or `proceed`. Valid choices are abort, proceed.
         :arg default_operator: The default operator for query string
-            query (AND or OR). Valid choices are AND, OR.
-        :arg df: The field to use as default where no field prefix is
-            given in the query string.
-        :arg expand_wildcards: Whether to expand wildcard expression to
-            concrete indices that are open, closed or both. Valid choices are all,
-            open, closed, hidden, none.
+            query: `AND` or `OR`. Valid choices are and, or.
+        :arg df: Field to use as default where no field prefix is given
+            in the query string.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg expand_wildcards: Type of index that wildcard patterns can
+            match.If the request can target data streams, this argument determines
+            whether wildcard expressions match hidden data streams.Supports comma-
+            separated values, such as `open,hidden`.Valid values are: `all`, `open`,
+            `closed`, `hidden`, `none`.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
-        :arg ignore_unavailable: Whether specified concrete indices
-            should be ignored when unavailable (missing or closed).
-        :arg lenient: Specify whether format-based query failures (such
-            as providing text to a numeric field) should be ignored.
-        :arg max_docs: Maximum number of documents to process (default:
-            all documents).
-        :arg pipeline: The pipeline id to preprocess incoming documents
-            with.
-        :arg preference: Specify the node or shard the operation should
-            be performed on. Default is random.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg ignore_unavailable: If `false`, the request returns an
+            error if it targets a missing or closed index.
+        :arg lenient: If `true`, format-based query failures (such as
+            providing text to a numeric field) in the query string will be ignored.
+        :arg max_docs: Maximum number of documents to process.Defaults
+            to all documents.
+        :arg pipeline: ID of the pipeline to use to preprocess incoming
+            documents.If the index has a default ingest pipeline specified, then
+            setting the value to `_none` disables the default ingest pipeline for
+            this request.If a final pipeline is configured it will always run,
+            regardless of the value of this parameter.
+        :arg preference: Specifies the node or shard the operation
+            should be performed on.Random by default. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
-        :arg refresh: Should the affected indexes be refreshed?.
-        :arg request_cache: Specify if request cache should be used for
-            this request or not, defaults to index level setting.
+        :arg refresh: If `true`, Opensearch refreshes affected shards to
+            make the operation visible to search.
+        :arg request_cache: If `true`, the request cache is used for
+            this request.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle. Default is 0.
-        :arg routing: Comma-separated list of specific routing values.
-        :arg scroll: Specify how long a consistent view of the index
-            should be maintained for scrolled search.
-        :arg scroll_size: Size on the scroll request powering the
+            requests per second. Default is 0.
+        :arg routing: Custom value used to route operations to a
+            specific shard.
+        :arg scroll: Period to retain the search context for scrolling.
+        :arg scroll_size: Size of the scroll request that powers the
             operation. Default is 100.
         :arg search_timeout: Explicit timeout for each search request.
-            Defaults to no timeout.
-        :arg search_type: Search operation type. Valid choices are
+        :arg search_type: The type of the search operation. Available
+            options: `query_then_fetch`, `dfs_query_then_fetch`. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg size: Deprecated, please use `max_docs` instead.
         :arg slices: The number of slices this task should be divided
-            into. Defaults to 1, meaning the task isn't sliced into subtasks. Can be
-            set to `auto`. Default is 1.
-        :arg sort: Comma-separated list of <field>:<direction> pairs.
-        :arg stats: Specific 'tag' of the request for logging and
+            into. Valid choices are auto.
+        :arg sort: A comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg stats: Specific `tag` of the request for logging and
             statistical purposes.
-        :arg terminate_after: The maximum number of documents to collect
-            for each shard, upon reaching which the query execution will terminate
-            early.
-        :arg timeout: Time each individual bulk request should wait for
-            shards that are unavailable. Default is 1m.
-        :arg version: Whether to return document version as part of a
-            hit.
-        :arg wait_for_active_shards: Sets the number of shard copies
-            that must be active before proceeding with the operation. Defaults to 1,
-            meaning the primary shard only. Set to `all` for all shard copies,
-            otherwise set to any non-negative value less than or equal to the total
-            number of copies for the shard (number of replicas + 1). Default is 1.
-        :arg wait_for_completion: Should this request wait until the
-            operation has completed before returning. Default is True.
+        :arg terminate_after: Maximum number of documents to collect for
+            each shard.If a query reaches this limit, Opensearch terminates the
+            query early.Opensearch collects documents before sorting.Use with
+            caution.Opensearch applies this parameter to each shard handling the
+            request.When possible, let Opensearch perform early termination
+            automatically.Avoid specifying this parameter for requests that target
+            data streams with backing indices across multiple data tiers.
+        :arg timeout: Period each update request waits for the following
+            operations: dynamic mapping updates, waiting for active shards.
+        :arg version: If `true`, returns the document version as part of
+            a hit.
+        :arg wait_for_active_shards: The number of shard copies that
+            must be active before proceeding with the operation.Set to `all` or any
+            positive integer up to the total number of shards in the index
+            (`number_of_replicas+1`). Valid choices are all, index-setting.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is True.
         """
         # from is a reserved word so it cannot be used, use from_ instead
         if "from_" in params:
             params["from"] = params.pop("from_")
 
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_update_by_query"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("requests_per_second")
-    def update_by_query_rethrottle(
+    @query_params(
+        "error_trace", "filter_path", "human", "pretty", "requests_per_second", "source"
+    )
+    async def update_by_query_rethrottle(
         self,
         task_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Changes the number of requests per second for a particular Update By Query
         operation.
 
 
-        :arg task_id: The task id to rethrottle.
+        :arg task_id: The ID for the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg requests_per_second: The throttle for this request in sub-
-            requests per second. -1 means no throttle.
+            requests per second.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if task_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'task_id'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path("_update_by_query", task_id, "_rethrottle"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    def get_script_context(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def get_script_context(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns all script contexts.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", "/_script_context", params=params, headers=headers
         )
 
-    @query_params()
-    def get_script_languages(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def get_script_languages(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Returns available script types, languages and contexts.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", "/_script_language", params=params, headers=headers
         )
 
     @query_params(
         "allow_partial_pit_creation",
+        "error_trace",
         "expand_wildcards",
+        "filter_path",
+        "human",
         "keep_alive",
         "preference",
+        "pretty",
         "routing",
+        "source",
     )
-    def create_pit(
+    async def create_pit(
         self,
         index: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Creates point in time context.
 
 
         :arg index: Comma-separated list of indices; use `_all` or empty
             string to perform the operation on all indices.
         :arg allow_partial_pit_creation: Allow if point in time can be
             created with partial failures.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg keep_alive: Specify the keep alive for point in time.
         :arg preference: Specify the node or shard the operation should
             be performed on. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg routing: Comma-separated list of specific routing values.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "POST",
             _make_path(index, "_search", "point_in_time"),
             params=params,
             headers=headers,
         )
 
-    @query_params()
-    def delete_all_pits(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def delete_all_pits(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes all active point in time searches.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "DELETE", "/_search/point_in_time/_all", params=params, headers=headers
         )
 
-    @query_params()
-    def delete_pit(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def delete_pit(
         self,
         body: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Deletes one or more point in time searches based on the IDs passed.
 
 
         :arg body: The point-in-time ids to be deleted
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "DELETE",
             "/_search/point_in_time",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
-    def get_all_pits(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    async def get_all_pits(
         self,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Lists all active point in time searches.
 
+
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        return self.transport.perform_request(
+        return await self.transport.perform_request(
             "GET", "/_search/point_in_time/_all", params=params, headers=headers
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/_patch.py` & `opensearch_py-2.6.0/opensearchpy/client/_patch.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/client/client.py` & `opensearch_py-2.6.0/opensearchpy/client/client.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/client/dangling_indices.py` & `opensearch_py-2.6.0/opensearchpy/_async/client/search_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,32 +2,14 @@
 #
 # The OpenSearch Contributors require contributions made to
 # this file be licensed under the Apache-2.0 license or a
 # compatible open source license.
 #
 # Modifications Copyright OpenSearch Contributors. See
 # GitHub history for details.
-#
-#  Licensed to Elasticsearch B.V. under one or more contributor
-#  license agreements. See the NOTICE file distributed with
-#  this work for additional information regarding copyright
-#  ownership. Elasticsearch B.V. licenses this file to you under
-#  the Apache License, Version 2.0 (the "License"); you may
-#  not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-# 	http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing,
-#  software distributed under the License is distributed on an
-#  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-#  KIND, either express or implied.  See the License for the
-#  specific language governing permissions and limitations
-#  under the License.
-
 
 # ------------------------------------------------------------------------------------------
 # THIS CODE IS AUTOMATICALLY GENERATED AND MANUAL EDITS WILL BE LOST
 #
 # To contribute, kindly make modifications in the opensearch-py client generator
 # or in the OpenSearch API specification, and run `nox -rs generate`. See DEVELOPER_GUIDE.md
 # and https://github.com/opensearch-project/opensearch-api-specification for details.
@@ -35,84 +17,135 @@
 
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class DanglingIndicesClient(NamespacedClient):
+class SearchPipelineClient(NamespacedClient):
     @query_params(
-        "accept_data_loss", "cluster_manager_timeout", "master_timeout", "timeout"
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
     )
-    def delete_dangling_index(
+    async def get(
         self,
-        index_uuid: Any,
+        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Deletes the specified dangling index.
+        Retrieves information about a specified search pipeline.
 
 
-        :arg index_uuid: The UUID of the dangling index.
-        :arg accept_data_loss: Must be set to true in order to delete
-            the dangling index.
-        :arg cluster_manager_timeout: Operation timeout for connection
+        :arg id: Comma-separated list of search pipeline ids. Wildcards
+            supported.
+        :arg cluster_manager_timeout: operation timeout for connection
             to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
-        if index_uuid in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
-
-        return self.transport.perform_request(
-            "DELETE",
-            _make_path("_dangling", index_uuid),
-            params=params,
-            headers=headers,
+        return await self.transport.perform_request(
+            "GET", _make_path("_search", "pipeline", id), params=params, headers=headers
         )
 
     @query_params(
-        "accept_data_loss", "cluster_manager_timeout", "master_timeout", "timeout"
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "timeout",
     )
-    def import_dangling_index(
+    async def delete(
         self,
-        index_uuid: Any,
+        id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Imports the specified dangling index.
+        Deletes the specified search pipeline.
 
 
-        :arg index_uuid: The UUID of the dangling index.
-        :arg accept_data_loss: Must be set to true in order to import
-            the dangling index.
+        :arg id: Pipeline ID.
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg timeout: Operation timeout.
         """
-        if index_uuid in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
+        if id in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'id'.")
 
-        return self.transport.perform_request(
-            "POST", _make_path("_dangling", index_uuid), params=params, headers=headers
+        return await self.transport.perform_request(
+            "DELETE",
+            _make_path("_search", "pipeline", id),
+            params=params,
+            headers=headers,
         )
 
-    @query_params()
-    def list_dangling_indices(
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    async def put(
         self,
+        id: Any,
+        body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns all dangling indices.
+        Creates or replaces the specified search pipeline.
 
+
+        :arg id: Pipeline ID.
+        :arg cluster_manager_timeout: operation timeout for connection
+            to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Operation timeout.
         """
-        return self.transport.perform_request(
-            "GET", "/_dangling", params=params, headers=headers
+        for param in (id, body):
+            if param in SKIP_IN_PATH:
+                raise ValueError("Empty value passed for a required argument.")
+
+        return await self.transport.perform_request(
+            "PUT",
+            _make_path("_search", "pipeline", id),
+            params=params,
+            headers=headers,
+            body=body,
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/features.py` & `opensearch_py-2.6.0/opensearchpy/client/features.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/client/http.py` & `opensearch_py-2.6.0/opensearchpy/client/http.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/client/ingest.py` & `opensearch_py-2.6.0/opensearchpy/client/dangling_indices.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,134 +35,131 @@
 
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class IngestClient(NamespacedClient):
-    @query_params("cluster_manager_timeout", "master_timeout")
-    def get_pipeline(
+class DanglingIndicesClient(NamespacedClient):
+    @query_params(
+        "accept_data_loss",
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def delete_dangling_index(
         self,
-        id: Any = None,
+        index_uuid: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns a pipeline.
+        Deletes the specified dangling index.
 
 
-        :arg id: Comma-separated list of pipeline ids. Wildcards
-            supported.
+        :arg index_uuid: The UUID of the dangling index
+        :arg accept_data_loss: Must be set to true in order to delete
+            the dangling index
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
-        return self.transport.perform_request(
-            "GET", _make_path("_ingest", "pipeline", id), params=params, headers=headers
-        )
-
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    def put_pipeline(
-        self,
-        id: Any,
-        body: Any,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Creates or updates a pipeline.
-
-
-        :arg id: Pipeline ID.
-        :arg body: The ingest definition
-        :arg cluster_manager_timeout: Operation timeout for connection
-            to cluster-manager node.
-        :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
-        """
-        for param in (id, body):
-            if param in SKIP_IN_PATH:
-                raise ValueError("Empty value passed for a required argument.")
+        if index_uuid in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
 
         return self.transport.perform_request(
-            "PUT",
-            _make_path("_ingest", "pipeline", id),
+            "DELETE",
+            _make_path("_dangling", index_uuid),
             params=params,
             headers=headers,
-            body=body,
         )
 
-    @query_params("cluster_manager_timeout", "master_timeout", "timeout")
-    def delete_pipeline(
+    @query_params(
+        "accept_data_loss",
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "master_timeout",
+        "pretty",
+        "source",
+        "timeout",
+    )
+    def import_dangling_index(
         self,
-        id: Any,
+        index_uuid: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Deletes a pipeline.
+        Imports the specified dangling index.
 
 
-        :arg id: Pipeline ID.
+        :arg index_uuid: The UUID of the dangling index
+        :arg accept_data_loss: Must be set to true in order to import
+            the dangling index
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg master_timeout (Deprecated: To promote inclusive language,
-            use 'cluster_manager_timeout' instead.): Operation timeout for
-            connection to master node.
-        :arg timeout: Operation timeout.
+            use 'cluster_manager_timeout' instead.): Specify timeout for connection
+            to master
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Explicit operation timeout
         """
-        if id in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'id'.")
+        if index_uuid in SKIP_IN_PATH:
+            raise ValueError("Empty value passed for a required argument 'index_uuid'.")
 
         return self.transport.perform_request(
-            "DELETE",
-            _make_path("_ingest", "pipeline", id),
-            params=params,
-            headers=headers,
+            "POST", _make_path("_dangling", index_uuid), params=params, headers=headers
         )
 
-    @query_params("verbose")
-    def simulate(
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
+    def list_dangling_indices(
         self,
-        body: Any,
-        id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Allows to simulate a pipeline with example documents.
-
-
-        :arg body: The simulate definition
-        :arg id: Pipeline ID.
-        :arg verbose: Verbose mode. Display data output for each
-            processor in executed pipeline. Default is false.
-        """
-        if body in SKIP_IN_PATH:
-            raise ValueError("Empty value passed for a required argument 'body'.")
+        Returns all dangling indices.
 
-        return self.transport.perform_request(
-            "POST",
-            _make_path("_ingest", "pipeline", id, "_simulate"),
-            params=params,
-            headers=headers,
-            body=body,
-        )
-
-    @query_params()
-    def processor_grok(
-        self,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Returns a list of the built-in patterns.
 
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         return self.transport.perform_request(
-            "GET", "/_ingest/processor/grok", params=params, headers=headers
+            "GET", "/_dangling", params=params, headers=headers
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/nodes.py` & `opensearch_py-2.6.0/opensearchpy/client/tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,192 +30,165 @@
 #
 # To contribute, kindly make modifications in the opensearch-py client generator
 # or in the OpenSearch API specification, and run `nox -rs generate`. See DEVELOPER_GUIDE.md
 # and https://github.com/opensearch-project/opensearch-api-specification for details.
 # -----------------------------------------------------------------------------------------+
 
 
+import warnings
 from typing import Any
 
-from .utils import NamespacedClient, _make_path, query_params
+from .utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
-class NodesClient(NamespacedClient):
-    @query_params("timeout")
-    def reload_secure_settings(
-        self,
-        body: Any = None,
-        node_id: Any = None,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Reloads secure settings.
-
-
-        :arg body: An object containing the password for the opensearch
-            keystore
-        :arg node_id: Comma-separated list of node IDs to span the
-            reload/reinit call. Should stay empty because reloading usually involves
-            all cluster nodes.
-        :arg timeout: Operation timeout.
-        """
-        return self.transport.perform_request(
-            "POST",
-            _make_path("_nodes", node_id, "reload_secure_settings"),
-            params=params,
-            headers=headers,
-            body=body,
-        )
-
-    @query_params("flat_settings", "timeout")
-    def info(
+class TasksClient(NamespacedClient):
+    @query_params(
+        "actions",
+        "detailed",
+        "error_trace",
+        "filter_path",
+        "group_by",
+        "human",
+        "nodes",
+        "parent_task_id",
+        "pretty",
+        "source",
+        "timeout",
+        "wait_for_completion",
+    )
+    def list(
         self,
-        node_id: Any = None,
-        metric: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns information about nodes in the cluster.
+        Returns a list of tasks.
 
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
+        :arg actions: Comma-separated list or wildcard expression of
+            actions used to limit the request.
+        :arg detailed: If `true`, the response includes detailed
+            information about shard recoveries. Default is false.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg group_by: Key used to group tasks in the response. Valid
+            choices are nodes, parents, none.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg nodes: Comma-separated list of node IDs or names to limit
             the returned information; use `_local` to return information from the
             node you're connecting to, leave empty to get information from all
             nodes.
-        :arg metric: Comma-separated list of metrics you wish returned.
-            Leave empty to return all. Valid choices are settings, os, process, jvm,
-            thread_pool, transport, http, plugins, ingest.
-        :arg flat_settings: Return settings in flat format. Default is
-            false.
-        :arg timeout: Operation timeout.
+        :arg parent_task_id: Parent task ID used to limit returned
+            information. To return all tasks, omit this parameter or use a value of
+            `-1`.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response. If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the operation is complete. Default is false.
         """
         return self.transport.perform_request(
-            "GET", _make_path("_nodes", node_id, metric), params=params, headers=headers
+            "GET", "/_tasks", params=params, headers=headers
         )
 
     @query_params(
-        "completion_fields",
-        "fielddata_fields",
-        "fields",
-        "groups",
-        "include_segment_file_sizes",
-        "level",
-        "timeout",
-        "types",
+        "actions",
+        "error_trace",
+        "filter_path",
+        "human",
+        "nodes",
+        "parent_task_id",
+        "pretty",
+        "source",
+        "wait_for_completion",
     )
-    def stats(
+    def cancel(
         self,
-        node_id: Any = None,
-        metric: Any = None,
-        index_metric: Any = None,
+        task_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns statistical information about nodes in the cluster.
+        Cancels a task, if it can be cancelled through an API.
 
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg metric: Limit the information returned to the specified
-            metrics. Valid choices are _all, breaker, fs, http, indices, jvm, os,
-            process, thread_pool, transport, discovery, indexing_pressure,
-            search_pipeline.
-        :arg index_metric: Limit the information returned for `indices`
-            metric to the specific index metrics. Isn't used if `indices` (or `all`)
-            metric isn't specified. Valid choices are _all, store, indexing, get,
-            search, merge, flush, refresh, query_cache, fielddata, docs, warmer,
-            completion, segments, translog, suggest, request_cache, recovery.
-        :arg completion_fields: Comma-separated list of fields for
-            `fielddata` and `suggest` index metric (supports wildcards).
-        :arg fielddata_fields: Comma-separated list of fields for
-            `fielddata` index metric (supports wildcards).
-        :arg fields: Comma-separated list of fields for `fielddata` and
-            `completion` index metric (supports wildcards).
-        :arg groups: Comma-separated list of search groups for `search`
-            index metric.
-        :arg include_segment_file_sizes: Whether to report the
-            aggregated disk usage of each one of the Lucene index files (only
-            applies if segment stats are requested). Default is false.
-        :arg level: Return indices stats aggregated at index, node or
-            shard level. Valid choices are indices, node, shards.
-        :arg timeout: Operation timeout.
-        :arg types: Comma-separated list of document types for the
-            `indexing` index metric.
+        :arg task_id: ID of the task.
+        :arg actions: Comma-separated list or wildcard expression of
+            actions used to limit the request.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg nodes: Comma-separated list of node IDs or names used to
+            limit the request.
+        :arg parent_task_id: Parent task ID used to limit the tasks.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg wait_for_completion: Should the request block until the
+            cancellation of the task and its descendant tasks is completed. Defaults
+            to false Default is false.
         """
         return self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "stats", metric, index_metric),
+            "POST",
+            _make_path("_tasks", task_id, "_cancel"),
             params=params,
             headers=headers,
         )
 
     @query_params(
-        "doc_type", "ignore_idle_threads", "interval", "snapshots", "threads", "timeout"
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "timeout",
+        "wait_for_completion",
     )
-    def hot_threads(
+    def get(
         self,
-        node_id: Any = None,
+        task_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
-        Returns information about hot threads on each node in the cluster.
-
-
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg doc_type: The type to sample. Valid choices are cpu, wait,
-            block.
-        :arg ignore_idle_threads: Don't show threads that are in known-
-            idle places, such as waiting on a socket select or pulling from an empty
-            task queue. Default is True.
-        :arg interval: The interval for the second sampling of threads.
-        :arg snapshots: Number of samples of thread stacktrace. Default
-            is 10.
-        :arg threads: Specify the number of threads to provide
-            information for. Default is 3.
-        :arg timeout: Operation timeout.
-        """
-        # type is a reserved word so it cannot be used, use doc_type instead
-        if "doc_type" in params:
-            params["type"] = params.pop("doc_type")
-
-        return self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "hot_threads"),
-            params=params,
-            headers=headers,
-        )
+        Returns information about a task.
 
-    @query_params("timeout")
-    def usage(
-        self,
-        node_id: Any = None,
-        metric: Any = None,
-        params: Any = None,
-        headers: Any = None,
-    ) -> Any:
-        """
-        Returns low-level information about REST actions usage on nodes.
 
+        :arg task_id: ID of the task.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
+        :arg timeout: Period to wait for a response.If no response is
+            received before the timeout expires, the request fails and returns an
+            error.
+        :arg wait_for_completion: If `true`, the request blocks until
+            the task has completed. Default is false.
+        """
+        if task_id in SKIP_IN_PATH:
+            warnings.warn(
+                "Calling client.tasks.get() without a task_id is deprecated "
+                "and will be removed in v8.0. Use client.tasks.list() instead.",
+                category=DeprecationWarning,
+                stacklevel=3,
+            )
 
-        :arg node_id: Comma-separated list of node IDs or names to limit
-            the returned information; use `_local` to return information from the
-            node you're connecting to, leave empty to get information from all
-            nodes.
-        :arg metric: Limit the information returned to the specified
-            metrics. Valid choices are _all, rest_actions.
-        :arg timeout: Operation timeout.
-        """
         return self.transport.perform_request(
-            "GET",
-            _make_path("_nodes", node_id, "usage", metric),
-            params=params,
-            headers=headers,
+            "GET", _make_path("_tasks", task_id), params=params, headers=headers
         )
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/plugins.py` & `opensearch_py-2.6.0/opensearchpy/client/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 
 import warnings
 from typing import Any
 
 from ..plugins.alerting import AlertingClient
 from ..plugins.index_management import IndexManagementClient
 from ..plugins.knn import KnnClient
+from ..plugins.notifications import NotificationsClient
+from ..plugins.rollups import RollupsClient
+from ..plugins.transforms import TransformsClient
 from .client import Client
 from .utils import NamespacedClient
 
 
 class PluginsClient(NamespacedClient):
     alerting: Any
     index_management: Any
 
     def __init__(self, client: Client) -> None:
         super(PluginsClient, self).__init__(client)
+        self.transforms = TransformsClient(client)
+        self.rollups = RollupsClient(client)
+        self.notifications = NotificationsClient(client)
         self.knn = KnnClient(client)
         # self.query_workbench = QueryWorkbenchClient(client)
         # self.reporting = ReportingClient(client)
         # self.notebooks = NotebooksClient(client)
         self.alerting = AlertingClient(client)
         # self.anomaly_detection = AnomalyDetectionClient(client)
         # self.trace_analytics = TraceAnalyticsClient(client)
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/remote.py` & `opensearch_py-2.6.0/opensearchpy/client/remote.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/client/remote_store.py` & `opensearch_py-2.6.0/opensearchpy/client/remote_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,46 @@
 
 from typing import Any
 
 from .utils import SKIP_IN_PATH, NamespacedClient, query_params
 
 
 class RemoteStoreClient(NamespacedClient):
-    @query_params("cluster_manager_timeout", "wait_for_completion")
+    @query_params(
+        "cluster_manager_timeout",
+        "error_trace",
+        "filter_path",
+        "human",
+        "pretty",
+        "source",
+        "wait_for_completion",
+    )
     def restore(
         self,
         body: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Restores from remote store.
 
 
         :arg body: Comma-separated list of index IDs
         :arg cluster_manager_timeout: Operation timeout for connection
             to cluster-manager node.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg wait_for_completion: Should this request wait until the
             operation has completed before returning. Default is false.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         return self.transport.perform_request(
```

### Comparing `opensearch-py-2.5.0/opensearchpy/client/utils.py` & `opensearch_py-2.6.0/opensearchpy/client/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/compat.py` & `opensearch_py-2.6.0/opensearchpy/compat.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/__init__.py` & `opensearch_py-2.6.0/opensearchpy/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/async_connections.py` & `opensearch_py-2.6.0/opensearchpy/connection/async_connections.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/base.py` & `opensearch_py-2.6.0/opensearchpy/connection/base.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/connections.py` & `opensearch_py-2.6.0/opensearchpy/connection/connections.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/http_async.py` & `opensearch_py-2.6.0/opensearchpy/connection/http_async.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/http_requests.py` & `opensearch_py-2.6.0/opensearchpy/connection/http_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 try:
     import requests
 
     REQUESTS_AVAILABLE = True
 except ImportError:
     REQUESTS_AVAILABLE = False
 
+from opensearchpy.metrics import Metrics, MetricsNone
+
 from ..compat import reraise_exceptions, string_types, urlencode
 from ..exceptions import (
     ConnectionError,
     ConnectionTimeout,
     ImproperlyConfigured,
     SSLError,
 )
@@ -65,14 +67,17 @@
         separate cert and key files (client_cert will contain only the cert)
     :arg headers: any custom http headers to be add to requests
     :arg http_compress: Use gzip compression
     :arg opaque_id: Send this value in the 'X-Opaque-Id' HTTP header
         For tracing all requests made by this transport.
     :arg pool_maxsize: Maximum connection pool size used by pool-manager
         For custom connection-pooling on current session
+    :arg metrics: metrics is an instance of a subclass of the
+        :class:`~opensearchpy.Metrics` class, used for collecting
+        and reporting metrics related to the client's operations;
     """
 
     def __init__(
         self,
         host: str = "localhost",
         port: Optional[int] = None,
         http_auth: Any = None,
@@ -82,16 +87,18 @@
         ca_certs: Any = None,
         client_cert: Any = None,
         client_key: Any = None,
         headers: Any = None,
         http_compress: Any = None,
         opaque_id: Any = None,
         pool_maxsize: Any = None,
+        metrics: Metrics = MetricsNone(),
         **kwargs: Any
     ) -> None:
+        self.metrics = metrics
         if not REQUESTS_AVAILABLE:
             raise ImproperlyConfigured(
                 "Please install requests to use RequestsHttpConnection."
             )
 
         # Initialize Session so .headers works before calling super().__init__().
         self.session = requests.Session()
@@ -184,14 +191,15 @@
         )
         send_kwargs: Any = {
             "timeout": timeout or self.timeout,
             "allow_redirects": allow_redirects,
         }
         send_kwargs.update(settings)
         try:
+            self.metrics.request_start()
             response = self.session.send(prepared_request, **send_kwargs)
             duration = time.time() - start
             raw_data = response.content.decode("utf-8", "surrogatepass")
         except reraise_exceptions:
             raise
         except Exception as e:
             self.log_request_fail(
@@ -203,14 +211,16 @@
                 exception=e,
             )
             if isinstance(e, requests.exceptions.SSLError):
                 raise SSLError("N/A", str(e), e)
             if isinstance(e, requests.Timeout):
                 raise ConnectionTimeout("TIMEOUT", str(e), e)
             raise ConnectionError("N/A", str(e), e)
+        finally:
+            self.metrics.request_end()
 
         # raise warnings if any from the 'Warnings' header.
         warnings_headers = (
             (response.headers["warning"],) if "warning" in response.headers else ()
         )
         self._raise_warnings(warnings_headers)
```

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/http_urllib3.py` & `opensearch_py-2.6.0/opensearchpy/connection/http_urllib3.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from typing import Any, Callable, Collection, Mapping, Optional, Union
 
 import urllib3
 from urllib3.exceptions import ReadTimeoutError
 from urllib3.exceptions import SSLError as UrllibSSLError
 from urllib3.util.retry import Retry
 
+from opensearchpy.metrics import Metrics, MetricsNone
+
 from ..compat import reraise_exceptions, urlencode
 from ..exceptions import (
     ConnectionError,
     ConnectionTimeout,
     ImproperlyConfigured,
     SSLError,
 )
@@ -90,14 +92,17 @@
     :arg pool_maxsize: the number of connections which will be kept open to this
         host. See https://urllib3.readthedocs.io/en/1.4/pools.html#api for more
         information.
     :arg headers: any custom http headers to be add to requests
     :arg http_compress: Use gzip compression
     :arg opaque_id: Send this value in the 'X-Opaque-Id' HTTP header
         For tracing all requests made by this transport.
+    :arg metrics: metrics is an instance of a subclass of the
+        :class:`~opensearchpy.Metrics` class, used for collecting
+        and reporting metrics related to the client's operations;
     """
 
     def __init__(
         self,
         host: str = "localhost",
         port: Optional[int] = None,
         http_auth: Any = None,
@@ -111,16 +116,18 @@
         ssl_assert_hostname: Any = None,
         ssl_assert_fingerprint: Any = None,
         pool_maxsize: Any = None,
         headers: Any = None,
         ssl_context: Any = None,
         http_compress: Any = None,
         opaque_id: Any = None,
+        metrics: Metrics = MetricsNone(),
         **kwargs: Any
     ) -> None:
+        self.metrics = metrics
         # Initialize headers before calling super().__init__().
         self.headers = urllib3.make_headers(keep_alive=True)
 
         super(Urllib3HttpConnection, self).__init__(
             host=host,
             port=port,
             use_ssl=use_ssl,
@@ -264,14 +271,16 @@
                 body = self._gzip_compress(body)
                 request_headers["content-encoding"] = "gzip"
 
             if self.http_auth is not None:
                 if isinstance(self.http_auth, Callable):  # type: ignore
                     request_headers.update(self.http_auth(method, full_url, body))
 
+            self.metrics.request_start()
+
             response = self.pool.urlopen(
                 method, url, body, retries=Retry(False), headers=request_headers, **kw
             )
             duration = time.time() - start
             raw_data = response.data.decode("utf-8", "surrogatepass")
         except reraise_exceptions:
             raise
@@ -280,14 +289,16 @@
                 method, full_url, url, orig_body, time.time() - start, exception=e
             )
             if isinstance(e, UrllibSSLError):
                 raise SSLError("N/A", str(e), e)
             if isinstance(e, ReadTimeoutError):
                 raise ConnectionTimeout("TIMEOUT", str(e), e)
             raise ConnectionError("N/A", str(e), e)
+        finally:
+            self.metrics.request_end()
 
         # raise warnings if any from the 'Warnings' header.
         warning_headers = response.headers.get_all("warning", ())
         self._raise_warnings(warning_headers)
 
         # raise errors based on http status codes, let the client handle those if needed
         if not (200 <= response.status < 300) and response.status not in ignore:
```

### Comparing `opensearch-py-2.5.0/opensearchpy/connection/pooling.py` & `opensearch_py-2.6.0/opensearchpy/connection/pooling.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/connection_pool.py` & `opensearch_py-2.6.0/opensearchpy/connection_pool.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/exceptions.py` & `opensearch_py-2.6.0/opensearchpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/__init__.py` & `opensearch_py-2.6.0/opensearchpy/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/actions.py` & `opensearch_py-2.6.0/opensearchpy/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/aggs.py` & `opensearch_py-2.6.0/opensearchpy/helpers/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/analysis.py` & `opensearch_py-2.6.0/opensearchpy/helpers/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,17 +229,21 @@
 
     def get_definition(self) -> Any:
         d = super(CustomTokenFilter, self).get_definition()
 
         if "filters" in d:
             d["filters"] = [
                 # comma delimited string given by user
-                fs if isinstance(fs, six.string_types) else
-                # list of strings or TokenFilter objects
-                ", ".join(f.to_dict() if hasattr(f, "to_dict") else f for f in fs)
+                (
+                    fs
+                    if isinstance(fs, six.string_types)
+                    else
+                    # list of strings or TokenFilter objects
+                    ", ".join(f.to_dict() if hasattr(f, "to_dict") else f for f in fs)
+                )
                 for fs in self.filters
             ]
         return d
 
     def get_analysis_definition(self) -> Any:
         if not hasattr(self, "filters"):
             return {}
```

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/asyncsigner.py` & `opensearch_py-2.6.0/opensearchpy/helpers/asyncsigner.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/document.py` & `opensearch_py-2.6.0/opensearchpy/helpers/document.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/errors.py` & `opensearch_py-2.6.0/opensearchpy/helpers/response/hit.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,26 +20,46 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
+from typing import Any
 
-from typing import Any, List
+from ..utils import AttrDict, HitMeta
 
-from ..exceptions import OpenSearchException
 
+class Hit(AttrDict):
+    def __init__(self, document: Any) -> None:
+        data = {}
+        if "_source" in document:
+            data = document["_source"]
+        if "fields" in document:
+            data.update(document["fields"])
 
-class BulkIndexError(OpenSearchException):
-    @property
-    def errors(self) -> List[Any]:
-        """List of errors from execution of the last chunk."""
-        return self.args[1]  # type: ignore
+        super(Hit, self).__init__(data)
+        # assign meta as attribute and not as key in self._d_
+        super(AttrDict, self).__setattr__("meta", HitMeta(document))
 
+    def __getstate__(self) -> Any:
+        # add self.meta since it is not in self.__dict__
+        return super(Hit, self).__getstate__() + (self.meta,)
 
-class ScanError(OpenSearchException):
-    scroll_id: str
+    def __setstate__(self, state: Any) -> None:
+        super(AttrDict, self).__setattr__("meta", state[-1])
+        super(Hit, self).__setstate__(state[:-1])
 
-    def __init__(self, scroll_id: str, *args: Any, **kwargs: Any) -> None:
-        super(ScanError, self).__init__(*args, **kwargs)
-        self.scroll_id = scroll_id
+    def __dir__(self) -> Any:
+        # be sure to expose meta in dir(self)
+        return super(Hit, self).__dir__() + ["meta"]
+
+    def __repr__(self) -> str:
+        return "<Hit({}): {}>".format(
+            "/".join(
+                getattr(self.meta, key) for key in ("index", "id") if key in self.meta
+            ),
+            super(Hit, self).__repr__(),
+        )
+
+
+__all__ = ["Hit", "HitMeta"]
```

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/faceted_search.py` & `opensearch_py-2.6.0/opensearchpy/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/field.py` & `opensearch_py-2.6.0/opensearchpy/helpers/field.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/function.py` & `opensearch_py-2.6.0/opensearchpy/helpers/function.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/index.py` & `opensearch_py-2.6.0/opensearchpy/helpers/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/mapping.py` & `opensearch_py-2.6.0/opensearchpy/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/query.py` & `opensearch_py-2.6.0/opensearchpy/helpers/query.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/response/__init__.py` & `opensearch_py-2.6.0/opensearchpy/helpers/response/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/response/aggs.py` & `opensearch_py-2.6.0/opensearchpy/helpers/response/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/search.py` & `opensearch_py-2.6.0/opensearchpy/helpers/search.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/signer.py` & `opensearch_py-2.6.0/opensearchpy/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/test.py` & `opensearch_py-2.6.0/opensearchpy/helpers/test.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/update_by_query.py` & `opensearch_py-2.6.0/opensearchpy/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/utils.py` & `opensearch_py-2.6.0/opensearchpy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/helpers/wrappers.py` & `opensearch_py-2.6.0/opensearchpy/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/plugins/alerting.py` & `opensearch_py-2.6.0/opensearchpy/plugins/alerting.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,17 +120,19 @@
         """
         Returns the details of a specific destination.
 
         :arg destination_id: The id of the destination we are trying to fetch. If None, returns all destinations
         """
         return self.transport.perform_request(
             "GET",
-            _make_path("_plugins", "_alerting", "destinations", destination_id)
-            if destination_id
-            else _make_path("_plugins", "_alerting", "destinations"),
+            (
+                _make_path("_plugins", "_alerting", "destinations", destination_id)
+                if destination_id
+                else _make_path("_plugins", "_alerting", "destinations")
+            ),
             params=params,
             headers=headers,
         )
 
     @query_params()
     def create_destination(
         self, body: Any = None, params: Any = None, headers: Any = None
```

### Comparing `opensearch-py-2.5.0/opensearchpy/plugins/index_management.py` & `opensearch_py-2.6.0/opensearchpy/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/plugins/knn.py` & `opensearch_py-2.6.0/opensearchpy/plugins/knn.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,49 +18,69 @@
 
 from typing import Any
 
 from ..client.utils import SKIP_IN_PATH, NamespacedClient, _make_path, query_params
 
 
 class KnnClient(NamespacedClient):
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     def delete_model(
         self,
         model_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Used to delete a particular model in the cluster.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if model_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'model_id'.")
 
         return self.transport.perform_request(
             "DELETE",
             _make_path("_plugins", "_knn", "models", model_id),
             params=params,
             headers=headers,
         )
 
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     def get_model(
         self,
         model_id: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Used to retrieve information about models present in the cluster.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if model_id in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'model_id'.")
 
         return self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", "models", model_id),
@@ -77,32 +97,37 @@
         "analyze_wildcard",
         "analyzer",
         "batched_reduce_size",
         "ccs_minimize_roundtrips",
         "default_operator",
         "df",
         "docvalue_fields",
+        "error_trace",
         "expand_wildcards",
         "explain",
+        "filter_path",
         "from_",
+        "human",
         "ignore_throttled",
         "ignore_unavailable",
         "lenient",
         "max_concurrent_shard_requests",
         "pre_filter_shard_size",
         "preference",
+        "pretty",
         "q",
         "request_cache",
         "rest_total_hits_as_int",
         "routing",
         "scroll",
         "search_type",
         "seq_no_primary_term",
         "size",
         "sort",
+        "source",
         "stats",
         "stored_fields",
         "suggest_field",
         "suggest_mode",
         "suggest_size",
         "suggest_text",
         "terminate_after",
@@ -147,20 +172,26 @@
             execution. Default is True.
         :arg default_operator: The default operator for query string
             query (AND or OR). Valid choices are AND, OR.
         :arg df: The field to use as default where no field prefix is
             given in the query string.
         :arg docvalue_fields: Comma-separated list of fields to return
             as the docvalue representation of a field for each hit.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
         :arg expand_wildcards: Whether to expand wildcard expression to
             concrete indices that are open, closed or both. Valid choices are all,
             open, closed, hidden, none.
         :arg explain: Specify whether to return detailed information
             about score computation as part of a hit.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
         :arg from_: Starting offset. Default is 0.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg ignore_throttled: Whether specified concrete, expanded or
             aliased indices should be ignored when throttled.
         :arg ignore_unavailable: Whether specified concrete indices
             should be ignored when unavailable (missing or closed).
         :arg lenient: Specify whether format-based query failures (such
             as providing text to a numeric field) should be ignored.
         :arg max_concurrent_shard_requests: The number of concurrent
@@ -172,14 +203,16 @@
             number of shards the search request expands to exceeds the threshold.
             This filter round-trip can limit the number of shards significantly if
             for instance a shard can not match any documents based on its rewrite
             method ie. if date filters are mandatory to match but the shard bounds
             and the query are disjoint.
         :arg preference: Specify the node or shard the operation should
             be performed on. Default is random.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
         :arg q: Query in the Lucene query string syntax.
         :arg request_cache: Specify if request cache should be used for
             this request or not, defaults to index level setting.
         :arg rest_total_hits_as_int: Indicates whether hits.total should
             be rendered as an integer or an object in the rest search response.
             Default is false.
         :arg routing: Comma-separated list of specific routing values.
@@ -187,14 +220,16 @@
             should be maintained for scrolled search.
         :arg search_type: Search operation type. Valid choices are
             query_then_fetch, dfs_query_then_fetch.
         :arg seq_no_primary_term: Specify whether to return sequence
             number and primary term of the last modification of each hit.
         :arg size: Number of hits to return. Default is 10.
         :arg sort: Comma-separated list of <field>:<direction> pairs.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg stats: Specific 'tag' of the request for logging and
             statistical purposes.
         :arg stored_fields: Comma-separated list of stored fields to
             return.
         :arg suggest_field: Specify which field to use for suggestions.
         :arg suggest_mode: Specify suggest mode. Valid choices are
             missing, popular, always.
@@ -222,15 +257,15 @@
             "POST",
             "/_plugins/_knn/models/_search",
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params("timeout")
+    @query_params("error_trace", "filter_path", "human", "pretty", "source", "timeout")
     def stats(
         self,
         node_id: Any = None,
         stat: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
@@ -239,75 +274,97 @@
 
 
         :arg node_id: Comma-separated list of node IDs or names to limit
             the returned information; use `_local` to return information from the
             node you're connecting to, leave empty to get information from all
             nodes.
         :arg stat: Comma-separated list of stats to retrieve; use `_all`
-            or empty string to retrieve all stats. Valid choices are
-            circuit_breaker_triggered, total_load_time, eviction_count, hit_count,
-            miss_count, graph_memory_usage, graph_memory_usage_percentage,
-            graph_index_requests, graph_index_errors, graph_query_requests,
-            graph_query_errors, knn_query_requests, cache_capacity_reached,
-            load_success_count, load_exception_count, indices_in_cache,
-            script_compilations, script_compilation_errors, script_query_requests,
-            script_query_errors, nmslib_initialized, faiss_initialized,
-            model_index_status, indexing_from_model_degraded, training_requests,
-            training_errors, training_memory_usage,
-            training_memory_usage_percentage.
+            or empty string to retrieve all stats.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         :arg timeout: Operation timeout.
         """
         return self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", node_id, "stats", stat),
             params=params,
             headers=headers,
         )
 
-    @query_params("preference")
+    @query_params(
+        "error_trace", "filter_path", "human", "preference", "pretty", "source"
+    )
     def train_model(
         self,
         body: Any,
         model_id: Any = None,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Create and train a model that can be used for initializing k-NN native library
         indexes during indexing.
 
 
         :arg model_id: The id of the model.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
         :arg preference: Preferred node to execute training.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if body in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'body'.")
 
         return self.transport.perform_request(
             "POST",
             _make_path("_plugins", "_knn", "models", model_id, "_train"),
             params=params,
             headers=headers,
             body=body,
         )
 
-    @query_params()
+    @query_params("error_trace", "filter_path", "human", "pretty", "source")
     def warmup(
         self,
         index: Any,
         params: Any = None,
         headers: Any = None,
     ) -> Any:
         """
         Preloads native library files into memory, reducing initial search latency for
-        specified indexes
+        specified indexes.
 
 
         :arg index: Comma-separated list of indices; use `_all` or empty
             string to perform the operation on all indices.
+        :arg error_trace: Whether to include the stack trace of returned
+            errors.
+        :arg filter_path: Comma-separated list of filters used to reduce
+            the response.
+        :arg human: Whether to return human readable values for
+            statistics.
+        :arg pretty: Whether to pretty format the returned JSON
+            response.
+        :arg source: The URL-encoded request definition. Useful for
+            libraries that do not accept a request body for non-POST requests.
         """
         if index in SKIP_IN_PATH:
             raise ValueError("Empty value passed for a required argument 'index'.")
 
         return self.transport.perform_request(
             "GET",
             _make_path("_plugins", "_knn", "warmup", index),
```

### Comparing `opensearch-py-2.5.0/opensearchpy/serializer.py` & `opensearch_py-2.6.0/opensearchpy/serializer.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.5.0/opensearchpy/transport.py` & `opensearch_py-2.6.0/opensearchpy/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 #  under the License.
 
 
 import time
 from itertools import chain
 from typing import Any, Callable, Collection, Dict, List, Mapping, Optional, Type, Union
 
+from opensearchpy.metrics import Metrics, MetricsNone
+
 from .connection import Connection, Urllib3HttpConnection
 from .connection_pool import ConnectionPool, DummyConnectionPool, EmptyConnectionPool
 from .exceptions import (
     ConnectionError,
     ConnectionTimeout,
     SerializationError,
     TransportError,
@@ -87,14 +89,15 @@
     seed_connections: List[Connection]
     sniffer_timeout: Optional[float]
     sniff_on_start: bool
     sniff_on_connection_fail: bool
     last_sniff: float
     sniff_timeout: Optional[float]
     host_info_callback: Any
+    metrics: Metrics
 
     def __init__(
         self,
         hosts: Any,
         connection_class: Optional[Type[Connection]] = None,
         connection_pool_class: Type[ConnectionPool] = ConnectionPool,
         host_info_callback: Callable[
@@ -108,14 +111,15 @@
         serializers: Optional[Mapping[str, Serializer]] = None,
         default_mimetype: str = "application/json",
         max_retries: int = 3,
         pool_maxsize: Optional[int] = None,
         retry_on_status: Collection[int] = (502, 503, 504),
         retry_on_timeout: bool = False,
         send_get_body_as: str = "GET",
+        metrics: Metrics = MetricsNone(),
         **kwargs: Any
     ) -> None:
         """
         :arg hosts: list of dictionaries, each containing keyword arguments to
             create a `connection_class` instance
         :arg connection_class: subclass of :class:`~opensearchpy.Connection` to use
         :arg connection_pool_class: subclass of :class:`~opensearchpy.ConnectionPool` to use
@@ -144,19 +148,23 @@
         :arg send_get_body_as: for GET requests with body this option allows
             you to specify an alternate way of execution for environments that
             don't support passing bodies with GET requests. If you set this to
             'POST' a POST method will be used instead, if to 'source' then the body
             will be serialized and passed as a query parameter `source`.
         :arg pool_maxsize: Maximum connection pool size used by pool-manager
             For custom connection-pooling on current session
+        :arg metrics: metrics is an instance of a subclass of the
+            :class:`~opensearchpy.Metrics` class, used for collecting
+            and reporting metrics related to the client's operations;
 
         Any extra keyword arguments will be passed to the `connection_class`
         when creating and instance unless overridden by that connection's
         options provided as part of the hosts parameter.
         """
+        self.metrics = metrics
         if connection_class is None:
             connection_class = self.DEFAULT_CONNECTION_CLASS
 
         # serialization config
         _serializers = DEFAULT_SERIALIZERS.copy()
         # if a serializer has been specified, use it for deserialization as well
         _serializers[serializer.mimetype] = serializer
@@ -238,15 +246,15 @@
                         return connection
 
             # previously unseen params, create new connection
             kwargs = self.kwargs.copy()
             kwargs.update(host)
             if self.pool_maxsize and isinstance(self.pool_maxsize, int):
                 kwargs["pool_maxsize"] = self.pool_maxsize
-            return self.connection_class(**kwargs)
+            return self.connection_class(metrics=self.metrics, **kwargs)
 
         connections = list(zip(map(_create_connection, hosts), hosts))
         if len(connections) == 1:
             self.connection_pool = DummyConnectionPool(connections)
         else:
             # pass the hosts dicts to the connection pool to optionally extract parameters from
             self.connection_pool = self.connection_pool_class(
```

### Comparing `opensearch-py-2.5.0/setup.py` & `opensearch_py-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,36 +50,38 @@
 MODULE_DIR = PACKAGE_NAME.replace("-", "")
 packages = [
     package
     for package in find_packages(where=".", exclude=("test_opensearchpy*",))
     if package == MODULE_DIR or package.startswith(MODULE_DIR + ".")
 ]
 install_requires = [
-    "urllib3>=1.26.18, <2",
+    'urllib3>=1.26.18,<1.27 ; python_version < "3.10"',
+    'urllib3>=1.26.18,!=2.2.0,<3 ; python_version >= "3.10"',
     "requests>=2.4.0, <3.0.0",
     "six",
     "python-dateutil",
     "certifi>=2022.12.07",
+    "Events",
 ]
 tests_require = [
     "requests>=2.0.0, <3.0.0",
     "coverage<8.0.0",
     "mock",
     "pyyaml",
     "pytest>=3.0.0",
     "pytest-cov",
     "pytz",
     "botocore",
     "pytest-mock<4.0.0",
 ]
 
-async_require = ["aiohttp>=3,<4"]
+async_require = ["aiohttp>=3.9.4,<4"]
 
 docs_require = ["sphinx", "sphinx_rtd_theme", "myst_parser", "sphinx_copybutton"]
-generate_require = ["black", "jinja2"]
+generate_require = ["black>=24.3.0", "jinja2"]
 
 setup(
     name=PACKAGE_NAME,
     description="Python client for OpenSearch",
     license="Apache-2.0",
     url="https://github.com/opensearch-project/opensearch-py",
     long_description=long_description,
@@ -100,22 +102,23 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4",
+    python_requires=">=3.8, <4",
     install_requires=install_requires,
     test_suite="test_opensearchpy.run_tests.run_all",
     tests_require=tests_require,
     extras_require={
         "develop": tests_require + docs_require + generate_require,
         "docs": docs_require + async_require,
         "async": async_require,
```

