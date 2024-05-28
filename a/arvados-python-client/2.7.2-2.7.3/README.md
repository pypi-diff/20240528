# Comparing `tmp/arvados-python-client-2.7.2.tar.gz` & `tmp/arvados-python-client-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.7.2.tar", last modified: Tue Apr  9 20:11:19 2024, max compression
+gzip compressed data, was "arvados-python-client-2.7.3.tar", last modified: Tue May 28 13:36:17 2024, max compression
```

## Comparing `arvados-python-client-2.7.2.tar` & `arvados-python-client-2.7.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2457 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7874 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2265 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3511 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_pycurlhelper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-04-09 20:11:17.000000 arvados-python-client-2.7.2/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21264 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    48875 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    93813 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6036 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    37771 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18760 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13311 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    24015 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11886 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1564 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      988 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9197 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13562 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/http_to_keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    63190 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1208 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/logging.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8586 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2902 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3833 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28299 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/vocabulary.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)   368111 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados-v1-discovery.json
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2149 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      348 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-ws
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    15250 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/discovery2pydoc.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    37955 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23177 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8687 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10920 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43718 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6363 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_cmd_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77476 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19428 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    78007 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6382 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_storage_classes.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9387 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.899599 arvados-python-client-2.7.3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-05-28 13:36:17.899599 arvados-python-client-2.7.3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2457 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.839594 arvados-python-client-2.7.3/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7874 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2265 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3511 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-05-28 13:36:16.000000 arvados-python-client-2.7.3/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21264 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    50268 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    93813 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.839594 arvados-python-client-2.7.3/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6036 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    37771 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18760 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13311 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    24015 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11886 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1564 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      988 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9231 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13562 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    63190 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1208 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/logging.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8586 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2902 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3833 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28299 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados/vocabulary.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)   368111 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados-v1-discovery.json
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.839594 arvados-python-client-2.7.3/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-05-28 13:36:17.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2149 2024-05-28 13:36:17.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 13:36:17.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      348 2024-05-28 13:36:17.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2024-05-28 13:36:17.000000 arvados-python-client-2.7.3/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.879597 arvados-python-client-2.7.3/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/bin/arv-ws
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    15250 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/discovery2pydoc.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 13:36:17.899599 arvados-python-client-2.7.3/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.899599 arvados-python-client-2.7.3/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:17.899599 arvados-python-client-2.7.3/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    37955 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23177 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8687 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10920 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43718 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6363 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_cmd_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77476 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19428 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    78007 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6382 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_storage_classes.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9387 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2024-05-28 13:36:07.000000 arvados-python-client-2.7.3/tests/test_vocabulary.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arvados-python-client-2.7.2/LICENSE-2.0.txt` & `arvados-python-client-2.7.3/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/PKG-INFO` & `arvados-python-client-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.7.2
+Version: 2.7.3
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.7.2/README.rst` & `arvados-python-client-2.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/__init__.py` & `arvados-python-client-2.7.3/arvados/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/_normalize_stream.py` & `arvados-python-client-2.7.3/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/_pycurlhelper.py` & `arvados-python-client-2.7.3/arvados/_pycurlhelper.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/_ranges.py` & `arvados-python-client-2.7.3/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/api.py` & `arvados-python-client-2.7.3/arvados/api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/arvfile.py` & `arvados-python-client-2.7.3/arvados/arvfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1044,26 +1044,35 @@
             if diff > 0:
                 self._segments.append(Range(padding.blockid, self.size(), diff, 0))
             self.set_committed(False)
         else:
             # size == self.size()
             pass
 
-    def readfrom(self, offset, size, num_retries, exact=False):
+    def readfrom(self, offset, size, num_retries, exact=False, return_memoryview=False):
         """Read up to `size` bytes from the file starting at `offset`.
 
-        :exact:
-         If False (default), return less data than requested if the read
-         crosses a block boundary and the next block isn't cached.  If True,
-         only return less data than requested when hitting EOF.
+        Arguments:
+
+        * exact: bool --- If False (default), return less data than
+         requested if the read crosses a block boundary and the next
+         block isn't cached.  If True, only return less data than
+         requested when hitting EOF.
+
+        * return_memoryview: bool --- If False (default) return a
+          `bytes` object, which may entail making a copy in some
+          situations.  If True, return a `memoryview` object which may
+          avoid making a copy, but may be incompatible with code
+          expecting a `bytes` object.
+
         """
 
         with self.lock:
             if size == 0 or offset >= self.size():
-                return b''
+                return memoryview(b'') if return_memoryview else b''
             readsegs = locators_and_ranges(self._segments, offset, size)
 
             prefetch = None
             prefetch_lookahead = self.parent._my_block_manager().prefetch_lookahead
             if prefetch_lookahead:
                 # Doing prefetch on every read() call is surprisingly expensive
                 # when we're trying to deliver data at 600+ MiBps and want
