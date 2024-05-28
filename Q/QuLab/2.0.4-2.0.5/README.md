# Comparing `tmp/qulab-2.0.4.tar.gz` & `tmp/qulab-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.4.tar", last modified: Tue May 28 05:05:32 2024, max compression
+gzip compressed data, was "qulab-2.0.5.tar", last modified: Tue May 28 07:37:19 2024, max compression
```

## Comparing `qulab-2.0.4.tar` & `qulab-2.0.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.706858 qulab-2.0.4/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-28 05:04:58.000000 qulab-2.0.4/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-28 05:04:58.000000 qulab-2.0.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 05:05:32.706625 qulab-2.0.4/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.706290 qulab-2.0.4/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-28 05:04:58.000000 qulab-2.0.4/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-28 05:04:58.000000 qulab-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.693181 qulab-2.0.4/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.694996 qulab-2.0.4/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.696805 qulab-2.0.4/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    17611 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    25598 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.697791 qulab-2.0.4/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.698023 qulab-2.0.4/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.699589 qulab-2.0.4/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.700359 qulab-2.0.4/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.701019 qulab-2.0.4/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.701321 qulab-2.0.4/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.702514 qulab-2.0.4/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.704348 qulab-2.0.4/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705567 qulab-2.0.4/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-28 05:05:32.706894 qulab-2.0.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-28 05:04:58.000000 qulab-2.0.4/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705689 qulab-2.0.4/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-28 05:04:58.000000 qulab-2.0.4/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705984 qulab-2.0.4/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-28 05:04:58.000000 qulab-2.0.4/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.530429 qulab-2.0.5/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-28 07:36:42.000000 qulab-2.0.5/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-28 07:36:42.000000 qulab-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 07:37:19.530205 qulab-2.0.5/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529869 qulab-2.0.5/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-28 07:36:42.000000 qulab-2.0.5/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-28 07:36:42.000000 qulab-2.0.5/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.519186 qulab-2.0.5/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.520628 qulab-2.0.5/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.522219 qulab-2.0.5/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    17938 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    25931 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.523076 qulab-2.0.5/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.523280 qulab-2.0.5/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.524445 qulab-2.0.5/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525010 qulab-2.0.5/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525623 qulab-2.0.5/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525875 qulab-2.0.5/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.526821 qulab-2.0.5/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.528357 qulab-2.0.5/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529294 qulab-2.0.5/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-28 07:37:19.530465 qulab-2.0.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-28 07:36:42.000000 qulab-2.0.5/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529417 qulab-2.0.5/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-28 07:36:42.000000 qulab-2.0.5/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529612 qulab-2.0.5/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-28 07:36:42.000000 qulab-2.0.5/tests/test_scan.py
```

### Comparing `qulab-2.0.4/LICENSE` & `qulab-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/PKG-INFO` & `qulab-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.4
+Version: 2.0.5
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.4/QuLab.egg-info/PKG-INFO` & `qulab-2.0.5/QuLab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.4
+Version: 2.0.5
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.4/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.5/QuLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/README.md` & `qulab-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/pyproject.toml` & `qulab-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/config.py` & `qulab-2.0.5/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/dataset.py` & `qulab-2.0.5/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/event_queue.py` & `qulab-2.0.5/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/mainwindow.py` & `qulab-2.0.5/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/monitor.py` & `qulab-2.0.5/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/ploter.py` & `qulab-2.0.5/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/qt_compat.py` & `qulab-2.0.5/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/monitor/toolbar.py` & `qulab-2.0.5/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/curd.py` & `qulab-2.0.5/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/expression.py` & `qulab-2.0.5/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/models.py` & `qulab-2.0.5/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/optimize.py` & `qulab-2.0.5/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/query_record.py` & `qulab-2.0.5/qulab/scan/query_record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/recorder.py` & `qulab-2.0.5/qulab/scan/recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,24 @@
         for key, value in self._items.items():
             if isinstance(value, BufferList):
                 value.flush()
 
         with open(self._file, 'wb') as f:
             dill.dump(self, f)
 
+    def __repr__(self):
+        return f"<Record: id={self.id} app={self.description['app']}, keys={self.keys()}>"
+    
+    # def _repr_html_(self):
+    #     return f"""
+    #     <h3>Record: id={self.id}, app={self.description['app']}</h3>
+    #     <p>keys={self.keys()}</p>
+    #     <p>dims={self.dims}</p>
+    #     """
+
 
 class Request():
     __slots__ = ['sock', 'identity', 'msg', 'method']
 
     def __init__(self, sock, identity, msg):
         self.sock = sock
         self.identity = identity
