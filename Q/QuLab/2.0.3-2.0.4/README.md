# Comparing `tmp/qulab-2.0.3.tar.gz` & `tmp/qulab-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.3.tar", last modified: Sat May 25 06:48:37 2024, max compression
+gzip compressed data, was "qulab-2.0.4.tar", last modified: Tue May 28 05:05:32 2024, max compression
```

## Comparing `qulab-2.0.3.tar` & `qulab-2.0.4.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.385120 qulab-2.0.3/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-25 06:48:04.000000 qulab-2.0.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-25 06:48:04.000000 qulab-2.0.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-25 06:48:37.384899 qulab-2.0.3/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384608 qulab-2.0.3/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2256 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-25 06:48:04.000000 qulab-2.0.3/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-25 06:48:04.000000 qulab-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.372473 qulab-2.0.3/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.375289 qulab-2.0.3/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.376668 qulab-2.0.3/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11521 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    15402 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    22494 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.377480 qulab-2.0.3/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.377762 qulab-2.0.3/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.378958 qulab-2.0.3/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.379432 qulab-2.0.3/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.379956 qulab-2.0.3/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.380203 qulab-2.0.3/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.381358 qulab-2.0.3/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.383003 qulab-2.0.3/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384104 qulab-2.0.3/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-25 06:48:37.385154 qulab-2.0.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-25 06:48:04.000000 qulab-2.0.3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384234 qulab-2.0.3/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-25 06:48:04.000000 qulab-2.0.3/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384354 qulab-2.0.3/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-25 06:48:04.000000 qulab-2.0.3/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.706858 qulab-2.0.4/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-28 05:04:58.000000 qulab-2.0.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-28 05:04:58.000000 qulab-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 05:05:32.706625 qulab-2.0.4/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.706290 qulab-2.0.4/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-28 05:05:32.000000 qulab-2.0.4/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-28 05:04:58.000000 qulab-2.0.4/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-28 05:04:58.000000 qulab-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.693181 qulab-2.0.4/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.694996 qulab-2.0.4/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.696805 qulab-2.0.4/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    17611 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    25598 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.697791 qulab-2.0.4/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.698023 qulab-2.0.4/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.699589 qulab-2.0.4/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.700359 qulab-2.0.4/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.701019 qulab-2.0.4/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.701321 qulab-2.0.4/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.702514 qulab-2.0.4/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.704348 qulab-2.0.4/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705567 qulab-2.0.4/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-28 05:04:58.000000 qulab-2.0.4/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-28 05:05:32.706894 qulab-2.0.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-28 05:04:58.000000 qulab-2.0.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705689 qulab-2.0.4/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-28 05:04:58.000000 qulab-2.0.4/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 05:05:32.705984 qulab-2.0.4/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-28 05:04:58.000000 qulab-2.0.4/tests/test_scan.py
```

### Comparing `qulab-2.0.3/LICENSE` & `qulab-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/PKG-INFO` & `qulab-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.3
+Version: 2.0.4
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.3/QuLab.egg-info/PKG-INFO` & `qulab-2.0.4/QuLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.3
+Version: 2.0.4
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.3/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.4/QuLab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 qulab/scan/curd.py
 qulab/scan/expression.py
 qulab/scan/models.py
 qulab/scan/optimize.py
 qulab/scan/query_record.py
 qulab/scan/recorder.py
 qulab/scan/scan.py
+qulab/scan/server.py
 qulab/scan/utils.py
 qulab/storage/__init__.py
 qulab/storage/__main__.py
 qulab/storage/base_dataset.py
 qulab/storage/chunk.py
 qulab/storage/dataset.py
 qulab/storage/file.py