@@ -1095,17 +1104,18 @@
         if prefetch:
             for lr in prefetch:
                 if lr.locator not in locs:
                     self.parent._my_block_manager().block_prefetch(lr.locator)
                     locs.add(lr.locator)
 
         if len(data) == 1:
-            return data[0]
+            return data[0] if return_memoryview else data[0].tobytes()
         else:
-            return b''.join(data)
+            return memoryview(b''.join(data)) if return_memoryview else b''.join(data)
+
 
     @must_be_writable
     @synchronized
     def writeto(self, offset, data, num_retries):
         """Write `data` to the file starting at `offset`.
 
         This will update existing bytes and/or extend the size of the file as
@@ -1262,41 +1272,57 @@
     def readinto(self, b):
         data = self.read(len(b))
         b[:len(data)] = data
         return len(data)
 
     @_FileLikeObjectBase._before_close
     @retry_method
-    def read(self, size=None, num_retries=None):
+    def read(self, size=-1, num_retries=None, return_memoryview=False):
         """Read up to `size` bytes from the file and return the result.
 
-        Starts at the current file position.  If `size` is None, read the
-        entire remainder of the file.
+        Starts at the current file position.  If `size` is negative or None,
+        read the entire remainder of the file.
+
+        Returns None if the file pointer is at the end of the file.
+
+        Returns a `bytes` object, unless `return_memoryview` is True,
+        in which case it returns a memory view, which may avoid an
+        unnecessary data copy in some situations.
+
         """
-        if size is None:
+        if size < 0 or size is None:
             data = []
-            rd = self.arvadosfile.readfrom(self._filepos, config.KEEP_BLOCK_SIZE, num_retries)
+            #
+            # specify exact=False, return_memoryview=True here so that we
+            # only copy data once into the final buffer.
+            #
+            rd = self.arvadosfile.readfrom(self._filepos, config.KEEP_BLOCK_SIZE, num_retries, exact=False, return_memoryview=True)
             while rd:
                 data.append(rd)
                 self._filepos += len(rd)
-                rd = self.arvadosfile.readfrom(self._filepos, config.KEEP_BLOCK_SIZE, num_retries)
-            return b''.join(data)
+                rd = self.arvadosfile.readfrom(self._filepos, config.KEEP_BLOCK_SIZE, num_retries, exact=False, return_memoryview=True)
+            return memoryview(b''.join(data)) if return_memoryview else b''.join(data)
         else:
-            data = self.arvadosfile.readfrom(self._filepos, size, num_retries, exact=True)
+            data = self.arvadosfile.readfrom(self._filepos, size, num_retries, exact=True, return_memoryview=return_memoryview)
             self._filepos += len(data)
             return data
 
     @_FileLikeObjectBase._before_close
     @retry_method
-    def readfrom(self, offset, size, num_retries=None):
+    def readfrom(self, offset, size, num_retries=None, return_memoryview=False):
         """Read up to `size` bytes from the stream, starting at the specified file offset.
 
         This method does not change the file position.
+
+        Returns a `bytes` object, unless `return_memoryview` is True,
+        in which case it returns a memory view, which may avoid an
+        unnecessary data copy in some situations.
+
         """
-        return self.arvadosfile.readfrom(offset, size, num_retries)
+        return self.arvadosfile.readfrom(offset, size, num_retries, exact=True, return_memoryview=return_memoryview)
 
     def flush(self):
         pass
 
 
 class ArvadosFileWriter(ArvadosFileReader):
     """Wraps ArvadosFile in a file-like object supporting both reading and writing.
```

### Comparing `arvados-python-client-2.7.2/arvados/cache.py` & `arvados-python-client-2.7.3/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/collection.py` & `arvados-python-client-2.7.3/arvados/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 
         return self.find_or_create(path, COLLECTION)
 
     def open(
             self,
             path: str,
             mode: str="r",
-            encoding: Optional[str]=None,
+            encoding: Optional[str]=None
     ) -> IO:
         """Open a file-like object within the collection
 
         This method returns a file-like object that can read and/or write the
         file located at `path` within the collection. If you attempt to write
         a `path` that does not exist, the file is created with `find_or_create`.
         If the file cannot be opened for any other reason, this method raises
@@ -357,14 +357,15 @@
 
         * mode: str --- The mode to open this file. Supports all the same
           values as `builtins.open`.
 
         * encoding: str | None --- The text encoding of the file. Only used
           when the file is opened in text mode. The default is
           platform-dependent.
+
         """
         if not re.search(r'^[rwa][bt]?\+?$', mode):
             raise errors.ArgumentError("Invalid mode {!r}".format(mode))
 
         if mode[0] == 'r' and '+' not in mode:
             fclass = ArvadosFileReader
             arvfile = self.find(path)
