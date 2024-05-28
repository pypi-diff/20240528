# Comparing `tmp/rtc-tools-interface-0.8.0b1.tar.gz` & `tmp/rtc-tools-interface-0.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-interface-0.8.0b1.tar", last modified: Tue May 14 13:15:55 2024, max compression
+gzip compressed data, was "rtc-tools-interface-0.8.0b2.tar", last modified: Tue May 28 10:50:28 2024, max compression
```

## Comparing `rtc-tools-interface-0.8.0b1.tar` & `rtc-tools-interface-0.8.0b2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14497 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.440740 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2253 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/rtctools_interface/
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/rtctools_interface/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.442740 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/closed_loop_dates.py
--rw-rw-rw-   0 root         (0) root         (0)     4893 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/results_construction.py
--rw-rw-rw-   0 root         (0) root         (0)     7597 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/runner.py
--rw-rw-rw-   0 root         (0) root         (0)    18717 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/time_series_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.444740 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10183 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_goal.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_generator_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5147 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_performance_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_table_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.444740 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/statistics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.445740 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11023 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    12382 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/subplot_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.445740 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/plot_table_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_plot_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7748 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/results_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/type_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/tests/closed_loop/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/test_read_xml.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/test_run_optization_problem_closed_loop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.448740 rtc-tools-interface-0.8.0b1/tests/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_passing_goals_directly.py
--rw-rw-rw-   0 root         (0) root         (0)     2076 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/tests/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/simulation/test_base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/simulation/test_plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/utils/get_test.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.292230 rtc-tools-interface-0.8.0b2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-28 10:50:28.292230 rtc-tools-interface-0.8.0b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14497 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.283230 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-28 10:50:28.000000 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-05-28 10:50:28.000000 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:50:28.000000 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-28 10:50:28.000000 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-28 10:50:28.000000 rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.293230 rtc-tools-interface-0.8.0b2/rtctools_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-28 10:50:28.293230 rtc-tools-interface-0.8.0b2/rtctools_interface/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.284230 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/closed_loop_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4893 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/results_construction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7597 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    18717 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/time_series_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.286230 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10195 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/base_goal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_generator_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5147 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_performance_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_table_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.286230 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/helpers/statistics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/plot_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.287230 rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11023 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    12382 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/subplot_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.288230 rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.289230 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/plot_table_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/read_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/read_plot_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7748 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/results_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/rtctools_interface/utils/type_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-28 10:50:28.293230 rtc-tools-interface-0.8.0b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.289230 rtc-tools-interface-0.8.0b2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.290230 rtc-tools-interface-0.8.0b2/tests/closed_loop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/closed_loop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/closed_loop/test_read_xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/closed_loop/test_run_optization_problem_closed_loop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.291230 rtc-tools-interface-0.8.0b2/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/optimization/test_base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/optimization/test_passing_goals_directly.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/optimization/test_plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/optimization/test_read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.291230 rtc-tools-interface-0.8.0b2/tests/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/simulation/test_base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/simulation/test_plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:50:28.292230 rtc-tools-interface-0.8.0b2/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/tests/utils/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2024-05-28 10:50:26.000000 rtc-tools-interface-0.8.0b2/versioneer.py
```

### Comparing `rtc-tools-interface-0.8.0b1/COPYING.LESSER` & `rtc-tools-interface-0.8.0b2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/README.md` & `rtc-tools-interface-0.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/SOURCES.txt` & `rtc-tools-interface-0.8.0b2/rtc_tools_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/closed_loop_dates.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/closed_loop_dates.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/results_construction.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/results_construction.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/runner.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/runner.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/time_series_handler.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/closed_loop/time_series_handler.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_goal.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/base_goal.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,17 @@
         self,
         optimization_problem: OptimizationProblem,
         function_min=np.nan,
         function_max=np.nan,
     ):
         """Set function bounds either by user specified value or calculated"""
         state_range = self._get_state_range(optimization_problem, self.state)
-        if (not np.isfinite(function_min) and not np.isfinite(state_range[0])) or (
-            not np.isfinite(function_max) and not np.isfinite(state_range[1])
-        ):
+        if (~np.isfinite(function_min) & ~np.isfinite(state_range[0])).any() or (
+            ~np.isfinite(function_max) & ~np.isfinite(state_range[1])
+        ).any():
             raise ValueError(
                 f"The upper/lower bound for state {self.state} for goal with id={self.goal_id} is not specified"
                 + " so the function range should be specified!"
             )
         if self.goal_type in ["range_rate_of_change"]:
             maximum_scaled_difference = (state_range[1] - state_range[0]) / np.diff(optimization_problem.times()).min()
             calculated_range = (-maximum_scaled_difference, maximum_scaled_difference)
@@ -211,16 +211,16 @@
         """
         Serialize the goal configuration into a dictionary.
         """
         goal_config: GoalConfig = {
             "goal_id": self.goal_id,
             "state": self.state,
             "goal_type": self.goal_type,
-            "function_min": self.function_range[0] if np.isfinite(self.function_range[0]) else None,
-            "function_max": self.function_range[1] if np.isfinite(self.function_range[1]) else None,
+            "function_min": self.function_range[0] if np.any(np.isfinite(self.function_range[0])) else None,
+            "function_max": self.function_range[1] if np.any(np.isfinite(self.function_range[1])) else None,
             "function_nominal": self.function_nominal if np.isfinite(self.function_nominal) else None,
             "target_min_series": None,
             "target_max_series": None,
             "target_min": self.target_min,
             "target_max": self.target_max,
             "priority": self.priority,
             "weight": self.weight,
```

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_optimization_problem.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_generator_mixin.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_generator_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_performance_metrics.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_table_schema.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/goal_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/statistics_mixin.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/helpers/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_mixin.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/read_goals.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/optimization/read_goals.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/plot_tools.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/plot_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/subplot_classes.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/plotting/subplot_classes.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/base_simulation_problem.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/plot_mixin.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/simulation/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/plot_table_schema.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/plot_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_goals_mixin.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/read_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_plot_table.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/read_plot_table.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/results_collection.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/results_collection.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/serialization.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/type_definitions.py` & `rtc-tools-interface-0.8.0b2/rtctools_interface/utils/type_definitions.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/closed_loop/test_run_optization_problem_closed_loop.py` & `rtc-tools-interface-0.8.0b2/tests/closed_loop/test_run_optization_problem_closed_loop.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/optimization/test_base_optimization_problem.py` & `rtc-tools-interface-0.8.0b2/tests/optimization/test_base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/optimization/test_passing_goals_directly.py` & `rtc-tools-interface-0.8.0b2/tests/optimization/test_passing_goals_directly.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/optimization/test_plot_goals_mixin.py` & `rtc-tools-interface-0.8.0b2/tests/optimization/test_plot_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/simulation/test_base_simulation_problem.py` & `rtc-tools-interface-0.8.0b2/tests/simulation/test_base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/simulation/test_plot_mixin.py` & `rtc-tools-interface-0.8.0b2/tests/simulation/test_plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/tests/utils/get_test.py` & `rtc-tools-interface-0.8.0b2/tests/utils/get_test.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.8.0b1/versioneer.py` & `rtc-tools-interface-0.8.0b2/versioneer.py`

 * *Files identical despite different names*