```

### Comparing `qulab-2.0.3/README.md` & `qulab-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/pyproject.toml` & `qulab-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/config.py` & `qulab-2.0.4/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/dataset.py` & `qulab-2.0.4/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/event_queue.py` & `qulab-2.0.4/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/mainwindow.py` & `qulab-2.0.4/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/monitor.py` & `qulab-2.0.4/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/ploter.py` & `qulab-2.0.4/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/qt_compat.py` & `qulab-2.0.4/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/monitor/toolbar.py` & `qulab-2.0.4/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/scan/curd.py` & `qulab-2.0.4/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/scan/expression.py` & `qulab-2.0.4/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/scan/models.py` & `qulab-2.0.4/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/scan/optimize.py` & `qulab-2.0.4/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/scan/query_record.py` & `qulab-2.0.4/qulab/scan/query_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     if isinstance(database, str) and database.startswith('tcp://'):
         with ZMQContextManager(zmq.DEALER, connect=database) as socket:
             socket.send_pyobj({
                 'method': 'record_description',
                 'record_id': id
             })
             d = dill.loads(socket.recv_pyobj())
-            print(d.keys())
             return Record(id, database, d)
     else:
         from .models import Record as RecordInDB
         from .models import create_engine, sessionmaker
 
         db_file = Path(database) / 'data.db'
         engine = create_engine(f'sqlite:///{db_file}')
```

### Comparing `qulab-2.0.3/qulab/scan/recorder.py` & `qulab-2.0.4/qulab/scan/recorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import asyncio
+import os
 import pickle
 import sys
 import time
 import uuid
+from collections import defaultdict
 from pathlib import Path
+from threading import Lock
 
 import click
 import dill
 import numpy as np
 import zmq
 from loguru import logger
 
 from qulab.sys.rpc.zmq_socket import ZMQContextManager
 
 from .curd import query_record, remove_tags, tag, update_tags
 from .models import Record as RecordInDB
 from .models import Session, create_engine, create_tables, sessionmaker, utcnow
 
 _notgiven = object()
-datapath = Path.home() / 'qulab' / 'data'
+
+try:
+    default_record_port = int(os.getenv('QULAB_RECORD_PORT', 6789))
+except:
+    default_record_port = 6789
+
+if os.getenv('QULAB_RECORD_PATH'):
+    datapath = Path(os.getenv('QULAB_RECORD_PATH'))
+else:
+    datapath = Path.home() / 'qulab' / 'data'
 datapath.mkdir(parents=True, exist_ok=True)
 
 record_cache = {}
 
 
 def random_path(base):
     while True:
@@ -37,60 +49,87 @@
     def __init__(self, pos_file=None, value_file=None):
         self._pos = []
         self._value = []
         self.lu = ()
         self.rd = ()
         self.pos_file = pos_file
         self.value_file = value_file
+        self._lock = Lock()
+
+    def __getstate__(self):
+        return {
+            'pos_file': self.pos_file,
+            'value_file': self.value_file,
+            '_pos': self._pos,
+            '_value': self._value,
+            'lu': self.lu,
+            'rd': self.rd
+        }
+
+    def __setstate__(self, state):
+        self.pos_file = state['pos_file']
+        self.value_file = state['value_file']
+        self._pos = state['_pos']
+        self._value = state['_value']
+        self.lu = state['lu']
+        self.rd = state['rd']
+        self._lock = Lock()
 
     @property
     def shape(self):
         return tuple([i - j for i, j in zip(self.rd, self.lu)])
 
     def flush(self):
-        if self.pos_file is not None:
-            with open(self.pos_file, 'ab') as f:
-                for pos in self._pos:
-                    dill.dump(pos, f)
-            self._pos.clear()
-        if self.value_file is not None:
-            with open(self.value_file, 'ab') as f:
-                for value in self._value:
-                    dill.dump(value, f)
-            self._value.clear()
-
-    def append(self, pos, value):
+        with self._lock:
+            if self.pos_file is not None:
+                with open(self.pos_file, 'ab') as f:
+                    for pos in self._pos:
+                        dill.dump(pos, f)
+                self._pos.clear()
+            if self.value_file is not None:
+                with open(self.value_file, 'ab') as f:
+                    for value in self._value:
+                        dill.dump(value, f)
+                self._value.clear()
+
+    def append(self, pos, value, dims=None):
+        if dims is not None:
+            if any([p != 0 for i, p in enumerate(pos) if i not in dims]):
+                return
+            pos = tuple([pos[i] for i in dims])
         self.lu = tuple([min(i, j) for i, j in zip(pos, self.lu)])
         self.rd = tuple([max(i + 1, j) for i, j in zip(pos, self.rd)])
         self._pos.append(pos)
         self._value.append(value)
         if len(self._value) > 1000:
             self.flush()
 
     def value(self):
         v = []