```

### Comparing `arvados-python-client-2.7.2/arvados/commands/_util.py` & `arvados-python-client-2.7.3/arvados/commands/_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/arv_copy.py` & `arvados-python-client-2.7.3/arvados/commands/arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/federation_migrate.py` & `arvados-python-client-2.7.3/arvados/commands/federation_migrate.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/get.py` & `arvados-python-client-2.7.3/arvados/commands/get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/keepdocker.py` & `arvados-python-client-2.7.3/arvados/commands/keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/ls.py` & `arvados-python-client-2.7.3/arvados/commands/ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/migrate19.py` & `arvados-python-client-2.7.3/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/put.py` & `arvados-python-client-2.7.3/arvados/commands/put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/run.py` & `arvados-python-client-2.7.3/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/commands/ws.py` & `arvados-python-client-2.7.3/arvados/commands/ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/config.py` & `arvados-python-client-2.7.3/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/crunch.py` & `arvados-python-client-2.7.3/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/diskcache.py` & `arvados-python-client-2.7.3/arvados/diskcache.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         # 'content' can None, an empty byte string, or a nonempty mmap
         # region.  If it is an mmap region, we want to advise the
         # kernel we're going to use it.  This nudges the kernel to
         # re-read most or all of the block if necessary (instead of
         # just a few pages at a time), reducing the number of page
         # faults and improving performance by 4x compared to not
         # calling madvise.
-        if self.content:
+        if self.content and hasattr(mmap.mmap, 'madvise'):
             self.content.madvise(mmap.MADV_WILLNEED)
         return self.content
 
     def set(self, value):
         tmpfile = None
         try:
             if value is None:
```

### Comparing `arvados-python-client-2.7.2/arvados/errors.py` & `arvados-python-client-2.7.3/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/events.py` & `arvados-python-client-2.7.3/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/http_to_keep.py` & `arvados-python-client-2.7.3/arvados/http_to_keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/keep.py` & `arvados-python-client-2.7.3/arvados/keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/logging.py` & `arvados-python-client-2.7.3/arvados/logging.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/retry.py` & `arvados-python-client-2.7.3/arvados/retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/safeapi.py` & `arvados-python-client-2.7.3/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/stream.py` & `arvados-python-client-2.7.3/arvados/stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/timer.py` & `arvados-python-client-2.7.3/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/util.py` & `arvados-python-client-2.7.3/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados/vocabulary.py` & `arvados-python-client-2.7.3/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados-v1-discovery.json` & `arvados-python-client-2.7.3/arvados-v1-discovery.json`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.7.3/arvados_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.7.2
+Version: 2.7.3
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.7.2/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.7.3/arvados_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/arvados_version.py` & `arvados-python-client-2.7.3/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/bin/arv-normalize` & `arvados-python-client-2.7.3/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/discovery2pydoc.py` & `arvados-python-client-2.7.3/discovery2pydoc.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/setup.py` & `arvados-python-client-2.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/arvados_testutil.py` & `arvados-python-client-2.7.3/tests/arvados_testutil.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/keepstub.py` & `arvados-python-client-2.7.3/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/manifest_examples.py` & `arvados-python-client-2.7.3/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/performance/performance_profiler.py` & `arvados-python-client-2.7.3/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/run_test_server.py` & `arvados-python-client-2.7.3/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_api.py` & `arvados-python-client-2.7.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_copy.py` & `arvados-python-client-2.7.3/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_get.py` & `arvados-python-client-2.7.3/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_keepdocker.py` & `arvados-python-client-2.7.3/tests/test_arv_keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_ls.py` & `arvados-python-client-2.7.3/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_normalize.py` & `arvados-python-client-2.7.3/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_put.py` & `arvados-python-client-2.7.3/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arv_ws.py` & `arvados-python-client-2.7.3/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_arvfile.py` & `arvados-python-client-2.7.3/tests/test_arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_benchmark_collections.py` & `arvados-python-client-2.7.3/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_cache.py` & `arvados-python-client-2.7.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_cmd_util.py` & `arvados-python-client-2.7.3/tests/test_cmd_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_collections.py` & `arvados-python-client-2.7.3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_crunch.py` & `arvados-python-client-2.7.3/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_errors.py` & `arvados-python-client-2.7.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_events.py` & `arvados-python-client-2.7.3/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_http.py` & `arvados-python-client-2.7.3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_keep_client.py` & `arvados-python-client-2.7.3/tests/test_keep_client.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_keep_locator.py` & `arvados-python-client-2.7.3/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_retry.py` & `arvados-python-client-2.7.3/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_retry_job_helpers.py` & `arvados-python-client-2.7.3/tests/test_retry_job_helpers.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_safeapi.py` & `arvados-python-client-2.7.3/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_sdk.py` & `arvados-python-client-2.7.3/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_storage_classes.py` & `arvados-python-client-2.7.3/tests/test_storage_classes.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_stream.py` & `arvados-python-client-2.7.3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_util.py` & `arvados-python-client-2.7.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.2/tests/test_vocabulary.py` & `arvados-python-client-2.7.3/tests/test_vocabulary.py`

 * *Files identical despite different names*