```

### Comparing `qulab-2.0.4/qulab/scan/scan.py` & `qulab-2.0.5/qulab/scan/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,26 +170,27 @@
         return super().__new__(cls)
 
     def __init__(self,
                  app: str = 'task',
                  tags: tuple[str] = (),
                  database: str | Path
                  | None = f'tcp://127.0.0.1:{default_record_port}',
+                 dump_globals: bool = False,
                  mixin=None):
         self.id = task_uuid()
         self.record = None
         self.namespace = {}
         self.description = {
             'app': app,
             'tags': tags,
             'loops': {},
             'consts': {},
             'functions': {},
             'optimizers': {},
-            'namespace': {},
+            'namespace': {} if dump_globals else None,
             'actions': {},
             'dependents': {},
             'order': {},
             'filters': {},
             'total': {},
             'database': database,
             'hiden': ['self', r'^__.*', r'.*__$'],
@@ -204,14 +205,15 @@
         self._main_task = None
         self._sock = None
         self._sem = asyncio.Semaphore(100)
         self._bar: dict[int, tqdm] = {}
         self._hide_pattern_re = re.compile('|'.join(self.description['hiden']))
         self._task_queue = asyncio.Queue()
         self._task_pool = []
+        self._single_step = True
 
     def __del__(self):
         try:
             self._main_task.cancel()
         except:
             pass
         for task in self._task_pool:
@@ -444,14 +446,17 @@
         while not self._task_queue.empty():
             evt = self._task_queue.get_nowait()
             if isinstance(evt, asyncio.Event):
                 evt.set()
             elif inspect.isawaitable(evt):
                 await evt
         task.cancel()
+        if self._single_step:
+            await self.emit(0, 0, 0, self.variables.copy())
+            await self.emit(-1, 0, 0, {})
         return self.variables
 
     async def done(self):
         if self._main_task is not None:
             try:
                 await self._main_task
             except asyncio.CancelledError:
@@ -500,14 +505,15 @@
                 self.variables,
                 self.description['loops'].get(self.current_level, []),
                 self.description['order'].get(self.current_level, []),
                 self.description['functions'], self.description['optimizers']):
             self._current_level += 1
             if await self._filter(variables, self.current_level - 1):
                 yield variables
+                self._single_step = False
                 asyncio.create_task(
                     self.emit(self.current_level - 1, step, position,
                               variables.copy()))
                 step += 1
             position += 1
             self._current_level -= 1
             self._task_queue.put_nowait(
@@ -610,15 +616,16 @@
     return namespace
 
 
 def assymbly(description):
     import __main__
     from IPython import get_ipython
 
-    description['namespace'] = dump_globals()
+    if isinstance(description['namespace'], dict):
+        description['namespace'] = dump_globals()
 
     ipy = get_ipython()
     if ipy is not None:
         description['entry']['shell'] = 'ipython'
         description['entry']['cmds'] = ipy.user_ns['In']
     else:
         try:
```

### Comparing `qulab-2.0.4/qulab/scan/server.py` & `qulab-2.0.5/qulab/scan/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/scan/utils.py` & `qulab-2.0.5/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/__main__.py` & `qulab-2.0.5/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/backend/redis.py` & `qulab-2.0.5/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/base_dataset.py` & `qulab-2.0.5/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/chunk.py` & `qulab-2.0.5/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/dataset.py` & `qulab-2.0.5/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/file.py` & `qulab-2.0.5/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/__init__.py` & `qulab-2.0.5/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/config.py` & `qulab-2.0.5/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/file.py` & `qulab-2.0.5/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/ipy.py` & `qulab-2.0.5/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/models.py` & `qulab-2.0.5/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/record.py` & `qulab-2.0.5/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/report.py` & `qulab-2.0.5/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/models/tag.py` & `qulab-2.0.5/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/storage/storage.py` & `qulab-2.0.5/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/chat.py` & `qulab-2.0.5/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/device/basedevice.py` & `qulab-2.0.5/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/device/loader.py` & `qulab-2.0.5/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/device/utils.py` & `qulab-2.0.5/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.5/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/ipy_events.py` & `qulab-2.0.5/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/bencoder.py` & `qulab-2.0.5/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/cli.py` & `qulab-2.0.5/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/dhcp.py` & `qulab-2.0.5/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/dhcpd.py` & `qulab-2.0.5/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/kad.py` & `qulab-2.0.5/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/kcp.py` & `qulab-2.0.5/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/net/nginx.py` & `qulab-2.0.5/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/progress.py` & `qulab-2.0.5/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/exceptions.py` & `qulab-2.0.5/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/msgpack.py` & `qulab-2.0.5/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.5/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/rpc.py` & `qulab-2.0.5/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/serialize.py` & `qulab-2.0.5/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/server.py` & `qulab-2.0.5/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/socket.py` & `qulab-2.0.5/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/utils.py` & `qulab-2.0.5/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/sys/rpc/zmq_socket.py` & `qulab-2.0.5/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/__init__.py` & `qulab-2.0.5/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/__main__.py` & `qulab-2.0.5/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/_autoplot.py` & `qulab-2.0.5/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/plot_layout.py` & `qulab-2.0.5/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/plot_seq.py` & `qulab-2.0.5/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/qdat.py` & `qulab-2.0.5/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/qulab/visualization/widgets.py` & `qulab-2.0.5/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.4/setup.py` & `qulab-2.0.5/setup.py`

 * *Files identical despite different names*