-        if self.value_file is not None:
-            with open(self.value_file, 'rb') as f:
-                while True:
-                    try:
-                        v.append(dill.load(f))
-                    except EOFError:
-                        break
+        if self.value_file is not None and self.value_file.exists():
+            with self._lock:
+                with open(self.value_file, 'rb') as f:
+                    while True:
+                        try:
+                            v.append(dill.load(f))
+                        except EOFError:
+                            break
         v.extend(self._value)
         return v
 
     def pos(self):
         p = []
-        if self.pos_file is not None:
-            with open(self.pos_file, 'rb') as f:
-                while True:
-                    try:
-                        p.append(dill.load(f))
-                    except EOFError:
-                        break
+        if self.pos_file is not None and self.pos_file.exists():
+            with self._lock:
+                with open(self.pos_file, 'rb') as f:
+                    while True:
+                        try:
+                            p.append(dill.load(f))
+                        except EOFError:
+                            break
         p.extend(self._pos)
         return p
 
     def array(self):
         pos = np.asarray(self.pos()) - np.asarray(self.lu)
         data = np.asarray(self.value())
         inner_shape = data.shape[1:]
@@ -110,29 +149,40 @@
         self._index = []
         self._pos = []
         self._last_vars = set()
         self._levels = {}
         self._file = None
         self.independent_variables = {}
         self.constants = {}
-
-        for level, group in self.description['order'].items():
-            for names in group:
-                for name in names:
-                    self._levels[name] = level
+        self.dims = {}
 
         for name, value in self.description['consts'].items():
             if name not in self._items:
                 self._items[name] = value
             self.constants[name] = value
+            self.dims[name] = ()
         for level, range_list in self.description['loops'].items():
             for name, iterable in range_list:
                 if isinstance(iterable, (np.ndarray, list, tuple, range)):
                     self._items[name] = iterable
-                    self.independent_variables[name] = (level, iterable)
+                    self.independent_variables[name] = iterable
+                    self.dims[name] = (level, )
+
+        for level, group in self.description['order'].items():
+            for names in group:
+                for name in names:
+                    self._levels[name] = level
+                    if name not in self.dims:
+                        if name not in self.description['dependents']:
+                            self.dims[name] = (level, )
+                        else:
+                            d = set()
+                            for n in self.description['dependents'][name]:
+                                d.update(self.dims[n])
+                            self.dims[name] = tuple(sorted(d))
 
         if self.is_local_record():
             self.database = Path(self.database)
             self._file = random_path(self.database / 'objects')
             self._file.parent.mkdir(parents=True, exist_ok=True)
 
     def is_local_record(self):
@@ -199,14 +249,15 @@
         if level < 0:
             self.flush()
             return
 
         for key in set(variables.keys()) - self._last_vars:
             if key not in self._levels:
                 self._levels[key] = level
+                self.dims[key] = tuple(range(level + 1))
 
         self._last_vars = set(variables.keys())
         self._keys.update(variables.keys())
 
         if level >= len(self._pos):
             l = level + 1 - len(self._pos)
             self._index.extend(([0] * (l - 1)) + [step])
@@ -233,17 +284,17 @@
                         f2 = random_path(self.database / 'objects')
                         f2.parent.mkdir(parents=True, exist_ok=True)
                         self._items[key] = BufferList(f1, f2)
                     else:
                         self._items[key] = BufferList()
                     self._items[key].lu = pos
                     self._items[key].rd = tuple([i + 1 for i in pos])
