# Comparing `tmp/datapools-1.0.63.tar.gz` & `tmp/datapools-1.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.63.tar", last modified: Fri May 24 13:27:01 2024, max compression
+gzip compressed data, was "datapools-1.0.64.tar", last modified: Tue May 28 10:48:13 2024, max compression
```

## Comparing `datapools-1.0.63.tar` & `datapools-1.0.64.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.295247 datapools-1.0.63/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 13:26:52.000000 datapools-1.0.63/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    20865 2024-05-24 13:26:52.000000 datapools-1.0.63/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-24 13:26:52.000000 datapools-1.0.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 13:26:52.000000 datapools-1.0.63/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 13:27:01.295247 datapools-1.0.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-24 13:26:52.000000 datapools-1.0.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.283247 datapools-1.0.63/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.283247 datapools-1.0.63/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.283247 datapools-1.0.63/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.283247 datapools-1.0.63/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.283247 datapools-1.0.63/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.287247 datapools-1.0.63/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-24 13:26:52.000000 datapools-1.0.63/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 13:27:01.000000 datapools-1.0.63/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:27:01.295247 datapools-1.0.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 13:26:52.000000 datapools-1.0.63/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:27:01.291247 datapools-1.0.63/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:26:52.000000 datapools-1.0.63/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-24 13:26:52.000000 datapools-1.0.63/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-24 13:26:52.000000 datapools-1.0.63/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-24 13:26:52.000000 datapools-1.0.63/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.828412 datapools-1.0.64/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 10:48:05.000000 datapools-1.0.64/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    21946 2024-05-28 10:48:05.000000 datapools-1.0.64/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-28 10:48:05.000000 datapools-1.0.64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 10:48:05.000000 datapools-1.0.64/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-28 10:48:13.828412 datapools-1.0.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-28 10:48:05.000000 datapools-1.0.64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.808412 datapools-1.0.64/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.828412 datapools-1.0.64/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 10:48:13.828412 datapools-1.0.64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-28 10:48:05.000000 datapools-1.0.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/test_session_manager.py
```

### Comparing `datapools-1.0.63/HISTORY.md` & `datapools-1.0.64/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,47 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge remote-tracking branch 'origin/master' into sergpsu-delete-all-
+  sessions. [sergpsu]
+- Merge pull request #50 from
+  torrentsai/dependabot/github_actions/codecov/codecov-action-4.
+  [voldmr]
+
+  Bump codecov/codecov-action from 3 to 4
+- Bump codecov/codecov-action from 3 to 4. [dependabot[bot]]
+
+  Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 3 to 4.
+  - [Release notes](https://github.com/codecov/codecov-action/releases)
+  - [Changelog](https://github.com/codecov/codecov-action/blob/main/CHANGELOG.md)
+  - [Commits](https://github.com/codecov/codecov-action/compare/v3...v4)
+
+  ---
+  updated-dependencies:
+  - dependency-name: codecov/codecov-action
+    dependency-type: direct:production
+    update-type: version-update:semver-major
+  ...
+- Merge pull request #82 from torrentsai/sergpsu-delete-all-sessions.
+  [S]
+
+  minor
+- Merge pull request #81 from torrentsai/sergpsu-delete-all-sessions.
+  [S]
+
+  Sergpsu delete all sessions
+- Bugfix. [sergpsu]
+
+
+1.0.63 (2024-05-24)
+-------------------
+- Release: version 1.0.63 🚀 [sergpsu]
 - Decode. [sergpsu]
 
 
 1.0.62 (2024-05-24)
 -------------------
 - Release: version 1.0.62 🚀 [sergpsu]
 - . [sergpsu]
```

### Comparing `datapools-1.0.63/LICENSE` & `datapools-1.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/PKG-INFO` & `datapools-1.0.64/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.63
+Version: 1.0.64
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.63/README.md` & `datapools-1.0.64/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/api.py` & `datapools-1.0.64/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/cli.py` & `datapools-1.0.64/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/backend_api.py` & `datapools-1.0.64/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/queues/__init__.py` & `datapools-1.0.64/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/queues/rabbitmq.py` & `datapools-1.0.64/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/queues/types.py` & `datapools-1.0.64/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/session_manager.py` & `datapools-1.0.64/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/stoppable.py` & `datapools-1.0.64/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/storage/base_storage.py` & `datapools-1.0.64/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/storage/file_storage.py` & `datapools-1.0.64/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.64/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.64/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/common/types.py` & `datapools-1.0.64/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/producer/base_producer.py` & `datapools-1.0.64/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/scheduler/scheduler.py` & `datapools-1.0.64/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.64/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/default/default.py` & `datapools-1.0.64/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.64/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.64/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.64/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,30 +194,32 @@
                     # content = fh.read()
                     # direct url seems to work better than API access
                     url = self._get_download_url(file_id)
                     content = await self.download(url)
                     if content is not None:
                         logger.info(f"file size={len(content)}")
 
+                        author_tag = None
                         if self.demo_mode:
                             path = f"{parent_path}{item['name']}"
                             logger.info(f"{path=}")
 
                             # if file full path matches any structural rule,
                             # then trying to create demo user from the match info
                             match = self._match_structure_rules(path)
                             if match and "user" in match:
                                 short_tag_id = BasePlugin.gen_demo_tag(match["user"])
+                                author_tag = BaseTag(short_tag_id)
                                 yield CrawlerDemoUser(
                                     user_name=match["user"], short_tag_id=short_tag_id, platform="drive.google.com"
                                 )
 
-                        author_tag = None
-                        if datapool_content_type == DatapoolContentType.Image:
-                            author_tag = BasePlugin.parse_image_tag(content)
+                        if not author_tag:
+                            if datapool_content_type == DatapoolContentType.Image:
+                                author_tag = BasePlugin.parse_image_tag(content)
 
                         # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
                         obj_url = url
                         # storage_id = self.ctx.storage.gen_id(obj_url)
                         # await self.ctx.storage.put(storage_id, content)
 
                         yield CrawlerContent(
```

### Comparing `datapools-1.0.63/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.64/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.64/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.64/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.64/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.64/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.64/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools/worker/worker.py` & `datapools-1.0.64/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/datapools.egg-info/PKG-INFO` & `datapools-1.0.64/datapools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.63
+Version: 1.0.64
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.63/datapools.egg-info/SOURCES.txt` & `datapools-1.0.64/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/setup.py` & `datapools-1.0.64/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/tests/test_base.py` & `datapools-1.0.64/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.63/tests/test_session_manager.py` & `datapools-1.0.64/tests/test_session_manager.py`

 * *Files identical despite different names*

