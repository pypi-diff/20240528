# Comparing `tmp/mappymatch-0.4.2.tar.gz` & `tmp/mappymatch-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappymatch-0.4.2.tar", last modified: Wed May  8 16:04:06 2024, max compression
+gzip compressed data, was "mappymatch-0.4.3.tar", last modified: Tue May 28 16:29:37 2024, max compression
```

## Comparing `mappymatch-0.4.2.tar` & `mappymatch-0.4.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.909045 mappymatch-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-08 16:04:00.000000 mappymatch-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 16:04:00.000000 mappymatch-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-08 16:04:06.909045 mappymatch-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/constructs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/geofence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/road.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/maps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/igraph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/igraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/igraph/igraph_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/map_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/nx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/nx_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/nx/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/readers/osm_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/matchers/lcss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/constructs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/lcss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/line_snap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/matcher_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/osrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/valhalla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/resources/traces/
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31962 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_3.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/mappymatch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/process_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/mappymatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-08 16:04:00.000000 mappymatch-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:06.909045 mappymatch-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:00.000000 mappymatch-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_geofence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_add_match_for_stationary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_drop_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_find_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_forward_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_reverse_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_same_trajectory_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_process_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.711582 mappymatch-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 16:29:31.000000 mappymatch-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 16:29:31.000000 mappymatch-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-28 16:29:37.711582 mappymatch-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-28 16:29:31.000000 mappymatch-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.699582 mappymatch-0.4.3/mappymatch/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/geofence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/road.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/constructs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/maps/igraph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/igraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/igraph/igraph_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/map_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/maps/nx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/nx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/nx/nx_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/maps/nx/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/nx/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/maps/nx/readers/osm_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.703582 mappymatch-0.4.3/mappymatch/matchers/lcss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/lcss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/lcss/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/lcss/lcss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/lcss/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/lcss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/line_snap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/osrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/matchers/valhalla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.707582 mappymatch-0.4.3/mappymatch/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.707582 mappymatch-0.4.3/mappymatch/resources/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31962 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_3.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.707582 mappymatch-0.4.3/mappymatch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 16:29:31.000000 mappymatch-0.4.3/mappymatch/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.711582 mappymatch-0.4.3/mappymatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-28 16:29:37.000000 mappymatch-0.4.3/mappymatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-28 16:29:37.000000 mappymatch-0.4.3/mappymatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:29:37.000000 mappymatch-0.4.3/mappymatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 16:29:37.000000 mappymatch-0.4.3/mappymatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 16:29:37.000000 mappymatch-0.4.3/mappymatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-28 16:29:31.000000 mappymatch-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:29:37.711582 mappymatch-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:29:31.000000 mappymatch-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:29:37.711582 mappymatch-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_geofence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_add_match_for_stationary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_drop_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_find_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_forward_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_reverse_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_lcss_same_trajectory_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-28 16:29:31.000000 mappymatch-0.4.3/tests/test_valhalla.py
```

### Comparing `mappymatch-0.4.2/LICENSE` & `mappymatch-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/PKG-INFO` & `mappymatch-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.4.2/README.md` & `mappymatch-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/constructs/coordinate.py` & `mappymatch-0.4.3/mappymatch/constructs/coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/constructs/geofence.py` & `mappymatch-0.4.3/mappymatch/constructs/geofence.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/constructs/match.py` & `mappymatch-0.4.3/mappymatch/constructs/match.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/constructs/road.py` & `mappymatch-0.4.3/mappymatch/constructs/road.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from typing import Any, Dict, NamedTuple, Optional, Union
 
 from shapely.geometry import LineString
 
 
 class RoadId(NamedTuple):
-    start: Union[int, str]
-    end: Union[int, str]
-    key: Union[int, str]
+    start: Optional[Union[int, str]]
+    end: Optional[Union[int, str]]
+    key: Optional[Union[int, str]]
 
     def to_string(self) -> str:
         return f"{self.start},{self.end},{self.key}"
 
     def to_json(self) -> Dict[str, Any]:
         return self._asdict()