-                    self._items[key].append(pos, value)
+                    self._items[key].append(pos, value, self.dims[key])
                 elif isinstance(self._items[key], BufferList):
-                    self._items[key].append(pos, value)
+                    self._items[key].append(pos, value, self.dims[key])
             elif self._levels[key] == -1 and key not in self._items:
                 self._items[key] = value
 
     def flush(self):
         if self.is_remote_record() or self.is_cache_record():
             return
 
@@ -279,29 +330,29 @@
 
 
 def flush_cache():
     for k, (t, r) in record_cache.items():
         r.flush()
 
 
-def get_record(session, id, datapath):
+def get_record(session: Session, id: int, datapath: Path) -> Record:
     if id not in record_cache:
         record_in_db = session.get(RecordInDB, id)
         record_in_db.atime = utcnow()
         path = datapath / 'objects' / record_in_db.file
         with open(path, 'rb') as f:
             record = dill.load(f)
     else:
         record = record_cache[id][1]
     clear_cache()
     record_cache[id] = time.time(), record
     return record
 
 
-def create_record(session, description, datapath):
+def record_create(session: Session, description: dict, datapath: Path) -> int:
     record = Record(None, datapath, description)
     record_in_db = RecordInDB()
     if 'app' in description:
         record_in_db.app = description['app']
     if 'tags' in description:
         record_in_db.tags = [tag(session, t) for t in description['tags']]
     record_in_db.file = '/'.join(record._file.parts[-4:])
@@ -313,34 +364,42 @@
         record_cache[record.id] = time.time(), record
         return record.id
     except:
         session.rollback()
         raise
 
 
+def record_append(session: Session, record_id: int, level: int, step: int,
+                  position: int, variables: dict, datapath: Path):
+    record = get_record(session, record_id, datapath)
+    record.append(level, step, position, variables)
+    try:
+        record_in_db = session.get(RecordInDB, record_id)
+        record_in_db.mtime = utcnow()
+        record_in_db.atime = utcnow()
+        session.commit()
+    except:
+        session.rollback()
+        raise
+
+
 @logger.catch
 async def handle(session: Session, request: Request, datapath: Path):
 
     msg = request.msg
 
     match request.method:
         case 'ping':
             await reply(request, 'pong')
         case 'record_create':
             description = dill.loads(msg['description'])
-            await reply(request, create_record(session, description, datapath))
+            await reply(request, record_create(session, description, datapath))
         case 'record_append':
-            record = get_record(session, msg['record_id'], datapath)
-            record.append(msg['level'], msg['step'], msg['position'],
-                          msg['variables'])
-            if msg['level'] < 0:
-                record_in_db = session.get(RecordInDB, msg['record_id'])
-                record_in_db.mtime = utcnow()
-                record_in_db.atime = utcnow()
-                session.commit()
+            record_append(session, msg['record_id'], msg['level'], msg['step'],
+                          msg['position'], msg['variables'], datapath)
         case 'record_description':
             record = get_record(session, msg['record_id'], datapath)
             await reply(request, dill.dumps(record.description))
         case 'record_getitem':
             record = get_record(session, msg['record_id'], datapath)
             await reply(request, record.get(msg['key'], buffer_to_array=False))
         case 'record_keys':
@@ -361,15 +420,15 @@
         case 'record_remove_tags':
             remove_tags(session, msg['record_id'], msg['tags'])
         case 'record_add_tags':
             update_tags(session, msg['record_id'], msg['tags'], True)
         case 'record_replace_tags':
             update_tags(session, msg['record_id'], msg['tags'], False)
         case _:
-            logger.error(f'Unknown method: {msg["method"]}')
+            logger.error(f"Unknown method: {msg['method']}")
 
 
 async def _handle(session: Session, request: Request, datapath: Path):
     try:
         await handle(session, request, datapath)
     except:
         await reply(request, 'error')
@@ -427,15 +486,17 @@
                        timeout=timeout,
                        buffer=buffer,
                        interval=interval)
     await task
 
 
 @click.command()
-@click.option('--port', default=6789, help='Port of the server.')
+@click.option('--port',
+              default=os.getenv('QULAB_RECORD_PORT', 6789),
+              help='Port of the server.')
 @click.option('--datapath', default=datapath, help='Path of the data.')
 @click.option('--url', default=None, help='URL of the database.')
 @click.option('--timeout', default=1, help='Timeout of ping.')
 @click.option('--buffer', default=1024, help='Buffer size (MB).')
 @click.option('--interval',
               default=60,
               help='Interval of flush cache, in unit of second.')
```

### Comparing `qulab-2.0.3/qulab/scan/scan.py` & `qulab-2.0.4/qulab/scan/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import datetime
 import inspect
 import itertools
 import os
 import re
 import sys
 import uuid
+import warnings
 from graphlib import TopologicalSorter
 from pathlib import Path
 from types import MethodType
 from typing import Any, Awaitable, Callable, Iterable, Type
 
 import dill
 import numpy as np
@@ -17,15 +18,15 @@
 import zmq
 from skopt.space import Categorical, Integer, Real
 from tqdm.notebook import tqdm
 
 from ..sys.rpc.zmq_socket import ZMQContextManager
 from .expression import Env, Expression, Symbol
 from .optimize import NgOptimizer
-from .recorder import Record
+from .recorder import Record, default_record_port
 from .utils import async_zip, call_function
 
 __process_uuid = uuid.uuid1()
 __task_counter = itertools.count()
 
 
 def task_uuid():
@@ -167,88 +168,120 @@
                 except:
                     pass
         return super().__new__(cls)
 
     def __init__(self,
                  app: str = 'task',
                  tags: tuple[str] = (),
-                 database: str | Path | None = 'tcp://127.0.0.1:6789',
+                 database: str | Path
+                 | None = f'tcp://127.0.0.1:{default_record_port}',
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
+            'namespace': {},
             'actions': {},
             'dependents': {},
             'order': {},
             'filters': {},
-            'total': {}
+            'total': {},
+            'database': database,
+            'hiden': ['self', r'^__.*', r'.*__$'],
+            'entry': {
+                'env': {},
+                'shell': '',
+                'cmds': []
+            },
         }
         self._current_level = 0
-        self.variables = {}
-        self._task = None
-        self.sock = None
-        self.database = database
+        self._variables = {}
+        self._main_task = None
+        self._sock = None
         self._sem = asyncio.Semaphore(100)
         self._bar: dict[int, tqdm] = {}
-        self._hide_patterns = [r'^__.*', r'.*__$']
-        self._hide_pattern_re = re.compile('|'.join(self._hide_patterns))
+        self._hide_pattern_re = re.compile('|'.join(self.description['hiden']))
         self._task_queue = asyncio.Queue()
+        self._task_pool = []
+
+    def __del__(self):
+        try:
+            self._main_task.cancel()
+        except:
+            pass
+        for task in self._task_pool:
+            try:
+                task.cancel()
+            except:
+                pass
 
     def __getstate__(self) -> dict:
         state = self.__dict__.copy()
         del state['record']
-        del state['sock']
-        del state['_task']
+        del state['_sock']
+        del state['_main_task']
+        del state['_bar']
+        del state['_task_queue']
+        del state['_task_pool']
         del state['_sem']
         return state
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__.update(state)
         self.record = None
-        self.sock = None
-        self._task = None
+        self._sock = None
+        self._main_task = None
+        self._bar = {}
+        self._task_queue = asyncio.Queue()
+        self._task_pool = []
         self._sem = asyncio.Semaphore(100)
         for opt in self.description['optimizers'].values():
             opt.scanner = self
 
     @property
     def current_level(self):
         return self._current_level
 
+    @property
+    def variables(self) -> dict[str, Any]:
+        return self._variables
+
     async def emit(self, current_level, step, position, variables: dict[str,
                                                                         Any]):
         for key, value in list(variables.items()):
             if inspect.isawaitable(value) and not self.hiden(key):
                 variables[key] = await value