```

### Comparing `mappymatch-0.4.2/mappymatch/constructs/trace.py` & `mappymatch-0.4.3/mappymatch/constructs/trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/maps/igraph/igraph_map.py` & `mappymatch-0.4.3/mappymatch/maps/igraph/igraph_map.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/maps/map_interface.py` & `mappymatch-0.4.3/mappymatch/maps/map_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/maps/nx/nx_map.py` & `mappymatch-0.4.3/mappymatch/maps/nx/nx_map.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/maps/nx/readers/osm_readers.py` & `mappymatch-0.4.3/mappymatch/maps/nx/readers/osm_readers.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/lcss/constructs.py` & `mappymatch-0.4.3/mappymatch/matchers/lcss/constructs.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/lcss/lcss.py` & `mappymatch-0.4.3/mappymatch/matchers/lcss/lcss.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/lcss/ops.py` & `mappymatch-0.4.3/mappymatch/matchers/lcss/ops.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/lcss/utils.py` & `mappymatch-0.4.3/mappymatch/matchers/lcss/utils.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/line_snap.py` & `mappymatch-0.4.3/mappymatch/matchers/line_snap.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/match_result.py` & `mappymatch-0.4.3/mappymatch/matchers/match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/matcher_interface.py` & `mappymatch-0.4.3/mappymatch/matchers/matcher_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/osrm.py` & `mappymatch-0.4.3/mappymatch/matchers/osrm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/matchers/valhalla.py` & `mappymatch-0.4.3/mappymatch/matchers/valhalla.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import polyline
 import requests
 from shapely.geometry import LineString
 
 from mappymatch.constructs.match import Match
-from mappymatch.constructs.road import Road
+from mappymatch.constructs.road import Road, RoadId
 from mappymatch.constructs.trace import Trace
 from mappymatch.matchers.matcher_interface import MatcherInterface, MatchResult
 from mappymatch.utils.crs import LATLON_CRS
 
 log = logging.getLogger(__name__)
 
 DEMO_VALHALLA_ADDRESS = "https://valhalla1.openstreetmap.de/trace_attributes"
@@ -41,29 +41,30 @@
 ) -> List[Road]:
     """
     builds a mappymatch path from the result of a Valhalla map matching request
     """
     path = []
     for edge in edges:
         way_id = edge["way_id"]
+        road_id = RoadId(start=None, end=None, key=way_id)
         start_point_i = edge["begin_shape_index"]
         end_point_i = edge["end_shape_index"]
         start_point = shape[start_point_i]
         end_point = shape[end_point_i]
         geom = LineString([start_point, end_point])
 
         speed = edge["speed"]
         length = edge["length"]
 
         metadata = {
             "speed_mph": speed,
             "length_miles": length,
         }
 
-        road = Road(road_id=way_id, geom=geom, metadata=metadata)
+        road = Road(road_id=road_id, geom=geom, metadata=metadata)
 
         path.append(road)
 
     return path
 
 
 def build_match_result(
```

### Comparing `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_1.csv` & `mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_1.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_2.csv` & `mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_2.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_3.csv` & `mappymatch-0.4.3/mappymatch/resources/traces/sample_trace_3.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/utils/geo.py` & `mappymatch-0.4.3/mappymatch/utils/geo.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/utils/plot.py` & `mappymatch-0.4.3/mappymatch/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch/utils/process_trace.py` & `mappymatch-0.4.3/mappymatch/utils/process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/mappymatch.egg-info/PKG-INFO` & `mappymatch-0.4.3/mappymatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.4.2/mappymatch.egg-info/SOURCES.txt` & `mappymatch-0.4.3/mappymatch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 tests/test_lcss_forward_merge.py
 tests/test_lcss_merge.py
 tests/test_lcss_reverse_merge.py
 tests/test_lcss_same_trajectory_scheme.py
 tests/test_match_result.py
 tests/test_osm.py
 tests/test_process_trace.py
-tests/test_trace.py
+tests/test_trace.py
+tests/test_valhalla.py
```

### Comparing `mappymatch-0.4.2/pyproject.toml` & `mappymatch-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mappymatch"
-version = "0.4.2"
+version = "0.4.3"
 description = "Package for mapmatching."
 readme = "README.md"
 authors = [{ name = "National Renewable Energy Laboratory" }]
 license = { text = "BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
```

### Comparing `mappymatch-0.4.2/tests/test_coordinate.py` & `mappymatch-0.4.3/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_add_match_for_stationary.py` & `mappymatch-0.4.3/tests/test_lcss_add_match_for_stationary.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_compress.py` & `mappymatch-0.4.3/tests/test_lcss_compress.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_drop_stationary_points.py` & `mappymatch-0.4.3/tests/test_lcss_drop_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_find_stationary_points.py` & `mappymatch-0.4.3/tests/test_lcss_find_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_forward_merge.py` & `mappymatch-0.4.3/tests/test_lcss_forward_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_merge.py` & `mappymatch-0.4.3/tests/test_lcss_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_reverse_merge.py` & `mappymatch-0.4.3/tests/test_lcss_reverse_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_lcss_same_trajectory_scheme.py` & `mappymatch-0.4.3/tests/test_lcss_same_trajectory_scheme.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_match_result.py` & `mappymatch-0.4.3/tests/test_match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_osm.py` & `mappymatch-0.4.3/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_process_trace.py` & `mappymatch-0.4.3/tests/test_process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.2/tests/test_trace.py` & `mappymatch-0.4.3/tests/test_trace.py`

 * *Files identical despite different names*