-        if self.sock is not None:
-            await self.sock.send_pyobj({
+        if self._sock is not None:
+            await self._sock.send_pyobj({
                 'task': self.id,
                 'method': 'record_append',
                 'record_id': self.record.id,
                 'level': current_level,
                 'step': step,
                 'position': position,
                 'variables': {
                     k: v
                     for k, v in variables.items() if not self.hiden(k)
                 }
             })
         else:
-            self.record.append(current_level, step, position, variables)
+            self.record.append(current_level, step, position, {
+                k: v
+                for k, v in variables.items() if not self.hiden(k)
+            })
 
     def hide(self, name: str):
-        self._hide_patterns.append(re.compile(name))
-        self._hide_pattern_re = re.compile('|'.join(self._hide_patterns))
+        self.description['hiden'].append(name)
+        self._hide_pattern_re = re.compile('|'.join(self.description['hiden']))
 
     def hiden(self, name: str) -> bool:
         return bool(self._hide_pattern_re.match(name))
 
     async def _filter(self, variables: dict[str, Any], level: int = 0):
         try:
             return all([
@@ -256,43 +289,28 @@
                     self.description['filters'].get(level, []),
                     self.description['filters'].get(-1, []))
             ])
         except:
             return True
 
     async def create_record(self):
-        import __main__
-        from IPython import get_ipython
-
-        ipy = get_ipython()
-        if ipy is not None:
-            scripts = ('ipython', ipy.user_ns['In'])
-        else:
-            try:
-                scripts = ('shell',
-                           [sys.executable, __main__.__file__, *sys.argv[1:]])
-            except:
-                scripts = ('', [])
-
-        self.description['ctime'] = datetime.datetime.now()
-        self.description['scripts'] = scripts
-        self.description['env'] = {k: v for k, v in os.environ.items()}
-        if self.sock is not None:
-            await self.sock.send_pyobj({
+        if self._sock is not None:
+            await self._sock.send_pyobj({
                 'task':
                 self.id,
                 'method':
                 'record_create',
                 'description':
                 dill.dumps(self.description)
             })
 
-            record_id = await self.sock.recv_pyobj()
-            return Record(record_id, self.database, self.description)
-        return Record(None, self.database, self.description)
+            record_id = await self._sock.recv_pyobj()
+            return Record(record_id, self.description['database'],
+                          self.description)
+        return Record(None, self.description['database'], self.description)
 
     def get(self, name: str):
         if name in self.description['consts']:
             return self.description['consts'][name]
         elif name in self.namespace:
             return self.namespace.get(name)
         else:
@@ -319,14 +337,18 @@
             level: The level of the scan to add the filter. -1 means any level.
         """
         if level not in self.description['filters']:
             self.description['filters'][level] = []
         self.description['filters'][level].append(func)
 
     def set(self, name: str, value):
+        try:
+            dill.dumps(value)
+        except:
+            raise ValueError('value is not serializable.')
         if isinstance(value, Expression):
             self.add_depends(name, value.symbols())
             self.description['functions'][name] = value
         elif callable(value):
             self.add_depends(name, _get_depends(value))
             self.description['functions'][name] = value
         else:
@@ -388,88 +410,112 @@
                 task.set()
             elif inspect.isawaitable(task):
                 await task
 
     async def _run(self):
         assymbly(self.description)
         task = asyncio.create_task(self._update_progress())
-        self.variables = self.description['consts'].copy()
+        self._task_pool.append(task)
+        self._variables = {'self': self}
+        self._variables.update(self.description['consts'])
         for level, total in self.description['total'].items():
             if total == np.inf:
                 total = None
             self._bar[level] = tqdm(total=total)
         for group in self.description['order'].get(-1, []):
             for name in group:
                 if name in self.description['functions']:
                     self.variables[name] = await call_function(
                         self.description['functions'][name], self.variables)
-        if isinstance(self.database,
-                      str) and self.database.startswith("tcp://"):
-            async with ZMQContextManager(zmq.DEALER,
-                                         connect=self.database) as socket:
-                self.sock = socket
+        if isinstance(
+                self.description['database'],
+                str) and self.description['database'].startswith("tcp://"):
+            async with ZMQContextManager(
+                    zmq.DEALER,
+                    connect=self.description['database']) as socket:
+                self._sock = socket
                 self.record = await self.create_record()
                 await self.work()
         else:
             self.record = await self.create_record()
             await self.work()
         for level, bar in self._bar.items():
             bar.close()
+
+        while not self._task_queue.empty():
+            evt = self._task_queue.get_nowait()
+            if isinstance(evt, asyncio.Event):
+                evt.set()
+            elif inspect.isawaitable(evt):
+                await evt
         task.cancel()
         return self.variables
 
     async def done(self):
-        if self._task is not None:
+        if self._main_task is not None:
             try:
-                await self._task
+                await self._main_task
             except asyncio.CancelledError:
                 pass
 
+    def finished(self):
+        return self._main_task.done()
+
     def start(self):
         import asyncio
-        self._task = asyncio.create_task(self._run())
+        self._main_task = asyncio.create_task(self._run())
+
+    async def submit(self, server='tcp://127.0.0.1:6788'):
+        assymbly(self.description)
+        async with ZMQContextManager(zmq.DEALER, connect=server) as socket:
+            await socket.send_pyobj({
+                'method': 'submit',
+                'description': dill.dumps(self.description)
+            })
+            self.id = await socket.recv_pyobj()
+            await socket.send_pyobj({'method': 'get_record_id', 'id': self.id})
+            record_id = await socket.recv_pyobj()
+            self.record = Record(record_id, self.description['database'],
+                                 self.description)
 
     def cancel(self):
-        if self._task is not None:
-            self._task.cancel()
+        if self._main_task is not None:
+            self._main_task.cancel()
 
     async def _reset_progress_bar(self, level):
         if level in self._bar:
             self._bar[level].reset()
 
     async def _update_progress_bar(self, level, n: int):
         if level in self._bar:
             self._bar[level].update(n)
 
     async def iter(self, **kwds):
         if self.current_level >= len(self.description['loops']):
             return
         step = 0
         position = 0
-        task = None
         self._task_queue.put_nowait(
             self._reset_progress_bar(self.current_level))
         async for variables in _iter_level(
                 self.variables,
                 self.description['loops'].get(self.current_level, []),
                 self.description['order'].get(self.current_level, []),
                 self.description['functions'], self.description['optimizers']):
             self._current_level += 1
             if await self._filter(variables, self.current_level - 1):
                 yield variables
-                task = asyncio.create_task(
+                asyncio.create_task(
                     self.emit(self.current_level - 1, step, position,
                               variables.copy()))
                 step += 1
             position += 1
             self._current_level -= 1
             self._task_queue.put_nowait(
                 self._update_progress_bar(self.current_level, 1))
-        if task is not None:
-            await task
         if self.current_level == 0:
             await self.emit(self.current_level - 1, 0, 0, {})
             for name, value in self.variables.items():
                 if inspect.isawaitable(value):
                     self.variables[name] = await value
             while not self._task_queue.empty():
                 task = self._task_queue.get_nowait()
@@ -515,15 +561,80 @@
             return Promise(task)
 
     async def _await(self, awaitable: Awaitable):
         async with self._sem:
             return await awaitable
 
 
+class Unpicklable:
+
+    def __init__(self, obj):
+        self.type = str(type(obj))
+        self.id = id(obj)
+
+    def __repr__(self):
+        return f'<Unpicklable: {self.type} at 0x{id(self):x}>'
+
+
+class TooLarge:
+
+    def __init__(self, obj):
+        self.type = str(type(obj))
+        self.id = id(obj)
+
+    def __repr__(self):
+        return f'<TooLarge: {self.type} at 0x{id(self):x}>'
+
+
+def dump_globals(ns=None, *, size_limit=10 * 1024 * 1024, warn=False):
+    import __main__
+
+    if ns is None:
+        ns = __main__.__dict__
+
+    namespace = {}
+
+    for name, value in ns.items():
+        try:
+            buf = dill.dumps(value)
+        except:
+            namespace[name] = Unpicklable(value)
+            if warn:
+                warnings.warn(f'Unpicklable: {name} {type(value)}')
+        if len(buf) > size_limit:
+            namespace[name] = TooLarge(value)
+            if warn:
+                warnings.warn(f'TooLarge: {name} {type(value)}')
+        else:
+            namespace[name] = buf
+
+    return namespace
+
+
 def assymbly(description):
+    import __main__
+    from IPython import get_ipython
+
+    description['namespace'] = dump_globals()
+
+    ipy = get_ipython()
+    if ipy is not None:
+        description['entry']['shell'] = 'ipython'
+        description['entry']['cmds'] = ipy.user_ns['In']
+    else:
+        try:
+            description['entry']['shell'] = 'shell'
+            description['entry']['cmds'] = [
+                sys.executable, __main__.__file__, *sys.argv[1:]
+            ]
+        except:
+            pass
+
+    description['entry']['env'] = {k: v for k, v in os.environ.items()}
+
     mapping = {
         label: level
         for level, label in enumerate(
             sorted(
                 set(description['loops'].keys())
                 | {k
                    for k in description['actions'].keys() if k >= 0}))
```

### Comparing `qulab-2.0.3/qulab/scan/utils.py` & `qulab-2.0.4/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/__main__.py` & `qulab-2.0.4/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/backend/redis.py` & `qulab-2.0.4/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/base_dataset.py` & `qulab-2.0.4/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/chunk.py` & `qulab-2.0.4/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/dataset.py` & `qulab-2.0.4/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/file.py` & `qulab-2.0.4/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/__init__.py` & `qulab-2.0.4/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/config.py` & `qulab-2.0.4/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/file.py` & `qulab-2.0.4/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/ipy.py` & `qulab-2.0.4/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/models.py` & `qulab-2.0.4/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/record.py` & `qulab-2.0.4/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/report.py` & `qulab-2.0.4/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/models/tag.py` & `qulab-2.0.4/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/storage/storage.py` & `qulab-2.0.4/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/chat.py` & `qulab-2.0.4/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/device/basedevice.py` & `qulab-2.0.4/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/device/loader.py` & `qulab-2.0.4/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/device/utils.py` & `qulab-2.0.4/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.4/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/ipy_events.py` & `qulab-2.0.4/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/bencoder.py` & `qulab-2.0.4/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/cli.py` & `qulab-2.0.4/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/dhcp.py` & `qulab-2.0.4/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/dhcpd.py` & `qulab-2.0.4/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/kad.py` & `qulab-2.0.4/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/kcp.py` & `qulab-2.0.4/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/net/nginx.py` & `qulab-2.0.4/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/progress.py` & `qulab-2.0.4/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/exceptions.py` & `qulab-2.0.4/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/msgpack.py` & `qulab-2.0.4/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.4/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/rpc.py` & `qulab-2.0.4/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/serialize.py` & `qulab-2.0.4/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/server.py` & `qulab-2.0.4/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/socket.py` & `qulab-2.0.4/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/utils.py` & `qulab-2.0.4/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/sys/rpc/zmq_socket.py` & `qulab-2.0.4/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/__init__.py` & `qulab-2.0.4/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/__main__.py` & `qulab-2.0.4/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/_autoplot.py` & `qulab-2.0.4/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/plot_layout.py` & `qulab-2.0.4/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/plot_seq.py` & `qulab-2.0.4/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/qdat.py` & `qulab-2.0.4/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/qulab/visualization/widgets.py` & `qulab-2.0.4/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.3/setup.py` & `qulab-2.0.4/setup.py`

 * *Files identical despite different names*

